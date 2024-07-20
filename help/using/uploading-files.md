---
title: Caricare i file
description: Scopri come caricare i file in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '3868'
ht-degree: 25%

---

# Caricare i file{#uploading-files}

Prima di caricare i file di risorse in Adobe Dynamic Media Classic, accertati che i nomi dei file di risorse siano corretti. Assicurati inoltre che la struttura delle cartelle sia configurata e organizzata nel modo desiderato. È possibile caricare file da un sito FTP fornito da Adobe Dynamic Media Classic o direttamente dal computer o dalla rete. Adobe Dynamic Media Classic offre opzioni per l’ottimizzazione dei file durante il caricamento. Se è stata installata l&#39;applicazione Adobe Dynamic Media Classic Desktop, è possibile caricare file e cartelle trascinandoli direttamente dal desktop. Consultate [Impostazioni generali applicazione](application-setup.md#general_settings).

## Preparare risorse e cartelle per il caricamento {#preparing-your-assets-and-folders-for-uploading}

Prima di caricare le risorse in Adobe Dynamic Media Classic, accertati che siano nel formato e nelle dimensioni corretti. È inoltre necessario osservare le regole di Adobe Dynamic Media Classic per la denominazione delle risorse. È anche utile organizzare e disporre i file in una cartella per semplificarne l’individuazione e l’utilizzo. 

### Formati di file di risorse supportati {#supported-asset-file-formats}

