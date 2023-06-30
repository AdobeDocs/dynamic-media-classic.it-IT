---
title: Caricare e codificare i video
description: Scopri come caricare e codificare i video in Adobe Dynamic Media Classic.
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '3967'
ht-degree: 56%

---

# Caricare e codificare i video{#uploading-and-encoding-videos}

Per creare un singolo video o set di video adattivi da distribuire sul web o sui dispositivi mobili, carica innanzitutto i file video principali su Adobe Dynamic Media Classic. Adobe Dynamic Media Classic codifica i video in formato MP4 e pubblica i video nei seguenti formati:

* **MP4** - Adobe Dynamic Media Classic consiglia MP4 come formato di file video preferito. Utilizzate i file MP4 per le seguenti operazioni:

   * Streaming dinamico HTTP su desktop.
   * Streaming dinamico HTTP (protocollo di streaming Apple).
   * Consegna video progressiva a dispositivi mobili Android™, BlackBerry® e Windows®

  Adobe Dynamic Media Classic offre due flussi di lavoro per il caricamento di file video:

* **Video precodificati** - Caricate i file MP4 direttamente su Adobe Dynamic Media Classic. Con questo flusso di lavoro, i file non vengono codificati durante il caricamento. I file vengono precodificati durante la preparazione per la visualizzazione sul desktop e sui dispositivi mobili.

