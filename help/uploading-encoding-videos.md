---
title: Caricamento e codifica dei video
seo-title: Caricamento e codifica dei video
description: Scopri come caricare e codificare i video.
seo-description: Scopri come caricare e codificare i video.
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
feature: Dynamic Media Classic,Visualizzatori,Video
role: Business Practitioner
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '3882'
ht-degree: 69%

---

# Caricamento e codifica dei video{#uploading-and-encoding-videos}

Per creare set video singoli o adattivi da distribuire sul Web o sui dispositivi mobili, carica prima i file video master in Dynamic Media Classic. Dynamic Media Classic codifica i video in formato MP4 e pubblica i video nei seguenti formati di file:

* **MP4**  - Dynamic Media Classic consiglia MP4 come formato di file video preferito. Utilizzate i file MP4 per le seguenti operazioni:

   * Streaming dinamico HTTP su desktop.
   * Streaming dinamico HTTP (protocollo di streaming Apple).
   * Distribuzione progressiva di video su dispositivi mobili Android™, BlackBerry® e Windows®

   Dynamic Media Classic offre due flussi di lavoro per il caricamento di file video:

* **Video precodificati**  - Puoi caricare i file MP4 direttamente in Dynamic Media Classic. Con questo flusso di lavoro, i file non vengono codificati durante il caricamento. I file vengono precodificati durante la preparazione per la visualizzazione sul desktop e sui dispositivi mobili.

