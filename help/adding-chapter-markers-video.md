---
title: Aggiungere marcatori capitolo al video
description: Scopri come aggiungere marcatori capitolo a un video in Dynamic Media Classic.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Visualizzatori,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 39%

---

# Aggiungere marcatori capitolo al video {#adding-chapter-markers-to-video}

Potete rendere più semplice la visualizzazione e la navigazione nei video di formato esteso aggiungendo marcatori capitolo a singoli video o a set video adattivi. Quando un utente riproduce il video, può selezionare i marcatori capitolo nella timeline del video (nota anche come scorrimento video). In questo modo è possibile spostarsi facilmente nel punto di interesse o passare immediatamente a nuovi contenuti, dimostrazioni, tutorial e così via.

>[!NOTE]
>
>il lettore video utilizzato deve supportare l’uso di marcatori capitolo.

Per configurare i punti di cue per la navigazione dei capitoli e il testo a comparsa del titolo del capitolo per il visualizzatore `Universal_HTML5_Video` (HTML5), consultate [Aggiungere o modificare un predefinito visualizzatore video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) .

Consulta anche [Aggiungere e modificare i predefiniti visualizzatore](application-setup.md#adding_and_editing_viewer_presets).

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

Nell’esempio riportato sopra, il `Chapter 1`capitolo  ( 1) è l’identificatore del cue point ed è opzionale. Il tempo di cue di `00:00:000 --> 01:04:364` specifica l&#39;ora di inizio e di fine del capitolo, in formato 00:00:000. Le ultime tre cifre rappresentano i millisecondi e, se preferite, possono essere lasciate a zero. Il titolo del capitolo di `The bicycle store behind it all` è la descrizione effettiva del contenuto del capitolo. L’identificatore di cue, il tempo di cue iniziale e il titolo del capitolo vengono visualizzati in un pop-up nel lettore video quando il puntatore passa sopra un punto di cue visivo nella timeline del video.

Poiché state usando un visualizzatore video HTML5, è necessario verificare che il file dei capitoli creato segua lo standard WebVTT (Web Video Text Tracks). L&#39;estensione del nome del capitolo è .VTT. Per ulteriori informazioni sullo standard per sottotitoli WebVTT:

Consultare [WebVTT: Il Testo Video Web Tiene Traccia Del Formato](https://w3c.github.io/webvtt/).

**Per aggiungere marcatori capitolo a video:**

1. Utilizzando un semplice editor di testo esterno a Dynamic Media Classic, crea il file dei capitoli video.

   >[!NOTE]
   >
   >Per il supporto globale dei capitoli video in lingue diverse dall&#39;inglese, lo standard WebVTT richiede la creazione di file .vtt separati e di chiamate per ogni lingua che si desidera supportare.

1. Salva il file VTT nella codifica UTF8 in modo da evitare problemi con il rendering dei caratteri nel testo del titolo del capitolo.

   In genere, si desidera assegnare al file VTT capitolo lo stesso nome del file video e aggiungerlo con `chapters`. In questo modo risulta più semplice automatizzare la generazione degli URL video utilizzando un sistema di gestione dei contenuti Web.

1. In Dynamic Media Classic, carica il file del capitolo WebVTT.

   Consulta [Caricare file](uploading-files.md#uploading_files).

1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video da associare al file dei capitoli che avete caricato.
1. Nel pannello delle risorse, seleziona una singola risorsa video, quindi, sotto l’immagine miniatura della risorsa, seleziona **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
1. Nella tabella Elenco visualizzatori, individuate il visualizzatore HTML5 denominato **Univeral_HTML5_Video** ed effettuate una delle seguenti operazioni:

   * Per un’esperienza di visualizzazione video a comparsa, seleziona **[!UICONTROL Copia URL]** all’estrema destra del nome.

      Aggiungi l’URL del video copiato con la sintassi seguente, in modo da poterlo associare all’URL copiato al file della didascalia:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Per un’esperienza di visualizzazione video incorporata, seleziona **[!UICONTROL Incorpora codice]** all’estrema destra del nome.

      Nella finestra di dialogo Incorpora codice selezionare **[!UICONTROL Copia negli Appunti]**.

      Per il visualizzatore HTML5 `Universal_HTML5_Video` , aggiungi il codice da incorporare copiato con quanto segue:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
