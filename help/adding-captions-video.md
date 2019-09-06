---
title: Aggiunta di sottotitoli a video
seo-title: Aggiunta di sottotitoli a video
description: 'null'
seo-description: Scopri come aggiungere sottotitoli a video
uuid: 4 cc 64469-4369-44 a 9-83 db -63 bad 51 aba 8 a
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Aggiunta di sottotitoli a video{#adding-captions-to-video}

Per ampliare il pubblico potenziale dei vostri video nel mercato globale, potete aggiungere sottotitoli a singoli video o a set di video adattivi. Aggiungendo i sottotitoli, potete evitare di dover doppiare l’audio in ogni lingua diversa. Il video viene riprodotto nella lingua in cui è stato registrato e in sovraimpressione compaiono i sottotitoli in lingua straniera, che permettono alle persone di altri paesi di comprendere comunque la porzione audio.

I sottotitoli, in particolare i sottotitoli per non udenti, garantiscono inoltre una maggiore accessibilità per le persone con problemi di udito.

>[!NOTE]
>
>il lettore video utilizzato deve supportare la visualizzazione delle didascalie.

Consultate [Aggiunta o modifica di un predefinito per visualizzatori video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) per configurare l’Effetto didascalia e per modificare il Menu didascalia, compreso il testo di menu per i seguenti visualizzatori.

* `Universal_HTML5_Video` visualizzatore.
* `Universal_HTML5_MixedMedia_dark` visualizzatore.
* `Universal_HTML5_MixedMedia_light` visualizzatore.

Consultate anche [Aggiunta e modifica dei predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets).

Dynamic Media Classic è in grado di convertire i file di sottotitoli in formato JSON (javascript Object Notation). Questa conversione significa che è possibile includere testo JSON in una pagina Web come trascrizione nascosta ma completa del video. I motori di ricerca possono quindi individuare e indicizzare tale contenuto per consentire agli utenti di trovare più facilmente i video e ottenere dettagli sul contenuto degli stessi.

See [Serving static (non-image) contents](https://marketing.adobe.com/resources/help/en_US/s7/is_ir_api/is_api/c_serving_static_nonimage_contents.html) in the *Adobe Image Serving API Help* for more information about using the JSON function in a URL.

**Per aggiungere sottotitoli a un video**

1. Utilizzando un’applicazione di terze parti esterna a Scene7 Publishing System, create il file di sottotitoli video basato sul tipo di visualizzatore in uso.

   | Tipo visualizzatore | File di sottotitoli |
   |--- |--- |
   | HTML5 | Se usate un visualizzatore video HTML5, assicuratevi che il file dei sottotitoli che create segua lo standard WebVTT (Web Video Text Tracks). L’estensione dei file di sottotitoli è .vtt. Per ulteriori informazioni sullo standard per sottotitoli WebVTT:<br><br>[Consultate webvtt](https://dev.w3.org/html5/webvtt/): Formato Tracce video Web. <br><br>Esistono strumenti e servizi gratuiti e a pagamento che potete utilizzare per creare file di sottotitoli all’esterno di Scene7 Publishing System. Ad esempio, per creare un semplice file di sottotitoli video senza alcuno stile, potete usare il seguente strumento online gratuito per la creazione e modifica di sottotitoli: <br><br>[Webvtt Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Per risultati ottimali, usate lo strumento in Internet Explorer 9 o versione successiva, Google Chrome o Safari. <br><br>In questo strumento, nel campo <b>Enter URL of video file</b> (Inserire l’URL del file video), incollate l’URL del file video e fate clic su <b>Load</b> (Carica). <br><br>Ad esempio, se usate un URL Dynamic Media Classic per il file video, in SPS fate doppio clic su una singola risorsa video (non un set video adattivo o un video principale) per aprirla in visualizzazione Dettagli. Nel pannello a destra della vista Dettagli, espandete URL e codice da incorporare. Quindi nel gruppo Mobile, a destra di Mobile (progressivo), fate clic su Copia URL. This process gives you the URL to the video file itself which you can then paste into the <b>Enter URL of video file</b> field. Internet Explorer, Chrome o Safari possono quindi riprodurre il video in modo nativo. Seguite ora le istruzioni visualizzate dal sito per creare e salvare il file WebVTT. Al termine, copiate il contenuto del file dei sottotitoli, incollatelo in un editor di solo testo e salvatelo con l’estensione .vtt. <br><br><b>Nota:</b> Per il supporto globale di sottotitoli video in lingue diverse dall'inglese, tenete presente che lo standard webvtt richiede che vengano creati file. vtt e chiamate separati per ogni lingua da supportare. <br><br>In genere, è consigliabile assegnare al file VTT dei sottotitoli lo stesso nome del file video, aggiungendo il suffisso captions. In questo modo risulta più semplice automatizzare la generazione degli URL video utilizzando un sistema di gestione dei contenuti Web. |

1. In Scene7 Publishing System, caricare il file di sottotitoli WebVTT, DFXP o SMPTE XML.

   Consultate [Caricamento dei file](uploading-files.md#uploading_files).

1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video da associare al file di sottotitoli che avete caricato.
1. Nel pannello delle risorse, selezionate una singola risorsa video, quindi, sotto la miniatura della risorsa, fate clic su **Anteprima** &gt; **Elenco visualizzatori**.
1. In the Viewer List table, find the HTML5 viewer named **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark**, or **Universal_HTML5_MixedMedia_light**, then do one of the following:

   * Per un’esperienza di visualizzazione con video a comparsa, fate clic su **Copia URL** all’estrema destra del nome.

      Aggiungete l’URL del video che avete copiato con la sintassi seguente per associarlo all’URL del l file dei sottotitoli:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Note the `,1` at the end of the caption URL path. Subito dopo l’estensione .vtt nel percorso, potete attivare o disattivare il pulsante dei sottotitoli nella barra del lettore video impostando rispettivamente `1` o `0`.

   * Per un’esperienza di visualizzazione con video incorporato, fate clic su **Incorpora codice** all’estrema destra del nome.

      Nella finestra di dialogo Codice da incorporare, fate clic su **Copia negli Appunti**.

      For the HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, or `Universal_HTML5_MixedMedia_light` viewers, append the copied embed code with the following:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Note the `,1` at the end of the URL path. Subito dopo l’estensione .vtt nel percorso dell’URL, potete attivare o disattivare il pulsante dei sottotitoli nella barra del lettore video impostando rispettivamente `1` o `0`.

