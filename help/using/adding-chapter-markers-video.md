---
title: Aggiungere marcatori capitolo al video
description: Scopri come aggiungere marcatori capitolo a un video in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 24%

---

# Aggiungere marcatori capitolo al video {#adding-chapter-markers-to-video}

Per semplificare la visualizzazione e la navigazione dei video lunghi, aggiungi marcatori capitolo ai singoli video o ai set di video adattivi. Quando un utente riproduce il video, può selezionare i contrassegni dei capitoli sulla timeline del video (noti anche come scorrimento video). In questo modo è possibile spostarsi facilmente nel punto di interesse o passare immediatamente a nuovi contenuti, dimostrazioni, tutorial e così via.

>[!NOTE]
>
>il lettore video utilizzato deve supportare l’uso di marcatori capitolo.

Consulta [Aggiungere o modificare un predefinito per visualizzatori video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) per configurare i cue point di navigazione del capitolo e il testo a comparsa del titolo del capitolo per `Universal_HTML5_Video` visualizzatore (HTML5).

Vedi anche [Aggiungere e modificare i predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets).

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

Nell’esempio precedente, `Chapter 1` è l’identificatore del cue ed è facoltativo. Il tempo di cue di `00:00:000 --> 01:04:364` specifica l&#39;ora di inizio e di fine del capitolo, in 00:00:formato 000. Le ultime tre cifre rappresentano i millisecondi e, se preferite, possono essere lasciate a zero. Titolo del capitolo di `The bicycle store behind it all` è la descrizione effettiva del contenuto del capitolo. L&#39;identificatore del cue, l&#39;ora di inizio del cue e il titolo del capitolo vengono visualizzati in un pop-up nel lettore video quando il puntatore viene posizionato su un punto di cue visivo nella timeline del video.

Poiché state usando un visualizzatore video HTML5, è necessario verificare che il file dei capitoli creato segua lo standard WebVTT (Web Video Text Tracks). L’estensione del nome file del capitolo è `.VTT`. Per ulteriori informazioni sullo standard per sottotitoli WebVTT:

Consulta [WebVTT: formato per tracce di testo video Web](https://w3c.github.io/webvtt/).

**Per aggiungere marcatori capitolo a un video:**

1. Utilizzando un semplice editor di testo esterno a Adobe Dynamic Media Classic, create il file del capitolo video.

   >[!NOTE]
   >
   >Per il supporto globale dei capitoli video in lingue diverse dall’inglese, lo standard WebVTT richiede la creazione di `.VTT` file e chiamate per ogni lingua da supportare.

1. Salvare il file VTT con codifica UTF8 in modo da evitare problemi con la rappresentazione dei caratteri nel testo del titolo del capitolo.

   In genere, si desidera assegnare al file VTT del capitolo lo stesso nome del file video e aggiungerlo con `chapters`. In questo modo, è possibile automatizzare la generazione degli URL video utilizzando il sistema di gestione dei contenuti web esistente.

1. In Adobe Dynamic Media Classic, carica il file del capitolo WebVTT.

   Consulta [Carica file](uploading-files.md#uploading_files).

1. Nel pannello Libreria risorse, a sinistra, individua la cartella delle risorse contenente il file video da associare al file del capitolo caricato.
1. Nel pannello Sfoglia risorse, seleziona una singola risorsa video, quindi sotto l’immagine di miniatura della risorsa seleziona **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
1. Nella tabella Elenco visualizzatori, individuate il visualizzatore HTML5 denominato **Univeral_HTML5_Video** ed effettuate una delle seguenti operazioni:

   * Per visualizzare un video a comparsa, seleziona **[!UICONTROL Copia URL]** all&#39;estrema destra del nome.

     Aggiungi l’URL copiato del video con la seguente sintassi, in modo da poterlo associare all’URL copiato nel file di didascalia:

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Per un’esperienza di visualizzazione video incorporata, seleziona **[!UICONTROL Codice di incorporamento]** all&#39;estrema destra del nome.

     Nella finestra di dialogo Incorpora codice, seleziona **[!UICONTROL Copia negli Appunti]**.

     Per il HTML 5 `Universal_HTML5_Video` visualizzatore, aggiungi al codice da incorporare copiato quanto segue:

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
