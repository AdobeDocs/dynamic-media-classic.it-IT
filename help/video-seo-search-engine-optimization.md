---
title: SEO (Search Engine Optimization) per i video
description: Scopri come configurare le impostazioni SEO video in Adobe Dynamic Media Classic.
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

Utilizzando Adobe Dynamic Media Classic Video SEO, puoi applicare metadati video per fornire ai motori di ricerca descrizioni dei tuoi video. Adobe Dynamic Media Classic consente di creare video Sitemap e feed mRSS. Questi file XML standard vengono utilizzati per inviare informazioni video ai motori di ricerca:

* **Video Sitemap** - Comunica a Google esattamente dove e quale contenuto video si trova su un sito. Quindi, i video sono completamente ricercabili su Google. In un Video Sitemap è possibile specificare ad esempio la durata e le categorie dei video. Per informazioni sulle mappe video dei siti, consulta [Mappe video e alternative per la mappa del sito video](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **Feed mRSS (Sincronizzazione Media Semplice)** - Utilizzato dagli editori di contenuti per alimentare i file multimediali in Yahoo! Video Search. Per informazioni sui feed mRSS, consulta [Mappe video e alternative per la mappa del sito video](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google supporta sia Video Sitemap che il protocollo di feed mRSS per la trasmissione di informazioni ai motori di ricerca.

Adobe Dynamic Media Classic può generare video Sitemap e feed mRSS dai metadati memorizzati con ogni video. Quando create dei Video Sitemap e feed mRSS, potete scegliere quali campi di metadati includere tra quelli presenti nei file video. Questo vi permette di descrivere i video per i motori di ricerca, che saranno quindi in grado di proporre con più precisione, tra i risultati di ricerca, i video presenti nel vostro sito Web.

>[!NOTE]
>
>prima di creare un Video Sitemap o feed mRSS, verificate quali campi occorre includere nel file XML e come devono essere strutturati, in base ai requisiti del motore di ricerca. Per creare un Video Sitemap o un feed mRSS di successo, questo deve soddisfare i requisiti del motore di ricerca.

Adobe Dynamic Media Classic crea rapporti su Video Sitemap e feed mRSS dopo la loro generazione. Questi report sono disponibili nella pagina Video SEO Report (Report SEO video) .

>[!NOTE]
>
>Per le mappe video e i feed mRSS, Adobe Dynamic Media Classic acquisisce i metadati solo dai video contrassegnati per la pubblicazione. Contrassegnate i video per la pubblicazione per includerne i metadati nei Video Sitemap e nei feed mRSS.

## Scegli le impostazioni SEO video {#choosing-video-seo-settings}

Selezionare le impostazioni SEO video per video Sitemap e feed mRSS sul **[!UICONTROL Impostazioni di ottimizzazione motore di ricerca video]** pagina. Per aprire questa pagina, nella barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL SEO video]** > **[!UICONTROL Impostazioni]**.

In **[!UICONTROL Impostazione generale]** scegli se generare mappe video, feed mRSS o entrambi. In **[!UICONTROL Impostazioni di generazione]** area, mappare i campi metadati ai campi di input.

Dopo aver scelto le impostazioni, seleziona **[!UICONTROL Salva]** o **[!UICONTROL Salva e genera]**) per creare la mappa del sito video, i feed mRSS o entrambi.

### Imposta impostazioni generali {#choosing-general-settings}

Sulla **[!UICONTROL Modalità di generazione]** dall’elenco a discesa, scegli una modalità rapporto:

* **Video Sitemap** - Creare una mappa del sito video.

* **Feed mRSS** - Crea un feed RSS (mRSS) multimediale.

* **Entrambi** - Crea entrambi i tipi di file XML.

* **Disattivato** - Per interrompere la generazione dei feed Video Sitemaps e Media RSS (mRSS), scegli questa opzione.

Sulla **[!UICONTROL Modalità automatica/manuale]** elenco a discesa, scegli se generare automaticamente o manualmente:

* **Modalità automatica** - Adobe Dynamic Media Classic genera automaticamente una mappa del sito video, un feed RSS (mRSS) o entrambi, ogni giorno. Seleziona la **[!UICONTROL Contrassegna per pubblicazione]** per contrassegnare automaticamente per la pubblicazione il file XML generato da Adobe Dynamic Media Classic.

   * **Contrassegna per pubblicazione** Indica la pubblicazione del file XML generato.

* **Modalità manuale** - Adobe Dynamic Media Classic genera la mappa del sito video, il feed RSS (mRSS) multimediale o entrambi quando si seleziona **[!UICONTROL Genera]** o **[!UICONTROL Salva e genera]** nella schermata Impostazioni ottimizzazione ricerca video. Selezionate inoltre le seguenti opzioni:

   * **Nessuna impostazione aggiuntiva** - Non contrassegna per pubblicare il file XML generato.

   * **Contrassegna per pubblicazione** - Indica la pubblicazione del file XML generato.

   * **Consenti generazione parziale** - I motori di ricerca possono rifiutare un file XML se non contiene informazioni complete sui metadati per tutti i video. Questa opzione genera il file XML anche se i metadati non sono disponibili per alcuni video. Nella schermata Rapporto compare un’avvertenza. Selezionate questa opzione se intendete esportare il file XML ed elaborare manualmente le informazioni mancanti.

### Scelta delle impostazioni di generazione {#choosing-generation-settings}

Nell’area Impostazioni generazione sono elencati i campi di input per la mappa del sito video, il feed mRSS o entrambi, nonché nel pannello Metadati, i nomi dei campi di metadati. Servitevi dell’area Impostazioni generazione per associare i campi di input ai relativi campi di metadati. Così facendo, si dice a Adobe Dynamic Media Classic dove ottenere i metadati per la mappa del sito video e/o il feed mRSS.

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
>Pubblica la mappa del sito video o il feed mRSS prima di inviarla ai motori di ricerca. I file del Video Sitemap e del feed mRSS vengono salvati nella cartella root della società. Contrassegna questi file XML per la pubblicazione, se necessario, e seleziona **[!UICONTROL Pubblica]**.

## Inviare file Video Sitemap e feed mRSS a un motore di ricerca {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

I file di Video Sitemap e feed mRSS vengono salvati nella cartella root della società:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Per trasmettere il file Video Sitemap o feed mRSS ai motori di ricerca, copiate uno di questi URL negli strumenti per webmaster del motore di ricerca.

## Visualizzare rapporti SEO video {#viewing-video-seo-reports}

Visualizzare i rapporti SEO video nella pagina Rapporto di ottimizzazione motore di ricerca video . Per aprire questa pagina, nella barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL SEO video]** > **[!UICONTROL Rapporti]**.

Se si sono verificati errori durante la generazione di un rapporto, questi vengono elencati nella pagina Rapporto .
