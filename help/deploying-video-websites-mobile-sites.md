---
title: Implementazione dei video nei siti Web e siti mobili
seo-title: Implementazione dei video nei siti Web e siti mobili
description: 'null'
seo-description: Scoprite come distribuire i video ai siti Web e ai siti mobili.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1689'
ht-degree: 69%

---


# Implementazione dei video nei siti Web e siti mobili{#deploying-video-to-your-websites-and-mobile-sites}

I siti Web, i siti mobili e le applicazioni desktop accedono al contenuto del server Dynamic Media Classic, inclusi i video, utilizzando stringhe URL o codice incorporato. Dynamic Media Classic attiva queste stringhe URL durante il processo di pubblicazione. Per inserire la stringa URL o il codice da incorporare per il video nelle pagine Web, nelle pagine mobili e nelle applicazioni desktop, copiatela da Dynamic Media Classic.

>[!NOTE]
>
>l’URL o il codice da incorporare diventa attivo solo dopo che la risorsa è stata pubblicata.

## Pubblicazione dei video {#publishing-video}

La pubblicazione di un video consente ai server Dynamic Media Classic di distribuire i video al sito Web, al sito mobile o all’applicazione.

Esistono due metodi diversi per pubblicare un video:

* **Pubblicare automaticamente i video in fase di caricamento**

   Come parte del processo di caricamento dei video, Dynamic Media Classic può pubblicare automaticamente i video quando vengono caricati e codificati. Grazie a questa possibilità di pubblicazione immediata, non è necessario pubblicare separatamente i video in un secondo tempo.

* **Pubblicare i video manualmente dopo il caricamento**

   Se non desiderate pubblicare subito i video, potete pubblicarli manualmente in qualsiasi momento.

Dopo aver pubblicato i video, Dynamic Media Classic attiva le stringhe URL per la pagina HTML o il codice dell’applicazione.

**Per pubblicare i video**

1. Effettuate una delle seguenti operazioni:

   * Per pubblicare automaticamente i video in fase di caricamento, nella schermata Carica fate clic su **Pubblica dopo il caricamento**. È tutto, non sono necessari ulteriori passaggi.
   * Per pubblicare i video manualmente in un secondo tempo dopo il caricamento, nel pannello Sfoglia selezionate i video e fate clic su **Pubblica** nella barra di navigazione globale.

## Collegamento di un URL per video a un sito mobile o a un sito Web {#linking-a-video-url-to-a-mobile-site-or-a-website}

Dopo aver pubblicato un video, potete ottenerne l’URL da usare in un sito Web, un sito mobile o in un’applicazione desktop. Usate l’URL del video per visualizzare il video in una finestra a comparsa o modale sopra alla pagina Web.

Quando un cliente fa clic sul collegamento, vengono automaticamente rilevati il tipo di dispositivo, la larghezza di banda e le dimensioni dello schermo. Viene visualizzato il video corretto da riprodurre con un visualizzatore predefinito per desktop o sul lettore nativo del dispositivo smartphone e tablet.

