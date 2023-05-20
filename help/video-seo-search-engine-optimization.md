---
title: SEO (Search Engine Optimization) per i video
description: Scopri come configurare le impostazioni Video SEO (Search Engine Optimization) in Adobe Dynamic Media Classic.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 37%

---

# SEO (Search Engine Optimization) per i video{#video-seo-search-engine-optimization}

L’ottimizzazione SEO (Search Engine Optimization, ottimizzazione per i motori di ricerca) consente di migliorare il volume di traffico verso un sito Web generato dai motori di ricerca. I motori di ricerca possono raccogliere informazioni sui contenuti testuali, ma non dai video a meno che le informazioni necessarie per le ricerche non siano appositamente specificate.

Utilizzando Adobe Systems Dynamic Media Video SEO classico, è possibile applicare video metadati per fornire ai motori ricerca descrizioni dei video. Adobe Systems Dynamic Media Classic offre la possibilità di creare Video Sitemap e feed mRSS. Questi file XML standard vengono utilizzati per inviare informazioni video ai motori ricerca:

* **Video Sitemap** -informa Google esattamente dove e cosa è il contenuti video su un sito. Così, i video sono completamente ricercabili su Google. In un Video Sitemap è possibile specificare ad esempio la durata e le categorie dei video. Per informazioni sulle mappe del sito video, consulta [Video sitemap e video sitemap alternative](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **Feed mRSS (Media Really Simple Syndication)** : utilizzato dagli editori di contenuti per inserire file multimediali in Yahoo. Video Search. Per informazioni sui feed mRSS, vedere [Video sitemap e video sitemap alternative](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google supporta sia Video Sitemap che il protocollo di feed mRSS per la trasmissione di informazioni ai motori di ricerca.

Adobe Dynamic Media Classic può generare Video Sitemap e feed mRSS dai metadati memorizzati con ogni video. Quando create dei Video Sitemap e feed mRSS, potete scegliere quali campi di metadati includere tra quelli presenti nei file video. Questo vi permette di descrivere i video per i motori di ricerca, che saranno quindi in grado di proporre con più precisione, tra i risultati di ricerca, i video presenti nel vostro sito Web.

>[!NOTE]
>
>prima di creare un Video Sitemap o feed mRSS, verificate quali campi occorre includere nel file XML e come devono essere strutturati, in base ai requisiti del motore di ricerca. Per creare un Video Sitemap o un feed mRSS di successo, questo deve soddisfare i requisiti del motore di ricerca.

Adobe Systems Dynamic Media Classic crea rapporti su Video Sitemaps e feed mRSS dopo averli generati. Questi rapporti sono disponibili nella pagina Video rapporto SEO.

>[!NOTE]
>
>Per le Sitemap Video e i feed mRSS, Adobe Systems Dynamic Media classiche acquisisce metadati solo da video contrassegnati per pubblicare. Contrassegnate i video per la pubblicazione per includerne i metadati nei Video Sitemap e nei feed mRSS.

## Scegli impostazioni video SEO {#choosing-video-seo-settings}

Seleziona Video impostazioni SEO per i video Sitemap e feed mRSS sulla pagina Video Search Ottimizzazione del **[!UICONTROL motore impostazioni]** . Per aprire questa pagina, nella barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Impostazioni]**.

In **[!UICONTROL Impostazione generale]** , scegliere se generare Video Sitemap, feed mRSS o entrambi. In **[!UICONTROL Impostazioni di generazione]** area, mappa i campi di metadati con i campi di input.

Dopo aver scelto le impostazioni, seleziona **[!UICONTROL Salva]** (o **[!UICONTROL Salva e genera]**) per creare Video Sitemap, feed mRSS o entrambi.

### Configurare le impostazioni generali {#choosing-general-settings}

Nell&#39; **[!UICONTROL elenco a discesa modalità]** generazione, scegliete una modalità di rapporto:

* **Video Sitemap** -Crea una Sitemap per video.

* **Feed** mRSS-crea un feed di RSS multimediale (mRSS).

* **Both** -Crea entrambi i tipi di file XML.

* **Disattiva** la generazione di video i feed Sitemap e media RSS (mRSS), scegli questa opzione.

Nell&#39; **[!UICONTROL elenco a discesa modalità]** automatica/manuale, scegli se generare automaticamente o manualmente:

* **Modalità** automatica-Adobe Systems Dynamic Media Classic genera automaticamente una Sitemap video, media RSS (mRSS) feed, o entrambi, ogni giorno. Seleziona la **[!UICONTROL Contrassegna per pubblicazione]** opzione per contrassegnare automaticamente per la pubblicazione il file XML generato da Adobe Dynamic Media Classic.

   * **Contrassegna per pubblicazione** Contrassegna per la pubblicazione del file XML generato.

* **Modalità manuale** - Adobe Dynamic Media Classic genera Video Sitemap, Media RSS (mRSS) feed, o entrambi, quando si seleziona **[!UICONTROL Genera]** o **[!UICONTROL Salva e genera]** nella schermata Impostazioni ottimizzazione ricerca video. Selezionate inoltre le seguenti opzioni:

   * **Nessuna ulteriore impostazione** - Non contrassegna per la pubblicazione il file XML generato.

   * **Contrassegna per Publish** -Marks per pubblicare il file XML generato.

   * **Consenti generazione** parziale-i motori Search possono rifiutare un file XML se non contiene informazioni complete metadati per tutti i video. Questa opzione genera il file XML lineare se metadati non è disponibile per alcuni video. Nella schermata Rapporto compare un’avvertenza. Selezionate questa opzione se intendete esportare il file XML ed elaborare manualmente le informazioni mancanti.

### Scelta delle impostazioni di generazione {#choosing-generation-settings}

L&#39;area generazione Impostazioni elenca i campi di input per la Video Sitemap, o mRSS feed, o entrambi, e nel pannello metadati, i nomi dei campi di metadati. Servitevi dell’area Impostazioni generazione per associare i campi di input ai relativi campi di metadati. In questo modo, l&#39;utente indica a Adobe Dynamic Media Classic dove ottenere i metadati per Video Sitemap e/o il feed mRSS.

1. Nel menu Visualizzazioni metadati, scegliete una visualizzazione per i metadati. I nomi dei campi di metadati compaiono quindi nel pannello Metadati.
Consultate [Visualizzazione metadati](application-setup.md#metadata_views).
1. Trascinate i nomi dei campi di metadati dal pannello Metadati ai campi di input Pagina di arrivo, Titolo, Descrizione, Tag e Categoria. I campi Pagina di arrivo, Titolo e Descrizione sono obbligatori.

   >[!NOTE]
   >
   >potete anche inserire manualmente i dati nei campi di input.

1. Effettuate una delle seguenti operazioni:

   * Per salvare le impostazioni senza generare il file XML, selezionare **[!UICONTROL Salva]**.
   * Per salvare e generare il file, seleziona **[!UICONTROL Salva e genera]**.

      Il file XML viene generato e registrato nel registro dei processi. I file del Video Sitemap (video-sitemap) e del feed mRSS (mrss-feed) vengono salvati nella cartella root della società.

>[!NOTE]
>
>Pubblica la Video Sitemap o il feed mRSS prima di inviarlo ai motori di ricerca. I file del Video Sitemap e del feed mRSS vengono salvati nella cartella root della società. Contrassegnare questi file XML per pubblicare, se necessario, e selezionare **[!UICONTROL Publish]** .

## Invia Video Sitemap e file mRSS-feed a un motore ricerca {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

I file di Video Sitemap e feed mRSS vengono salvati nella cartella root della società:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Per trasmettere il file Video Sitemap o feed mRSS ai motori di ricerca, copiate uno di questi URL negli strumenti per webmaster del motore di ricerca.

## Visualizza Video rapporti SEO {#viewing-video-seo-reports}

Visualizza Video rapporti SEO nella pagina di report ottimizzazione del motore di Video Search. Per aprire questa pagina, nella barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Rapporti]**.

Se si sono verificati errori durante la generazione di un rapporto, questi vengono elencati nella pagina Rapporto.
