---
title: Collegare gli URL all’applicazione web
description: Scopri come collegare gli URL all’applicazione web da Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 27%

---

# Collegare gli URL all’applicazione web{#linking-urls-to-your-web-application}

I siti Web e le applicazioni accedono al contenuto di Dynamic Medie Image Server tramite stringhe URL. Dopo aver pubblicato un’immagine, Adobe Dynamic Media Classic attiva una stringa URL che fa riferimento al predefinito immagine nei server immagini Dynamic Medie. Potete incollare questi URL in un browser Web per la verifica.

Per inserire queste stringhe URL nelle pagine Web e nelle applicazioni, copiale da Adobe Dynamic Media Classic. Per ottenere una stringa URL generata con un predefinito immagine, passa alla schermata Anteprima o al pannello Sfoglia (in Vista dettagli).

## Ottenere un URL per un predefinito immagine {#obtaining-an-image-preset-url}

Potete ottenere una stringa URL generata da un predefinito per immagini dalla schermata Anteprima o dalla visualizzazione Dettagli. Una volta copiato, l’URL viene inserito negli Appunti ed è pronto per essere incollato.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

### Ottieni un URL per predefinito immagine da Anteprima {#obtaining-an-image-preset-url-from-preview}

1. Nel pannello Libreria risorse, a sinistra, passa alla cartella Risorse che contiene la risorsa immagine da visualizzare in anteprima.
1. Effettuate una delle seguenti operazioni:

   * Sopra la finestra Risorse, sul lato destro della barra degli strumenti, seleziona **[!UICONTROL Vista griglia]**. Nella finestra Risorsa, seleziona una singola risorsa di immagine, quindi vai a sotto dell’immagine di miniatura **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco predefiniti immagine]**.
   * Sopra la finestra Risorse, sul lato destro della barra degli strumenti, seleziona **[!UICONTROL Vista a elenco]**. Nella finestra Risorsa, seleziona una singola risorsa di immagine, quindi a destra dell’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco predefiniti immagine]**.
   * Sopra la finestra Risorse, sul lato destro della barra degli strumenti, seleziona **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco predefiniti immagine]**.

1. (Facoltativo) Nell’elenco Predefiniti immagine, seleziona l’URL encoding for the image asset (Codifica URL per copia generazione URL) da applicare all’URL della risorsa immagine quando viene copiata.
1. Nella finestra Elenco predefiniti immagine, in alto a destra nel riquadro di anteprima, seleziona **[!UICONTROL Copia URL]** per il tipo di predefinito selezionato.
1. Nell&#39;angolo inferiore destro della finestra Elenco predefiniti immagine, seleziona **[!UICONTROL Chiudi]** per tornare alla schermata Risorse.

### Ottenere un URL per un predefinito immagine dal pannello Sfoglia {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Nel pannello Libreria risorse, a sinistra, passa alla cartella Risorse contenente la risorsa immagine da visualizzare in anteprima.
1. Sopra la finestra Risorse, sul lato destro della barra degli strumenti, seleziona **[!UICONTROL Vista griglia]**. Nella finestra Risorse, selezionate una singola risorsa di immagine.
1. Sopra la finestra Risorse, sul lato destro della barra degli strumenti, seleziona **[!UICONTROL Vista dettagli]**.
1. Seleziona **[!UICONTROL URL]** sul pannello a destra dello schermo, in modo da poter visualizzare l’elenco dei predefiniti immagine.
1. Seleziona **[!UICONTROL Copia URL]** Accanto al nome del predefinito immagine è presente il collegamento con l’URL da copiare negli Appunti.

## Stringhe URL di predefiniti per immagini {#about-image-preset-url-strings}

Una chiamata URL per Image Sizing to Dynamic Medie Image Server ha la seguente sintassi di base:

*percorso*/*nome del server immagini*/*nome dell’account*/*nome dell’immagine*?*modificatore1*&amp;*modificatore2*&amp;...

In un URL di Dynamic Medie Image Server, le istruzioni per la visualizzazione dell&#39;immagine al server vengono visualizzate dopo il punto interrogativo (?). Ad esempio, questa chiamata URL fornisce un’immagine denominata &quot;zaino&quot; con una larghezza di 250 pixel:

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

I nomi dei predefiniti per immagini negli URL sono racchiusi tra simboli di dollaro ($). Quando un server immagini Dynamic Medie rileva la porzione dell’URL relativa al predefinito immagine (il `Large` in questo caso), utilizzando le istruzioni di dimensione e formattazione definite dal predefinito per immagini di grandi dimensioni.

## Aggiungere immagini dinamiche alla pagina web {#adding-dynamic-images-to-your-web-page}

Per aggiungere immagini dinamiche alla pagina web, `<IMG>` nel codice della pagina web HTML in genere viene modificato utilizzando la stringa URL Adobe Dynamic Media Classic per effettuare una richiesta ai server immagini Dynamic Medie. La stringa produce l’immagine secondo le specifiche di formattazione e ridimensionamento definite dal predefinito per immagini.

Ad esempio, al posto della tipica richiesta di apertura di un’immagine statica, ovvero

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Ora utilizzi il `<IMG>`per sostituire il riferimento a un’immagine statica con una chiamata di predefinito immagine alla piattaforma Adobe Dynamic Media Classic. Esempio di richiesta:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

In questo esempio, un server immagini di Dynamic Medie &quot;cerca&quot; la definizione di `$thumbnail$` e genera dinamicamente l&#39;immagine appropriata con le specifiche di dimensionamento e formattazione definite dal `thumbnail`Predefinito immagine. In una stringa URL, tutti gli elementi eccetto il nome del file dell’immagine del prodotto ( `backpack_trns` in questo caso) sono tipicamente cablate per il modello di pagina. L’unico elemento che viene inserito automaticamente nel modello di pagina dal vostro server commerciale è l’ID IPS o il nome dell’immagine.
