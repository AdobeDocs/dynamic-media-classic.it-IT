---
title: Collegare gli URL all’applicazione web
description: Scopri come collegare gli URL all’applicazione web da Adobe Dynamic Media Classic.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 37%

---

# Collegare gli URL all’applicazione web{#linking-urls-to-your-web-application}

I siti web e le applicazioni accedono al contenuto di Dynamic Media Image Server tramite stringhe URL. Dopo aver pubblicato un’immagine, Adobe Dynamic Media Classic attiva una stringa URL che fa riferimento al predefinito immagine sui server di immagini Dynamic Media. Potete incollare questi URL in un browser Web per la verifica.

Per inserire queste stringhe URL nelle pagine web e nelle applicazioni, copiale da Adobe Dynamic Media Classic. Per ottenere una stringa URL generata con un predefinito per immagini, passate alla schermata Anteprima o al pannello Sfoglia (in Vista dettagli).

## Ottenere un URL di predefinito per immagini {#obtaining-an-image-preset-url}

Potete ottenere una stringa URL generata da un predefinito per immagini dalla schermata Anteprima o dalla visualizzazione Dettagli. Una volta copiato, l’URL viene inserito negli Appunti ed è pronto per essere incollato.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

### Ottenere un URL predefinito per immagini da Anteprima {#obtaining-an-image-preset-url-from-preview}

1. Nel pannello Libreria risorse a sinistra, individuate la cartella contenente la risorsa immagine da visualizzare in anteprima.
1. Effettuate una delle seguenti operazioni:

   * Sopra la finestra Risorse, seleziona **[!UICONTROL Vista griglia]** sul lato destro della barra degli strumenti. Nella finestra Risorsa, seleziona una singola risorsa immagine, quindi, sotto l’immagine miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco predefiniti immagine]**.
   * Sopra la finestra Risorse, sul lato destro della barra degli strumenti, seleziona **[!UICONTROL Vista a elenco]**. Nella finestra Risorsa, seleziona una singola risorsa immagine, quindi, a destra della miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco predefiniti immagine]**.
   * Sopra la finestra Risorse, seleziona **[!UICONTROL Vista dettagli]** sul lato destro della barra degli strumenti. Sulla stessa barra degli strumenti, passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco predefiniti immagine]**.

1. (Facoltativo) Nell’elenco a discesa Codifica URL per generazione copia URL dell’elenco Predefiniti immagine , seleziona la codifica URL da applicare all’URL della risorsa immagine quando viene copiata.
1. Nella finestra Elenco predefiniti immagine, nell’area in alto a destra del riquadro di anteprima, seleziona **[!UICONTROL Copia URL]** per il tipo di predefinito selezionato.
1. Nell’angolo in basso a destra della finestra Elenco predefiniti immagine, seleziona **[!UICONTROL Chiudi]** per tornare alla schermata Risorse.

### Ottenere un URL di un predefinito per immagini dal pannello di navigazione {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Nel pannello Libreria risorse a sinistra, individuate la cartella contenente la risorsa immagine da visualizzare in anteprima.
1. Sopra la finestra Risorse, seleziona **[!UICONTROL Vista griglia]** sul lato destro della barra degli strumenti. Nella finestra Risorse, selezionate una singola risorsa di immagine.
1. Sopra la finestra Risorse, seleziona **[!UICONTROL Vista dettagli]** sul lato destro della barra degli strumenti.
1. Seleziona **[!UICONTROL URL]** nel pannello sul lato destro dello schermo per aprire l’elenco dei predefiniti immagine.
1. Seleziona il collegamento **[!UICONTROL Copia URL]** accanto al nome del predefinito immagine con l’URL da copiare negli Appunti.

## Stringhe URL di predefiniti per immagini {#about-image-preset-url-strings}

Una chiamata URL per il dimensionamento dell&#39;immagine nei server di immagini Dynamic Media ha la seguente sintassi di base:

*percorso*/*nome del server immagini*/*nome dell’account*/*nome dell’immagine*?*modificatore1*&amp;*modificatore2*&amp;...

In un URL di Dynamic Media Image Server, le istruzioni per la visualizzazione dell&#39;immagine sul server vengono visualizzate dopo il punto interrogativo (?). Ad esempio, questa richiesta URL fornisce un’immagine denominata “backpack” con una larghezza di 250 pixel:

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

I nomi dei predefiniti per immagini negli URL sono racchiusi tra simboli di dollaro ($). Quando un server di immagini di Dynamic Media incontra la porzione Predefinito immagine dell&#39;URL (in questo caso `Large`), utilizzando le istruzioni per la dimensione e la formattazione definite dal predefinito di immagini &quot;Grande&quot;.

## Aggiungere immagini dinamiche alla pagina web {#adding-dynamic-images-to-your-web-page}

Per aggiungere immagini dinamiche alla pagina web, in genere il tag `<IMG>` nel codice della pagina web HTML viene modificato utilizzando la stringa URL Adobe Dynamic Media Classic per effettuare una richiesta ai server di immagini Dynamic Media. La stringa produce l’immagine secondo le specifiche di formattazione e ridimensionamento definite dal predefinito per immagini.

Ad esempio, al posto della tipica richiesta di apertura di un’immagine statica, ovvero

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Ora utilizzi il tag `<IMG>`per sostituire il riferimento a un’immagine statica con una chiamata Image Preset alla piattaforma Adobe Dynamic Media Classic. Esempio di richiesta:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In questo esempio, un server immagini Dynamic Media &quot;cerca&quot; la definizione di `$thumbnail$` e genera in modo dinamico l&#39;immagine appropriata con le specifiche di ridimensionamento e formattazione definite dal `thumbnail`predefinito immagine. In una stringa URL, tutti gli elementi eccetto il nome del file immagine del prodotto (in questo esempio, `backpack_trns`) vengono generalmente collegati per modello di pagina. L’unico elemento che viene inserito automaticamente nel modello di pagina dal vostro server commerciale è l’ID IPS o il nome dell’immagine.