Consultate anche [Incorporamento di un visualizzatore video in una pagina Web](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Per collegare l’URL di un video a un sito mobile o a un sito Web**

1. Nel pannello delle risorse, nell’elenco a discesa Mostra, fate clic su **Video** o **Set video adattivo**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video o set di video adattivi che desiderate collegare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Fate clic su **Visualizzazione griglia** o **Visualizzazione elenco**. Nella finestra delle risorse, fate doppio clic sulla miniatura video di una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, nella sezione Streaming HTTP, fate clic su **Copia URL** a destra del visualizzatore desiderato. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.
   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, sotto la miniatura, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

   * Fate clic su **Visualizzazione elenco**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, a destra della miniatura, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

   * Fate clic su **Visualizzazione griglia**, **Visualizzazione elenco** o **Visualizzazione dettagli**. Nella stessa barra degli strumenti, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

1. Inserite il collegamento URL per il video HTML5 nel sito Web e nel sito mobile.

## Incorporamento di un visualizzatore video in una pagina Web {#embedding-the-video-viewer-on-a-web-page}

Per riprodurre il video incorporato nella pagina Web, utilizzate la funzione Incorpora codice. Puoi copiare il codice da incorporare negli Appunti, per poi incollarlo nelle pagine web. La modifica del codice non è consentita nella finestra di dialogo Incorpora codice.

Consultate anche [Collegamento di un URL per video a un sito mobile o a un sito Web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Per incorporare il visualizzatore video in una pagina Web**

1. Nel pannello delle risorse, nell’elenco a discesa Mostra, fate clic su **Video** o **Set video adattivo**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video o set video adattivo di cui desiderate copiare il codice da incorporare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Fate clic su **Visualizzazione griglia** o **Visualizzazione elenco**. Nella finestra delle risorse, fate doppio clic sulla miniatura video di una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, in Streaming HTTP, fate clic su **Incorpora codice** a destra del visualizzatore desiderato. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.
   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, sotto la miniatura video, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

   * Fate clic su **Visualizzazione elenco**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, a destra della miniatura, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

   * Fate clic su **Visualizzazione griglia**, **Visualizzazione elenco** o **Visualizzazione dettagli**. Nella stessa barra degli strumenti, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

1. Nella finestra di dialogo Codice da incorporare, fate clic su **Copia negli Appunti**.

   La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

1. Fai clic su **Chiudi**.
1. Incollate il codice da incorporare nelle pagine Web.

### Implementing embed code for using HTML5 video with MP4 video assets {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

If you do not use the Dynamic Media Classic HTML5 video player, but instead want to use the native HTML5 `<video>` tag with MP4 video assets, you can use the following embed code sample:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Replace `"S7 video thumbnail URL"` with the video’s thumbnail URL. Si tratta della miniatura del video che l’utente vede prima che venga riprodotto il video.

   Consultate [Reperimento degli URL delle miniature video](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Replace `"S7 OGG video asset URL (no player)"` with the video’s progressive URL for OGG video.

   Consultate [Collegamento di un URL per video a un sito mobile o a un sito Web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Sostituisci `"S7 MP4 mobile progressive video asset URL (no player)"` con l’URL progressivo mobile del video.

   Consultate [Collegamento di un URL per video a un sito mobile o a un sito Web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Implementazione di video mediante un lettore video di terze parti {#deploying-video-using-a-third-party-video-player}

Se utilizzate un lettore video di terze parti o personalizzato anziché un visualizzatore video Dynamic Media Classic, potete ottenere l’URL video diretto che funziona per lo streaming di video con bitrate multiplo HLS o per il download progressivo.

**Per implementare video mediante un lettore video di terze parti**

1. In Dynamic Media Classic, on the Global Navigation bar, click **Setup** > **Application Setup** > **General Settings**.
1. A seconda del tipo di URL che desiderate usare, effettuate una delle seguenti operazioni:
* Per generare un URL diretto per lo streaming video HLS (bitrate multiplo)

   Nella pagina Impostazioni **generali** applicazione, nel campo di testo Nome **server** pubblicato del gruppo **Server** , create l’URL diretto utilizzando la sintassi seguente: `server/is/content/company/folder/filename.m3u8`
Ad esempio, se il nome del server pubblicato `https://s7d9.scene7.com/.` utilizza la sintassi del passaggio 2, l’URL diretto potrebbe essere simile al seguente:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Per generare un URL diretto per lo streaming video HLS (bitrate singolo)

   On the **Application General Settings** page, in the **Servers** group, in the **HLS Streaming Server Name** text field, construct the direct URL using the following syntax:
   `server/company/folder/filename.ext.m3u8`
Ad esempio, se il nome del server di streaming HLS è `https://s7mbrstream.scene7.com/hls-vod/`. in base alla sintassi del punto 2 l’URL diretto potrebbe essere:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Per generare un URL diretto per video progressivo

   Nella pagina **Impostazioni generali applicazione**, nel campo di testo **Nome server video progressivo** che si trova nel gruppo **Server**, create l’URL diretto con la sintassi seguente: `server/company/folder/filename`
For example, suppose the progressive video server name is `https://s7d9.scene7.com/is/content/`. in base alla sintassi del punto 2 l’URL diretto potrebbe essere:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Utilizzo delle miniature video {#working-with-video-thumbnails}

Dynamic Media Classic genera le miniature per i video codificati e per i video precodificati. Potete usare le miniature video come qualsiasi altra risorsa di immagini. Inoltre, potete ottenere gli URL per le miniature video generate da Dynamic Media Classic e implementarli al di fuori di Dynamic Media Classic. Ad esempio, potete implementare le miniature nei risultati di ricerca, negli elenchi dei relativi video e negli elenchi di riproduzione video pubblicati in un sito Web.

Le miniature vengono generate in base al primo fotogramma eterogeneo (fotogramma che non sia tutto nero, tutto bianco e così via) del video.

### Reperimento degli URL delle miniature video {#obtaining-video-thumbnail-urls}

Dynamic Media Classic genera automaticamente le miniature video durante il processo di caricamento. Le miniature vengono visualizzate nel pannello Sfoglia in visualizzazione Elenco e Griglia.

Per generare gli URL delle miniature video, effettuate un’operazione di pubblicazione.

Consultate [Pubblicazione dei video](deploying-video-websites-mobile-sites.md#publishing_video).

Una volta effettuata la pubblicazione, potete reperire gli URL delle miniature video nella visualizzazione Dettagli del pannello URL e codice da incorporare. Fate clic su **Copia URL** a destra della miniatura del video miniatura per copiarne l’URL.

### Modifica dei fotogrammi poster nei visualizzatori video {#modifying-poster-frames-in-video-viewers}

Il *fotogramma poster* è il fotogramma iniziale che viene visualizzato nei visualizzatori per video prima che venga riprodotto il video. Dynamic Media Classic utilizza le miniature video come fotogrammi poster.

Potete applicare al fotogramma poster i modificatori di immagini. Ad esempio, potete ritagliare il fotogramma poster o renderlo trasparente. Per modificare il fotogramma poster, aprite la schermata di configurazione del visualizzatore per video e inserite i modificatori nella sezione Modificatori immagini poster. 

Consultate [Aggiunta o modifica di un predefinito per visualizzatori video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)

Consultate [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en).

Potete inoltre modificare le miniature video aggiungendo dei modificatori ai relativi URL.

>[!MORELIKETHIS]
>
>* [Pubblicazione di file ](publishing-files.md#publishing_files)

