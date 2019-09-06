---
title: SEO (Search Engine Optimization) per i video
seo-title: SEO (Search Engine Optimization) per i video
description: 'null'
seo-description: Scopri come configurare le impostazioni Video SEO.
uuid: bac 2 c 6 a 9-8466-4 b 8 f-b 835-6 cb 0 b 4168513
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/setup
discoiquuid: 34 ecd 868-775 f -452 b-b 26 e-d 139 f 0 e 280 ae
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# SEO (Search Engine Optimization) per i video{#video-seo-search-engine-optimization}

L’ottimizzazione SEO (Search Engine Optimization, ottimizzazione per i motori di ricerca) consente di migliorare il volume di traffico verso un sito Web generato dai motori di ricerca. I motori di ricerca possono raccogliere informazioni sui contenuti testuali, ma non dai video a meno che le informazioni necessarie per le ricerche non siano appositamente specificate.

Con Dynamic Media Classic SEO potete sfruttare i metadati video per fornire ai motori di ricerca le descrizioni dei video. Dynamic Media Classic consente di creare Video Sitemap e feed mrss. Si tratta di file XML standard per la trasmissione di informazioni sui video ai motori di ricerca:

**Video Sitemap** informa Google esattamente su dove e quali contenuti video si trovano su un sito. I video possono quindi essere inclusi nei risultati delle ricerche Google. In un Video Sitemap è possibile specificare ad esempio la durata e le categorie dei video. Per informazioni su Video Sitemap, consultate https://www.google.com/support/webmasters/bin/answer.py?answer=80471.

**Feed mrss (Media Really Simple Syndication) Feed** utilizzato dagli editori di contenuto per feed di file multimediali in Yahoo! Video Search. Per informazioni sui feed mrss, consultate https://www.rssboard.org/media-rss.

>[!NOTE]
>
>Google supporta sia Video Sitemap che il protocollo di feed mRSS per la trasmissione di informazioni ai motori di ricerca.

Dynamic Media Classic può generare Video Sitemap e feed mrss dai metadati memorizzati con ciascun video. Quando create dei Video Sitemap e feed mRSS, potete scegliere quali campi di metadati includere tra quelli presenti nei file video. Questo vi permette di descrivere i video per i motori di ricerca, che saranno quindi in grado di proporre con più precisione, tra i risultati di ricerca, i video presenti nel vostro sito Web.

>[!NOTE]
>
>prima di creare un Video Sitemap o feed mRSS, verificate quali campi occorre includere nel file XML e come devono essere strutturati, in base ai requisiti del motore di ricerca. Per creare un Video Sitemap o un feed mRSS di successo, questo deve soddisfare i requisiti del motore di ricerca.

Dynamic Media Classic crea rapporti su Video Sitemap e feed mrss dopo la generazione. disponibili nella schermata Rapporto Video SEO.

>[!NOTE]
>
>Per i Video Sitemap e i feed mrss, Dynamic Media Classic acquisisce i metadati solo dai video contrassegnati per la pubblicazione. Contrassegnate i video per la pubblicazione per includerne i metadati nei Video Sitemap e nei feed mRSS.

## Choosing video SEO settings {#choosing-video-seo-settings}

Potete scegliere le impostazioni Video SEO per i Video Sitemap e i feed mRSS nella schermata Impostazioni ottimizzazione motore di ricerca video. che potete aprire scegliendo Configurazione &gt; Impostazione applicazione &gt; Video SEO &gt; Impostazioni.

Nell’area Impostazioni generali, scegliete se generare Video Sitemap, feed mRSS o entrambi. Nell’area Impostazioni generazione, assegnate i campi di metadati ai campi di input.

Al termine, fate clic su Genera (o su Salva e genera) per creare il Video Sitemap, il feed mRSS o entrambi.

### Scelta delle impostazioni generali {#choosing-general-settings}

Dall’elenco a discesa Modalità generazione, scegliete una modalità di rapporto:

**Video Sitemap** Create un Video Sitemap.

**Feed mrss** Crea un feed Mrss (mrss).

