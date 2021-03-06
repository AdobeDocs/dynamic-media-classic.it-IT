---
title: Caricare i file
description: Scopri come caricare i file in Adobe Dynamic Media Classic.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
source-git-commit: ec1a981dd5cfa92ce4ae8e2676dd131d1509216f
workflow-type: tm+mt
source-wordcount: '3926'
ht-degree: 32%

---

# Caricare i file{#uploading-files}

Prima di caricare i file di risorse in Adobe Dynamic Media Classic, accertati che i file di risorse siano denominati correttamente e che la struttura delle cartelle sia impostata e organizzata nel modo desiderato. Puoi caricare i file da un sito FTP fornito da Adobe Dynamic Media Classic o direttamente dal computer o dalla rete. Adobe Dynamic Media Classic offre opzioni per l’ottimizzazione dei file durante il caricamento. Se hai installato l’applicazione desktop Adobe Dynamic Media Classic, puoi caricare file e cartelle trascinandoli direttamente dal desktop. Consultate [Impostazioni generali applicazione](application-setup.md#general_settings).

## Prepara le risorse e le cartelle per il caricamento {#preparing-your-assets-and-folders-for-uploading}

Prima di caricare le risorse in Adobe Dynamic Media Classic, accertati che siano nel formato e nelle dimensioni corretti. È inoltre necessario osservare le regole Adobe Dynamic Media Classic per la denominazione delle risorse. È anche utile organizzare e disporre i file in una cartella per semplificarne l’individuazione e l’utilizzo. 

### Formati di file di risorse supportati {#supported-asset-file-formats}

In questa tabella sono elencati i formati di file delle risorse supportati da Adobe Dynamic Media Classic. Per informazioni sui file Camera Raw supportati, consulta [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

| Formati di file di risorse | Descrizione |
| --- | --- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Cascading Style Sheet | CSS |
| Profili colore | ICC, ICM |
| Font | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Immagini | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (solo Windows®), TIF, TIFF |
| InDesign | INDD, INDT |
| MS® Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG e Camera Raw |
| PostScript | EPS, PS |
| Creazione immagini Adobe Dynamic Media Classic | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Video | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

Il supporto per il caricamento di file TAR e ZIP comprende una casella di controllo per selezionare la decompressione dei file.

### Formati immagine non supportati in Dynamic Media {#unsupported-image-formats-dynamic-media}

L&#39;elenco seguente descrive i sottotipi di formati di file immagine raster che sono *not* supportato in Dynamic Media.

Vedi anche [Rilevare formati di file non supportati per Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* File PNG con una dimensione del blocco IDAT superiore a 100 MB.
* File PSB.
* I file PSD con uno spazio colore diverso da CMYK, RGB, Scala di grigio o Bitmap non sono supportati. Gli spazi colore DuoTone, Lab e Indexed non sono supportati.
* File PSD con una profondità di bit maggiore di 16.
* File TIFF con dati a virgola mobile.
* File TIFF con spazio colore Lab.

### Tipi di risorse {#asset-types}

Per ottenere risultati ottimali con il programma Adobe Dynamic Media Classic, assicurati di utilizzare i formati e le dimensioni di file consigliati. Nella tabella seguente sono elencati i tipi di risorse con i formati e le dimensioni di file consigliati per le risorse usate comunemente.

| Tipo di risorsa | Descrizione/Consigli |
| --- | --- |
| Audio | I formati per l’input di risorse audio comprendono AAC, HE-AAC, AC3, WAV, WMA, AIFF e MP3. Potete transcodificare l’audio nei seguenti formati: MP3, AAC e HE-AAC. |
| Immagini (per Ridimensionamento immagini, Zoom, Set immagini, Set 360 gradi) | Le immagini devono essere di almeno 2000 pixel per le dimensioni più lunghe; Le dimensioni tipiche delle immagini variano da 1500 a 2500 pixel nel formato più lungo. Si consiglia di usare formati immagine senza perdita di dati, come i formati TIFF e PNG. Per le immagini JPEG, usate le impostazioni di qualità massima. I file GIF animati vengono gestiti come altri contenuti statici. |
| eCatalog | Utilizza file PDF ad alta risoluzione creati in Adobe Acrobat o un&#39;applicazione di Creative Suite Adobe salvata come &quot;pronto per la stampa&quot;. I file PDF includono tutti i font, le immagini, le maschere e gli elementi grafici di riferimento necessari nel formato a pagina singola, a due pagine affiancate o a più pagine. Ordinate le pagine assegnando ai file nomi in ordine alfanumerico. Salvate tutti i file PDF dell’eCatalog in un’unica cartella per semplificarne il caricamento. Potete selezionare le opzioni di ritaglio al momento del caricamento per rimuovere l’area di ritaglio dai file PDF, inclusi gli indicatori di taglio, i crocini di registro o le barre colore. La maggior parte dei file PDF pronti per la usano lo spazio cromatico CMYK; è quindi importante ottenere il profilo colore ICC CMYK usato con i file PDF. |
| Modelli | Un’immagine con livelli o un layout può includere testo, immagini e livelli. I livelli immagine, le stringhe di testo e gli attributi, quali il colore e le dimensioni, possono essere parametrizzati in modo da personalizzare i dati variabili. I requisiti delle immagini da usare nei modelli sono gli stessi delle altre immagini. Preparate gli elementi grafici in Photoshop o in un altro programma di modifica delle immagini. Salvate ogni elemento grafico come file trasparente a livello unico nel formato TIFF o PNG. Assicuratevi che la risoluzione delle immagini sia appropriata all’uso previsto. Le immagini per la stampa sono a 300 ppi. |
| Video | Adobe Dynamic Media Classic supporta i file video salvati in formato OGV e MP4. Potete transcodificare i file in formato MP4 al momento del caricamento. Consultate [Formati di file di risorse supportati](#supported-static-file-formats). |
| Font | Caratteri TrueType, Type1 (solo Windows®), OpenType® e PhotoFonts caricati. |
| Immagini | Immagini e file immagine con più livelli. |
| Set di immagini e set di campioni | Set di immagini correlate che possono essere visualizzate in un visualizzatore. |
| Profili ICC | Profilo colore che potete usare per convertire un’immagine caricata dallo spazio colore di origine in un altro spazio colore. |
| Vignettature | Immagini create con il programma Image Authoring e file correlati. |
| File contenuto | File di contenuto Adobe InDesign, Illustrator o Photoshop. |
| File FXG | File di formato grafico indipendenti dalla risoluzione che potete usare per creare modelli personalizzabili per la stampa, il Web, l’e-mail, il desktop e i dispositivi.  |
| File SVG | File di grafica vettoriale scalabile che possono essere sottoposti a rendering sui server Image Server.  |
| File XML | File che definiscono le regole di pre-elaborazione usate per modificare il percorso e le porzioni di query delle richieste.  |
| File Cascading Style Sheet. | Potete caricare interfacce CSS per personalizzare i visualizzatori HTML5. |
| File JavaScript | I file JavaScript vengono utilizzati per la strumentazione del visualizzatore per contenere le informazioni sull’account. Adobe Security consiglia questo tipo di risorsa solo per gli account client con un dominio separato in uso per la consegna (per evitare vulnerabilità cross-site scripting). |

>[!NOTE]
>
>Quando carichi file immagine e PDF in Adobe Dynamic Media Classic, il sistema converte questi file sorgente in file P-TIFF (Pyramid TIFF). Questi TIFF sono i file che vengono successivamente pubblicati sui server di immagini Dynamic Media. Adobe Dynamic Media Classic utilizza il formato file TIF piramidale perché contiene vari rapporti di zoom che consentono un rapido zoom quando viene visualizzato con un visualizzatore zoom Adobe Dynamic Media Classic.

### Formati di file statici supportati {#supported-static-file-formats}

Adobe Dynamic Media Classic supporta diversi formati di file statici. Per contenuto statico si intende qualsiasi risorsa pubblicata &quot;così com’è&quot;, ad esempio CSS, PDF, SVG e XML.

È possibile pubblicare i seguenti tipi di file:

* GIF animata
* File audio
* CSS
* JavaScript (se la società è configurata con un proprio dominio)
* Video Master
* PDF (quando PDF è contrassegnato per la pubblicazione dopo il caricamento, per evitare la consegna di tutti i PDF per il flusso di lavoro esistente di eCatalog/PDF)
* Video PrX
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic non fornisce l’opzione per generare un URL di anteprima del contenuto statico.

### Requisiti per i nomi di file {#filename-requirements}

Poiché nelle estensioni viene rimosso il nome del file durante il processo di caricamento, nel sistema non sono consentiti file con lo stesso nome radice. Nel sistema Adobe Dynamic Media Classic, il nome del file della risorsa meno l’estensione del nome del file diventa l’ID della risorsa. Per questo motivo non sono consentite due risorse con lo stesso nome.

Assicuratevi che le seguenti regole di denominazione dei file vengano comprese da tutti gli utenti della società:

* Non sono consentiti nel sistema ID di risorse con lo stesso identico nome.
* I nomi degli ID risorsa sono sensibili all’uso di maiuscole e minuscole.
* Come procedura consigliata assicuratevi che gli ID delle risorse non contengano spazi vuoti, ad esempio evitate di usare nomi come giacca nera.tif o giacca blu.jpg. Il codice ASCII di Adobe Dynamic Media Classic codifica gli spazi vuoti nei nomi delle risorse quando utilizza i nomi delle risorse per creare stringhe URL. Poiché questi codici ASCII sono difficili da leggere, la lettura degli URL può risultare più complicata.
* I nomi file possono contenere caratteri specifici per particolari lingue. Tuttavia, non possono contenere i seguenti caratteri:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; { } %

   Se il nome del file contiene uno o più di questi caratteri, questi vengono eliminati dal nome del file al momento del caricamento.

Di solito, un nome file di una risorsa può essere lo stesso del numero di articolo, SKU del prodotto o altro nome come nel seguente:

| Elemento | Nome file | ID risorsa |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organizzazione e struttura delle cartelle {#folder-organization-and-structure}

Organizzare e strutturare cartelle e sottocartelle per i contenuti in Adobe Dynamic Media Classic prima di caricare i contenuti nel sistema. La pianificazione preventiva di questa procedura presenta i due grandi vantaggi seguenti:

* Quando carichi il contenuto in Adobe Dynamic Media Classic tramite FTP, puoi dire al sistema di replicare la struttura delle cartelle durante il caricamento. In questo modo, il contenuto viene organizzato nelle stesse cartelle e sottocartelle di Adobe Dynamic Media Classic presenti sul computer o sulla rete. Per replicare la struttura delle cartelle in Adobe Dynamic Media Classic, seleziona l’opzione Includi sottocartelle quando carichi le risorse tramite FTP.
* Riorganizzare le cartelle all’interno del sistema dopo il caricamento dei file è molto più difficile rispetto a iniziare la procedura con una struttura di cartelle pianificata con attenzione.

L’approccio e la struttura per la denominazione delle cartelle scelti per memorizzare i contenuti in Adobe Dynamic Media Classic dipende dalle esigenze della tua organizzazione. Di seguito sono riportati alcune strutture di cartelle di esempio:

**Basato su SKU** - Le cartelle vengono denominate in base a SKU o numeri di elemento. Vengono ad esempio create cartelle separate per tutte le serie di numeri 0-, 20-, 30.

**Basato sul marchio** - Per i produttori con più linee di marchio e i rivenditori che commercializzano altri marchi di altre aziende, separare i file in cartelle di prodotti denominate per marchi diversi.

**Basato su progetto** - Le cartelle sono organizzate in base alla data di rollout/drop o al nome del progetto. Questa procedura è preferita dai clienti che si occupano principalmente della produzione di eCatalog. 

**Mirror della gerarchia delle cartelle del sito Web** - Questa struttura di cartelle rispecchia la struttura delle cartelle del sito web, con le cartelle denominate, ad esempio, per le categorie di prodotti.

## Informazioni sul caricamento dei file {#uploading-your-files}

Potete caricare singoli file dal desktop oppure caricare le cartelle mediante FTP. Se desideri caricare più di 100 MB di file o caricare intere cartelle e sottocartelle, seleziona la **VIA FTP** scheda .

Adobe Dynamic Media Classic invia un messaggio e-mail per confermare l’inizio e la fine del processo di caricamento e per segnalare eventuali problemi.

Durante (o subito dopo) un grande lavoro di caricamento, alcuni nuovi elementi potrebbero visualizzare il messaggio &quot;Immagine non ancora ottimizzata&quot;. Questo messaggio viene visualizzato perché i file non sono ancora stati completamente elaborati e aggiunti a Adobe Dynamic Media Classic. Potete ottimizzare questi file successivamente. Vedi [Ottimizzare i file](application-setup.md#optimize_files).

### Caricare file utilizzando la scheda Da desktop {#upload-files-using-sps-desktop-application}

L’applicazione Adobe Dynamic Media Classic Desktop consente di caricare file e cartelle mediante trascinamento.

1. Nell’applicazione Adobe Dynamic Media Classic Desktop, nella barra di navigazione globale, seleziona **[!UICONTROL Carica]**.
1. Nella pagina Carica , seleziona la **[!UICONTROL Da desktop]** scheda .
1. Sul lato sinistro della pagina Carica , nella sezione **[!UICONTROL Selezionare i file da caricare]** area, selezionare **[!UICONTROL Sfoglia]** per selezionare i file o le cartelle da caricare, seleziona **[!UICONTROL Apri]**.
1. Sul lato destro della pagina Carica , nella sezione **Scegli destinazione cartella** vai a una cartella di destinazione in cui desideri aggiungere i file o le cartelle caricati.
1. (Facoltativo) Vicino alla parte inferiore della pagina Carica, nel campo di testo Nome processo, immetti il nuovo nome del processo di caricamento. Oppure, puoi semplicemente utilizzare il nome predefinito generato dal sistema fornito da Adobe Dynamic Media Classic. Il processo in corso e gli altri processi di caricamento e pubblicazione vengono registrati nella pagina Processi dove è possibile controllarne lo stato. Consultate [Verifica dei file di processo](checking-job-files.md#checking_job_files).
1. (Facoltativo) Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Pubblica dopo il caricamento]** per pubblicare automaticamente le risorse caricate.
Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. (Facoltativo) Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Sovrascrivi in qualsiasi cartella, lo stesso nome della risorsa di base indipendentemente dall’estensione]** se desideri che i file caricati sostituiscano quelli esistenti con gli stessi nomi. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni in **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali]** > **[!UICONTROL Carica nell’applicazione]** > **[!UICONTROL Sovrascrivi immagini]**.
1. Nell’angolo in basso a destra della pagina Carica, seleziona **[!UICONTROL Opzioni processo]**, quindi specifica le opzioni desiderate.

   Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

1. Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Salva]**.
1. Nell’angolo in basso a destra della pagina Carica, seleziona **[!UICONTROL Invia caricamento]**.
Per visualizzare l’avanzamento del caricamento, seleziona **[!UICONTROL Processi]** sulla barra di navigazione globale. Puoi continuare a lavorare in Adobe Dynamic Media Classic e tornare alla pagina Processi in qualsiasi momento per rivedere un processo in corso. Per annullare un processo di caricamento in corso, fate clic sul pulsante **[!UICONTROL Annulla]** accanto alla durata.

### Caricare file utilizzando la scheda VIA FTP {#upload-files-using-via-ftp}

1. Accedi al sito FTP Adobe Dynamic Media Classic specifico per la tua area geografica. Utilizzate il nome utente e la password per FTP ricevuti dall’amministratore.
1. In Adobe Dynamic Media Classic, nella barra di navigazione globale, seleziona **[!UICONTROL Carica]**.
1. Nella pagina Carica , seleziona la **[!UICONTROL VIA FTP]** scheda .
1. Sul lato sinistro della pagina Carica , nella sezione **[!UICONTROL Scegliere la cartella FTP da caricare]** scegli una cartella FTP da cui caricare i file.
1. Sul lato destro della pagina Carica , nella sezione **[!UICONTROL Scegli la destinazione della cartella Dynamic Media di Adobe]** scegli una cartella di destinazione in Adobe Dynamic Media Classic.
1. (Facoltativo) Vicino alla parte inferiore della pagina Carica, nel campo di testo Nome processo, immetti il nuovo nome del processo di caricamento. Oppure, puoi semplicemente utilizzare il nome predefinito generato dal sistema fornito da Adobe Dynamic Media Classic. Il processo in corso e gli altri processi di caricamento e pubblicazione vengono registrati nella pagina Processi dove è possibile controllarne lo stato.
Consultate [Verifica dei file di processo](checking-job-files.md#checking_job_files).
1. (Facoltativo) Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Pubblica dopo il caricamento]** per pubblicare automaticamente le risorse caricate.
Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. (Facoltativo) Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Sovrascrivi in qualsiasi cartella, lo stesso nome della risorsa di base indipendentemente dall’estensione]** se desideri che i file caricati sostituiscano quelli esistenti con gli stessi nomi. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali]** > **[!UICONTROL Carica nell’applicazione]** > **[!UICONTROL Sovrascrivi immagini]**.
1. Facoltativo; disponibile solo se hai fatto clic su **[!UICONTROL VIA FTP]** scheda . Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Decomprimi file Zip o Tar durante il caricamento]** se desideri estrarre automaticamente tutti i file dal file ZIP o TAR caricato. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. Nell’angolo in basso a destra della pagina Carica, seleziona **[!UICONTROL Opzioni processo]**, quindi specifica le opzioni desiderate.

   Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

1. Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Salva]**.
1. Nell’angolo in basso a destra della pagina Carica, seleziona **[!UICONTROL Invia caricamento]**.

   Per visualizzare l’avanzamento del caricamento, seleziona nella barra di navigazione globale **[!UICONTROL Processi]**. Viene visualizzata la pagina Processi che mostra l’avanzamento del caricamento. Puoi continuare a lavorare in Adobe Dynamic Media Classic e tornare alla pagina Processi in qualsiasi momento per rivedere un processo in corso.

Per annullare un processo di caricamento in corso, fate clic sul pulsante **[!UICONTROL Annulla]** accanto alla durata.

## Finestra di dialogo Opzioni processo di caricamento {#upload-options}

Durante il caricamento dei file, puoi scegliere tra le seguenti opzioni nella finestra di dialogo Opzioni processo di caricamento :

* **LAVORO** - Seleziona **[!UICONTROL LAVORO]** per scegliere le opzioni che interessano l’intero processo di caricamento.

   Puoi anche scegliere *default* opzioni per il caricamento dei processi utilizzando la **[!UICONTROL Opzioni di caricamento predefinite]** in Impostazioni generali. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali]** > **[!UICONTROL Opzioni di caricamento predefinite]**, quindi imposta le opzioni predefinite desiderate.

   * **[!UICONTROL Quando]** - Questa opzione è disponibile solo se è stata selezionata la **[!UICONTROL VIA FTP]** scheda .
      * **[!UICONTROL Una tantum]** - Specifica un processo di caricamento da eseguire una volta. Le opzioni includono:
         * **[!UICONTROL Ora]** - Esegue il processo di caricamento immediatamente dopo aver selezionato **[!UICONTROL Salva]** nella finestra di dialogo Opzioni processo di caricamento , quindi seleziona **[!UICONTROL Invia caricamento]** nella pagina Carica .
         * **[!UICONTROL Pianificazione per un momento successivo]** - Seleziona l’anno, il mese, il giorno e l’ora (con incrementi di 15 minuti) in cui desideri eseguire il processo di caricamento.
      * **[!UICONTROL Ricorrente]** - Specifica un processo di caricamento che viene eseguito quotidianamente, settimanalmente o mensilmente. Oppure, personalizza il processo di caricamento secondo le tue specifiche.
         * **[!UICONTROL Giornaliero]** - Impostare l&#39;ora in cui si desidera eseguire il processo ogni giorno. Se si desidera eseguire il processo solo dal lunedì al venerdì, selezionare **[!UICONTROL Solo giorni feriali]**.
         * **[!UICONTROL Settimanale]** - Scegliere un giorno specifico della settimana e dell&#39;ora in cui si desidera eseguire il processo.
         * **[!UICONTROL Mensile]** - Scegliere un giorno specifico del mese o del giorno della settimana, inclusa l&#39;ora di inizio, in cui si desidera eseguire il processo.
         * **[!UICONTROL Personalizzato]** - Personalizza un intervallo di tempo del lavoro di caricamento o pubblicazione in base alle tue specifiche. Vedi [Crea un intervallo personalizzato per il processo di caricamento o pubblicazione](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **[!UICONTROL Pubblica dopo il caricamento]** - Disponibile se è stato selezionato il **[!UICONTROL DA DESKTOP]** oppure **[!UICONTROL VIA FTP]** scheda . Selezionate questa opzione per pubblicare automaticamente le risorse caricate. Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa opzione è disponibile anche nella pagina di caricamento.

   * **[!UICONTROL Sovrascrivi in qualsiasi cartella, lo stesso nome della risorsa di base indipendentemente dall’estensione]** - Disponibile se è stato selezionato il **[!UICONTROL DA DESKTOP]** oppure **[!UICONTROL VIA FTP]** scheda . Selezionate questa opzione per sostituire i file esistenti con quelli caricati mantenendo gli stessi nomi. Questa opzione è disponibile anche nella pagina di caricamento. Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali]** > **[!UICONTROL Carica nell’applicazione]** > **[!UICONTROL Sovrascrivi immagini]**.

   * **[!UICONTROL Decomprimi file Zip o Tar durante il caricamento]** - Disponibile se è stato selezionato il **[!UICONTROL DA DESKTOP]** oppure **[!UICONTROL VIA FTP]** scheda .
