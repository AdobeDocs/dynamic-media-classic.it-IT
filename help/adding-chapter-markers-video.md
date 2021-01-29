---
title: Aggiunta di marcatori capitolo a video
description: Scoprite come aggiungere marcatori capitolo a un video.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 85%

---


# Aggiunta di marcatori capitolo a video{#adding-chapter-markers-to-video}

Potete rendere più semplice la visualizzazione e la navigazione nei video di formato esteso aggiungendo marcatori capitolo a singoli video o a set video adattivi. Quando un utente riproduce il video, può fare clic sui marcatori capitolo nella timeline del video (detta anche cursore di scorrimento video) per navigare con facilità verso il suo punto di interesse, oppure passare immediatamente su altri contenuti, dimostrazioni, esercitazioni e così via.

>[!NOTE]
>
>il lettore video utilizzato deve supportare l’uso di marcatori capitolo.

Consultate [Aggiunta o modifica di un predefinito per visualizzatori ](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) per configurare i cue point di navigazione dei capitoli e il testo del titolo della finestra a comparsa del capitolo per il visualizzatore `Universal_HTML5_Video`_Video (HTML5).

Consultate anche [Aggiunta e modifica dei predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets).

Gli elenchi di capitoli si creano in modo analogo alle didascalie, Quindi creando un file WebVTT. Tuttavia, non è possibile utilizzare lo stesso file WebVTT anche per i sottotitoli; non è possibile impostare didascalie e capitoli in un unico file WebVTT.

Un esempio del formato da utilizzare creando un file WebVTT con navigazione dei capitoli è il seguente:

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

Nell’esempio riportato sopra, il `Chapter 1`capitolo  ( 1) è l’identificatore del cue point ed è opzionale. L’indicatore temporale del cue point `00:00:000 --> 01:04:364` indica il minutaggio iniziale e finale del capitolo, in formato 00:00:000. Le ultime tre cifre rappresentano i millisecondi e, se preferite, possono essere lasciate a zero. Il titolo del capitolo di `The bicycle store behind it all` è la descrizione effettiva del contenuto del capitolo. L’identificatore del cue point, il cue point iniziale e il titolo del capitolo vengono visualizzati in una finestra a comparsa del lettore video quando l’utente passa il puntatore del mouse sul riferimento visivo nella timeline del video.

Poiché state usando un visualizzatore video HTML5, è necessario verificare che il file dei capitoli creato segua lo standard WebVTT (Web Video Text Tracks). L’estensione dei file dei capitoli è .vtt. Per ulteriori informazioni sullo standard per sottotitoli WebVTT:

Vedere [WebVTT: Il formato Web Video Text Tracks](https://dev.w3.org/html5/webvtt/).

**Per aggiungere marcatori capitolo a video**

1. Utilizzando un semplice editor di testo esterno ad Dynamic Media Classic, create il file video del capitolo.

   >[!NOTE]
   >
   >per il supporto globale di capitoli a video in lingue diverse dall’inglese, tenete presente che lo standard WebVTT richiede che vengano creati file .vtt e chiamate separati per ogni lingua da supportare.

1. Salvate il file .vtt in codifica UTF8 per evitare problemi di rendering dei carattere nel titolo del capitolo.

   In genere, è consigliabile assegnare al file VTT dei capitoli lo stesso nome del file video, aggiungendo il suffisso `chapters`. In questo modo risulta più semplice automatizzare la generazione degli URL video utilizzando un sistema di gestione dei contenuti Web.

1. In Dynamic Media Classic, caricate il file WebVTT dei capitoli.

   Consultate [Caricamento dei file](uploading-files.md#uploading_files).

1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video da associare al file dei capitoli che avete caricato.
1. Nel pannello delle risorse, selezionate una singola risorsa video, quindi, sotto la miniatura della risorsa, fate clic su **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
1. Nella tabella Elenco visualizzatori, individuate il visualizzatore HTML5 denominato **Univeral_HTML5_Video** ed effettuate una delle seguenti operazioni:

   * Per un’esperienza di visualizzazione con video a comparsa, fate clic su **[!UICONTROL Copia URL]** all’estrema destra del nome.

      Aggiungete l’URL del video che avete copiato con la sintassi seguente per associarlo all’URL del l file dei sottotitoli:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Per un’esperienza di visualizzazione con video incorporato, fate clic su **[!UICONTROL Incorpora codice]** all’estrema destra del nome.

      Nella finestra di dialogo Codice da incorporare, fate clic su **[!UICONTROL Copia negli Appunti]**.

      Per il visualizzatore HTML5 `Universal_HTML5_Video`, aggiungete il codice da incorporare copiato con la seguente sintassi:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`