* **Video sorgente principale** : carica i file video sorgente primari e, al momento del caricamento, li codifica in file MP4. Nel pannello Sfoglia, i video codificati sono etichettati “Video”. Adobe Dynamic Media Classic supporta la codifica di file video in molti formati.

   * Assicurati che i file video sorgente principali che desideri codificare siano supportati.

     Consultate [Tipi di file video supportati per la codifica](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

   * Scegliete un predefinito di codifica video.

     Consultate [Predefiniti video per la codifica di file video](application-setup.md#video-presets-for-encoding-video-files).

     Consultate [Procedure ottimali per la codifica video](uploading-encoding-videos.md#best-practices-for-video-encoding).

Adobe Dynamic Media Classic genera anche le miniature video. Per ulteriori informazioni sulle miniature video, su come ottenerne gli URL e come modificare i fotogrammi poster,

Consulta [Operazioni con le miniature video](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Per caricare e codificare i video:**

Effettuate una delle seguenti operazioni.

*Se i video sono stati già codificati*

1. Sulla barra di navigazione globale, seleziona **[!UICONTROL Carica]**.
1. Nella pagina Carica, seleziona **[!UICONTROL Da desktop]** scheda.
1. Nella pagina Carica, in **[!UICONTROL Seleziona i file da caricare]** pannello, seleziona **[!UICONTROL Sfoglia]**, passare a un file video MP4, quindi selezionare **[!UICONTROL Apri]**.
1. In **[!UICONTROL Scegliete la destinazione della cartella]** selezionare una cartella per il file caricato.
1. Nella pagina Carica, assicurati che **[!UICONTROL Pubblica dopo il caricamento]** è selezionato.
1. Seleziona **[!UICONTROL Invia caricamento]**.

*Se desideri codificare i video utilizzando Adobe Dynamic Media Classic*

1. Sulla barra di navigazione globale, seleziona **[!UICONTROL Carica]**.
1. Nella pagina Carica, seleziona **[!UICONTROL Da desktop]** scheda.
1. In **[!UICONTROL Seleziona i file da caricare]** pannello, seleziona **[!UICONTROL Sfoglia]**, passare a un file video di origine principale, quindi selezionare **[!UICONTROL Apri]**.
1. In **[!UICONTROL Scegliete la destinazione della cartella]** selezionare una cartella per il file caricato.
1. Nell’angolo inferiore destro della pagina, seleziona **[!UICONTROL Opzioni processo]**,
1. Nella finestra di dialogo Opzioni processo di caricamento, espandi **[!UICONTROL Opzioni eVideo]**, quindi eseguire una delle operazioni seguenti:

   * Si consiglia di selezionare **[!UICONTROL Codifica video adattiva]**. Consultate [Video adattivo (predefinito)](application-setup.md#adaptive-video-default).
   * Facoltativo. Per utilizzare le singole impostazioni di codifica, espandere **[!UICONTROL Predefiniti codifica singola]**, quindi selezionare le opzioni di codifica desiderate per Desktop, Mobile e Tablet.
Consultate [Predefiniti di codifica video per computer desktop](application-setup.md#desktop-video-encoding-presets), [Predefiniti di codifica per video per dispositivi mobili](application-setup.md#mobile-video-encoding-presets), [Predefiniti di codifica per video per tablet](application-setup.md#tablet-video-encoding-presets).
1. Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Salva]**.
1. Nella pagina Carica, assicurati che **[!UICONTROL Pubblica dopo il caricamento]** è selezionato.
1. Nella pagina Carica, nell’angolo inferiore destro, seleziona **[!UICONTROL Invia caricamento]**.

*Se desiderate ricodificare un file video precedentemente caricato*

1. In Adobe Dynamic Media Classic, nel pannello Sfoglia, individua il video e selezionalo.
1. Vai a **[!UICONTROL File]** > **[!UICONTROL Rielabora]**.
1. Nella finestra di dialogo Rielabora risorse espandere **[!UICONTROL Opzioni eVideo]**, quindi eseguire una delle operazioni seguenti:
   * Come procedura ottimale, si consiglia di utilizzare il metodo seguente. Selezionate **Video adattivo**. Consultate [Video adattivo (predefinito)](application-setup.md#adaptive-video-default).
   * Facoltativo. Per utilizzare le singole impostazioni di codifica, espandere **[!UICONTROL Predefiniti codifica singola]**, quindi selezionare le opzioni di codifica desiderate per Desktop, Mobile e Tablet.
Consultate [Predefiniti di codifica video per computer desktop](application-setup.md#desktop-video-encoding-presets), [Predefiniti di codifica per video per dispositivi mobili](application-setup.md#mobile-video-encoding-presets), [Predefiniti di codifica per video per tablet](application-setup.md#tablet-video-encoding-presets).
1. Nella finestra di dialogo Rielabora risorse, seleziona **[!UICONTROL Invia]**.

Quando utilizzate un predefinito di codifica per video adattivi oppure più predefiniti di codifica singola, viene creato automaticamente un set di video adattivi con più codifiche video. Potete anche creare manualmente un set di video adattivi, selezionando i singoli video.

Quando generate un set di video adattivi automaticamente o manualmente vengono creati solo i tipi di file MP4 e M4V.

## Tipi di file video supportati per la codifica {#supported-video-file-types-for-encoding}

La seguente tabella indica i tipi di file video (con i codec video consentiti) che potete codificare in formato MP4 o OGV quando caricate i file. La tabella elenca i formati file e i codec:

* **Formati di file video** - Analogamente a un file ZIP, un formato di file video determina il modo in cui i file sono contenuti nel file video. Generalmente, un file video contiene più tracce (una traccia video senza audio e una o più tracce audio senza video) che vengono associate e sincronizzate. Il formato file del video determina come le diverse tracce di dati e metadati vengono organizzate.

* **Codec video** - Un codec video descrive l&#39;algoritmo di codifica di un video. Un lettore video decodifica il video in base al relativo codec, quindi visualizza una serie di immagini o fotogrammi sullo schermo. I codec riducono la quantità di informazioni richieste dai file video per memorizzare e riprodurre il video. Invece delle informazioni su ciascun fotogramma, vengono memorizzate solo le informazioni relative alle differenze tra l’uno e l’altro. Poiché la maggior parte dei video cambia poco da un fotogramma all&#39;altro, i codec consentono tassi di compressione elevati, che si traducono in dimensioni di file più piccole.

  | Formato file video | Codec video |
  | --- | --- |
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
  >La schermata Processi invia una notifica se caricate e tentate di codificare un file video e il file viene rifiutato perché contiene un codec o un contenitore file incompatibile. Per ulteriori informazioni, consulta [Verifica file di processo](checking-job-files.md).

## Best practice per la codifica video {#best-practices-for-video-encoding}

Di seguito sono riportati alcuni suggerimenti sulle best practice per la codifica di file video sorgente in Adobe Dynamic Media Classic.

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### File video sorgente {#source-video-files}

Per la codifica di un file video, occorre usare un file video sorgente della massima qualità possibile. Evitate di usare file video precedentemente codificati in quanto sono già compressi e un’ulteriore codifica causerebbe il deterioramento della qualità del video.

Nella tabella seguente vengono descritte le dimensioni, le proporzioni e la velocità bit minima consigliate per i file video sorgente durante la codifica:

| Dimensioni | Proporzioni | Bitrate minimo |
| --- | --- | --- |
| 1024x768 | 4:3 | 4500 Kbps per la maggior parte dei video. |
| 1280x720 | 16:9 | 3000 - 6000 Kbps, a seconda della quantità di movimento presente del video. |
| 1920x1080 | 16:9 | 6000 - 8000 Kbps, a seconda della quantità di movimento presente del video. |

### Ottenere i metadati di un file {#obtaining-a-file-s-metadata}

Puoi ottenere i metadati di un file visualizzandone i metadati in Adobe Dynamic Media Classic, utilizzando uno strumento di modifica video o un’applicazione progettata per ottenere i metadati. Seguono istruzioni per l’utilizzo di MediaInfo, un’applicazione di terze parti che consente di ottenere i metadati di un file video:

1. Vai a questa pagina Web: [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo).
1. Selezionate e scaricate il programma di installazione per la versione GUI, quindi seguite le istruzioni di installazione.
1. Dopo l&#39;installazione, fare clic con il pulsante destro del mouse sul file video (solo Windows®) e selezionare MediaInfo, oppure aprire MediaInfo e trascinare il file video nell&#39;applicazione. Potete vedere tutti i metadati associati al file video, inclusi i valori di larghezza, altezza e fotogrammi al secondo.

### Proporzioni {#aspect-ratio}

Quando scegliete o create un predefinito di codifica video per il file video principale, accertatevi che il predefinito abbia le stesse proporzioni del file video principale. Le *proporzioni* sono il rapporto tra la larghezza e l’altezza del video. 

Per determinare le proporzioni di un file video, ottieni i metadati del file e annota la larghezza e l’altezza del file (consulta [Ottenere i metadati di un file](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Quindi applicate questa formula per determinare le proporzioni:

larghezza/altezza = proporzioni

Nella tabella che segue, i risultati della formula vengono correlati alle relative scelte di proporzioni più comuni:

| Risultato della formula | Proporzioni |
| --- | --- |
| 1,33 | 4:3 |
| 0,75 | 3:4 |
| 1,78 | 16:9 |
| 0,56 | 9:16 |

Ad esempio, un video con larghezza 1440 x altezza 1080 ha proporzioni 1440/1080 o 1,33. In questo caso, scegliete un predefinito di codifica video con proporzioni 4:3 per codificare il file video.

### Velocità dati {#data-rate}

Per *velocità dati* (o *bitrate*) si intende la quantità di dati che vengono codificati per ottenere un secondo di riproduzione video. La velocità dati è misurata in kilobit al secondo (Kbps).

>[!NOTE]
>
>poiché tutti i codec usano metodi di compressione con perdita di dati, la velocità dati è il fattore che influisce maggiormente sulla qualità video. Con la compressione con perdita di dati, infatti, a una maggiore compressione di un file video corrisponde un maggior degrado della qualità. Per questa ragione, a parità di tutte le altre caratteristiche (risoluzione, frequenza fotogrammi e codec), una velocità dati inferiore genera file compressi di qualità inferiore.

Quando scegli un predefinito di codifica video, ricorda di tenere conto della velocità di connessione dell’utente finale target. Scegli un predefinito con una velocità dati pari all’80% di quella velocità. Ad esempio, se la connessione dell’utente finale è di 1000 Kbps, scegliete un predefinito con velocità dati video di 800 Kbps.

La tabella di seguito riporta la velocità dati per velocità di connessioni tipiche.

| Velocità (Kbps) | Tipo di connessione  |
| --- | --- |
| 256 | Connessione via modem. |
| 800 | Connessione mobile tipica. Per questa connessione, scegliete una velocità dati di circa 400, con un massimo di 800 per esperienze 3G. |
| 2000 | Connessione desktop tipica a banda larga. Per questa connessione, eseguire il targeting di una velocità di dati nell&#39;intervallo 800-2000 Kbps, con la maggior parte delle destinazioni in media 1200-1500 Kbps. |
| 5000 | Connessione a banda larga elevata tipica. Non si consiglia di applicare la codifica per questo valore elevato, in quanto la maggior parte dei clienti non dispone di trasmissione video di tale velocità.  |

### Risoluzione {#resolution}

La *Risoluzione* descrive l’altezza e la larghezza di un file video, in pixel. La maggior parte delle sorgenti video è memorizzata ad alta risoluzione (ad esempio, 1920x1080). Per lo streaming, il video sorgente viene compresso in una risoluzione inferiore (per un valore massimo di 640x480).

La risoluzione e la velocità dati sono due fattori strettamente correlati da cui dipende la qualità video. Per mantenere la stessa qualità video, più elevato è il numero di pixel in un file video (ossia più elevata è la risoluzione), più elevata deve essere anche la velocità dati. Ad esempio, considerate il numero di pixel per fotogramma in due file video, rispettivamente con risoluzione 320x240 e 640x480:

| Risoluzione | Pixel per fotogramma |
| --- | --- |
| 320x240 | 76.800 |
| 640x480 | 307.200 |

Il file da 640x480 ha quattro volte il numero di pixel per fotogramma. Per ottenere la stessa velocità dati per queste due risoluzioni, occorre applicare una compressione quattro volte maggiore al file da 640x480, riducendone quindi la qualità video. Di conseguenza. una velocità dati video pari a 250 Kbps produce risultati di alta qualità a una risoluzione di 320x240, ma non a una risoluzione di 640x480.

>[!NOTE]
>
>In generale, maggiore è la velocità di dati utilizzata, migliore è la visualizzazione del video e maggiore è la risoluzione utilizzata, maggiore è la velocità di dati da mantenere la qualità di visualizzazione (rispetto a risoluzioni inferiori).

Data la correlazione tra risoluzione e velocità dati, per la codifica video è possibile considerare due opzioni:

* Scegli una velocità dati e quindi codificala alla risoluzione più alta che appare migliore alla velocità dati scelta.
* Scegliere una risoluzione e quindi effettuare la codifica con una velocità dati tale da produrre video di alta qualità per la risoluzione scelta.

Quando scegli (o crei) un predefinito di codifica video per il file video principale, utilizza questa tabella per impostare la risoluzione corretta:

| Risoluzione | Altezza (pixel) | Dimensione schermo |
| --- | --- | --- |
| 240p | 240 | Schermo molto piccolo |
| 300p | 300 | Schermo piccolo tipico per dispositivi mobili |
| 360p | 360 | Schermo piccolo |
| 480p | 480 | Schermo medio |
| 720p | 720 | Schermo grande |
| 1080p | 1080 | Schermo grande ad alta definizione |

### Fps (fotogrammi al secondo) {#fps-frames-per-second}

Negli Stati Uniti e in Giappone, i video sono in genere ripresi a 29,97 fotogrammi al secondo (fps); in Europa sono invece ripresi a 25 fps. I film sono ripresi a 24 fps.

Scegli un predefinito di codifica video che corrisponda alla velocità fps del file video principale. Ad esempio, se il video principale è a 25 fps, scegliete un predefinito di codifica con 25 fps. Per impostazione predefinita, tutta la codifica personalizzata utilizza il fps del file video principale. Quando create un predefinito di codifica video non è pertanto necessario specificare l’impostazione fps.

### Dimensioni di codifica video {#video-encoding-dimensions}

Per ottenere risultati ottimali, selezionate dimensioni di codifica tali che il video sorgente sia un multiplo intero di tutti i video codificati.

Per calcolare questo rapporto, dividete la larghezza sorgente per la larghezza codificata per ottenere il rapporto di larghezza. Quindi, dividete l’altezza sorgente per l’altezza codificata per ottenere il rapporto di altezza.

Se il rapporto risultante è un numero intero, il video viene ridimensionato in scala in modo ottimale. Se il rapporto risultante non è un numero intero, questo può influire sulla qualità del video e generare artefatti di pixel superflui sul display, particolarmente evidente nel caso di video con testo.

Ad esempio, supponete che il video sia di 1920x1080. Nella tabella seguente, i tre video codificati forniscono impostazioni di codifica ottimali.

| Tipo di video | Larghezza x altezza | Rapporto larghezza | Rapporto altezza |
| --- | --- | --- | --- |
| Sorgente | 1920x1080 | 1 | 1 |
| Codificato | 960x540 | 2 | 2 |
| Codificato | 640x360 | 3 | 3 |
| Codificato | 480x270 | 4 | 4 |

### Formato di file video codificato {#encoded-video-file-format}

Adobe Dynamic Media Classic consiglia di utilizzare i predefiniti di codifica video MP4 H.264. Poiché i file MP4 utilizzano il codec video H.264, il video è di alta qualità ma la dimensione file è comunque ridotta.

## Utilizzare i predefiniti di codifica video {#working-with-video-encoding-presets}

I file video primari creati con apparecchiature di produzione video e software di editing video sono spesso troppo grandi e non sono nel formato corretto per la consegna a destinazioni online. Per convertire i video digitali nel formato e nelle specifiche corretti per la riproduzione su diversi schermi, potete *transcodificare* i file video (un processo noto anche come *codifica*). Durante il processo di codifica, il video viene compresso per ridurne le dimensioni e ottimizzarlo per la riproduzione sul Web e dispositivi mobili.

Consulta [Caricare e codificare i video](uploading-encoding-videos.md#uploading-and-encoding-videos).

Adobe Dynamic Media Classic offre una libreria di predefiniti di codifica video che riflettono le impostazioni di codifica più comuni attualmente in uso. Questi predefiniti di codifica sono stati ottimizzati per la riproduzione sugli schermi di destinazione. Inoltre, gli amministratori possono creare predefiniti di codifica video con proprie impostazioni di codifica, in base alla dimensione e alla qualità di riproduzione dei video presentata agli utenti finali. Tutti i predefiniti di codifica video, preconfigurati da Adobe Dynamic Media Classic o personalizzati, producono video in formato MP4.

Nella schermata Predefiniti video, gli amministratori possono impostare e gestire la codifica video. Possono effettuare le seguenti operazioni:

* Attivare e disattivare i predefiniti di codifica video
* Creare un predefinito di codifica video
* Modificare i predefiniti di codifica video.
* Eliminare i predefiniti per video

Qualsiasi video caricato su Adobe Dynamic Media Classic o che codifichi in Adobe Dynamic Media Classic viene considerato come &quot;video&quot;. In altre parole potete trasmettere i video da riprodurre su computer desktop, dispositivi mobili o entrambi. Ad esempio, puoi visualizzare in anteprima questi tipi di video in Adobe Dynamic Media Classic. Potete inoltre generare URL (mediante la funzione Copia URL) e codice da incorporare (mediante la funzione Incorpora codice) da usare per lettori video, siti Web e così via.

Consulta [Anteprima di video in un visualizzatore video](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Consulta [Collegare l’URL di un video a un sito mobile o a un sito web](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Consulta [Incorporare il visualizzatore video in una pagina web](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Per le risorse video caricate e codificate in Adobe Dynamic Media Classic, il video viene consegnato nel seguente formato di file:

**MP4 H.264** Utilizzare file MP4 per:

* Streaming dinamico HTTP su desktop.
* HLS (HTTP Live Streaming, protocollo di streaming di Apple).
* Consegna video progressiva a dispositivi mobili Android™, BlackBerry® e Windows®.

Qualsiasi altro formato video e codec viene considerato come un &quot;Video primario&quot;. ossia come file video sorgente che non può essere utilizzato per la riproduzione su computer desktop o dispositivi mobili. Ad esempio, non è possibile visualizzare in anteprima questi tipi di video in Adobe Dynamic Media Classic. Non potete inoltre generare URL da copiare e codice da incorporare e da usare per lettori video, siti Web e così via.

### Filtrare l’elenco dei predefiniti di codifica video {#filtering-the-list-of-video-encoding-presets}

Le pagine Predefiniti video e Predefiniti video adattivi sono costituite da una tabella che elenca lo stato attivo, il nome del predefinito, il dispositivo di riproduzione desiderato, le dimensioni del video e la velocità dati di ciascun predefinito video.

Per regolare l’elenco potete scegliere Entrambi, Attivo o Inattivo per visualizzare tutti i predefiniti per video o limitare l’elenco ai soli predefiniti attivi o inattivi.

Potete anche scegliere un’opzione per il dispositivo di riproduzione e limitare così l’elenco ai soli predefiniti per video creati per la riproduzione di video per tutti i dispositivi, per computer desktop, per dispositivi mobili o per tablet.

**Per filtrare l’elenco dei predefiniti di codifica video:**

1. In Adobe Dynamic Media Classic, nella barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti per video]** > **[!UICONTROL Predefiniti video adattivo]** o **[!UICONTROL Predefiniti codifica singola]**.

   Le pagine dei predefiniti per video adattivo e dei predefiniti a codifica singola includono una tabella che elenca lo stato attivo, il nome del predefinito, il dispositivo di riproduzione desiderato, le dimensioni video e la velocità dati di ciascun predefinito video.

1. Nella pagina Predefiniti codifica singola denominata Predefiniti video, nella barra degli strumenti Predefiniti video, utilizzate i due elenchi a discesa per definire l’elenco dei predefiniti riportato nella tabella in base allo stato Attivo e al dispositivo di riproduzione.

   * Nel primo elenco a discesa, più stretto, scegliete **[!UICONTROL Entrambi]** per vedere tutti i predefiniti per video, oppure scegliete **[!UICONTROL Attivo]** o **[!UICONTROL Inattivo]** per visualizzare solo i predefiniti per video con lo stato Attivo o Inattivo.
   * Nel secondo elenco a discesa, più largo, scegliete un’opzione per il dispositivo di riproduzione in modo da limitare l’elenco ai soli predefiniti per video creati per la riproduzione di video per computer desktop oppure per dispositivi mobili o tablet.

### Attivare o disattivare i predefiniti di codifica video {#activating-or-deactivating-video-encoding-presets}

I predefiniti per video attivati vengono visualizzati nella finestra di dialogo Opzioni processo di caricamento La finestra di dialogo viene visualizzata quando un utente carica file video durante il processo di caricamento. L’utente può quindi scegliere tra tutti i predefiniti di codifica attivati.

1. In Adobe Dynamic Media Classic, nella barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti per video]**.
1. Effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Predefiniti video adattivo]**.
   * Seleziona **[!UICONTROL Predefiniti codifica singola]**.

1. Effettuate una delle seguenti operazioni:

   * Per attivare un predefinito per video, nella pagina dei predefiniti, selezionate la casella accanto al nome di un predefinito nella colonna Attivo.
   * Per disattivare un predefinito per video, deselezionate la casella accanto al predefinito per video da rendere inattivo.

     >[!NOTE]
     >
     >I predefiniti per video disattivati non vengono elencati nella finestra di dialogo Opzioni processo di caricamento.

1. Nell’angolo inferiore destro della pagina, seleziona **[!UICONTROL Chiudi]**.

### Aggiungere o modificare un predefinito di codifica video {#adding-or-editing-a-video-encoding-preset}

Potete creare predefiniti video personalizzati con codifica singola e aggiungerli alla tabella Predefiniti video. È inoltre possibile modificare qualsiasi predefinito per video a codifica singola predefinito fornito con Adobe Dynamic Media Classic, a condizione di salvare il predefinito modificato con un nuovo nome.

Adobe Dynamic Media Classic ha impostato i limiti massimi per la velocità dati di destinazione, l’altezza della risoluzione e la larghezza della risoluzione per garantire un’esperienza di riproduzione corretta. Se superate questi limiti, vengono visualizzati alcuni messaggi di avvertenza:

* Per la riproduzione da computer, i limiti sono: (Larghezza/16) &#42; (Altezza/16) &lt; 8192.
* Per la riproduzione mobile, i limiti sono: (Larghezza/16) &#42; (Altezza/16) &lt; 660; velocità dati target &lt; 4000.
* Per la riproduzione del tablet, i limiti sono: (Larghezza/16) &#42; (Altezza/16) &lt; 3600.

**Per aggiungere o modificare un predefinito di codifica video:**

1. In Adobe Dynamic Media Classic, nella barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti per video]**.
1. Seleziona **[!UICONTROL Predefiniti codifica singola]**.
1. Nella pagina Predefiniti per video, effettuate una delle seguenti operazioni:

   * Sulla barra degli strumenti Predefiniti video, seleziona **[!UICONTROL Aggiungi]** in modo da poter aggiungere un predefinito video.
   * Selezionate un predefinito per video. Nella barra degli strumenti, seleziona **[!UICONTROL Modifica]**.

     Non potete modificare i predefiniti predefiniti di Adobe Dynamic Media Classic; potete creare un predefinito solo da un predefinito esistente scegliendo **[!UICONTROL Salva con nome]**.

1. Nella pagina Aggiungi predefinito video o Modifica predefinito video, impostate le opzioni Predefinito per video desiderate.

   Per informazioni sulle impostazioni consigliate, consultate [Procedure ottimali per la codifica video](uploading-encoding-videos.md#best-practices-for-video-encoding).

   | Opzione Predefinito per video | Descrizione |
   | --- | --- |
   | Nome predefinito | Inserite un nome descrittivo per il predefinito per video. Il nome inserito verrà visualizzato nella finestra di dialogo Opzioni processo di caricamento, nella quale gli utenti scelgono le opzioni di transcodifica. |
   | Descrizione | Descrivete il predefinito per video. Il testo immesso viene visualizzato come descrizione quando si posiziona il puntatore sul nome del predefinito nella finestra di dialogo Opzioni processo di caricamento, in cui gli utenti scelgono le opzioni di trascodifica. |
   | Dispositivo di riproduzione | Scegliete il dispositivo su cui riprodurre il video. Le opzioni sono Computer (desktop), Mobile (iPhone, iPad, Android™) o Tablet (solo iPad). Questa impostazione determina automaticamente il codec video e audio appropriato utilizzato durante la codifica. |
   | Velocità dati di destinazione | Inserite una velocità di connessione Internet media (in kilobit al secondo) dell’utente finale di destinazione. Potete inserire il valore desiderato oppure trascinare il cursore per impostarlo. La gamma di velocità di connessione utente indica le velocità tipiche per connessioni banda larga, DSL, mobile e mediante modem. Questa impostazione determina automaticamente la velocità di dati audio e video combinata, ossia la quantità di dati codificati necessaria per creare un secondo di riproduzione video. Più alta è la velocità dati, migliore sarà la qualità del video. Tuttavia, valori di velocità dati elevati aumentano le dimensioni dei file a scapito dell’esperienza di visualizzazione degli utenti che dispongono di una larghezza di banda ridotta. Si consiglia quindi di trovare un compromesso tra valori di velocità dati elevati e ridotti. Mirate a creare un’esperienza di riproduzione con qualità adeguata, senza limitare gli utenti con larghezze di banda ridotte. |
   | Proporzioni | Le proporzioni sono il rapporto tra la larghezza e l’altezza del video. Le prime due proporzioni elencate di seguito sono comunemente utilizzate per visualizzare video in orizzontale:<ul><li> 4:3 - Usata per quasi tutti i contenuti di trasmissione TV con definizione standard.</li><li>16:9 - Utilizzato per quasi tutti i contenuti e i film in formato widescreen su televisori ad alta definizione (HDTV).</li><li>Scala automatica (impostazione predefinita) - Per creare video da distribuire a dispositivi mobili, tablet e computer desktop; predefinito codifica singola che funziona con qualsiasi proporzione. I video sorgente caricati e codificati con questo predefinito sono impostati su un’altezza specifica. Tuttavia, il valore della larghezza viene ridimensionato automaticamente per mantenere le proporzioni del video (rapporto larghezza per altezza).</li><li>Personale - Usata quando si desidera definire una dimensione video non standard.</li><li>Le proporzioni selezionate determinano le impostazioni di larghezza e altezza per Dimensione risoluzione. I valori di larghezza e altezza vengono automaticamente scalati in base alle proporzioni appropriate.</li></ul> |
   | Dimensione risoluzione | La dimensione della risoluzione, espressa dal numero di pixel di larghezza per il numero di pixel di altezza, determina la dimensione. Potete inserire i valori di larghezza e altezza in pixel oppure trascinare il relativo cursore per impostarli. La gamma di risoluzioni elenca le dimensioni di risoluzioni tipiche. I valori di larghezza e altezza si adattano automaticamente alle proporzioni selezionate. Ad esempio, se selezionate 4:3 come proporzione e inserite 400 per la larghezza, 300 viene inserito automaticamente per l’altezza. Se per le proporzioni avete selezionato Scala automatica, il valore Larghezza di Dimensione risoluzione viene impostato automaticamente su Auto. Seleziona **[!UICONTROL Anteprima]** in modo da poter aprire una finestra del browser e visualizzare le scelte di risoluzione. |
   | Suffisso file codifica | Inserite un suffisso. Questo suffisso viene aggiunto al file video codificato. Potete inserire un trattino o un trattino basso nel nome; gli spazi bianchi e i caratteri speciali non sono consentiti. |
   | Altre impostazioni | Adobe Dynamic Media Classic determina automaticamente tutte le altre impostazioni di codifica in base alle linee guida per la codifica consigliate. |

1. Effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Salva]** se hai aggiunto o modificato un predefinito video.
   * Seleziona **[!UICONTROL Salva con nome]** se hai aggiunto un predefinito video partendo da un predefinito esistente.

### Eliminare un predefinito di codifica video {#deleting-a-video-encoding-preset}

Gli amministratori possono eliminare i predefiniti per video personalizzati. Non è possibile eliminare i predefiniti video forniti con Adobe Dynamic Media Classic.

1. In Adobe Dynamic Media Classic, nella barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti per video]**.
1. Seleziona **[!UICONTROL Predefiniti codifica singola]**.
1. Nella pagina Predefiniti per video, selezionate nella tabella il predefinito per video da eliminare.
1. Sulla barra degli strumenti Predefiniti video, seleziona **[!UICONTROL Elimina]**.
1. Nella finestra di dialogo Elimina predefinito, seleziona **[!UICONTROL Elimina]**.

>[!MORELIKETHIS]
>
>* [Guida introduttiva: Video in Adobe Dynamic Media Classic](quick-start-video.md#quick-start-video)
>* [Caricare e codificare i video](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Utilizzare i predefiniti visualizzatore video](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
>* [Predefiniti video](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) video di formazione
