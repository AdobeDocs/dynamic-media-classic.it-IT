---
title: Implementare i video nei siti Web e siti mobili
description: Scopri come distribuire i video da Adobe Dynamic Media Classic ai siti web e mobili.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
topic: Content Management
level: Intermediate
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '1702'
ht-degree: 30%

---

# Implementare i video nei siti Web e siti mobili{#deploying-video-to-your-websites-and-mobile-sites}

I siti Web, i siti mobili e le applicazioni desktop accedono ai contenuti del server Adobe Dynamic Media Classic, incluso il video, utilizzando stringhe URL o codice incorporato. Adobe Dynamic Media Classic attiva queste stringhe URL durante il processo di pubblicazione. Per inserire la stringa URL o il codice da incorporare per il video nelle pagine web, nelle pagine mobili e nelle applicazioni desktop, copialo da Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL o il codice da incorporare diventa attivo solo dopo che la risorsa è stata pubblicata.

## Pubblicare i video {#publishing-video}

La pubblicazione di un video consente ai server Adobe Dynamic Media Classic di distribuire video al sito Web, al sito mobile o all&#39;applicazione.

Esistono due metodi diversi per pubblicare il video:

* **Pubblica i video automaticamente e immediatamente al caricamento** - Come parte del processo di caricamento dei video, Adobe Dynamic Media Classic può pubblicare automaticamente i video caricati e codificati. Grazie a questa possibilità di pubblicazione immediata, non è necessario pubblicare separatamente i video in un secondo tempo.

* **Pubblica video manualmente dopo il caricamento** - Se non desideri pubblicare subito i video, puoi pubblicarli manualmente in qualsiasi momento.

Dopo la pubblicazione dei video, Adobe Dynamic Media Classic attiva le stringhe URL per la pagina HTML o il codice dell’applicazione.

**Per pubblicare un video:**

1. Effettuate una delle seguenti operazioni:

   * Per pubblicare i video automaticamente e immediatamente al momento del caricamento, nella pagina Carica seleziona **[!UICONTROL Pubblica dopo il caricamento]**. È tutto, non sono necessari ulteriori passaggi.
   * Per pubblicare i video manualmente dopo il caricamento, seleziona i video nel pannello Sfoglia e quindi nella barra di navigazione globale seleziona **Pubblica**.

## Collegare l’URL di un video a un sito mobile o a un sito web {#linking-a-video-url-to-a-mobile-site-or-a-website}

Quando pubblichi un video, puoi ottenere l’URL associato da utilizzare nel sito web, nel sito mobile o nell’applicazione desktop. Usate l’URL del video per visualizzare il video in una finestra a comparsa o modale sopra alla pagina Web.

Quando un cliente seleziona il collegamento, il dispositivo, la larghezza di banda e le dimensioni dello schermo vengono rilevati automaticamente. Viene visualizzato il video corretto da riprodurre con un visualizzatore predefinito per desktop o sul lettore nativo del dispositivo smartphone e tablet.

Vedi anche [Incorporare il visualizzatore video in una pagina web](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Per collegare un URL video a un sito mobile o a un sito web:**

1. Nel pannello Sfoglia risorse, nella **[!UICONTROL Spettacolo]** elenco a discesa, seleziona **[!UICONTROL Video]**, o **[!UICONTROL Set video adattivo]**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video o set di video adattivi che desiderate collegare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Vista griglia]** o **[!UICONTROL Vista a elenco]**. Nella finestra delle risorse, fate doppio clic sulla miniatura video di una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e Codice di incorporamento a destra, in Streaming HTTP, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato. Come best practice, copia l’URL associato al `Universal_HTML5_Video` visualizzatore.
   * Seleziona **[!UICONTROL Vista griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi sotto l’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Copia URL]**. Come best practice, copia l’URL associato al `Universal_HTML5_Video` visualizzatore.

   * Seleziona **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Copia URL]**. Come best practice, copia l’URL associato al `Universal_HTML5_Video` visualizzatore.

   * Seleziona **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]**, o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Copia URL]**. Come best practice, copia l’URL associato al `Universal_HTML5_Video` visualizzatore.

