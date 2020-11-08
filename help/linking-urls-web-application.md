---
title: Collegamento degli URL all’applicazione Web
seo-title: Collegamento degli URL all’applicazione Web
description: 'null'
seo-description: Scoprite come collegare gli URL all’applicazione Web.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 72%

---


# Collegamento degli URL all’applicazione Web{#linking-urls-to-your-web-application}

I siti Web e le applicazioni accedono al contenuto del server di immagini per elementi multimediali dinamici tramite le stringhe URL. Dopo aver pubblicato un’immagine, Dynamic Media Classic attiva una stringa URL che fa riferimento al predefinito per immagini sui server immagini per file multimediali dinamici. Potete incollare questi URL in un browser Web per la verifica.

Per inserire queste stringhe URL nelle pagine Web e nelle applicazioni, copiatele da Dynamic Media Classic. Per ottenere una stringa URL generata tramite un predefinito per immagini, passate alla schermata Anteprima o al pannello Sfoglia (in visualizzazione Dettagli).

## Ottenimento di un URL di un predefinito per immagini {#obtaining-an-image-preset-url}

Potete ottenere una stringa URL generata da un predefinito per immagini dalla schermata Anteprima o dalla visualizzazione Dettagli. Una volta copiato, l’URL viene inserito negli Appunti ed è pronto per essere incollato.

***Nota **: L’URL diventa attivo solo dopo che la risorsa è stata pubblicata.*

### Ottenimento di un URL di un predefinito per immagini da Anteprima {#obtaining-an-image-preset-url-from-preview}

1. Nel pannello Libreria risorse a sinistra, individuate la cartella contenente la risorsa immagine da visualizzare in anteprima.
1. Effettuate una delle seguenti operazioni:

   * Sopra la finestra Risorse, fate clic su Visualizzazione griglia a destra della barra degli strumenti. Nella finestra Risorse, selezionate una singola risorsa immagine; quindi fate clic su Anteprima > Elenco predefiniti immagine, sotto la miniatura.
   * Sopra la finestra Risorse, fate clic su Visualizzazione elenco a destra della barra degli strumenti. Nella finestra Risorse, selezionate una singola risorsa immagine; quindi fate clic su Anteprima > Elenco predefiniti immagine, a destra della miniatura.
   * Sopra la finestra Risorse, fate clic su Visualizzazione dettagli a destra della barra degli strumenti. Nella stessa barra degli strumenti, fate clic su Anteprima > Elenco predefiniti immagine.

1. (Facoltativo) Nella finestra Elenco predefiniti immagine, nell’elenco a discesa Codifica URL per Copia generazione URL che si trova in basso, selezionate la codifica URL da applicare all’URL della risorsa immagine quando viene copiato.
1. Nella finestra Elenco predefiniti immagine, in alto a destra nel riquadro di anteprima, fate clic su Copia URL per il tipo di predefinito selezionato.
1. Nell’angolo in basso a destra della finestra Elenco predefiniti immagine, fate clic su Chiudi per tornare alla schermata Risorse.

### Ottenimento di un URL di un predefinito per immagini dal pannello Sfoglia {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Nel pannello Libreria risorse a sinistra, individuate la cartella contenente la risorsa immagine da visualizzare in anteprima.
1. Sopra la finestra Risorse, fate clic su Visualizzazione griglia a destra della barra degli strumenti. Nella finestra Risorse, selezionate una singola risorsa di immagine.
1. Sopra la finestra Risorse, fate clic su Visualizzazione dettagli a destra della barra degli strumenti. 
1. Per aprire l’elenco dei predefiniti per immagini, selezionate URL nel pannello sul lato destro della schermata.
1. Selezionate il collegamento Copia URL accanto al nome del predefinito per immagini con l’URL che desiderate copiare negli Appunti.

## Stringhe URL di predefiniti per immagini {#about-image-preset-url-strings}

Una richiesta URL per il ridimensionamento delle immagini sui server immagini per file multimediali dinamici presenta la seguente sintassi di base:

*percorso*/*nome del server immagini*/*nome dell’account*/*nome dell’immagine*?*modificatore1*&amp;*modificatore2*&amp;...

In un URL di Dynamic Media Image Server, le istruzioni per la visualizzazione dell’immagine nel server vengono visualizzate dopo il punto interrogativo (?). Ad esempio, questa richiesta URL fornisce un’immagine denominata “backpack” con una larghezza di 250 pixel:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

L’URL di un predefinito per immagini contiene tutte le istruzioni sui modificatori necessarie per presentare l’immagine secondo le specifiche di formattazione e ridimensionamento corrette. Se non si usa un predefinito per immagini, vengono riportate tutte le istruzioni sui modificatori dopo il punto interrogativo (?) come in questa stringa URL:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

In una stringa URL generata con un predefinito per immagini, invece, il nome di quest’ultimo viene visualizzato al posto delle diverse istruzioni che sono definite dal predefinito stesso. Ad esempio, per l’URL lungo di cui sopra, la stringa URL è:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

I nomi dei predefiniti per immagini negli URL sono racchiusi tra simboli di dollaro ($). When a Dynamic Media Image Server encounters the Image Preset portion of the URL (the `Large` in this case), using the size and formatting instructions defined by the “Large” Image Preset.

## Aggiunta di immagini dinamiche alla pagina Web {#adding-dynamic-images-to-your-web-page}

To add dynamic images to your web page, the `<IMG>` tag in your HTML web page code typically is modified using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. La stringa produce l’immagine secondo le specifiche di formattazione e ridimensionamento definite dal predefinito per immagini.

Ad esempio, al posto della tipica richiesta di apertura di un’immagine statica, ovvero

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

you now use the `<IMG>`tag to replace the reference to a static image with an Image Preset call to the Dynamic Media Classic platform. Esempio di richiesta:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In this example, a Dynamic Media Image Server “looks up” the definition of `$thumbnail$` and dynamically generates the appropriate image with the sizing and formatting specifications defined by the `thumbnail`Image Preset. In una stringa URL, tutti gli elementi eccetto il nome del file immagine del prodotto (in questo esempio, `backpack_trns`) vengono generalmente collegati per modello di pagina. L’unico elemento che viene inserito automaticamente nel modello di pagina dal vostro server commerciale è l’ID IPS o il nome dell’immagine.
