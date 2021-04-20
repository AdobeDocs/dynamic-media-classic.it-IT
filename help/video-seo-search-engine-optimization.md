---
title: SEO (Search Engine Optimization) per i video
description: Scopri come configurare le impostazioni SEO video.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Administrator
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 62%

---


# SEO (Search Engine Optimization) per i video{#video-seo-search-engine-optimization}

L’ottimizzazione SEO (Search Engine Optimization, ottimizzazione per i motori di ricerca) consente di migliorare il volume di traffico verso un sito Web generato dai motori di ricerca. I motori di ricerca possono raccogliere informazioni sui contenuti testuali, ma non dai video a meno che le informazioni necessarie per le ricerche non siano appositamente specificate.

Utilizzando Dynamic Media Classic Video SEO, è possibile applicare metadati video per fornire ai motori di ricerca descrizioni dei video. Dynamic Media Classic consente di creare video Sitemap e feed mRSS. Questi file XML standard vengono utilizzati per inviare informazioni video ai motori di ricerca:

**Video** SitemapInforma Google esattamente dove e quale contenuto video si trova su un sito. Quindi, i video sono completamente ricercabili su Google. In un Video Sitemap è possibile specificare ad esempio la durata e le categorie dei video. Per informazioni sulle mappe video dei siti, consulta https://www.google.com/support/webmasters/bin/answer.py?answer=80471.

**** Feed mRSS (Media Veramente Simple Syndication) Utilizzato dagli editori di contenuti per alimentare file multimediali in Yahoo! Video Search. Per informazioni sui feed mRSS, vedere https://www.rssboard.org/media-rss.

>[!NOTE]
>
>Google supporta sia Video Sitemap che il protocollo di feed mRSS per la trasmissione di informazioni ai motori di ricerca.

Dynamic Media Classic può generare video Sitemap e feed mRSS dai metadati memorizzati con ogni video. Quando create dei Video Sitemap e feed mRSS, potete scegliere quali campi di metadati includere tra quelli presenti nei file video. Questo vi permette di descrivere i video per i motori di ricerca, che saranno quindi in grado di proporre con più precisione, tra i risultati di ricerca, i video presenti nel vostro sito Web.

>[!NOTE]
>
>prima di creare un Video Sitemap o feed mRSS, verificate quali campi occorre includere nel file XML e come devono essere strutturati, in base ai requisiti del motore di ricerca. Per creare un Video Sitemap o un feed mRSS di successo, questo deve soddisfare i requisiti del motore di ricerca.

Dynamic Media Classic crea rapporti su Video Sitemap e feed mRSS dopo la loro generazione. disponibili nella schermata Rapporto Video SEO.

>[!NOTE]
>
>Per le mappe video e i feed mRSS, Dynamic Media Classic acquisisce i metadati solo dai video contrassegnati per la pubblicazione. Contrassegnate i video per la pubblicazione per includerne i metadati nei Video Sitemap e nei feed mRSS.

## Scelta delle impostazioni SEO video {#choosing-video-seo-settings}

Potete scegliere le impostazioni Video SEO per i Video Sitemap e i feed mRSS nella schermata Impostazioni ottimizzazione motore di ricerca video. che potete aprire scegliendo Configurazione > Impostazione applicazione > Video SEO > Impostazioni.

Nell’area Impostazioni generali, scegliete se generare Video Sitemap, feed mRSS o entrambi. Nell’area Impostazioni generazione, assegnate i campi di metadati ai campi di input.

Al termine, fate clic su Genera (o su Salva e genera) per creare il Video Sitemap, il feed mRSS o entrambi.

### Scelta delle impostazioni generali  {#choosing-general-settings}

Dall’elenco a discesa Modalità generazione, scegliete una modalità di rapporto:

**Video** SitemapCreare una mappa del sito video.

**Feed** RSSCreazione di un feed RSS (mRSS) multimediale.

**** Entrambi: consente di creare entrambi i tipi di file XML.

