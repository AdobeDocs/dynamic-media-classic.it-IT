---
title: Implementare i video nei siti Web e siti mobili
description: Scopri come distribuire video ai siti web e mobile da Adobe Dynamic Media Classic.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 35%

---

# Implementare i video nei siti Web e siti mobili{#deploying-video-to-your-websites-and-mobile-sites}

I siti web, i siti mobili e le applicazioni desktop accedono al contenuto del server Adobe Dynamic Media Classic, incluso il video, utilizzando stringhe URL o codice incorporato. Adobe Dynamic Media Classic attiva queste stringhe URL durante il processo di pubblicazione. Per inserire la stringa URL o il codice di incorporamento per il video nelle pagine web, nelle pagine mobili e nelle applicazioni desktop, copiala da Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL o il codice da incorporare diventa attivo solo dopo che la risorsa è stata pubblicata.

## Pubblicare i video {#publishing-video}

La pubblicazione di un video consente ad Adobe Dynamic Media Classic Server di distribuire video al sito web, al sito mobile o all’applicazione.

Esistono due metodi diversi per pubblicare un video:

* **Pubblicare automaticamente i video in fase di caricamento** - Come parte del processo di caricamento dei video, Adobe Dynamic Media Classic può pubblicare automaticamente i video quando vengono caricati e codificati. Grazie a questa possibilità di pubblicazione immediata, non è necessario pubblicare separatamente i video in un secondo tempo.

* **Pubblicare i video manualmente dopo il caricamento** - Se non desiderate pubblicare subito i video, potete pubblicarli manualmente in qualsiasi momento.

Dopo aver pubblicato i video, Adobe Dynamic Media Classic attiva le stringhe URL per la pagina HTML o il codice dell&#39;applicazione.

**Per pubblicare i video:**

1. Effettuate una delle seguenti operazioni:

   * Per pubblicare i video in modo automatico e istantaneo al momento del caricamento, nella pagina Carica , seleziona **[!UICONTROL Pubblica dopo il caricamento]**. È tutto, non sono necessari ulteriori passaggi.
   * Per pubblicare manualmente i video dopo il caricamento, nel pannello Sfoglia seleziona i video, quindi nella barra di navigazione globale seleziona **Pubblica**.

## Collegamento di un URL video a un sito mobile o a un sito web {#linking-a-video-url-to-a-mobile-site-or-a-website}

Dopo aver pubblicato un video, potete ottenerne l’URL da usare in un sito Web, un sito mobile o in un’applicazione desktop. Usate l’URL del video per visualizzare il video in una finestra a comparsa o modale sopra alla pagina Web.

Quando un cliente seleziona il collegamento, vengono rilevati automaticamente il dispositivo, la larghezza di banda e le dimensioni dello schermo. Viene visualizzato il video corretto da riprodurre con un visualizzatore predefinito per desktop o sul lettore nativo del dispositivo smartphone e tablet.

Consulta anche [Incorporare il visualizzatore video in una pagina web](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Per collegare l’URL di un video a un sito mobile o a un sito Web:**

1. Nel pannello Sfoglia risorse, nell’elenco a discesa **[!UICONTROL Mostra]** , seleziona **[!UICONTROL Video]** o **[!UICONTROL Set video adattivo]**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video o set di video adattivi che desiderate collegare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Vista griglia]** o **[!UICONTROL Vista a elenco]**. Nella finestra delle risorse, fate doppio clic sulla miniatura video di una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, in Streaming HTTP, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato. Come best practice, copia l’URL associato al visualizzatore `Universal_HTML5_Video` .
   * Selezionare **[!UICONTROL Vista griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi, sotto l’immagine miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Copia URL]**. Come best practice, copia l’URL associato al visualizzatore `Universal_HTML5_Video` .

   * Selezionare **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi, a destra della miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Copia URL]**. Come best practice, copia l’URL associato al visualizzatore `Universal_HTML5_Video` .

   * Selezionare **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]** o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Copia URL]**. Come best practice, copia l’URL associato al visualizzatore `Universal_HTML5_Video` .

