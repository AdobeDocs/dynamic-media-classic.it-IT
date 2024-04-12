---
title: SEO (Search Engine Optimization) per i video
description: Scopri come configurare le impostazioni Video SEO (Search Engine Optimization) in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 30%

---

# SEO (Search Engine Optimization) per i video{#video-seo-search-engine-optimization}

L’ottimizzazione SEO (Search Engine Optimization, ottimizzazione per i motori di ricerca) consente di migliorare il volume di traffico verso un sito Web generato dai motori di ricerca. I motori di ricerca possono raccogliere informazioni sui contenuti testuali, ma non dai video a meno che le informazioni necessarie per le ricerche non siano appositamente specificate.

Utilizzando Adobe Dynamic Media Classic Video SEO, puoi applicare metadati video per fornire ai motori di ricerca le descrizioni dei tuoi video. Adobe Dynamic Media Classic consente di creare Video Sitemap e feed mRSS. Questi file XML standard vengono utilizzati per inviare informazioni video ai motori di ricerca:

* **Video Sitemap** : indica a Google esattamente dove e cosa si trova il contenuto video su un sito. I video sono completamente ricercabili su Google. In un Video Sitemap è possibile specificare ad esempio la durata e le categorie dei video. Per informazioni sulle mappe del sito video, consulta [Video sitemap e video sitemap alternative](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **Feed mRSS (Media Really Simple Syndication)** : utilizzato dagli editori di contenuti per inserire file multimediali in Yahoo. Video Search. Per informazioni sui feed mRSS, vedere [Video sitemap e video sitemap alternative](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google supporta sia Video Sitemap che il protocollo di feed mRSS per la trasmissione di informazioni ai motori di ricerca.

Adobe Dynamic Media Classic può generare Video Sitemap e feed mRSS dai metadati memorizzati con ogni video. Quando create dei Video Sitemap e feed mRSS, potete scegliere quali campi di metadati includere tra quelli presenti nei file video. In questo modo, descrivi i video ai motori di ricerca in modo che i motori di ricerca possano indirizzare più accuratamente il traffico ai video sul sito web.

>[!NOTE]
>
>prima di creare un Video Sitemap o feed mRSS, verificate quali campi occorre includere nel file XML e come devono essere strutturati, in base ai requisiti del motore di ricerca. Per creare un Video Sitemap o un feed mRSS di successo, questo deve soddisfare i requisiti del motore di ricerca.

Dopo la generazione, Adobe Dynamic Media Classic crea rapporti sulle mappe del sito video e sui feed mRSS. Questi rapporti sono disponibili nella pagina Video SEO Report (Rapporto SEO video).

>[!NOTE]
>
>Per le mappe del sito video e i feed mRSS, Adobe Dynamic Media Classic acquisisce i metadati solo dai video contrassegnati per la pubblicazione. Contrassegna i video per la pubblicazione per includerne i metadati in Video Sitemap e feed mRSS.

## Scegli impostazioni Video SEO (Search Engine Optimization)

Selezionare le impostazioni Video SEO per Video Sitemap e feed mRSS sul **[!UICONTROL Impostazioni di ottimizzazione motore di ricerca video]** pagina. Per aprire questa pagina, nella barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Impostazioni]**.

In **[!UICONTROL Impostazione generale]** , scegliere se generare Video Sitemap, feed mRSS o entrambi. In **[!UICONTROL Impostazioni di generazione]** area, mappa i campi di metadati con i campi di input.

Dopo aver scelto le impostazioni, seleziona **[!UICONTROL Salva]** (o **[!UICONTROL Salva e genera]**) per creare Video Sitemap, feed mRSS o entrambi.

### Configurare le impostazioni generali {#choosing-general-settings}

Il giorno **[!UICONTROL Modalità di generazione]** dall&#39;elenco a discesa, scegli una modalità di rapporto:

* **Video Sitemap** : crea una Video Sitemap.

* **Feed mRSS** : crea un feed Media RSS (mRSS).

* **Entrambi** : consente di creare entrambi i tipi di file XML.

* **Disattivato** - Scegliere questa opzione per interrompere la generazione di Video Sitemap e feed Media RSS (mRSS).

Il giorno **[!UICONTROL Modalità automatica/manuale]** dall&#39;elenco a discesa, scegliere se generare automaticamente o manualmente:

* **Modalità automatica** - Adobe Dynamic Media Classic genera automaticamente una Video Sitemap, un feed Media RSS (mRSS), o entrambi, ogni giorno. Seleziona la **[!UICONTROL Contrassegna per pubblicazione]** opzione per contrassegnare automaticamente per la pubblicazione il file XML generato da Adobe Dynamic Media Classic.

   * **Contrassegna per pubblicazione** Contrassegna per la pubblicazione del file XML generato.

* **Modalità manuale** - Adobe Dynamic Media Classic genera Video Sitemap, Media RSS (mRSS) feed, o entrambi, quando si seleziona **[!UICONTROL Genera]** o **[!UICONTROL Salva e genera]** nella schermata Impostazioni ottimizzazione ricerca video. Selezionate inoltre le seguenti opzioni:

   * **Nessuna ulteriore impostazione** - Non contrassegna per la pubblicazione il file XML generato.

   * **Contrassegna per pubblicazione** : contrassegna per la pubblicazione del file XML generato.

   * **Consenti generazione parziale** - I motori di ricerca possono rifiutare un file XML se non contiene informazioni complete sui metadati per tutti i video. Questa opzione genera il file XML anche se i metadati non sono disponibili per alcuni video. Nella schermata Rapporto compare un’avvertenza. Selezionate questa opzione se intendete esportare il file XML ed elaborare manualmente le informazioni mancanti.

### Scelta delle impostazioni di generazione {#choosing-generation-settings}

Nell&#39;area Impostazioni di generazione sono elencati i campi di input per Video Sitemap, o feed mRSS, o entrambi, e nel pannello Metadati sono elencati i nomi dei campi di metadati. Servitevi dell’area Impostazioni generazione per associare i campi di input ai relativi campi di metadati. In questo modo, l&#39;utente indica a Adobe Dynamic Media Classic dove ottenere i metadati per Video Sitemap e/o il feed mRSS.

1. Nel menu Visualizzazioni metadati, scegliete una visualizzazione per i metadati. Dopo aver scelto una vista, i nomi dei campi di metadati vengono visualizzati nel pannello Metadati.
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
>Pubblica la Video Sitemap o il feed mRSS prima di inviarlo ai motori di ricerca. I file del Video Sitemap e del feed mRSS vengono salvati nella cartella root della società. Contrassegna questi file XML per la pubblicazione, se necessario, e seleziona **[!UICONTROL Pubblica]**.

## Invio di file Video Sitemap e feed mRSS a un motore di ricerca {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

I file di Video Sitemap e feed mRSS vengono salvati nella cartella root della società:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copia uno di questi URL negli strumenti webmaster del motore di ricerca per inviare il file di feed Video Sitemap o Media RSS (mRSS) ai motori di ricerca.

## Visualizza rapporti Video SEO {#viewing-video-seo-reports}

Visualizza i rapporti Video SEO (Search Engine Optimization) nella pagina Rapporto Ottimizzazione motore di ricerca video. Per aprire questa pagina, nella barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Rapporti]**.

Se si sono verificati errori durante la generazione di un rapporto, questi vengono elencati nella pagina Rapporto.