Seleziona questa opzione se desideri estrarre automaticamente tutti i file dal file ZIP o TAR caricato. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.

   * **[!UICONTROL Includi sottocartelle]** - Disponibile solo se è stata selezionata la **[!UICONTROL VIA FTP]** scheda .
Selezionate questa opzione per caricare le sottocartelle della cartella che intendete caricare. I nomi della cartella e delle relative sottocartelle caricate vengono inseriti automaticamente in Adobe Dynamic Media Classic.

   * **[!UICONTROL File di metadati del processo]** - Disponibile solo se è stata selezionata una delle seguenti opzioni **[!UICONTROL VIA FTP]** scheda . Selezionate questa opzione se desiderate caricare un file delimitato da tabulazioni o XML per aggiungere metadati a più risorse. Consultate [Importare metadati (tramite FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **Opzioni di ritaglio** - Per ritagliare automaticamente i pixel dello spazio bianco da un’immagine, apri le **[!UICONTROL Ritaglio]** menu, seleziona **[!UICONTROL Manuale]**, quindi immetti le misure dei pixel nei campi di testo Superiore, Destro, Inferiore e Sinistro da ritagliare dai lati. Puoi anche selezionare **[!UICONTROL Rifila]** nel menu Ritaglio, scegliete le seguenti opzioni:

   * **[!UICONTROL Rifila in base a]** - Scegli se ritagliare in base al colore o alla trasparenza:
      * **[!UICONTROL Colore]** - Scegliere l&#39;opzione Colore. Dal menu Angolo scegliete quindi l’angolo dell’immagine con il colore che rappresenta meglio quello dello spazio bianco da ritagliare.
Rifilatura in base al colore: Specificare 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell&#39;angolo dell&#39;immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 
      * **[!UICONTROL Trasparenza]** - Scegli la **[!UICONTROL Trasparenza]** opzione .
Rifilatura in base alla trasparenza: Specificare 0 per ritagliare i pixel solo se sono trasparenti; numeri più vicini a 1 assicurano una maggiore trasparenza.
      * **[!UICONTROL Tolleranza]** - Trascinare il cursore per specificare una tolleranza da 0 a 1.

* **Opzioni del profilo colore** - Scegli una conversione del colore quando crei file ottimizzati utilizzati per la distribuzione dinamica Adobe Dynamic Media Classic:

   * **[!UICONTROL Conservazione colore predefinita]** - mantiene i colori dell&#39;immagine sorgente ogni volta che le immagini contengono informazioni sullo spazio colore; non vi è alcuna conversione del colore. In quasi tutte le immagini è incorporato il relativo profilo colore. Tuttavia, se un’immagine sorgente CMYK non contiene un profilo colore incorporato, i colori vengono convertiti nello spazio colore sRGB. sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.
   * **[!UICONTROL Mantieni spazio colore originale]** - Mantiene i colori originali senza alcuna conversione al momento dell&#39;acquisizione in Adobe Dynamic Media Classic. Per le immagini prive di un profilo colore incorporato, la conversione del colore necessaria per elaborare le richieste di immagine viene effettuata utilizzando i profili colore predefiniti, come configurato nelle impostazioni di pubblicazione. Questi profili di colore non sempre si allineano al colore nei file creati con questa opzione. Si consiglia quindi di utilizzare l’opzione Mantenimento colore predefinito.
   * **[!UICONTROL Personalizzato da]** > **[!UICONTROL A]** - Apre i menu per scegliere un **[!UICONTROL Converti da]** e **[!UICONTROL Converti in]** spazio colore. Questa opzione avanzata ha priorità rispetto a eventuali informazioni di colore incorporate nel file sorgente. Selezionare questa opzione solo quando tutte le immagini che si stanno inviando contengono dati di profilo colore errati o mancanti.

* **Opzioni di modifica delle immagini** - È possibile mantenere le maschere di ritaglio &lt;> nelle immagini e scegliere un profilo colore.
Vedi [Opzioni di ottimizzazione delle immagini al caricamento](image-editing-options-upload.md#image-editing-options-at-upload).

* **Opzioni PostScript®** - È possibile rasterizzare file di PostScript®, ritagliare file, mantenere sfondi trasparenti, scegliere una risoluzione e scegliere uno spazio colore.
Vedi [Utilizzare i file PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Opzioni Photoshop** - È possibile creare modelli da file Adobe® Photoshop®, mantenere i livelli, specificare il nome dei livelli, estrarre il testo e specificare il modo in cui le immagini vengono ancorate ai modelli.
Consultate [Opzioni di caricamento PSD](psd-files.md#psd_upload_options).

* **Opzioni di PDF** - È possibile rasterizzare i file, estrarre parole di ricerca e collegamenti, generare automaticamente un eCatalog, impostare la risoluzione e scegliere uno spazio colore.
Consultate [Opzioni di caricamento PDF](pdfs.md#pdf_upload_options).

* **Opzioni Illustrator** - È possibile rasterizzare i file Adobe Illustrator®, mantenere sfondi trasparenti, scegliere una risoluzione e scegliere uno spazio colore.
Vedi [Utilizzare i file PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Opzioni EVIDEO** - È possibile transcodificare un file video scegliendo un predefinito per video.
Vedi [Utilizzare i predefiniti di codifica video](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Metadati aggiuntivi** - Immetti le parole chiave che descrivono i file che intendi caricare. Separate le parole chiave con una virgola. Le parole chiave consentono di effettuare ricerche di risorse in modo semplificato. Vedi [Eseguire una ricerca avanzata](searching-assets.md#conducting_an_advanced_search). Vedi anche [Caricare le parole chiave](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) video di formazione.

* **Predefiniti set di batch** - Se desideri creare un set di immagini, un set 360 gradi o un set di campioni dai file caricati, seleziona la **[!UICONTROL Attivo]** per il predefinito da utilizzare. Potete selezionare più di un predefinito. Potete creare i predefiniti nella pagina Impostazione applicazione/Predefiniti set di batch. Consultate [Predefiniti per set di batch](application-setup.md#batch_set_presets).

* **Avanzate** - Vedi [Seguire un caricamento con un altro processo](uploading-files.md#follow-an-upload-with-another-job).

## Avviare un altro processo al termine di un caricamento {#follow-an-upload-with-another-job}

Quando carichi elementi tramite FTP, puoi pianificare un processo successivo per iniziare una volta completato il caricamento. Se l&#39;inizio di altri lavori è programmato, il lavoro programmato qui viene messo in coda dopo di essi.

Il nuovo processo invia una notifica all’indirizzo specificato per poter attivare il codice nella posizione esatta. Questo processo di pubblicazione sequenziale usa lo stesso nome del processo di caricamento, con l’aggiunta del testo *Pub_* all’inizio.

**Per avviare un altro processo al termine di un caricamento:**

1. Seleziona **[!UICONTROL Carica]**, quindi seleziona la **[!UICONTROL VIA FTP]** scheda .
1. Nell’angolo in basso a destra della pagina Carica, seleziona **[!UICONTROL Opzioni processo]**.
1. Nella finestra di dialogo Opzioni processo di caricamento , espandi la **[!UICONTROL AVANZATO]** sezione .
1. Scegli una delle seguenti opzioni dalla **[!UICONTROL Segui il caricamento con un altro processo]** elenco a discesa:

   * Nessuno
   * Richiesta HTTP
   * Pubblicazione da Image Server
   * Pubblicazione da Image Rendering
   * Pubblicazione video

1. Specificate l’indirizzo HTTP.
1. Specifica se desideri eseguire solo se i file sono stati caricati.
1. Specificate se la richiesta deve essere eseguita ogni volta che termina il processo oppure solo quando i file sono stati pubblicati. 

   >[!NOTE]
   >
   >A volte i lavori pianificati regolarmente non possono causare la pubblicazione di file.

>[!MORELIKETHIS]
>
>* [Utilizzare le cartelle di risorse](asset-folders.md#working_with_asset_folders)
>* [Gestire processi di caricamento e pubblicazione ricorrenti](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Utilizzare un processo di caricamento o pubblicazione come attivatore](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