In questa tabella sono elencati i formati di file di risorse supportati da Adobe Dynamic Media Classic. Per informazioni sui file Camera Raw supportati, vedere [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

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
| Authoring immagini Adobe Dynamic Media Classic | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Video | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

Il supporto per il caricamento di file TAR e ZIP comprende una casella di controllo per selezionare la decompressione dei file.

### Formati di immagine non supportati in Dynamic Medie {#unsupported-image-formats-dynamic-media}

Nell&#39;elenco seguente vengono descritti i sottotipi di formati di file immagine raster *non* supportati in Dynamic Medie.

Vedere anche [Rileva formati di file non supportati per Dynamic Medie](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* File PNG con dimensioni del blocco IDAT superiori a 100 MB.
* File PSB.
* I file PSD con uno spazio colore diverso da CMYK, RGB, Gradazioni di grigio o Bitmap non sono supportati. DuoTone, Lab e gli spazi colore indicizzati non sono supportati.
* File PSD con profondità di bit maggiore di 16.
* File TIFF con dati a virgola mobile.
* File TIFF con spazio colore Lab.

### Tipi di risorse {#asset-types}

Per ottenere risultati ottimali con il programma Adobe Dynamic Media Classic, assicurati di utilizzare i formati e le dimensioni di file consigliati. Nella tabella seguente sono elencati i tipi di risorse con i formati e le dimensioni di file consigliati per le risorse usate comunemente.

| Tipo di risorsa | Descrizione/Consigli |
| --- | --- |
| Audio | I formati per l’input di risorse audio comprendono AAC, HE-AAC, AC3, WAV, WMA, AIFF e MP3. Potete transcodificare l’audio nei seguenti formati: MP3, AAC e HE-AAC. |
| Immagini (per Ridimensionamento immagini, Zoom, Set immagini, Set 360 gradi) | Le immagini devono essere di almeno 2000 pixel alle dimensioni più lunghe; le dimensioni tipiche variano da 1500 a 2500 pixel nelle dimensioni più lunghe. Si consiglia di usare formati immagine senza perdita di dati, come i formati TIFF e PNG. Per le immagini JPEG, usate le impostazioni di qualità massima. I file di animazione GIF vengono gestiti come altri contenuti statici. |
| eCatalog | Utilizza i file PDF ad alta risoluzione creati in Adobe Acrobat o un’applicazione di Creative Suite di Adobe salvata come &quot;press-ready&quot;. I PDF includono tutti i font, le immagini e le maschere necessari. Inoltre, includi tutti gli elementi grafici di riferimento necessari, come pagine singole, pagine doppie o in formato multipagina. Ordinate le pagine assegnando ai file nomi in ordine alfanumerico. Salvate tutti i file PDF dell’eCatalog in un’unica cartella per semplificarne il caricamento. Potete selezionare le opzioni di ritaglio al momento del caricamento per rimuovere l’area di ritaglio dai file PDF, inclusi gli indicatori di taglio, i crocini di registro o le barre colore. La maggior parte dei file PDF pronti per la usano lo spazio cromatico CMYK; è quindi importante ottenere il profilo colore ICC CMYK usato con i file PDF. |
| Modelli | Un’immagine con livelli o un layout può includere testo, immagini e livelli. I livelli immagine, le stringhe di testo e gli attributi, quali il colore e le dimensioni, possono essere parametrizzati in modo da personalizzare i dati variabili. I requisiti delle immagini da usare nei modelli sono gli stessi delle altre immagini. Preparate gli elementi grafici in Photoshop o in un altro programma di modifica delle immagini. Salvate ogni elemento grafico come file trasparente a livello unico nel formato TIFF o PNG. Assicuratevi che la risoluzione delle immagini sia appropriata all’uso previsto. Le immagini da stampare sono 300 ppi. |
| Video | Adobe Dynamic Media Classic supporta i file video salvati in formato OGV e MP4. Al momento del caricamento, è possibile trascodificare i file in formato MP4. Consultate [Formati di file di risorse supportati](#supported-static-file-formats). |
| Font | Sono stati caricati TrueType, `Type1` (solo Windows®), OpenType ® font e PhotoFonts. |
| Immagini | Immagini e file immagine con più livelli. |
| Set di immagini e set di campioni | Set di immagini correlate che possono essere visualizzate in un visualizzatore. |
| Profili ICC | Un profilo colore che puoi utilizzare per convertire un’immagine caricata dal suo spazio colore sorgente in uno spazio colore diverso. |
| Vignettature | Immagini create con il programma Image Authoring e file correlati. |
| File contenuto | File di contenuto Adobe InDesign, Illustrator o Photoshop. |
| File FXG | File di formato grafico indipendenti dalla risoluzione che potete usare per creare modelli personalizzabili per la stampa, il Web, l’e-mail, il desktop e i dispositivi.  |
| File SVG | File di grafica vettoriale scalabile che possono essere sottoposti a rendering sui server Image Server.  |
| File XML | File che definiscono le regole di pre-elaborazione usate per modificare il percorso e le porzioni di query delle richieste.  |
| File Cascading Style Sheet. | Carica gli skin CSS per personalizzare i visualizzatori HTML5. |
| File JavaScript | I file JavaScript vengono utilizzati per la strumentazione del visualizzatore per memorizzare le informazioni sull&#39;account. Adobe di protezione consiglia questo tipo di risorsa solo per gli account client che hanno un dominio separato in uso per la distribuzione (per evitare script tra siti). |

>[!NOTE]
>
>Quando si caricano file di immagine e PDF in Adobe Dynamic Media Classic, questi vengono convertiti in file P-TIFF (Pyramid TIFF). Questi TIFF-P sono i file che vengono successivamente pubblicati nei server immagini Dynamic Medie. Adobe Dynamic Media Classic utilizza il formato di file Tiff piramidale perché contiene vari rapporti di zoom che consentono uno zoom rapido quando viene visualizzato con un Visualizzatore zoom di Adobe Dynamic Media Classic.

### Formati di file statici supportati {#supported-static-file-formats}

Adobe Dynamic Media Classic supporta diversi formati di file statici. Il contenuto statico è qualsiasi risorsa pubblicata &quot;così com’è&quot;, ad esempio CSS, PDF, SVG e XML.

È possibile pubblicare i seguenti tipi di file:

* GIF animata
* File audio
* CSS
* JavaScript (se la società è configurata con un proprio dominio)
* Video principale
* PDF (quando PDF è contrassegnato per la pubblicazione dopo il caricamento, per evitare la consegna di tutti i PDF per il flusso di lavoro eCatalog/PDF esistente)
* Video PrX
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic non fornisce l’opzione per generare un URL di anteprima con contenuto statico.

### Requisiti per i nomi di file {#filename-requirements}

Poiché nelle estensioni viene rimosso il nome del file durante il processo di caricamento, nel sistema non sono consentiti file con lo stesso nome radice. Nel sistema Adobe Dynamic Media Classic, il nome file della risorsa meno l’estensione del nome file diventa l’ID risorsa della risorsa. Per questo motivo non sono consentite due risorse con lo stesso nome.

Assicurati che tutti gli utenti della tua azienda comprendano queste regole per la denominazione dei file:

* Gli ID risorsa con lo stesso nome non sono consentiti nel sistema.
* I nomi ID risorsa fanno distinzione tra maiuscole e minuscole.
* Come procedura consigliata assicuratevi che gli ID delle risorse non contengano spazi vuoti, ad esempio evitate di usare nomi come giacca nera.tif o giacca blu.jpg. Quando si utilizzano nomi di risorse per creare stringhe URL, Adobe Dynamic Media Classic ASCII codifica spazi vuoti nei nomi delle risorse. Poiché questi codici ASCII sono difficili da leggere, la lettura degli URL può risultare più complicata.
* I nomi file possono contenere caratteri specifici per particolari lingue. Tuttavia, non possono contenere i seguenti caratteri:

  `\ ; / ? : @ & = + $ , &#42; " &lt; > | ' { } %`

  Se il nome del file contiene uno o più di questi caratteri, questi vengono eliminati dal nome del file al momento del caricamento.

Di solito, il nome del file di una risorsa può essere uguale al numero dell’articolo, allo SKU del prodotto o a un altro nome, come illustrato di seguito:

| Elemento | Nome file | ID risorsa |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organizzazione e struttura delle cartelle {#folder-organization-and-structure}

Organizza e struttura cartelle e sottocartelle per i contenuti in Adobe Dynamic Media Classic prima di caricarli. La pianificazione preventiva di questa procedura presenta i due grandi vantaggi seguenti:

* Quando carichi il contenuto in Adobe Dynamic Media Classic tramite FTP, puoi chiedere al sistema di replicare la struttura delle cartelle durante il caricamento. In questo modo, il contenuto viene organizzato nelle stesse cartelle e sottocartelle di Adobe Dynamic Media Classic presenti nel computer o in rete. Per replicare la struttura di cartelle in Adobe Dynamic Media Classic, seleziona l’opzione Includi sottocartelle quando carichi le risorse tramite FTP.
* Riorganizzare le cartelle all’interno del sistema dopo il caricamento dei file è molto più difficile rispetto a iniziare la procedura con una struttura di cartelle pianificata con attenzione.

L’approccio e la struttura di denominazione delle cartelle scelti per memorizzare il contenuto sul Adobe Dynamic Media Classic dipende dalle esigenze della tua organizzazione. Di seguito sono riportati alcune strutture di cartelle di esempio:

**Basato su SKU**: le cartelle sono denominate in base agli SKU o ai numeri di elemento. Ad esempio, vengono create cartelle separate per tutte le serie di numeri da 0, 20 e 30.

**Basato su marchio**: per i produttori con più linee di marchio e i rivenditori che commercializzano altri marchi di altre aziende, separa i file in cartelle di prodotto denominate per marchi diversi.

**Basato su progetto**: le cartelle sono organizzate in base alla data di rollout/rilascio o al nome del progetto. Questa procedura è preferita dai clienti che si occupano principalmente della produzione di eCatalog. 

**Mirror della gerarchia di cartelle del sito Web**: questa struttura di cartelle esegue il mirroring della struttura di cartelle del sito Web, con le cartelle denominate, ad esempio, per le categorie di prodotti.

## Informazioni sul caricamento di file {#uploading-your-files}

Puoi caricare singoli file dal desktop o cartelle tramite FTP. Per caricare più di 100 MB di file o intere cartelle e sottocartelle, selezionare la scheda **VIA FTP**.

Adobe Dynamic Media Classic ti invia un messaggio e-mail per confermare quando inizia e termina il processo di caricamento e per avvisarti di eventuali problemi.

Durante (o immediatamente dopo) un processo di caricamento di grandi dimensioni, alcuni nuovi elementi potrebbero visualizzare il messaggio &quot;Immagine non ancora ottimizzata&quot;. Questo messaggio viene visualizzato perché i file non sono ancora completamente elaborati e aggiunti a Adobe Dynamic Media Classic. Potete ottimizzare questi file successivamente. Vedi [Ottimizzare i file](application-setup.md#optimize_files).

### Caricare i file utilizzando la scheda Da desktop {#upload-files-using-sps-desktop-application}

L&#39;applicazione Adobe Dynamic Media Classic Desktop consente di caricare file e cartelle trascinandoli.

1. Nell&#39;applicazione Adobe Dynamic Media Classic Desktop, nella barra di navigazione globale, selezionare **[!UICONTROL Carica]**.
1. Nella pagina Carica, seleziona la scheda **[!UICONTROL Dal desktop]**.
1. Nella parte sinistra della pagina Carica, nell&#39;area **[!UICONTROL Seleziona i file da caricare]**, selezionare **[!UICONTROL Sfoglia]** per selezionare i file o le cartelle da caricare, quindi selezionare **[!UICONTROL Apri]**.
1. Nella parte destra della pagina Caricamento, nell&#39;area **Destinazione cartella** selezionata, passare a una cartella di destinazione in cui si desidera aggiungere i file o le cartelle caricati.
1. (Facoltativo) Nella parte inferiore della pagina Carica, inserisci il nuovo nome del processo di caricamento nel campo di testo Nome processo. In alternativa, è possibile utilizzare semplicemente il nome predefinito generato dal sistema fornito da Adobe Dynamic Media Classic. I processi di caricamento e pubblicazione vengono registrati nella pagina Processi, in cui è possibile controllare lo stato dei processi. Consultate [Verifica dei file di processo](checking-job-files.md#checking_job_files).
1. (Facoltativo) Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Publish dopo il caricamento]** per pubblicare automaticamente le risorse caricate.
Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. La stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. (Facoltativo) Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Sovrascrivi in qualsiasi cartella, nome come risorsa base, a prescindere dall&#39;estensione]** se desideri che i file caricati sostituiscano i file esistenti con gli stessi nomi. La stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni in **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Impostazioni generali]** > **[!UICONTROL Carica nell&#39;applicazione]** > **[!UICONTROL Sovrascrivi immagini]**.
1. Nell&#39;angolo inferiore destro della pagina Carica, seleziona **[!UICONTROL Opzioni processo]**, quindi specifica le opzioni desiderate.

   Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

1. Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Salva]**.
1. Nell&#39;angolo inferiore destro della pagina Carica, seleziona **[!UICONTROL Invia caricamento]**.
Per visualizzare l&#39;avanzamento del caricamento, seleziona **[!UICONTROL Processi]** nella barra di navigazione globale. Puoi continuare a lavorare in Adobe Dynamic Media Classic. Tornare alla pagina Processi in qualsiasi momento per esaminare un processo in corso. Per annullare un processo di caricamento in corso, fate clic sul pulsante **[!UICONTROL Annulla]** accanto alla durata.

### Caricare i file tramite la scheda FTP VIA {#upload-files-using-via-ftp}

1. Accedi al sito FTP di Adobe Dynamic Media Classic specifico per la tua area geografica. Utilizzate il nome utente e la password per FTP ricevuti dall’amministratore.
1. In Adobe Dynamic Media Classic, nella barra di navigazione globale, seleziona **[!UICONTROL Carica]**.
1. Nella pagina Carica selezionare la scheda **[!UICONTROL VIA FTP]**.
1. Nella parte sinistra della pagina Caricamento, nell&#39;area **[!UICONTROL Scegli cartella FTP per caricamento]**, scegliere una cartella FTP da cui caricare i file.
1. Nella parte destra della pagina Carica, nell&#39;area **[!UICONTROL Destinazione cartella Dynamic Medie Adobe]** selezionata, scegliere una cartella di destinazione in Adobe Dynamic Media Classic.
1. (Facoltativo) Nella parte inferiore della pagina Carica, inserisci il nuovo nome del processo di caricamento nel campo di testo Nome processo. In alternativa, è possibile utilizzare semplicemente il nome predefinito generato dal sistema fornito da Adobe Dynamic Media Classic. I processi di caricamento e pubblicazione vengono registrati nella pagina Processi, in cui è possibile controllare lo stato dei processi.
Consultate [Verifica dei file di processo](checking-job-files.md#checking_job_files).
1. (Facoltativo) Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Publish dopo il caricamento]** per pubblicare automaticamente le risorse caricate.
Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. La stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. (Facoltativo) Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Sovrascrivi in qualsiasi cartella, nome come risorsa base, a prescindere dall&#39;estensione]** se desideri che i file caricati sostituiscano i file esistenti con gli stessi nomi. La stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni in **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Impostazioni generali]** > **[!UICONTROL Carica nell&#39;applicazione]** > **[!UICONTROL Sovrascrivi immagini]**.
1. Facoltativo; disponibile solo se è stata selezionata la scheda **[!UICONTROL VIA FTP]**. Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Decomprimi file ZIP o Tar al caricamento]** per estrarre automaticamente tutti i file dal file ZIP o TAR caricato. La stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. Nell&#39;angolo inferiore destro della pagina Carica, seleziona **[!UICONTROL Opzioni processo]**, quindi specifica le opzioni desiderate.

   Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

1. Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Salva]**.
1. Nell&#39;angolo inferiore destro della pagina Carica, seleziona **[!UICONTROL Invia caricamento]**.

   Per visualizzare l&#39;avanzamento del caricamento, sulla barra di navigazione globale, seleziona **[!UICONTROL Processi]**. Viene visualizzata la pagina Processi che mostra l’avanzamento del caricamento. Puoi continuare a lavorare in Adobe Dynamic Media Classic. Tornare alla pagina Processi in qualsiasi momento per esaminare un processo in corso.

Per annullare un processo di caricamento in corso, fate clic sul pulsante **[!UICONTROL Annulla]** accanto alla durata.

## Finestra di dialogo Carica opzioni processo {#upload-options}

Durante il caricamento dei file, nella finestra di dialogo Opzioni processo di caricamento è possibile scegliere una delle opzioni seguenti:

* **PROCESSO**: selezionare **[!UICONTROL PROCESSO]** per scegliere le opzioni che influiscono sull&#39;intero processo di caricamento.

  Puoi anche scegliere le opzioni *default* per caricare i processi utilizzando la finestra di dialogo **[!UICONTROL Opzioni di caricamento predefinite]** in Impostazioni generali. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Impostazioni generali]** > **[!UICONTROL Opzioni di caricamento predefinite]**, quindi imposta le opzioni predefinite desiderate.

   * **[!UICONTROL Quando]**: questa opzione è disponibile solo se è stata selezionata la scheda **[!UICONTROL VIA FTP]**.
      * **[!UICONTROL Occasionale]**: specifica un processo di caricamento che viene eseguito una volta. Le opzioni includono:
         * **[!UICONTROL Ora]**: esegue il processo di caricamento subito dopo aver selezionato **[!UICONTROL Salva]** nella finestra di dialogo Opzioni processo di caricamento, quindi selezionare **[!UICONTROL Invia caricamento]** nella pagina Caricamento.
         * **[!UICONTROL Pianifica per più tardi]**: seleziona l&#39;anno, il mese, il giorno e l&#39;ora (con incrementi di 15 minuti) in cui desideri eseguire il processo di caricamento.
      * **[!UICONTROL Ricorrente]**: specifica un processo di caricamento che viene eseguito ogni giorno, ogni settimana o ogni mese. In alternativa, è possibile personalizzare il processo di caricamento in base alle proprie specifiche.
         * **[!UICONTROL Giornaliero]**: impostare l&#39;ora di esecuzione giornaliera del processo. Se si desidera eseguire il processo solo dal lunedì al venerdì, selezionare **[!UICONTROL Solo giorni feriali]**.
         * **[!UICONTROL Settimanale]**: scegli un giorno della settimana e un&#39;ora specifici per l&#39;esecuzione del processo.
         * **[!UICONTROL Mensile]**: scegliere un giorno specifico del mese o della settimana, inclusa l&#39;ora di inizio, in cui si desidera eseguire il processo.
         * **[!UICONTROL Personalizzato]**: personalizza l&#39;intervallo di tempo di un processo di caricamento o pubblicazione in base alle tue specifiche. Vedere [Intervallo di tempo caricamento o pubblicazione personalizzato](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).

   * **[!UICONTROL Publish dopo il caricamento]**: disponibile se è stata selezionata la scheda **[!UICONTROL FROM DESKTOP]** o **[!UICONTROL VIA FTP]**. Seleziona questa opzione per pubblicare automaticamente le risorse caricate. Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa opzione è disponibile anche nella pagina di caricamento.

   * **[!UICONTROL Sovrascrivi in qualsiasi cartella, nome come risorsa base, indipendentemente dall&#39;estensione]**: disponibile se è stata selezionata la scheda **[!UICONTROL FROM DESKTOP]** o **[!UICONTROL VIA FTP]**. Selezionate questa opzione per sostituire i file esistenti con quelli caricati mantenendo gli stessi nomi. Questa opzione è disponibile anche nella pagina di caricamento. Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni in **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Impostazioni generali]** > **[!UICONTROL Carica nell&#39;applicazione]** > **[!UICONTROL Sovrascrivi immagini]**.

   * **[!UICONTROL Decomprimi file Zip o Tar al caricamento]**: disponibile se è stata selezionata la scheda **[!UICONTROL FROM DESKTOP]** o **[!UICONTROL VIA FTP]**.
Seleziona questa opzione per estrarre automaticamente tutti i file dal file ZIP o TAR caricato. La stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.

   * **[!UICONTROL Includi sottocartelle]**: disponibile solo se è stata selezionata la scheda **[!UICONTROL VIA FTP]**.
Selezionate questa opzione per caricare le sottocartelle della cartella che intendete caricare. I nomi della cartella e delle relative sottocartelle caricate vengono immessi automaticamente in Adobe Dynamic Media Classic.

   * **[!UICONTROL Elabora file di metadati]**: disponibile solo se è stata selezionata la scheda **[!UICONTROL VIA FTP]**. Seleziona questa opzione se desideri caricare un file XML o delimitato da tabulazioni per aggiungere metadati a più risorse.
Consultate [Importare metadati (tramite FTP)](viewing-adding-exporting-metadata.md#import-metadata).

* **Opzioni di ritaglio**: ritaglia automaticamente i pixel dello spazio vuoto da un&#39;immagine. Apri il menu **[!UICONTROL Ritaglia]**, seleziona **[!UICONTROL Manuale]** e immetti le misure in pixel nei campi di testo In alto, A destra, In basso e A sinistra per ritagliare i lati. Puoi anche selezionare **[!UICONTROL Rifila]** dal menu Ritaglia e scegliere le seguenti opzioni:

   * **[!UICONTROL Rifila in base a]**: scegli se ritagliare in base al colore o alla trasparenza:
      * **[!UICONTROL Colore]**: scegliere l&#39;opzione Colore. Selezionate quindi il menu Angolo (Corner) e scegliete l&#39;angolo dell&#39;immagine con il colore che meglio rappresenta lo spazio bianco da ritagliare.
Rifilatura in base al colore: specifica 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell’angolo dell’immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 
      * **[!UICONTROL Trasparenza]**: scegliere l&#39;opzione **[!UICONTROL Trasparenza]**.
Rifilatura in base alla trasparenza: specificate 0 per ritagliare i pixel solo se sono trasparenti; i numeri più vicini a 1 consentono una maggiore trasparenza.
      * **[!UICONTROL Tolleranza]**: trascinare il dispositivo di scorrimento per specificare una tolleranza da 0 a 1.

* **Opzioni profilo colore**: scegli una conversione colore quando crei file ottimizzati utilizzati per la consegna dinamica di Adobe Dynamic Media Classic:

   * **[!UICONTROL Preservazione colore predefinita]**: mantiene i colori dell&#39;immagine di origine ogni volta che le immagini contengono informazioni sullo spazio colore. Non è presente alcuna conversione colore. In quasi tutte le immagini è incorporato il relativo profilo colore. Tuttavia, se un’immagine sorgente CMYK non contiene un profilo colore incorporato, i colori vengono convertiti nello spazio colore sRGB. sRGB è lo spazio colore consigliato per la visualizzazione delle immagini nelle pagine Web.
   * **[!UICONTROL Mantieni spazio colore originale]**: mantiene i colori originali senza alcuna conversione di colore al punto di acquisizione in Adobe Dynamic Media Classic. Per le immagini senza un profilo colore incorporato, l’eventuale conversione colore necessaria per elaborare le richieste per l’immagine viene eseguita utilizzando i profili colore predefiniti configurati nelle impostazioni di pubblicazione. Questi profili colore non sono sempre allineati con i colori dei file creati con questa opzione. Si consiglia quindi di utilizzare l’opzione Mantenimento colore predefinito.
   * **[!UICONTROL Personalizza da]** > **[!UICONTROL A]**: apre i menu per scegliere uno spazio colore **[!UICONTROL Converti da]** e **[!UICONTROL Converti in]**. Questa opzione avanzata ha priorità rispetto a eventuali informazioni di colore incorporate nel file sorgente. Seleziona questa opzione solo se tutte le immagini che stai inviando contengono dati di profilo colore errati o mancanti.

* **Opzioni di modifica immagine**: è possibile mantenere le maschere di ritaglio &lt;> nelle immagini e scegliere un profilo colore.
Consulta [Opzioni di ottimizzazione immagine al caricamento](image-editing-options-upload.md#image-editing-options-at-upload).

* **Opzioni di PostScript®**: è possibile rasterizzare i file di PostScript®, ritagliare i file, mantenere sfondi trasparenti, scegliere una risoluzione e scegliere uno spazio colore.
Consulta [Utilizzare i file PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Opzioni Photoshop**: è possibile creare modelli da file Adobe® Photoshop®, gestire i livelli, specificare il nome dei livelli, estrarre il testo e specificare come le immagini vengono ancorate nei modelli.
Consultate [Opzioni di caricamento PSD](psd-files.md#psd_upload_options).

* **Opzioni PDF**: è possibile rasterizzare i file, estrarre le parole e i collegamenti di ricerca, generare automaticamente un eCatalog, impostare la risoluzione e scegliere uno spazio colore.
Consultate [Opzioni di caricamento PDF](pdfs.md#pdf_upload_options).

* **Opzioni Illustrator**: puoi rasterizzare i file Adobe Illustrator®, mantenere sfondi trasparenti, scegliere una risoluzione e scegliere uno spazio colore.
Consulta [Utilizzare i file PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Opzioni EVIDEO**: è possibile trascodificare un file video scegliendo un predefinito per video.
Consulta [Utilizzare i predefiniti di codifica video](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Altri metadati**: immettere le parole chiave che descrivono i file che si intende caricare. Separate le parole chiave con una virgola. Le parole chiave facilitano la ricerca delle risorse.
Consulta [Eseguire una ricerca avanzata](searching-assets.md#conducting_an_advanced_search).
Vedi anche il video di formazione [Carica parole chiave](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS).

* **Predefiniti set di batch**: per creare un set di immagini, un set 360 gradi o un set di campioni dai file caricati, seleziona la colonna **[!UICONTROL Attivo]** per il predefinito che desideri utilizzare. Potete selezionare più di un predefinito. È possibile creare i predefiniti nella pagina Impostazione applicazione/Predefiniti set di batch.
Consultate [Predefiniti per set di batch](application-setup.md#batch_set_presets).

* **Avanzate**: vedi [Segui un caricamento con un altro processo](uploading-files.md#follow-an-upload-with-another-job).

## Avviare un altro processo al termine di un caricamento {#follow-an-upload-with-another-job}

Quando carichi gli elementi utilizzando l’FTP, puoi pianificare l’inizio di un processo successivo una volta completato il caricamento. Se è stato programmato l&#39;inizio di altri processi, i processi pianificati in questa posizione vengono messi in coda dopo di essi.

Il nuovo processo invia una notifica all&#39;indirizzo specificato in modo che il codice in tale posizione possa essere attivato. Questo processo di pubblicazione sequenziale usa lo stesso nome del processo di caricamento, con l’aggiunta del testo *Pub_* all’inizio.

**Per seguire un caricamento con un altro processo:**

1. Seleziona **[!UICONTROL Carica]**, quindi seleziona la scheda **[!UICONTROL VIA FTP]**.
1. Nell&#39;angolo inferiore destro della pagina Carica, seleziona **[!UICONTROL Opzioni processo]**.
1. Nella finestra di dialogo Opzioni processo di caricamento espandere la sezione **[!UICONTROL AVANZATE]**.
1. Scegliere una delle opzioni seguenti dall&#39;elenco a discesa **[!UICONTROL Segui caricamento con un altro processo]**:

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
   >I processi pianificati regolarmente possono talvolta impedire la pubblicazione di file.

>[!MORELIKETHIS]
>
>* [Utilizzare le cartelle di risorse](asset-folders.md#working_with_asset_folders)
>* [Gestisci processi di caricamento e pubblicazione ricorrenti](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Utilizza un processo di caricamento o pubblicazione come trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