1. Inserite il collegamento URL per il video HTML5 nel sito Web e nel sito mobile.

## Incorporare il visualizzatore video in una pagina web {#embedding-the-video-viewer-on-a-web-page}

Per riprodurre il video incorporato nella pagina Web, utilizzate la funzione Incorpora codice. Puoi copiare il codice da incorporare negli Appunti, per poi incollarlo nelle pagine web. La modifica del codice non è consentita nella finestra di dialogo Incorpora codice.

Consulta anche [Collegare un URL video a un sito mobile o a un sito web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Per incorporare il visualizzatore video in una pagina Web:**

1. Nel pannello Sfoglia risorse, nell’elenco a discesa Mostra , seleziona **[!UICONTROL Video]** o **[!UICONTROL Set video adattivo]**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il video o set video adattivo di cui desiderate copiare il codice da incorporare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Vista griglia]** o **[!UICONTROL Vista a elenco]**. Nella finestra delle risorse, fate doppio clic sulla miniatura video di una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, in Streaming HTTP, seleziona **[!UICONTROL Incorpora codice]** a destra del visualizzatore desiderato. Come best practice, seleziona **[!UICONTROL Incorpora codice]** associato al visualizzatore `Universal_HTML5_Video`.
   * Selezionare **[!UICONTROL Vista griglia]**. Nel pannello delle risorse, seleziona una singola risorsa, quindi, sotto l’immagine miniatura del video, seleziona **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**. Come best practice, seleziona **[!UICONTROL Incorpora codice]** associato al visualizzatore `Universal_HTML5_Video`.

   * Selezionare **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi, a destra della miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**. Come best practice, seleziona **[!UICONTROL Incorpora codice]** associato al visualizzatore `Universal_HTML5_Video`.

   * Selezionare **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]** o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**. Come best practice, seleziona **[!UICONTROL Incorpora codice]** associato al visualizzatore `Universal_HTML5_Video`.

1. Nella finestra di dialogo Incorpora codice selezionare **[!UICONTROL Copia negli Appunti]**.

   La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

1. selezionare **[!UICONTROL Chiudi]**.
1. Incollate il codice da incorporare nelle pagine Web.