**Entrambe** creano entrambi i tipi di file XML.

**Disattiva** Questa opzione per interrompere la generazione di Video Sitemap e di feed Mrss.

Nell’elenco a discesa Modalità automatica o Modalità manuale, scegliete se la generazione deve essere automatica o manuale:

**La modalità** automatica Dynamic Media Classic genera automaticamente un Video Sitemap, un feed Mrss (mrss) o entrambi ogni giorno. Scegliete l'opzione Contrassegna per pubblicazione per contrassegnare automaticamente per la pubblicazione il file XML generato da Dynamic Media Classic.

**La modalità** Manuale Dynamic Media Classic genera il Video Sitemap, il feed Media RSS (mrss) o entrambi quando fate clic su Genera o Salva e genera nella schermata Impostazioni ottimizzazione motore di ricerca video. Selezionate inoltre le seguenti opzioni:

**Nessuna ulteriore impostazione** Non contrassegna per la pubblicazione il file XML generato.

**Contrassegnate per la pubblicazione** gli indicatori di pubblicazione per la pubblicazione del file XML generato.

**Consenti ai motori** di ricerca di generazione parziale potrebbe rifiutare un file XML se non contiene informazioni complete sui metadati per tutti i video. Con questa opzione il file XML viene generato anche se per alcuni video non sono disponibili i metadati necessari. Nella schermata Rapporto compare un’avvertenza. Selezionate questa opzione se intendete esportare il file XML ed elaborare manualmente le informazioni mancanti.

### Scelta delle impostazioni di generazione {#choosing-generation-settings}

Nell’area Impostazioni generazione sono elencati i campi di input per Video Sitemap e/o feed mRSS; nel pannello Metadati sono elencati i nomi dei campi di metadati. Servitevi dell’area Impostazioni generazione per associare i campi di input ai relativi campi di metadati. In questo modo, potete indicare a Dynamic Media Classic dove ottenere i metadati per Video Sitemap e/o feed mrss.

1. Nel menu Visualizzazioni metadati, scegliete una visualizzazione per i metadati. I nomi dei campi di metadati compaiono quindi nel pannello Metadati. Per informazioni sulle visualizzazioni di metadati, consultate [Visualizzazione metadati](application-setup.md#metadata_views).
1. Trascinate i nomi dei campi di metadati dal pannello Metadati ai campi di input Pagina di arrivo, Titolo, Descrizione, Tag e Categoria. I campi Pagina di arrivo, Titolo e Descrizione sono obbligatori.

   >[!NOTE]
   >
   >potete anche inserire manualmente i dati nei campi di input.

1. Fate clic su Salva (per salvare le impostazioni senza generare il file XML), Genera (per generare il file XML) oppure Salva e genera (per salvare e generare il file).

   Il file XML viene generato e registrato nel registro dei processi. I file del Video Sitemap (video-sitemap) e del feed mRSS (mrss-feed) vengono salvati nella cartella root della società.

>[!NOTE]
>
>prima di poter essere trasmesso ai motori di ricerca, il Video Sitemap o feed mRSS deve essere pubblicato. I file del Video Sitemap e del feed mRSS vengono salvati nella cartella root della società. Se necessario, contrassegnate tali file XML per la pubblicazione e fate clic su Pubblica.

## Trasmissione dei file Video Sitemap e feed mRSS ai motori di ricerca {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

I file di Video Sitemap e feed mRSS vengono salvati nella cartella root della società:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Per trasmettere il file Video Sitemap o feed mRSS ai motori di ricerca, copiate uno di questi URL negli strumenti per webmaster del motore di ricerca.

## Visualizzazione dei rapporti Video SEO {#viewing-video-seo-reports}

Potete visualizzare i rapporti Video SEO nella schermata Report di ottimizzazione motore di ricerca video Per aprire questa schermata, fate clic su Configurazione &gt; Impostazione applicazione &gt; Video SEO &gt; Rapporti.

Se durante la generazione del rapporto si erano verificati degli errori, questi vengono elencati nella schermata Rapporto.
