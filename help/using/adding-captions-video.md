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
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 32%

---

# Aggiungi didascalie al video {#adding-captions-to-video}

Per ampliare il pubblico potenziale dei vostri video nel mercato globale, potete aggiungere sottotitoli a singoli video o a set di video adattivi. Aggiungendo i sottotitoli, potete evitare di dover doppiare l’audio in ogni lingua diversa. Il video viene riprodotto nella lingua in cui è stato registrato e in sovraimpressione compaiono i sottotitoli in lingua straniera, che permettono alle persone di altri paesi di comprendere comunque la porzione audio.

I sottotitoli, in particolare i sottotitoli per non udenti, garantiscono inoltre una maggiore accessibilità per le persone con problemi di udito.

>[!NOTE]
>
>il lettore video utilizzato deve supportare la visualizzazione delle didascalie.

Per configurare l&#39;effetto Didascalia e modificare il menu Didascalia stesso, incluso il testo del menu per uno dei seguenti visualizzatori:

* `Universal_HTML5_Video` visualizzatore
* `Universal_HTML5_MixedMedia_dark` visualizzatore
* `Universal_HTML5_MixedMedia_light` visualizzatore

Consulta [Aggiungere o modificare un predefinito visualizzatore video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Vedi anche [Aggiungere e modificare i predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic può convertire i file di didascalia in formato JSON (JavaScript Object Notation). Questa conversione significa che è possibile includere testo JSON in una pagina Web come trascrizione nascosta ma completa del video. I motori di ricerca possono quindi eseguire la ricerca per indicizzazione e indicizzare il contenuto per rendere i video più facilmente individuabili e fornire ai clienti maggiori dettagli sul contenuto video.

Consulta [Distribuisci contenuti statici (non immagine)](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) nel *Guida API di Image Server di Adobe* per ulteriori informazioni sull’utilizzo della funzione JSON in un URL.

**Per aggiungere sottotitoli a un video:**

1. Utilizzando un’applicazione di terze parti esterna a Adobe Dynamic Media Classic, crea il file di sottotitoli video in base al tipo di visualizzatore in uso.

   | Tipo visualizzatore | File di sottotitoli |
   |--- |--- |
   | HTML5 | Se usate un visualizzatore video HTML5, assicuratevi che il file dei sottotitoli che create segua lo standard WebVTT (Web Video Text Tracks). L’estensione dei file di sottotitoli è .vtt. Per ulteriori informazioni sullo standard per sottotitoli WebVTT:<br><br>[Vedi WebVTT](https://w3c.github.io/webvtt/): formato dei brani di testo per video web. <br><br>Esistono strumenti e servizi gratuiti e a pagamento che puoi utilizzare per creare file di didascalia al di fuori di Adobe Dynamic Media Classic. Ad esempio, per creare un file di sottotitoli video semplice senza stile, potete utilizzare il seguente strumento di creazione e modifica di sottotitoli online gratuito: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Per ottenere risultati ottimali, utilizza lo strumento in Internet Explorer 9 o versioni successive, Google Chrome o Safari. <br><br>Nello strumento, nella sezione <b>Inserisci l’URL del file video</b> , incollare l&#39;URL del file video e quindi selezionare <b>Carica</b>. <br><br>Ad esempio, se per il file video utilizzi un URL Adobe Dynamic Media Classic, fai doppio clic su una singola risorsa video (non un set video adattivo o un video principale) per aprirla in Vista dettagli. Nel pannello a destra della vista Dettagli, espandete URL e codice da incorporare. Quindi, nel gruppo Mobile, a destra di Mobile (Progressive), seleziona <b>Copia URL</b>. Questo processo ti fornisce l’URL del file video stesso che puoi incollare nel <b>Inserisci l’URL del file video</b> campo. Internet Explorer, Chrome o Safari possono quindi riprodurre il video in modo nativo. Seguite ora le istruzioni visualizzate dal sito per creare e salvare il file WebVTT. Al termine, copiate il contenuto del file di didascalia e incollatelo in un editor di testo normale e salvatelo con un&#39;estensione VTT. <br><br><b>Nota:</b> Per il supporto globale dei sottotitoli video in lingue diverse dall&#39;inglese, lo standard WebVTT richiede la creazione di file .vtt e chiamate separati per ogni lingua che si desidera supportare. <br><br>In genere, è consigliabile assegnare al file VTT dei sottotitoli lo stesso nome del file video, aggiungendo il suffisso captions. In questo modo risulta più semplice automatizzare la generazione degli URL video utilizzando un sistema di gestione dei contenuti Web. |

1. In Adobe Dynamic Media Classic, carica il file di didascalia XML WebVTT, DFXP o SMPTE.

   Consulta [Carica file](uploading-files.md#uploading_files).

1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video da associare al file di sottotitoli che avete caricato.
1. Nel pannello Sfoglia risorse, seleziona una singola risorsa video, quindi sotto l’immagine di miniatura della risorsa seleziona **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
1. Nella tabella Elenco visualizzatori, individua il visualizzatore HTML5 denominato **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark**, o **Universal_HTML5_MixedMedia_light**, quindi eseguire una delle operazioni seguenti:

   * Per visualizzare un video a comparsa, seleziona **[!UICONTROL Copia URL]** all&#39;estrema destra del nome.

     Aggiungi l’URL copiato del video con la seguente sintassi, in modo da poterlo associare all’URL copiato nel file di didascalia:

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Osserva `,1` alla fine del percorso URL della didascalia. Subito dopo l’estensione del nome file VTT nel percorso, puoi facoltativamente abilitare o disabilitare il pulsante dei sottotitoli codificati nella barra del lettore video impostando su `1` o `0`, rispettivamente.

   * Per un’esperienza di visualizzazione video incorporata, seleziona **[!UICONTROL Codice di incorporamento]** all&#39;estrema destra del nome.

     Nella finestra di dialogo Incorpora codice, seleziona **[!UICONTROL Copia negli Appunti]**.

     Per il HTML 5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, o `Universal_HTML5_MixedMedia_light` visualizzatori, aggiungi il codice da incorporare copiato con quanto segue:

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Osserva `,1` alla fine del percorso URL. Immediatamente dopo l’estensione del nome file VTT nel percorso URL, puoi facoltativamente abilitare o disabilitare il pulsante della didascalia sulla barra del lettore video impostando su `1` o `0`, rispettivamente.
