---
title: Aggiungi didascalie al video
description: Scopri come aggiungere sottotitoli ai video in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 17%

---

# Aggiungi didascalie al video {#add-captions-to-video}

Estendi la portata dei tuoi video ai mercati globali. A tale scopo, puoi aggiungere i sottotitoli a singoli video o set di video adattivi. Aggiungendo i sottotitoli, potete evitare di dover doppiare l’audio in ogni lingua diversa. Il video viene riprodotto nella lingua in cui è stato registrato e in sovraimpressione compaiono i sottotitoli in lingua straniera, che permettono alle persone di altri paesi di comprendere comunque la porzione audio.

I sottotitoli, in particolare i sottotitoli per non udenti, garantiscono inoltre una maggiore accessibilità per le persone con problemi di udito.

>[!NOTE]
>
>il lettore video utilizzato deve supportare la visualizzazione delle didascalie.

Per configurare l&#39;effetto Didascalia e modificare il menu Didascalia stesso, incluso il testo del menu per uno dei seguenti visualizzatori:

* `Universal_HTML5_Video` visualizzatore
* `Universal_HTML5_MixedMedia_dark` visualizzatore
* `Universal_HTML5_MixedMedia_light` visualizzatore

Consulta [Aggiungere o modificare un predefinito per visualizzatori video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Vedi anche [Aggiungere e modificare i predefiniti visualizzatore](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic può convertire i file di didascalia in formato JSON (JavaScript Object Notation). Questa conversione ti consente di incorporare il testo JSON in una pagina web come trascrizione nascosta ma completa del video. I motori di ricerca possono quindi eseguire la ricerca per indicizzazione e indicizzare il contenuto per rendere i video più facilmente individuabili e fornire ai clienti maggiori dettagli sul contenuto video.

Per ulteriori informazioni sull&#39;utilizzo della funzione JSON in un URL, vedere [Server static (non-image) contents](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) in.

**Per aggiungere didascalie a un video:**

1. Utilizzando un’applicazione di terze parti esterna a Adobe Dynamic Media Classic, crea il file di sottotitoli video in base al tipo di visualizzatore in uso.

   | Tipo visualizzatore | File di sottotitoli |
   |--- |--- |
   | HTML5 | Se usate un visualizzatore video HTML5, assicuratevi che il file dei sottotitoli che create segua lo standard WebVTT (Web Video Text Tracks). L&#39;estensione del nome file dei sottotitoli è `.VTT`. Per ulteriori informazioni sullo standard per sottotitoli WebVTT:<br><br>[Vedere WebVTT](https://w3c.github.io/webvtt/): formato dei brani di testo per video Web. <br><br>Esistono molti siti Web che offrono strumenti e servizi gratuiti e a pagamento che è possibile utilizzare per creare file di sottotitoli WebVTT. <br><br>Seguire le istruzioni visualizzate da un sito per creare e salvare il file WebVTT. Al termine, copiate il contenuto del file di didascalia e incollatelo in un editor di testo normale e salvatelo con un&#39;estensione VTT. <br><br><b>Nota:</b> per il supporto globale dei sottotitoli video in lingue diverse dall&#39;inglese, lo standard WebVTT richiede la creazione di `.VTT` file e chiamate separati per ogni lingua che si desidera supportare. <br><br>In genere, si desidera assegnare al file VTT della didascalia lo stesso nome del file video e aggiungerlo ai sottotitoli. In questo modo, è possibile automatizzare la generazione degli URL video utilizzando il sistema di gestione dei contenuti web esistente. |

1. In Adobe Dynamic Media Classic, carica il file di didascalia XML WebVTT, DFXP o SMPTE.

   Vedi [Carica file](uploading-files.md#uploading_files).

1. Nel pannello Libreria risorse, a sinistra, individua la cartella di risorse contenente il file video da associare al file di didascalia caricato.
1. Nel pannello Sfoglia risorse, seleziona una singola risorsa video, quindi seleziona **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]** sotto l&#39;immagine di anteprima della risorsa.
1. Nella tabella Elenco visualizzatori trovare il visualizzatore HTML5 denominato **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** o **Universal_HTML5_MixedMedia_light**, quindi eseguire una delle operazioni seguenti:

   * Per visualizzare un video popup, seleziona **[!UICONTROL Copia URL]** all&#39;estrema destra del nome.

     Aggiungi l’URL copiato del video con la seguente sintassi, in modo da poterlo associare all’URL copiato nel file di didascalia:

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Nota `,1` alla fine del percorso dell&#39;URL della didascalia. Subito dopo l&#39;estensione del nome file VTT nel percorso, è possibile abilitare o disabilitare il pulsante dei sottotitoli codificati sulla barra del lettore video impostando rispettivamente su `1` o `0`.

   * Per un&#39;esperienza di visualizzazione video incorporata, seleziona **[!UICONTROL Incorpora codice]** all&#39;estrema destra del nome.

     Nella finestra di dialogo Incorpora codice, seleziona **[!UICONTROL Copia negli Appunti]**.

     Per i visualizzatori HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark` o `Universal_HTML5_MixedMedia_light`, aggiungi il codice di incorporamento copiato con quanto segue:

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Nota `,1` alla fine del percorso URL. Immediatamente dopo l&#39;estensione del nome file VTT nel percorso URL, è possibile abilitare o disabilitare il pulsante della didascalia sulla barra del lettore video impostando rispettivamente su `1` o `0`.
