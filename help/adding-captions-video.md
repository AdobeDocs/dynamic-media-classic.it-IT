---
title: Aggiunta di sottotitoli a video
description: Scopri come aggiungere sottotitoli al video
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Visualizzatori,Video
role: Business Practitioner
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: 210c501f56f97b7fab08b71c263be1c03d3d0fac
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 50%

---

# Aggiunta di sottotitoli a video{#adding-captions-to-video}

Per ampliare il pubblico potenziale dei vostri video nel mercato globale, potete aggiungere sottotitoli a singoli video o a set di video adattivi. Aggiungendo i sottotitoli, potete evitare di dover doppiare l’audio in ogni lingua diversa. Il video viene riprodotto nella lingua in cui è stato registrato e in sovraimpressione compaiono i sottotitoli in lingua straniera, che permettono alle persone di altri paesi di comprendere comunque la porzione audio.

I sottotitoli, in particolare i sottotitoli per non udenti, garantiscono inoltre una maggiore accessibilità per le persone con problemi di udito.

>[!NOTE]
>
>il lettore video utilizzato deve supportare la visualizzazione delle didascalie.

Per configurare l’effetto didascalia e modificare il menu della didascalia, incluso il testo del menu per uno dei seguenti visualizzatori:

* `Universal_HTML5_Video` visualizzatore
* `Universal_HTML5_MixedMedia_dark` visualizzatore
* `Universal_HTML5_MixedMedia_light` visualizzatore

consulta [Aggiunta o modifica di un predefinito visualizzatore video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consultate anche [Aggiunta e modifica dei predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets).

Dynamic Media Classic può convertire i file di didascalie in formato JSON (JavaScript™ Object Notation). Questa conversione significa che è possibile includere testo JSON in una pagina Web come trascrizione nascosta ma completa del video. I motori di ricerca possono quindi eseguire ricerche per indicizzazione e indicizzazione del contenuto per rendere i video più facilmente individuabili e fornire ai clienti ulteriori dettagli sul contenuto video.

Per ulteriori informazioni sull’utilizzo della funzione JSON in un URL, consulta [Serving static (non-image) content](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) in Guida API di Adobe Image Serving *.*

**Per aggiungere sottotitoli a un video**

1. Utilizzando un’applicazione di terze parti esterna a Dynamic Media Classic, crea il file dei sottotitoli video in base al tipo di visualizzatore in uso.

   | Tipo visualizzatore | File di sottotitoli |
   |--- |--- |
   | HTML5 | Se usate un visualizzatore video HTML5, assicuratevi che il file dei sottotitoli che create segua lo standard WebVTT (Web Video Text Tracks). L’estensione dei file di sottotitoli è .vtt. Per ulteriori informazioni sullo standard per sottotitoli WebVTT:<br><br>[Consultare WebVTT](https://w3c.github.io/webvtt/): Il formato Tracce testo video web. <br><br>Sono disponibili strumenti e servizi gratuiti e a pagamento che è possibile utilizzare per creare file di sottotitoli all’esterno di Dynamic Media Classic. Ad esempio, per creare un semplice file di sottotitoli video senza stili, è possibile utilizzare il seguente strumento online gratuito per la creazione e modifica di sottotitoli: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Per risultati ottimali, utilizzare lo strumento in Internet Explorer 9 o versioni successive, Google Chrome o Safari. <br><br>In questo strumento, nel campo <b>Enter URL of video file</b> (Inserire l’URL del file video), incollate l’URL del file video e fate clic su <b>Load</b> (Carica). <br><br>Ad esempio, se utilizzi un URL Dynamic Media Classic per il file video, fai doppio clic su una singola risorsa video (non un set video adattivo o un video master) per aprirla in visualizzazione Dettagli. Nel pannello a destra della vista Dettagli, espandete URL e codice da incorporare. Quindi nel gruppo Mobile, a destra di Mobile (progressivo), fate clic su Copia URL. Questo processo ti dà l&#39;URL del file video stesso che puoi quindi incollare nel campo <b>Enter URL of video file</b> (Inserisci URL del file video). A quel punto, Internet Explorer, Chrome o Safari possono riprodurre il video in modalità nativa. Seguite ora le istruzioni visualizzate dal sito per creare e salvare il file WebVTT. Al termine, copiate il contenuto del file dei sottotitoli, incollatelo in un editor di solo testo e salvatelo con l’estensione .vtt. <br><br><b>Nota:</b> per il supporto globale dei sottotitoli video in lingue diverse dall&#39;inglese, lo standard WebVTT richiede la creazione di file .vtt separati e di chiamate per ogni lingua che si desidera supportare. <br><br>In genere, è consigliabile assegnare al file VTT dei sottotitoli lo stesso nome del file video, aggiungendo il suffisso captions. In questo modo risulta più semplice automatizzare la generazione degli URL video utilizzando un sistema di gestione dei contenuti Web. |

1. In Dynamic Media Classic, carica il file di sottotitoli XML WebVTT, DFXP o SMPTE.

   Consultate [Caricamento dei file](uploading-files.md#uploading_files).

1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video da associare al file di sottotitoli che avete caricato.
1. Nel pannello delle risorse, selezionate una singola risorsa video, quindi, sotto la miniatura della risorsa, fate clic su **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
1. Nella tabella Elenco visualizzatori, individua il visualizzatore HTML5 denominato **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** o **Universal_HTML5_MixedMedia_light**, quindi effettua una delle seguenti operazioni:

   * Per un’esperienza di visualizzazione con video a comparsa, fate clic su **[!UICONTROL Copia URL]** all’estrema destra del nome.

      Aggiungete l’URL del video che avete copiato con la sintassi seguente per associarlo all’URL del l file dei sottotitoli:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Osserva `,1` alla fine del percorso URL della didascalia. Immediatamente dopo l’estensione .vtt nel percorso, è possibile abilitare o disabilitare il pulsante closed caption sulla barra del lettore video impostando rispettivamente `1` o `0`.

   * Per un’esperienza di visualizzazione con video incorporato, fate clic su **[!UICONTROL Incorpora codice]** all’estrema destra del nome.

      Nella finestra di dialogo Codice da incorporare, fate clic su **[!UICONTROL Copia negli Appunti]**.

      Per i visualizzatori HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark` o `Universal_HTML5_MixedMedia_light` , aggiungi il codice di incorporamento copiato con quanto segue:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Osserva il percorso `,1` alla fine del percorso URL. Subito dopo l’estensione .vtt nel percorso URL, puoi facoltativamente abilitare o disabilitare il pulsante della didascalia sulla barra del lettore video impostando rispettivamente `1` o `0`.