1. Inserite il collegamento URL per il video HTML5 nel sito Web e nel sito mobile.

## Incorporare il visualizzatore video in una pagina web {#embedding-the-video-viewer-on-a-web-page}

Per riprodurre il video incorporato nella pagina Web, utilizzate la funzione Incorpora codice. Potete copiare il codice da incorporare negli Appunti per poi incollarlo nelle pagine Web. La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

Vedi anche [Collegare l’URL di un video a un sito mobile o a un sito web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Per incorporare il visualizzatore video in una pagina web:**

1. Nel pannello Sfoglia risorse, nell’elenco a discesa Mostra, seleziona **[!UICONTROL Video]**, o **[!UICONTROL Set video adattivo]**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video o set video adattivo di cui desiderate copiare il codice da incorporare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Vista griglia]** o **[!UICONTROL Vista a elenco]**. Nella finestra delle risorse, fate doppio clic sulla miniatura video di una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e Codice di incorporamento a destra, in Streaming HTTP, seleziona **[!UICONTROL Codice di incorporamento]** a destra del visualizzatore desiderato. Come best practice, seleziona **[!UICONTROL Codice di incorporamento]** associato al `Universal_HTML5_Video` visualizzatore.
   * Seleziona **[!UICONTROL Vista griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi sotto l’immagine della miniatura video seleziona **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**. Come best practice, seleziona **[!UICONTROL Codice di incorporamento]** associato al `Universal_HTML5_Video` visualizzatore.

   * Seleziona **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**. Come best practice, seleziona **[!UICONTROL Codice di incorporamento]** associato al `Universal_HTML5_Video` visualizzatore.

   * Seleziona **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]**, o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**. Come best practice, seleziona **[!UICONTROL Codice di incorporamento]** associato al `Universal_HTML5_Video` visualizzatore.

1. Nella finestra di dialogo Incorpora codice, seleziona **[!UICONTROL Copia negli Appunti]**.

   La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

1. seleziona **[!UICONTROL Chiudi]**.
1. Incollate il codice da incorporare nelle pagine Web.