**** DisattivatoPer interrompere la generazione dei feed Video Sitemap e Media RSS (mRSS), scegli questa opzione.

Nell’elenco a discesa Modalità automatica o Modalità manuale, scegliete se la generazione deve essere automatica o manuale:

**Modalità automatica** Dynamic Media Classic genera automaticamente una mappa del sito video, un feed RSS (mRSS) o entrambi, ogni giorno. Scegli l’opzione Contrassegna per pubblicazione per contrassegnare automaticamente per la pubblicazione il file XML generato da Dynamic Media Classic.

**Modalità manualeDynamic Media Classic genera la mappa del sito video, il feed RSS (mRSS) o entrambi quando si fa clic su Genera o Salva e genera nella schermata Impostazioni ottimizzazione ricerca video.** Selezionate inoltre le seguenti opzioni:

**Nessun&#39;altra** impostazioneNon contrassegna per pubblicare il file XML generato.

**Contrassegna per** PublishMarks per pubblicare il file XML generato.

**Consenti ai motori** di ricerca parziale di rifiutare un file XML se non contiene informazioni complete sui metadati per tutti i video. Con questa opzione il file XML viene generato anche se per alcuni video non sono disponibili i metadati necessari. Nella schermata Rapporto compare un’avvertenza. Selezionate questa opzione se intendete esportare il file XML ed elaborare manualmente le informazioni mancanti.

### Scelta delle impostazioni di generazione  {#choosing-generation-settings}

Nell’area Impostazioni generazione sono elencati i campi di input per Video Sitemap e/o feed mRSS; nel pannello Metadati sono elencati i nomi dei campi di metadati. Servitevi dell’area Impostazioni generazione per associare i campi di input ai relativi campi di metadati. In questo modo, si comunica a Dynamic Media Classic dove ottenere i metadati per la mappa del sito video e/o il feed mRSS.

1. Nel menu Visualizzazioni metadati, scegliete una visualizzazione per i metadati. I nomi dei campi di metadati compaiono quindi nel pannello Metadati. Per informazioni sulle visualizzazioni di metadati, consultate [Visualizzazione metadati](application-setup.md#metadata_views).
1. Trascinate i nomi dei campi di metadati dal pannello Metadati ai campi di input Pagina di arrivo, Titolo, Descrizione, Tag e Categoria. I campi Pagina di arrivo, Titolo e Descrizione sono obbligatori.

   >[!NOTE]
   >
   >potete anche inserire manualmente i dati nei campi di input.

1. Fate clic su Salva (per salvare le impostazioni senza generare il file XML), Genera (per generare il file XML) oppure Salva e genera (per salvare e generare il file).

   Il file XML viene generato e registrato nel registro dei processi. I file del Video Sitemap (video-sitemap) e del feed mRSS (mrss-feed) vengono salvati nella cartella root della società.

>[!NOTE]
>
>Pubblica la mappa del sito video o il feed mRSS prima di inviarla ai motori di ricerca. I file del Video Sitemap e del feed mRSS vengono salvati nella cartella root della società. Se necessario, contrassegnate tali file XML per la pubblicazione e fate clic su Pubblica.

## Trasmissione dei file Video Sitemap e feed mRSS ai motori di ricerca  {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

I file di Video Sitemap e feed mRSS vengono salvati nella cartella root della società:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Per trasmettere il file Video Sitemap o feed mRSS ai motori di ricerca, copiate uno di questi URL negli strumenti per webmaster del motore di ricerca.

## Visualizzazione dei rapporti Video SEO  {#viewing-video-seo-reports}

Potete visualizzare i rapporti Video SEO nella schermata Report di ottimizzazione motore di ricerca video Per aprire questa schermata, fai clic su Configurazione > Impostazione applicazione > Video SEO > Rapporti.

Se durante la generazione del rapporto si erano verificati degli errori, questi vengono elencati nella schermata Rapporto.
