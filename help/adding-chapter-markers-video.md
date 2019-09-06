---
title: Aggiunta di marcatori capitolo a video
seo-title: Aggiunta di marcatori capitolo a video
description: 'null'
seo-description: Scoprite come aggiungere marcatori capitolo a un video.
uuid: 4 e 1 e 6 daf-afc 6-49 d 9-ac 90-183 fe 2 a 903 b 2
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/video
discoiquuid: 8 bc 5 e 552-2 abb -41 f 0-89 d 2-bdf 3 ae 5 d 96 c 2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

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

Nell’esempio riportato sopra, il `Chapter 1`capitolo  ( 1) è l’identificatore del cue point ed è opzionale. L’indicatore temporale del cue point `00:00:000 --> 01:04:364` indica il minutaggio iniziale e finale del capitolo, in formato 00:00:000. Le ultime tre cifre rappresentano i millisecondi e, se preferite, possono essere lasciate a zero. The chapter title of `The bicycle store behind it all` is the actual description of the chapter’s contents. L’identificatore del cue point, il cue point iniziale e il titolo del capitolo vengono visualizzati in una finestra a comparsa del lettore video quando l’utente passa il puntatore del mouse sul riferimento visivo nella timeline del video.

Poiché state usando un visualizzatore video HTML5, è necessario verificare che il file dei capitoli creato segua lo standard WebVTT (Web Video Text Tracks). L’estensione dei file dei capitoli è .vtt. Per ulteriori informazioni sullo standard per sottotitoli WebVTT:

See [WebVTT: The Web Video Text Tracks format](https://dev.w3.org/html5/webvtt/).

**Per aggiungere marcatori capitolo a video**

1. Create il file video del capitolo usando un semplice editor di testo esterno a Scene7 Publishing System.

   >[!NOTE]
   >
   >per il supporto globale di capitoli a video in lingue diverse dall’inglese, tenete presente che lo standard WebVTT richiede che vengano creati file .vtt e chiamate separati per ogni lingua da supportare.

1. Salvate il file .vtt in codifica UTF8 per evitare problemi di rendering dei carattere nel titolo del capitolo.

   Generally, you want to name the chapter VTT file the same name as the video file, and append it with `chapters`. In questo modo risulta più semplice automatizzare la generazione degli URL video utilizzando un sistema di gestione dei contenuti Web.

1. In Scene7 Publishing System, caricate il file WebVTT dei capitoli.

   Consultate [Caricamento dei file](uploading-files.md#uploading_files).

1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video da associare al file dei capitoli che avete caricato.
1. Nel pannello delle risorse, selezionate una singola risorsa video, quindi, sotto la miniatura della risorsa, fate clic su **Anteprima** &gt; **Elenco visualizzatori**.
1. Nella tabella Elenco visualizzatori, individuate il visualizzatore HTML5 denominato **Univeral_HTML5_Video** ed effettuate una delle seguenti operazioni:

   * Per un’esperienza di visualizzazione con video a comparsa, fate clic su **Copia URL** all’estrema destra del nome.

      Aggiungete l’URL del video che avete copiato con la sintassi seguente per associarlo all’URL del l file dei sottotitoli:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Per un’esperienza di visualizzazione con video incorporato, fate clic su **Incorpora codice** all’estrema destra del nome.

      Nella finestra di dialogo Codice da incorporare, fate clic su **Copia negli Appunti**.

      For the HTML5 `Universal_HTML5_Video` viewer, append the copied embed code with the following:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`

