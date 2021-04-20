---
title: Implementazione dei video nei siti Web e siti mobili
description: Scopri come distribuire i video ai siti web e mobili.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1687'
ht-degree: 68%

---


# Implementazione dei video nei siti Web e siti mobili{#deploying-video-to-your-websites-and-mobile-sites}

I siti web, i siti mobili e le applicazioni desktop accedono al contenuto del server Dynamic Media Classic, incluso il video, utilizzando stringhe URL o codice incorporato. Dynamic Media Classic attiva queste stringhe URL durante il processo di pubblicazione. Per inserire la stringa URL o il codice di incorporamento per il video nelle pagine web, nelle pagine mobili e nelle applicazioni desktop, copiala da Dynamic Media Classic.

>[!NOTE]
>
>l’URL o il codice da incorporare diventa attivo solo dopo che la risorsa è stata pubblicata.

## Pubblicazione dei video  {#publishing-video}

La pubblicazione di un video consente ai server Dynamic Media Classic di distribuire video al sito web, al sito mobile o all’applicazione.

Esistono due metodi diversi per pubblicare un video:

* **Pubblicare automaticamente i video in fase di caricamento**

   Come parte del processo di caricamento dei video, Dynamic Media Classic può pubblicare automaticamente i video quando vengono caricati e codificati. Grazie a questa possibilità di pubblicazione immediata, non è necessario pubblicare separatamente i video in un secondo tempo.

* **Pubblicare i video manualmente dopo il caricamento**

   Se non desiderate pubblicare subito i video, potete pubblicarli manualmente in qualsiasi momento.

Dopo la pubblicazione dei video, Dynamic Media Classic attiva le stringhe URL per la pagina HTML o il codice dell&#39;applicazione.

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

   * Fate clic su **Visualizzazione griglia** o **Visualizzazione elenco**. Nella finestra delle risorse, fate doppio clic sulla miniatura video di una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, nella sezione Streaming HTTP, fate clic su **Copia URL** a destra del visualizzatore desiderato. Come best practice, copia l’URL associato al visualizzatore `Universal_HTML5_Video` .
   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, sotto la miniatura, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**. Come best practice, copia l’URL associato al visualizzatore `Universal_HTML5_Video` .

   * Fate clic su **Visualizzazione elenco**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, a destra della miniatura, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**. Come best practice, copia l’URL associato al visualizzatore `Universal_HTML5_Video` .

   * Fate clic su **Visualizzazione griglia**, **Visualizzazione elenco** o **Visualizzazione dettagli**. Nella stessa barra degli strumenti, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**. Come best practice, copia l’URL associato al visualizzatore `Universal_HTML5_Video` .

1. Inserite il collegamento URL per il video HTML5 nel sito Web e nel sito mobile.

## Incorporamento di un visualizzatore video in una pagina Web  {#embedding-the-video-viewer-on-a-web-page}

Per riprodurre il video incorporato nella pagina Web, utilizzate la funzione Incorpora codice. Puoi copiare il codice da incorporare negli Appunti, per poi incollarlo nelle pagine web. La modifica del codice non è consentita nella finestra di dialogo Incorpora codice.