* **Video sorgente master**  - Carica i file video sorgente master e, al momento del caricamento, codifica questi file in file MP4. Nel pannello Sfoglia, i video codificati sono etichettati “Video”. Dynamic Media Classic supporta la codifica di file video in molti formati.

   * Assicurati che i file video sorgente master che desideri codificare siano supportati.

      Consultate [Tipi di file video supportati per la codifica](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

   * Scegliete un predefinito di codifica video.

      Consultate [Predefiniti video per la codifica di file video](application-setup.md#video-presets-for-encoding-video-files).

      Consultate [Procedure ottimali per la codifica video](uploading-encoding-videos.md#best-practices-for-video-encoding).

Dynamic Media Classic genera anche miniature video. Per ulteriori informazioni sulle miniature video, su come ottenerne gli URL e come modificare i fotogrammi poster,

consultate [Utilizzo delle miniature video](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Per caricare e codificare i video:**

Effettuate una delle seguenti operazioni.

*Se i video sono stati già codificati*

1. Nella barra di navigazione globale, fate clic su **[!UICONTROL Carica]**.
1. Nella pagina Carica , fai clic sulla scheda **[!UICONTROL Da desktop]** .
1. Nella pagina Carica, nel pannello **[!UICONTROL Seleziona file da caricare]** fai clic su **[!UICONTROL Sfoglia]**, individua un file video MP4 e fai clic su **[!UICONTROL Apri]**.
1. Nel pannello **[!UICONTROL Scegli destinazione cartella]** , seleziona una cartella per il file caricato.
1. Nella pagina Carica , accertati che sia selezionato **[!UICONTROL Pubblica dopo aver caricato]**.
1. Fate clic su **[!UICONTROL Invia caricamento]**.

*Per codificare i video con Dynamic Media Classic*

1. Nella barra di navigazione globale, fate clic su **[!UICONTROL Carica]**.
1. Nella pagina Carica , fai clic sulla scheda **[!UICONTROL Da desktop]** .
1. Nel pannello **[!UICONTROL Seleziona file da caricare]**, fai clic su **[!UICONTROL Sfoglia]**, individua un file video sorgente principale e fai clic su **[!UICONTROL Apri]**.
1. Nel pannello **[!UICONTROL Scegli destinazione cartella]** , seleziona una cartella per il file caricato.
1. Nell’angolo inferiore destro della pagina fate clic su **[!UICONTROL Opzioni processo]**.
1. Nella finestra di dialogo Opzioni processo di caricamento , espandi **[!UICONTROL Opzioni eVideo]**, quindi effettua una delle seguenti operazioni:

   * Si consiglia di selezionare **[!UICONTROL Codifica video adattiva]**. Consultate [Video adattivo (predefinito)](application-setup.md#adaptive-video-default).
   * Facoltativo. Per utilizzare le singole impostazioni di codifica, espandere **[!UICONTROL Predefiniti codifica singola]**, quindi selezionare le opzioni di codifica desiderate per Desktop, Mobile e Tablet.
Consultate [Predefiniti di codifica video per computer desktop](application-setup.md#desktop-video-encoding-presets), [Predefiniti di codifica per video per dispositivi mobili](application-setup.md#mobile-video-encoding-presets), [Predefiniti di codifica per video per tablet](application-setup.md#tablet-video-encoding-presets).
1. Nella finestra di dialogo Opzioni processo di caricamento, fate clic su **[!UICONTROL Salva]**.
1. Nella pagina Carica , accertati che sia selezionato **[!UICONTROL Pubblica dopo aver caricato]**.
1. Nella pagina Carica, nell’angolo in basso a destra, fate clic su **[!UICONTROL Invia caricamento]**.

*Se desiderate ricodificare un file video precedentemente caricato*

1. In Dynamic Media Classic, nel pannello Sfoglia, individuate il video e selezionatelo.
1. Fate clic su **[!UICONTROL File]** > **[!UICONTROL Rielabora]**.
1. Nella finestra di dialogo Rielabora risorse , espandi **[!UICONTROL Opzioni eVideo]**, quindi effettua una delle seguenti operazioni:
   * Come procedura ottimale, si consiglia di utilizzare il metodo seguente. Selezionate **Video adattivo**. Consultate [Video adattivo (predefinito)](application-setup.md#adaptive-video-default).
   * Facoltativo. Per utilizzare le singole impostazioni di codifica, espandere ****[!UICONTROL Predefiniti codifica singola]****, quindi selezionare le opzioni di codifica desiderate per Desktop, Mobile e Tablet.
Consultate [Predefiniti di codifica video per computer desktop](application-setup.md#desktop-video-encoding-presets), [Predefiniti di codifica per video per dispositivi mobili](application-setup.md#mobile-video-encoding-presets), [Predefiniti di codifica per video per tablet](application-setup.md#tablet-video-encoding-presets).
1. Nella finestra di dialogo Rielabora risorse, fate clic su **[!UICONTROL Invia]**.

Quando utilizzate un predefinito di codifica per video adattivi oppure più predefiniti di codifica singola, viene creato automaticamente un set di video adattivi con più codifiche video. Potete anche creare manualmente un set di video adattivi, selezionando i singoli video.

Quando generate un set di video adattivi automaticamente o manualmente vengono creati solo i tipi di file MP4 e M4V.

## Tipi di file video supportati per la codifica {#supported-video-file-types-for-encoding}

La seguente tabella indica i tipi di file video (con i codec video consentiti) che potete codificare in formato MP4 o OGV quando caricate i file. La tabella elenca i formati file e i codec:

* **Formati di file video**  - Simili a un file ZIP, un formato di file video determina il modo in cui i file sono contenuti nel file video. Generalmente, un file video contiene più tracce (una traccia video senza audio e una o più tracce audio senza video) che vengono associate e sincronizzate. Il formato file del video determina come le diverse tracce di dati e metadati vengono organizzate.

* **Codec video**  - Un codec video descrive l’algoritmo con cui un video viene codificato. Un lettore video decodifica il video in base al relativo codec, quindi visualizza una serie di immagini o fotogrammi sullo schermo. I codec riducono la quantità di informazioni richieste dai file video per memorizzare e riprodurre il video. Invece delle informazioni su ciascun fotogramma, vengono memorizzate solo le informazioni relative alle differenze tra l’uno e l’altro. Poiché la maggior parte dei video cambia poco da un fotogramma all&#39;altro, i codec consentono elevati tassi di compressione, che si traducono in dimensioni di file più piccole.

   | Formato file video | Codec video |
   |:--- |:--- |
   | 3GP | H.263, H.264 |
   | AVI | DivX, DV |
   | M2P | MPEG-2 PS |
   | M2T | MPEG-2 TS |
   | M2TS | MPEG-2 TS |
   | M2V | MPEG-2 ES |
   | M4V | H.264 |
   | MOV | DV, DVCPro 50, H.261, H.263, H.264, Sorenson Video 1 |
   | MP4 | H.264/MPEG-4 AVC |
   | MPEG | MPEG-2 SS |
   | MPG | MPEG-2 SS |
   | MTS | MPEG-2 |
   | ProRes | APCN, APCS, APCO, APCH, AP4H |
   | TS | DVCPro 50 |
   | VOB | MPEG-2 |
   | WMV/ASF | VC-1, Windows® Media Video 7, Windows® Media Video 8 |

   >[!NOTE]
   >
   >La schermata Processi invia una notifica se caricate e tentate di codificare un file video e il file viene rifiutato perché contiene un codec o un contenitore file incompatibile. Per ulteriori informazioni, consultate [Verifica dei file di processo](checking-job-files.md).

## Best practice per la codifica video {#best-practices-for-video-encoding}

Di seguito sono riportati alcuni suggerimenti per la codifica di file video di origine in Dynamic Media Classic.

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### File video sorgente {#source-video-files}

Per la codifica di un file video, occorre usare un file video sorgente della massima qualità possibile. Evitate di usare file video precedentemente codificati in quanto sono già compressi e un’ulteriore codifica causerebbe il deterioramento della qualità del video.

La tabella seguente descrive le dimensioni, le proporzioni e il bit rate minimo consigliati che i file video sorgente devono avere quando li codifichi:

| Dimensioni | Proporzioni | Bitrate minimo |
|--- |--- |--- |
| 1024x768 | 4:3 | 4500 Kbps per la maggior parte dei video. |
| 1280x720 | 16:9 | 3000 - 6000 Kbps, a seconda della quantità di movimento presente del video. |
| 1920x1080 | 16:9 | 6000 - 8000 Kbps, a seconda della quantità di movimento presente del video. |

### Ottenimento dei metadati dei file {#obtaining-a-file-s-metadata}

È possibile ottenere i metadati di un file visualizzandone i metadati in Dynamic Media Classic, utilizzando uno strumento di editing video o un&#39;applicazione progettata per ottenere i metadati. Seguono istruzioni per l’utilizzo di MediaInfo, un’applicazione di terze parti che consente di ottenere i metadati di un file video:

1. Vai a questa pagina web: [https://mediainfo.sourceforge.net/en/Download](https://mediainfo.sourceforge.net/en/Download).
1. Selezionate e scaricate il programma di installazione per la versione GUI, quindi seguite le istruzioni di installazione.
1. Dopo l&#39;installazione, fare clic con il pulsante destro del mouse sul file video (solo Windows®) e selezionare MediaInfo oppure aprire MediaInfo e trascinare il file video nell&#39;applicazione. Potete vedere tutti i metadati associati al file video, inclusi i valori di larghezza, altezza e fotogrammi al secondo.

### Proporzioni {#aspect-ratio}

Quando scegliete o create un predefinito di codifica video da applicare al file video principale, accertatevi che il predefinito abbia le stesse proporzioni del file video principale. Le *proporzioni* sono il rapporto tra la larghezza e l’altezza del video. 

Per determinare le proporzioni di un file video, ottenete i metadati del file e prendete nota dei valori di larghezza e altezza (consultate [Ottenimento dei metadati dei file](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Quindi applicate questa formula per determinare le proporzioni:

larghezza/altezza = proporzioni

Nella tabella che segue, i risultati della formula vengono correlati alle relative scelte di proporzioni più comuni:

| Risultato della formula | Proporzioni |
|--- |--- |
| 1,33 | 4:3 |
| 0,75 | 3:4 |
| 1,78 | 16:9 |
| 0,56 | 9:16 |

Ad esempio, un video con una larghezza x 1080 di 1440 ha un rapporto di formato di 1440/1080 o 1,33. In questo caso, scegli un predefinito di codifica video con un rapporto di formato 4:3 per codificare il file video.

### Velocità dati {#data-rate}

Per *velocità dati* (o *bitrate*) si intende la quantità di dati che vengono codificati per ottenere un secondo di riproduzione video. La velocità dati è misurata in kilobit al secondo (Kbps).

>[!NOTE]
>
>poiché tutti i codec usano metodi di compressione con perdita di dati, la velocità dati è il fattore che influisce maggiormente sulla qualità video. Con la compressione con perdita di dati, infatti, a una maggiore compressione di un file video corrisponde un maggior degrado della qualità. Per questa ragione, a parità di tutte le altre caratteristiche (risoluzione, frequenza fotogrammi e codec), una velocità dati inferiore genera file compressi di qualità inferiore.

Quando scegli un predefinito di codifica video, ricorda di tenere conto della velocità di connessione dell’utente finale di destinazione. Scegli un predefinito con una velocità dati pari all&#39;80% di quella velocità. Ad esempio, se la connessione dell’utente finale è di 1000 Kbps, scegliete un predefinito con velocità dati video di 800 Kbps.

La tabella di seguito riporta la velocità dati per velocità di connessioni tipiche.

| Velocità (Kbps) | Tipo di connessione  |
|--- |--- |
| 256 | Connessione via modem. |
| 800 | Connessione mobile tipica. Per questa connessione, scegliete una velocità dati di circa 400, con un massimo di 800 per esperienze 3G. |
| 2000 | Connessione desktop tipica a banda larga. Per questa connessione, eseguire il targeting di una velocità dati nell&#39;intervallo 800-2000 Kbps, con la maggior parte delle destinazioni con una media di 1200-1500 Kbps. |
| 5000 | Connessione a banda larga elevata tipica. Non si consiglia di applicare la codifica per questo valore elevato, in quanto la maggior parte dei clienti non dispone di trasmissione video di tale velocità.  |

### Risoluzione {#resolution}

La *Risoluzione* descrive l’altezza e la larghezza di un file video, in pixel. La maggior parte delle sorgenti video è memorizzata ad alta risoluzione (ad esempio, 1920x1080). Per lo streaming, il video sorgente viene compresso in una risoluzione inferiore (per un valore massimo di 640x480).

La risoluzione e la velocità dati sono due fattori strettamente correlati da cui dipende la qualità video. Per mantenere la stessa qualità video, più elevato è il numero di pixel in un file video (ossia più elevata è la risoluzione), più elevata deve essere anche la velocità dati. Ad esempio, considerate il numero di pixel per fotogramma in due file video, rispettivamente con risoluzione 320x240 e 640x480:

| Risoluzione | Pixel per fotogramma |
|--- |--- |
| 320x240 | 76.800 |
| 640x480 | 307.200 |

Il file da 640x480 ha quattro volte il numero di pixel per fotogramma. Per ottenere la stessa velocità dati per queste due risoluzioni, occorre applicare una compressione quattro volte maggiore al file da 640x480, riducendone quindi la qualità video. Di conseguenza. una velocità dati video pari a 250 Kbps produce risultati di alta qualità a una risoluzione di 320x240, ma non a una risoluzione di 640x480.

>[!NOTE]
>
>In generale, maggiore è la velocità dei dati utilizzata, migliore sarà l&#39;aspetto del video e maggiore è la risoluzione utilizzata, maggiore è la velocità dei dati che è necessario mantenere la qualità di visualizzazione (rispetto alle risoluzioni più basse).

Data la correlazione tra risoluzione e velocità dati, per la codifica video è possibile considerare due opzioni:

* Scegli una velocità dati e quindi codifica alla risoluzione più alta che appare meglio alla velocità dati scelta.
* Scegliere una risoluzione e quindi effettuare la codifica con una velocità dati tale da produrre video di alta qualità per la risoluzione scelta.

Quando scegliete (o create) un predefinito di codifica video per il file video principale, fate riferimento alla tabella di seguito per conseguire la risoluzione corretta:

| Risoluzione | Altezza (pixel) | Dimensione schermo |
|--- |--- |--- |
| 240p | 240 | Schermo molto piccolo |
| 300p | 300 | Schermo piccolo tipico per dispositivi mobili |
| 360p | 360 | Schermo piccolo |
| 480p | 480 | Schermo medio |
| 720p | 720 | Schermo grande |
| 1080p | 1080 | Schermo grande ad alta definizione |

### Fps (fotogrammi al secondo) {#fps-frames-per-second}

Negli Stati Uniti e in Giappone, i video sono in genere ripresi a 29,97 fotogrammi al secondo (fps); in Europa sono invece ripresi a 25 fps. I film sono ripresi a 24 fps.

Scegliete un predefinito di codifica video con un valore fps pari a quello del file video principale. Ad esempio, se il video principale ha una frequenza fotogrammi di 25 fps, scegliete un predefinito di codifica a 25 fps. Per impostazione predefinita, per tutte le codifiche personalizzate viene usato lo stesso valore fps del file video principale. Quando create un predefinito di codifica video non è pertanto necessario specificare l’impostazione fps.

### Dimensioni di codifica video {#video-encoding-dimensions}

Per ottenere risultati ottimali, selezionate dimensioni di codifica tali che il video sorgente sia un multiplo intero di tutti i video codificati.

Per calcolare questo rapporto, dividete la larghezza sorgente per la larghezza codificata per ottenere il rapporto di larghezza. Quindi, dividete l’altezza sorgente per l’altezza codificata per ottenere il rapporto di altezza.

Se il rapporto risultante è un numero intero, il video viene ridimensionato in scala in modo ottimale. Se il rapporto risultante non è un numero intero, questo può influire sulla qualità del video e generare artefatti di pixel superflui sul display, particolarmente evidente nel caso di video con testo.

Ad esempio, supponete che il video sia di 1920x1080. Nella tabella seguente, i tre video codificati forniscono impostazioni di codifica ottimali.

| Tipo di video | Larghezza x altezza | Rapporto larghezza | Rapporto altezza |
|--- |--- |--- |--- |
| Sorgente | 1920x1080 | 1 | 1 |
| Codificato | 960x540 | 2 | 2 |
| Codificato | 640x360 | 3 | 3 |
| Codificato | 480x270 | 4 | 4 |

### Formato di file video codificato {#encoded-video-file-format}

Adobe Dynamic Media Classic consiglia di utilizzare i predefiniti di codifica video MP4 H.264. Poiché i file MP4 utilizzano il codec video H.264, il video è di alta qualità ma la dimensione file è comunque ridotta.

## Utilizzo dei predefiniti di codifica video {#working-with-video-encoding-presets}

I file video principali creati con le apparecchiature di produzione video e con un software per la modifica di video sono spesso troppo grandi e in formato errato per essere riprodotti in destinazioni online. Per convertire i video digitali nel formato e nelle specifiche corretti per la riproduzione su diversi schermi, potete *transcodificare* i file video (un processo noto anche come *codifica*). Durante il processo di codifica, il video viene compresso per ridurne le dimensioni e ottimizzarlo per la riproduzione sul Web e dispositivi mobili.

Consultate [Caricamento e codifica dei video](uploading-encoding-videos.md#uploading-and-encoding-videos).

Dynamic Media Classic offre una libreria di predefiniti di codifica video che riflettono le impostazioni di codifica più comuni utilizzate attualmente. Questi predefiniti di codifica sono stati ottimizzati per la riproduzione sugli schermi di destinazione. Inoltre, gli amministratori possono creare predefiniti di codifica video con proprie impostazioni di codifica, in base alla dimensione e alla qualità di riproduzione dei video presentata agli utenti finali. Tutti i predefiniti di codifica video, preconfigurati da Dynamic Media Classic o personalizzati, producono video in formato MP4.

Nella schermata Predefiniti video, gli amministratori possono impostare e gestire la codifica video. Possono effettuare le seguenti operazioni:

* Attivare e disattivare i predefiniti di codifica video
* Creare un predefinito di codifica video
* Modificare i predefiniti di codifica video.
* Eliminare i predefiniti per video

Tutti i video caricati in Dynamic Media Classic o codificati in Dynamic Media Classic vengono trattati come &quot;video&quot;. In altre parole potete trasmettere i video da riprodurre su computer desktop, dispositivi mobili o entrambi. Ad esempio, puoi visualizzare in anteprima questi tipi di video in Dynamic Media Classic. Potete inoltre generare URL (mediante la funzione Copia URL) e codice da incorporare (mediante la funzione Incorpora codice) da usare per lettori video, siti Web e così via.

Consultate [Anteprima dei video in un visualizzatore video](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Consultate [Collegamento di un URL per video a un sito mobile o a un sito Web](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Consultate [Incorporamento di un visualizzatore video in una pagina Web](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Per le risorse video caricate e codificate in Dynamic Media Classic, il video viene distribuito nel seguente formato di file:

**MP4 H.264** Utilizza i file MP4 per i seguenti elementi:

* Streaming dinamico HTTP su desktop.
* HLS (HTTP Live Streaming, protocollo di streaming Apple).
* Distribuzione progressiva di video su dispositivi mobili Android™, BlackBerry® e Windows®.

Qualsiasi altro formato video e codec viene trattato come un &quot;video principale&quot;. ossia come file video sorgente che non può essere utilizzato per la riproduzione su computer desktop o dispositivi mobili. Ad esempio, non puoi visualizzare in anteprima questi tipi di video in Dynamic Media Classic. Non potete inoltre generare URL da copiare e codice da incorporare e da usare per lettori video, siti Web e così via.

### Applicazione di filtri all’elenco di predefiniti di codifica video {#filtering-the-list-of-video-encoding-presets}

La pagina Predefiniti video e la pagina Predefiniti video adattivi sono costituite da una tabella che elenca lo stato attivo, il nome del predefinito, il dispositivo di riproduzione previsto, le dimensioni del video e la velocità dati di ciascun predefinito video.

Per regolare l’elenco potete scegliere Entrambi, Attivo o Inattivo per visualizzare tutti i predefiniti per video o limitare l’elenco ai soli predefiniti attivi o inattivi.

Potete anche scegliere un’opzione per il dispositivo di riproduzione e limitare così l’elenco ai soli predefiniti per video creati per la riproduzione di video per tutti i dispositivi, per computer desktop, per dispositivi mobili o per tablet.

**Per filtrare l’elenco dei predefiniti di codifica video:**

1. In Dynamic Media Classic, nella barra di navigazione globale, fate clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti video]** > **[!UICONTROL Predefiniti video adattivi]** o **[!UICONTROL Predefiniti di codifica singola]**.

   Le pagine Predefiniti per video adattivi e Predefiniti codifica singola includono una tabella che elenca lo stato Attivo, il nome del predefinito, il dispositivo di riproduzione previsto, le dimensioni video e la velocità dati di ciascun predefinito video.

1. Nella pagina Predefiniti codifica singola denominata Predefiniti video, nella barra degli strumenti Predefiniti video, utilizzate i due elenchi a discesa per definire l’elenco dei predefiniti riportato nella tabella in base allo stato Attivo e al dispositivo di riproduzione.

   * Nel primo elenco a discesa, più stretto, scegliete **[!UICONTROL Entrambi]** per vedere tutti i predefiniti per video, oppure scegliete **[!UICONTROL Attivo]** o **[!UICONTROL Inattivo]** per visualizzare solo i predefiniti per video con lo stato Attivo o Inattivo.
   * Nel secondo elenco a discesa, più largo, scegliete un’opzione per il dispositivo di riproduzione in modo da limitare l’elenco ai soli predefiniti per video creati per la riproduzione di video per computer desktop oppure per dispositivi mobili o tablet.

### Attivazione o disattivazione dei predefiniti di codifica video {#activating-or-deactivating-video-encoding-presets}

I predefiniti per video attivati vengono visualizzati nella finestra di dialogo Opzioni processo di caricamento La finestra di dialogo viene visualizzata quando un utente carica file video durante il processo di caricamento. L’utente può quindi scegliere tra tutti i predefiniti di codifica attivati.

1. In Dynamic Media Classic, nella barra di navigazione globale, fate clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti video]**.
1. Effettuate una delle seguenti operazioni:

   * Fate clic su **[!UICONTROL Predefiniti video adattati]**.
   * Fate clic su **[!UICONTROL Predefiniti codifica singola]**.

1. Effettuate una delle seguenti operazioni:

   * Per attivare un predefinito per video, nella pagina dei predefiniti, selezionate la casella accanto al nome di un predefinito nella colonna Attivo.
   * Per disattivare un predefinito per video, deselezionate la casella accanto al predefinito per video da rendere inattivo.

      >[!NOTE]
      >
      >I predefiniti per video disattivati non vengono elencati nella finestra di dialogo Opzioni processo di caricamento.

1. Nell’angolo in basso a destra della pagina, fate clic su **[!UICONTROL Chiudi]**.

### Aggiunta o modifica di un predefinito di codifica video {#adding-or-editing-a-video-encoding-preset}

Potete creare dei predefiniti per video con codifica singola personalizzati e aggiungerli alla tabella Predefiniti per video. È inoltre possibile modificare i predefiniti video con codifica singola predefiniti forniti con Dynamic Media Classic, purché venga salvato il predefinito modificato con un nuovo nome.

Dynamic Media Classic ha impostato limiti massimi per la velocità dei dati di destinazione, l&#39;altezza della risoluzione e la larghezza della risoluzione per garantire un&#39;esperienza di riproduzione corretta. Se superate questi limiti, vengono visualizzati alcuni messaggi di avvertenza:

* Per la riproduzione su computer, i limiti sono: (larghezza/16) * (altezza/16) &lt; 8192. 
* Per la riproduzione sui dispositivi mobili, i limiti sono: (larghezza/16) * (altezza/16) &lt; 660; frequenza dati di destinazione &lt; 4000. 
* Per la riproduzione sui tablet, i limiti sono: (larghezza/16) * (altezza/16) &lt; 3600.

**Per aggiungere o modificare un predefinito di codifica video:**

1. In Dynamic Media Classic, nella barra di navigazione globale, fate clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti video]**.
1. Fate clic su **[!UICONTROL Predefiniti codifica singola]**.
1. Nella pagina Predefiniti per video, effettuate una delle seguenti operazioni:

   * Nella barra degli strumenti Predefiniti video, fai clic su **[!UICONTROL Aggiungi]** per aggiungere un predefinito video.
   * Selezionate un predefinito per video. Nella barra degli strumenti, fate clic su **[!UICONTROL Modifica]**.

      Non è possibile modificare i predefiniti di Dynamic Media Classic; puoi creare un predefinito solo da uno esistente scegliendo **[!UICONTROL Salva con nome]**.

1. Nella pagina Aggiungi predefinito video o Modifica predefinito video, impostate le opzioni Predefinito per video desiderate.

   Per informazioni sulle impostazioni consigliate, consultate [Procedure ottimali per la codifica video](uploading-encoding-videos.md#best-practices-for-video-encoding).

   | Opzione Predefinito per video | Descrizione |
   |--- |--- |
   | Nome predefinito | Inserite un nome descrittivo per il predefinito per video. Il nome inserito verrà visualizzato nella finestra di dialogo Opzioni processo di caricamento, nella quale gli utenti scelgono le opzioni di transcodifica. |
   | Descrizione | Descrivete il predefinito per video. Il contenuto immesso viene visualizzato come descrizione quando si sposta il puntatore sul nome del predefinito nella finestra di dialogo Opzioni processo di caricamento, in cui gli utenti scelgono le opzioni di transcodifica. |
   | Dispositivo di riproduzione | Scegliete il dispositivo su cui riprodurre il video. Le opzioni sono Computer (desktop), Mobile (iPhone, iPad, Android™); o Tablet (solo iPad). Questa impostazione determina automaticamente il codec video e audio appropriato utilizzato durante la codifica. |
   | Velocità dati di destinazione | Inserite una velocità di connessione Internet media (in kilobit al secondo) dell’utente finale di destinazione. Potete inserire il valore desiderato oppure trascinare il cursore per impostarlo. La gamma di velocità di connessione utente indica le velocità tipiche per connessioni banda larga, DSL, mobile e mediante modem. Questa impostazione determina automaticamente la velocità di dati audio e video combinata, ossia la quantità di dati codificati necessaria per creare un secondo di riproduzione video. Più alta è la velocità dati, migliore sarà la qualità del video. Tuttavia, valori di velocità dati elevati aumentano le dimensioni dei file a scapito dell’esperienza di visualizzazione degli utenti che dispongono di una larghezza di banda ridotta. Si consiglia quindi di trovare un compromesso tra valori di velocità dati elevati e ridotti. Mirate a creare un’esperienza di riproduzione con qualità adeguata, senza limitare gli utenti con larghezze di banda ridotte. |
   | Proporzioni | Le proporzioni sono il rapporto tra la larghezza e l’altezza del video. Le prime due proporzioni elencate di seguito sono comunemente utilizzate per visualizzare video in orizzontale:<ul><li> 4:3 - Usata per quasi tutti i contenuti di trasmissione TV con definizione standard.</li><li>16:9 - Usata per quasi tutti i contenuti e filmati TV ad alta definizione (HDTV) in formato widescreen.</li><li>Scala automatica (impostazione predefinita) - Per creare video da distribuire a dispositivi mobili, tablet e computer desktop; predefinito codifica singola che funziona con qualsiasi proporzione. I video sorgente caricati e codificati con questo predefinito sono impostati su un’altezza specifica. Tuttavia, il valore della larghezza viene ridimensionato automaticamente per mantenere le proporzioni del video (rapporto larghezza per altezza).</li><li>Personale - Usata quando si desidera definire una dimensione video non standard.</li><li>Le proporzioni scelte determinano le impostazioni di larghezza e altezza per Dimensione risoluzione; i valori di larghezza e altezza vengono automaticamente modificati in base alle proporzioni corrette.</li></ul> |
   | Dimensione risoluzione | La dimensione della risoluzione, espressa dal numero di pixel di larghezza per il numero di pixel di altezza, determina la dimensione. Potete inserire i valori di larghezza e altezza in pixel oppure trascinare il relativo cursore per impostarli. La gamma di risoluzioni elenca le dimensioni di risoluzioni tipiche. I valori di larghezza e altezza aderiscono automaticamente alle proporzioni selezionate. Ad esempio, se selezionate 4:3 come proporzione e inserite 400 per la larghezza, 300 viene inserito automaticamente per l’altezza. Se per le proporzioni avete selezionato Scala automatica, il valore Larghezza di Dimensione risoluzione viene impostato automaticamente su Auto. Fai clic su Anteprima per aprire una finestra del browser e vedere le scelte relative alla risoluzione. |
   | Suffisso file codifica | Inserite un suffisso. Questo suffisso viene aggiunto al file video codificato. Potete inserire un trattino o un trattino basso nel nome; gli spazi bianchi e i caratteri speciali non sono consentiti. |
   | Altre impostazioni | Dynamic Media Classic determina automaticamente tutte le altre impostazioni di codifica in base alle linee guida per la codifica best practice. |

1. Effettuate una delle seguenti operazioni:

   * Fate clic su **[!UICONTROL Salva]** se avete aggiunto o modificato un predefinito per video.
   * Fate clic su **[!UICONTROL Salva con nome]** se avete aggiunto un predefinito per video a partire da un predefinito esistente.

### Eliminazione un predefinito di codifica video {#deleting-a-video-encoding-preset}

Gli amministratori possono eliminare i predefiniti per video personalizzati. I predefiniti video forniti con Dynamic Media Classic non possono essere eliminati.

1. In Dynamic Media Classic, nella barra di navigazione globale, fate clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti video]**.
1. Fate clic su **[!UICONTROL Predefiniti codifica singola]**.
1. Nella pagina Predefiniti per video, selezionate nella tabella il predefinito per video da eliminare.
1. Nella barra degli strumenti dei predefiniti per video, fate clic su **[!UICONTROL Elimina]**.
1. Nella finestra di dialogo Elimina predefinito, fate clic su **[!UICONTROL Elimina]**.

>[!MORELIKETHIS]
>
>* [Avvio rapido: video](quick-start-video.md#quick-start-video)
* [Caricamento e codifica dei video](uploading-encoding-videos.md#uploading-and-encoding-videos)
* [Utilizzo dei predefiniti per visualizzatori video](previewing-videos-video-viewer.md#working-with-video-viewer-presets)

