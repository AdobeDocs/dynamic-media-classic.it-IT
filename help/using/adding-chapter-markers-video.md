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
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 22%

---

# Aggiungere marcatori capitolo al video {#adding-chapter-markers-to-video}

Per semplificare la visualizzazione e la navigazione dei video lunghi, aggiungi marcatori capitolo ai singoli video o ai set di video adattivi. Quando un utente riproduce il video, può selezionare i contrassegni dei capitoli sulla timeline del video (noti anche come scorrimento video). In questo modo è possibile spostarsi facilmente nel punto di interesse o passare immediatamente a nuovi contenuti, dimostrazioni, tutorial e così via.

>[!NOTE]
>
>Il lettore video deve supportare l’uso dei contrassegni dei capitoli.

Per configurare i cue point di navigazione del capitolo e il testo a comparsa del titolo del capitolo per il visualizzatore [&#x200B; (HTML5), consulta &#x200B;](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)Aggiungere o modificare un predefinito per visualizzatore video`Universal_HTML5_Video`.

Vedi anche [Aggiungere e modificare i predefiniti visualizzatore](application-setup.md#adding_and_editing_viewer_presets).

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

Nell&#39;esempio precedente, `Chapter 1` è l&#39;identificatore del cue ed è facoltativo. Il cue time di `00:00:000 --> 01:04:364` specifica l&#39;ora di inizio e l&#39;ora di fine del capitolo, nel formato 00:00:000. Le ultime tre cifre rappresentano i millisecondi e, se preferite, possono essere lasciate a zero. Il titolo del capitolo di `The bicycle store behind it all` è la descrizione effettiva del contenuto del capitolo. L&#39;identificatore del cue, l&#39;ora di inizio del cue e il titolo del capitolo vengono visualizzati in un pop-up nel lettore video quando il puntatore viene posizionato su un punto di cue visivo nella timeline del video.

Poiché state usando un visualizzatore video HTML5, è necessario verificare che il file dei capitoli creato segua lo standard WebVTT (Web Video Text Tracks). L&#39;estensione del nome file del capitolo è `.VTT`. Per ulteriori informazioni sullo standard per sottotitoli WebVTT:

Vedere [WebVTT: formato dei brani di testo per video Web](https://w3c.github.io/webvtt/).

**Per aggiungere marcatori capitolo a un video:**

1. Utilizzando un semplice editor di testo esterno a Adobe Dynamic Media Classic, create il file del capitolo video.

   >[!NOTE]
   >
   >Per il supporto globale dei capitoli video in lingue diverse dall&#39;inglese, lo standard WebVTT richiede la creazione di `.VTT` file e chiamate separati per ogni lingua che si desidera supportare.

1. Salvare il file VTT con codifica UTF8 in modo da evitare problemi con la rappresentazione dei caratteri nel testo del titolo del capitolo.

   In genere, si desidera assegnare al file VTT del capitolo lo stesso nome del file video e aggiungerlo con `chapters`. In questo modo, è possibile automatizzare la generazione degli URL video utilizzando il sistema di gestione dei contenuti web esistente.

1. In Adobe Dynamic Media Classic, carica il file del capitolo WebVTT.

   Vedi [Carica file](uploading-files.md#uploading_files).

1. Nel pannello Libreria risorse, a sinistra, individua la cartella delle risorse contenente il file video da associare al file del capitolo caricato.
1. Nel pannello Sfoglia risorse, seleziona una singola risorsa video, quindi seleziona **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]** sotto l&#39;immagine di anteprima della risorsa.
1. Nella tabella Elenco visualizzatori, individuate il visualizzatore HTML5 denominato **Univeral_HTML5_Video** ed effettuate una delle seguenti operazioni:

   * Per visualizzare un video popup, seleziona **[!UICONTROL Copia URL]** all&#39;estrema destra del nome.

     Aggiungi l’URL copiato del video con la seguente sintassi, in modo da poterlo associare all’URL copiato nel file di didascalia:

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Per un&#39;esperienza di visualizzazione video incorporata, seleziona **[!UICONTROL Incorpora codice]** all&#39;estrema destra del nome.

     Nella finestra di dialogo Incorpora codice, seleziona **[!UICONTROL Copia negli Appunti]**.

     Per il visualizzatore HTML5 `Universal_HTML5_Video`, aggiungi il codice di incorporamento copiato con quanto segue:

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