### Implementare il codice di incorporamento per utilizzare video HTML5 con risorse video MP4 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Se non utilizzi il lettore video Adobe Dynamic Media Classic HTML5, ma desideri invece utilizzare il HTML nativo `<video>` con i tag delle risorse video MP4, puoi utilizzare il seguente codice di incorporamento di esempio:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Sostituisci `"S7 video thumbnail URL"` con l’URL della miniatura del video, che è l’immagine della miniatura del video che un utente vede prima di riprodurre il video.

  Consulta [Ottenere gli URL delle miniature video](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Sostituisci `"S7 OGG video asset URL (no player)"` con l’URL progressivo del video per il video OGG.

  Consulta [Collegare l’URL di un video a un sito mobile o a un sito web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Sostituisci `"S7 MP4 mobile progressive video asset URL (no player)"` con l’URL progressivo mobile del video.

  Consulta [Collegare l’URL di un video a un sito mobile o a un sito web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Distribuire video utilizzando un lettore video di terze parti {#deploying-video-using-a-third-party-video-player}

Se utilizzi un lettore video di terze parti o un lettore video personalizzato invece di un visualizzatore video Dynamic Media Classic, ottieni l’URL del video diretto che funziona per lo streaming video con bitrate multiplo HLS o il download progressivo.

**Per distribuire un video utilizzando un lettore video di terze parti:**

1. In Adobe Dynamic Media Classic, nella barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali]**.
1. A seconda del tipo di URL che desiderate usare, effettuate una delle seguenti operazioni:

* Per generare un URL video streaming HLS diretto (multibitrate)

  Il giorno **[!UICONTROL Impostazioni generali applicazione]** pagina, nella **[!UICONTROL Server]** gruppo, nel **[!UICONTROL Nome server pubblicato]** campo di testo, crea l’URL diretto. Utilizza la seguente sintassi: `server/is/content/company/folder/filename.m3u8`

  Si supponga ad esempio che il nome del server Pubblicato sia `https://s7d9.scene7.com/.` Utilizzando la sintassi del passaggio 2, l’URL diretto potrebbe avere un aspetto simile al seguente:
  `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Per generare un URL video streaming HLS diretto (velocità bit singola)

  Il giorno **[!UICONTROL Impostazioni generali applicazione]** pagina, nella **[!UICONTROL Server]** gruppo, nel **[!UICONTROL Nome server di streaming HLS]** campo di testo, crea l’URL diretto utilizzando la seguente sintassi:

  `server/company/folder/filename.ext.m3u8`

  Si supponga ad esempio che il nome del server di streaming HLS sia `https://s7mbrstream.scene7.com/hls-vod/`. Utilizzando la sintassi del passaggio 2, l’URL diretto potrebbe avere un aspetto simile al seguente:
  `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Per generare un URL diretto per video progressivo

  Nella pagina **[!UICONTROL Impostazioni generali applicazione]**, nel campo di testo **[!UICONTROL Nome server video progressivo]** che si trova nel gruppo **[!UICONTROL Server]**, create l’URL diretto con la sintassi seguente:

  `server/company/folder/filename`

  Si supponga, ad esempio, che il nome del server video progressivo sia `https://s7d9.scene7.com/is/content/`. Utilizzando la sintassi del passaggio 2, l’URL diretto potrebbe avere un aspetto simile al seguente:
  `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Operazioni con le miniature video {#working-with-video-thumbnails}

Adobe Dynamic Media Classic genera miniature per video codificati e video precodificati. Potete usare le miniature video come qualsiasi altra risorsa di immagini. Inoltre, puoi ottenere gli URL per le miniature dei video generate da Adobe Dynamic Media Classic. Puoi quindi distribuire questi URL al di fuori di Adobe Dynamic Media Classic. Ad esempio, potete implementare le miniature nei risultati di ricerca, negli elenchi dei relativi video e negli elenchi di riproduzione video pubblicati in un sito Web.

Le miniature vengono generate in base al primo fotogramma eterogeneo (fotogramma che non sia tutto nero, tutto bianco e così via) del video.

### Ottenere gli URL delle miniature video {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic genera automaticamente le miniature video durante il processo di caricamento. Le miniature vengono visualizzate nel pannello Sfoglia in Vista a elenco e Vista griglia.

Per generare gli URL delle miniature video, effettuate un’operazione di pubblicazione.

Consulta [Pubblica video](deploying-video-websites-mobile-sites.md#publishing_video).

Una volta effettuata la pubblicazione, potete reperire gli URL delle miniature video nella visualizzazione Dettagli del pannello URL e codice da incorporare. Seleziona **[!UICONTROL Copia URL]** sulla destra della miniatura del video, in modo da poterne copiare l’URL associato.

### Modificare i fotogrammi poster nei visualizzatori video {#modifying-poster-frames-in-video-viewers}

Il *fotogramma poster* è il fotogramma iniziale che viene visualizzato nei visualizzatori per video prima che venga riprodotto il video. Adobe Dynamic Media Classic utilizza le miniature video come fotogrammi poster.

Potete applicare al fotogramma poster i modificatori di immagini. Ad esempio, potete ritagliare il fotogramma poster o renderlo trasparente. Per modificare il fotogramma poster, aprite la schermata di configurazione del visualizzatore per video e inserite i modificatori nella sezione Modificatori immagini poster. 

Consulta [Aggiungere o modificare un predefinito visualizzatore video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulta [Guida a Image Server](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home#image-serving-api).

Potete inoltre modificare le miniature video aggiungendo dei modificatori ai relativi URL.

>[!MORELIKETHIS]
>
>* [Pubblicare i file](publishing-files.md#publishing_files)