### Implementare il codice di incorporamento per utilizzare video HTML5 con risorse video MP4 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Se non utilizzi il lettore video HTML5 Adobe Classic Dynamic Media Classic, ma desideri utilizzare il tag nativo HTML5 `<video>` con risorse video MP4, puoi utilizzare il seguente esempio di codice da incorporare:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Sostituisci `"S7 video thumbnail URL"` con l’URL della miniatura del video, che è l’immagine miniatura del video che un utente vede prima di riprodurre il video.

   Consulta [Ottenere gli URL delle miniature video](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Sostituisci `"S7 OGG video asset URL (no player)"` con l’URL progressivo del video per OGG.

   Consulta [Collegare un URL video a un sito mobile o a un sito web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Sostituisci `"S7 MP4 mobile progressive video asset URL (no player)"` con l’URL progressivo mobile del video.

   Consulta [Collegare un URL video a un sito mobile o a un sito web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Distribuzione di video tramite un lettore video di terze parti {#deploying-video-using-a-third-party-video-player}

Se utilizzi un lettore video di terze parti o un lettore video personalizzato invece di un visualizzatore video Dynamic Media Classic, ottieni l’URL video diretto che funziona per lo streaming video a più bit HLS o per il download progressivo.

**Per implementare video mediante un lettore video di terze parti:**

1. In Adobe Dynamic Media Classic, nella barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali]**.
1. A seconda del tipo di URL che desiderate usare, effettuate una delle seguenti operazioni:

* Per generare un URL video in streaming HLS diretto (con bitrate multiplo)

   Nella pagina **[!UICONTROL Impostazioni generali dell&#39;applicazione]**, nel gruppo **[!UICONTROL Server]**, nel campo di testo **[!UICONTROL Nome server pubblicato]**, crea l&#39;URL diretto. Utilizza la sintassi seguente: `server/is/content/company/folder/filename.m3u8`

   Ad esempio, supponiamo che il nome del server pubblicato sia `https://s7d9.scene7.com/.` Utilizzando la sintassi nel passaggio 2, l&#39;URL diretto potrebbe avere il seguente aspetto:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Per generare un URL video in streaming HLS diretto (a bit rate singolo)

   Nella pagina **[!UICONTROL Impostazioni generali dell&#39;applicazione]**, nel gruppo **[!UICONTROL Server]**, nel campo di testo **[!UICONTROL Nome server di streaming HLS]**, crea l&#39;URL diretto utilizzando la seguente sintassi:

   `server/company/folder/filename.ext.m3u8`

   Ad esempio, supponiamo che il nome del server di streaming HLS sia `https://s7mbrstream.scene7.com/hls-vod/`. Utilizzando la sintassi nel passaggio 2, l’URL diretto potrebbe avere il seguente aspetto:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Per generare un URL diretto per video progressivo

   Nella pagina **[!UICONTROL Impostazioni generali applicazione]**, nel campo di testo **[!UICONTROL Nome server video progressivo]** che si trova nel gruppo **[!UICONTROL Server]**, create l’URL diretto con la sintassi seguente:

   `server/company/folder/filename`

   Ad esempio, supponiamo che il nome del server video progressivo sia `https://s7d9.scene7.com/is/content/`. Utilizzando la sintassi nel passaggio 2, l’URL diretto potrebbe avere il seguente aspetto:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Utilizzare le miniature video {#working-with-video-thumbnails}

Adobe Dynamic Media Classic genera miniature per video codificati e video precodificati. Potete usare le miniature video come qualsiasi altra risorsa di immagini. Inoltre, puoi ottenere gli URL per le miniature video generate da Adobe Dynamic Media Classic e distribuirli al di fuori di Adobe Dynamic Media Classic. Ad esempio, potete implementare le miniature nei risultati di ricerca, negli elenchi dei relativi video e negli elenchi di riproduzione video pubblicati in un sito Web.

Le miniature vengono generate in base al primo fotogramma eterogeneo (fotogramma che non sia tutto nero, tutto bianco e così via) del video.

### Ottenere gli URL delle miniature video {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic genera automaticamente le miniature video durante il processo di caricamento. Le miniature vengono visualizzate nel pannello Sfoglia in Vista a elenco e Vista a griglia.

Per generare gli URL delle miniature video, effettuate un’operazione di pubblicazione.

Consulta [Pubblicare video](deploying-video-websites-mobile-sites.md#publishing_video).

Una volta effettuata la pubblicazione, potete reperire gli URL delle miniature video nella visualizzazione Dettagli del pannello URL e codice da incorporare. Seleziona **[!UICONTROL Copia URL]** a destra della miniatura del video in modo da poter copiare il relativo URL.

### Modificare i fotogrammi poster nei visualizzatori video {#modifying-poster-frames-in-video-viewers}

Il *fotogramma poster* è il fotogramma iniziale che viene visualizzato nei visualizzatori per video prima che venga riprodotto il video. Adobe Dynamic Media Classic utilizza le miniature video come fotogrammi poster.

Potete applicare al fotogramma poster i modificatori di immagini. Ad esempio, potete ritagliare il fotogramma poster o renderlo trasparente. Per modificare il fotogramma poster, aprite la schermata di configurazione del visualizzatore per video e inserite i modificatori nella sezione Modificatori immagini poster. 

Consulta [Aggiungere o modificare un predefinito visualizzatore video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulta [Guida all&#39;Image Serving](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

Potete inoltre modificare le miniature video aggiungendo dei modificatori ai relativi URL.

>[!MORELIKETHIS]
>
>* [Pubblicare i file](publishing-files.md#publishing_files)