Consultate anche [Collegamento di un URL per video a un sito mobile o a un sito Web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Per incorporare il visualizzatore video in una pagina Web**

1. Nel pannello delle risorse, nell’elenco a discesa Mostra, fate clic su **Video** o **Set video adattivo**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video o set video adattivo di cui desiderate copiare il codice da incorporare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Fate clic su **Visualizzazione griglia** o **Visualizzazione elenco**. Nella finestra delle risorse, fate doppio clic sulla miniatura video di una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, in Streaming HTTP, fate clic su **Incorpora codice** a destra del visualizzatore desiderato. Come best practice, fai clic su **Incorpora codice** associato al visualizzatore `Universal_HTML5_Video`.
   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, sotto la miniatura video, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**. Come best practice, fai clic su **Incorpora codice** associato al visualizzatore `Universal_HTML5_Video`.

   * Fate clic su **Visualizzazione elenco**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, a destra della miniatura, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**. Come best practice, fai clic su **Incorpora codice** associato al visualizzatore `Universal_HTML5_Video`.

   * Fate clic su **Visualizzazione griglia**, **Visualizzazione elenco** o **Visualizzazione dettagli**. Nella stessa barra degli strumenti, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**. Come best practice, fai clic su **Incorpora codice** associato al visualizzatore `Universal_HTML5_Video`.

1. Nella finestra di dialogo Codice da incorporare, fate clic su **Copia negli Appunti**.

   La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

1. Fai clic su **Chiudi**.
1. Incollate il codice da incorporare nelle pagine Web.

### Implementazione del codice di incorporamento per utilizzare video HTML5 con risorse video MP4 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Se non utilizzi il lettore video HTML5 di Dynamic Media Classic, ma desideri utilizzare il tag nativo HTML5 `<video>` con risorse video MP4, puoi utilizzare il seguente esempio di codice da incorporare:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Sostituisci `"S7 video thumbnail URL"` con l’URL della miniatura del video. Si tratta della miniatura del video che l’utente vede prima che venga riprodotto il video.

   Consultate [Reperimento degli URL delle miniature video](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Sostituisci `"S7 OGG video asset URL (no player)"` con l’URL progressivo del video per OGG.

   Consultate [Collegamento di un URL per video a un sito mobile o a un sito Web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Sostituisci `"S7 MP4 mobile progressive video asset URL (no player)"` con l’URL progressivo mobile del video.

   Consultate [Collegamento di un URL per video a un sito mobile o a un sito Web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Implementazione di video mediante un lettore video di terze parti  {#deploying-video-using-a-third-party-video-player}

Se utilizzi un lettore video di terze parti o un lettore video personalizzato anziché un visualizzatore video Dynamic Media Classic, puoi ottenere l’URL video diretto che funziona per lo streaming video a più bit o il download progressivo HLS.

**Per implementare video mediante un lettore video di terze parti**

1. In Dynamic Media Classic, nella barra di navigazione globale, fate clic su **Configurazione** > **Impostazione applicazione** > **Impostazioni generali**.
1. A seconda del tipo di URL che desiderate usare, effettuate una delle seguenti operazioni:
* Per generare un URL video in streaming HLS diretto (con bitrate multiplo)

   Nella pagina **Impostazioni generali dell&#39;applicazione**, nel gruppo **Server**, nel campo di testo **Nome server pubblicato**, crea l&#39;URL diretto utilizzando la seguente sintassi: `server/is/content/company/folder/filename.m3u8`
Ad esempio, supponiamo che il nome del server pubblicato sia `https://s7d9.scene7.com/.` Utilizzando la sintassi nel passaggio 2, l’URL diretto potrebbe avere il seguente aspetto:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Per generare un URL video in streaming HLS diretto (a bit rate singolo)

   Nella pagina **Impostazioni generali dell&#39;applicazione**, nel gruppo **Server**, nel campo di testo **Nome server di streaming HLS**, crea l&#39;URL diretto utilizzando la seguente sintassi:
   `server/company/folder/filename.ext.m3u8`
Ad esempio, supponiamo che il nome del server di streaming HLS sia  `https://s7mbrstream.scene7.com/hls-vod/`. in base alla sintassi del punto 2 l’URL diretto potrebbe essere:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Per generare un URL diretto per video progressivo

   Nella pagina **Impostazioni generali applicazione**, nel campo di testo **Nome server video progressivo** che si trova nel gruppo **Server**, create l’URL diretto con la sintassi seguente:  `server/company/folder/filename`
Ad esempio, supponiamo che il nome del server video progressivo sia  `https://s7d9.scene7.com/is/content/`. in base alla sintassi del punto 2 l’URL diretto potrebbe essere:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Utilizzo delle miniature video {#working-with-video-thumbnails}

Dynamic Media Classic genera miniature per video codificati e video precodificati. Potete usare le miniature video come qualsiasi altra risorsa di immagini. Inoltre, puoi ottenere gli URL per le miniature video generate da Dynamic Media Classic e distribuirli al di fuori di Dynamic Media Classic. Ad esempio, potete implementare le miniature nei risultati di ricerca, negli elenchi dei relativi video e negli elenchi di riproduzione video pubblicati in un sito Web.

Le miniature vengono generate in base al primo fotogramma eterogeneo (fotogramma che non sia tutto nero, tutto bianco e così via) del video.

### Reperimento degli URL delle miniature video {#obtaining-video-thumbnail-urls}

Dynamic Media Classic genera automaticamente le miniature video durante il processo di caricamento. Le miniature vengono visualizzate nel pannello Sfoglia in visualizzazione Elenco e Griglia.

Per generare gli URL delle miniature video, effettuate un’operazione di pubblicazione.

Consultate [Pubblicazione dei video](deploying-video-websites-mobile-sites.md#publishing_video).

Una volta effettuata la pubblicazione, potete reperire gli URL delle miniature video nella visualizzazione Dettagli del pannello URL e codice da incorporare. Fate clic su **Copia URL** a destra della miniatura del video miniatura per copiarne l’URL.

### Modifica dei fotogrammi poster nei visualizzatori video  {#modifying-poster-frames-in-video-viewers}

Il *fotogramma poster* è il fotogramma iniziale che viene visualizzato nei visualizzatori per video prima che venga riprodotto il video. Dynamic Media Classic utilizza le miniature video come fotogrammi poster.

Potete applicare al fotogramma poster i modificatori di immagini. Ad esempio, potete ritagliare il fotogramma poster o renderlo trasparente. Per modificare il fotogramma poster, aprite la schermata di configurazione del visualizzatore per video e inserite i modificatori nella sezione Modificatori immagini poster. 

Consultate [Aggiunta o modifica di un predefinito per visualizzatori video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)

Vedere [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en).

Potete inoltre modificare le miniature video aggiungendo dei modificatori ai relativi URL.

>[!MORELIKETHIS]
>
>* [Pubblicazione di file ](publishing-files.md#publishing_files)

