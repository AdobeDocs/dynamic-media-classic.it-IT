---
title: Caricare i file
description: Scopri come caricare i file in Adobe Systems Dynamic Media Classic.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '3929'
ht-degree: 31%

---

# Caricare i file{#uploading-files}

Prima di caricare risorse file in Adobe Systems Dynamic Media Classic, accertatevi che i file di risorsa siano denominati correttamente e che la struttura della cartella sia configurata e organizzata nel modo desiderato. Potete caricare i file da un Adobe Systems Dynamic Media sito FTP fornito in versione classica o direttamente dal computer o dalla rete. Adobe Systems Dynamic Media Classic offre opzioni per ottimizzare i file mentre li caricate. Se hai installato Adobe Systems Dynamic Media applicazione desktop classici, puoi caricare file e cartelle trascinandoli direttamente dal desktop. Consultate [Impostazioni generali applicazione](application-setup.md#general_settings).

## Prepara le risorse e le cartelle per il caricamento {#preparing-your-assets-and-folders-for-uploading}

Prima di caricare risorse in Adobe Systems Dynamic Media Classic, accertatevi che siano nel formato e nelle dimensioni giuste. È inoltre necessario osservare il Adobe Systems Dynamic Media regole classiche per la denominazione dei risorse. È anche utile organizzare e disporre i file in una cartella per semplificarne l’individuazione e l’utilizzo. 

### Formati di file di risorse supportati {#supported-asset-file-formats}

In questa tabella sono elencati i formati di file di risorse supportati da Adobe Dynamic Media Classic. Per informazioni sui file Camera Raw supportati, consulta [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

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

### Formati di immagine non supportati in Dynamic Media {#unsupported-image-formats-dynamic-media}

Nell&#39;elenco seguente sono descritti i sottotipi di formati file di immagine raster che non *sono* supportati in Dynamic Media.

Vedi anche [ rilevare i formati di file non supportati per Dynamic Media ](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html) .

* File PNG con una dimensione di blocco IDAT maggiore di 100 MB.
* File PSB.
* I file PSD con uno spazio colore diverso da CMYK, RGB, Scala di grigi o Bitmap non sono supportati. DuoTone, Lab e gli spazi colore indicizzati non sono supportati.
* File PSD con una profondità di bit maggiore di 16.
* File TIFF con dati a virgola mobile.
* File TIFF con spazio colore Lab.

### Tipi di risorse {#asset-types}

Per ottenere risultati ottimali con il programma Adobe Systems Dynamic Media Classic, assicuratevi di utilizzare i formati e le dimensioni dei file consigliati. Nella tabella seguente sono elencati i tipi di risorse con i formati e le dimensioni di file consigliati per le risorse usate comunemente.

| Tipo di risorsa | Descrizione/Consigli |
| --- | --- |
| Audio | I formati per l’input di risorse audio comprendono AAC, HE-AAC, AC3, WAV, WMA, AIFF e MP3. Potete transcodificare l’audio nei seguenti formati: MP3, AAC e HE-AAC. |
| Immagini (per Ridimensionamento immagini, Zoom, Set immagini, Set 360 gradi) | Le immagini devono avere almeno 2000 pixel alla dimensione più lunga; le dimensioni delle immagini tipiche variano da 1500 a 2500 pixel nella dimensione più lunga. Si consiglia di usare formati immagine senza perdita di dati, come i formati TIFF e PNG. Per le immagini JPEG, usate le impostazioni di qualità massima. I file di animazione GIF vengono gestiti come altri contenuti statici. |
| eCatalog | Utilizza i file PDF ad alta risoluzione creati in Adobe Acrobat o un’applicazione di Creative Suite di Adobe salvata come &quot;press-ready&quot;. I file PDF includono tutti i font, le immagini, le maschere e gli elementi grafici di riferimento necessari nel formato a pagina singola, a due pagine affiancate o a più pagine. Ordinate le pagine assegnando ai file nomi in ordine alfanumerico. Salvate tutti i file PDF dell’eCatalog in un’unica cartella per semplificarne il caricamento. Potete selezionare le opzioni di ritaglio al momento del caricamento per rimuovere l’area di ritaglio dai file PDF, inclusi gli indicatori di taglio, i crocini di registro o le barre colore. La maggior parte dei file PDF pronti per la usano lo spazio cromatico CMYK; è quindi importante ottenere il profilo colore ICC CMYK usato con i file PDF. |
| Modelli | Un’immagine con livelli o un layout può includere testo, immagini e livelli. I livelli immagine, le stringhe di testo e gli attributi, quali il colore e le dimensioni, possono essere parametrizzati in modo da personalizzare i dati variabili. I requisiti delle immagini da usare nei modelli sono gli stessi delle altre immagini. Preparate gli elementi grafici in Photoshop o in un altro programma di modifica delle immagini. Salvate ogni elemento grafico come file trasparente a livello unico nel formato TIFF o PNG. Assicuratevi che la risoluzione delle immagini sia appropriata all’uso previsto. Le immagini da stampare sono 300 ppi. |
| Video | Adobe Systems Dynamic Media Classic supporta i file video salvati in formato OGV e MP4. Potete transcodificare i file in formato MP4 al momento del caricamento. Consultate [Formati di file di risorse supportati](#supported-static-file-formats). |
| Font | Sono stati caricati TrueType, Type1 (solo Windows®), OpenType ® font e PhotoFonts. |
| Immagini | Immagini e file immagine con più livelli. |
| Set di immagini e set di campioni | Set di immagini correlate che possono essere visualizzate in un visualizzatore. |
| Profili ICC | Un profilo colore che puoi utilizzare per convertire un’immagine caricata dal suo spazio colore sorgente in uno spazio colore diverso. |
| Vignettature | Immagini create con il programma di authoring Immagine e i relativi file. |
| File contenuto | File di contenuto Adobe InDesign, Illustrator o Photoshop. |
| File FXG | File di formato grafico indipendenti dalla risoluzione che potete usare per creare modelli personalizzabili per la stampa, il Web, l’e-mail, il desktop e i dispositivi.  |
| File SVG | File di grafica vettoriale scalabile che possono essere sottoposti a rendering sui server Image Server.  |
| File XML | File che definiscono le regole di pre-elaborazione usate per modificare il percorso e le porzioni di query delle richieste.  |
| File Cascading Style Sheet. | Potete caricare interfacce CSS per personalizzare i visualizzatori HTML5. |
| File JavaScript | I file JavaScript vengono utilizzati per la strumentazione del visualizzatore per memorizzare le informazioni sull&#39;account. Adobe di protezione consiglia questo tipo di risorsa solo per gli account client che hanno un dominio separato in uso per la distribuzione (per evitare script tra siti). |

>[!NOTE]
>
>Quando si caricano file di immagine e PDF in Adobe Dynamic Media Classic, questi vengono convertiti in file P-TIFF (Pyramid TIFF). Questi TIFF-P sono i file che vengono successivamente pubblicati nei server immagini Dynamic Media. Adobe Dynamic Media Classic utilizza il formato di file Tiff piramidale perché contiene vari rapporti di zoom che consentono uno zoom rapido quando viene visualizzato con un Visualizzatore zoom di Adobe Dynamic Media Classic.

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

Adobe Systems Dynamic Media Classic non fornisce l&#39;opzione per generare un&#39;anteprima URL di contenuto statiche.

### Requisiti per i nomi di file {#filename-requirements}

Poiché nelle estensioni viene rimosso il nome del file durante il processo di caricamento, nel sistema non sono consentiti file con lo stesso nome radice. Nel sistema Adobe Systems Dynamic Media Classic, il nome del file risorsa meno l&#39;estensione del nome file diventa l&#39;ID risorsa per la risorsa. Per questo motivo non sono consentite due risorse con lo stesso nome.

Assicurati che tutti gli utenti della tua azienda comprendano queste regole per la denominazione dei file:

* Non sono consentiti nel sistema ID di risorse con lo stesso identico nome.
* I nomi degli ID risorsa fanno distinzione tra maiuscole e minuscole.
* Come procedura consigliata assicuratevi che gli ID delle risorse non contengano spazi vuoti, ad esempio evitate di usare nomi come giacca nera.tif o giacca blu.jpg. Adobe Systems Dynamic Media Classic ASCII-codifica spazi vuoti nei nomi risorsa quando utilizza risorsa nomi per costruire URL stringhe. Poiché questi codici ASCII sono difficili da leggere, la lettura degli URL può risultare più complicata.
* I nomi file possono contenere caratteri specifici per particolari lingue. Tuttavia, non possono contenere i seguenti caratteri:

   \ ; / ? : @ &amp; = + $ , &#42; &quot; &lt; > | &#39; { } %

   Se il nome del file contiene uno o più di questi caratteri, questi vengono eliminati dal nome del file al momento del caricamento.

In genere, un nome di file risorsa può corrispondere al numero di elemento, al referenza di magazzino del prodotto o a un altro, come nel seguente:

| Elemento | Nome file | ID risorsa |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organizzazione e struttura delle cartelle {#folder-organization-and-structure}

Organizza e struttura cartelle e sottocartelle per i contenuti in Adobe Dynamic Media Classic prima di caricarli. La pianificazione preventiva di questa procedura presenta i due grandi vantaggi seguenti:

* Quando caricate il contenuto per Adobe Systems Dynamic Media Classic tramite FTP, potete dire al sistema di replicare la struttura delle cartelle durante il caricamento. In questo modo, il contenuto viene organizzato nelle stesse cartelle e sottocartelle di Adobe Dynamic Media Classic presenti nel computer o in rete. Per replicare la struttura di cartelle in Adobe Dynamic Media Classic, seleziona l’opzione Includi sottocartelle quando carichi le risorse tramite FTP.
* Riorganizzare le cartelle all’interno del sistema dopo il caricamento dei file è molto più difficile rispetto a iniziare la procedura con una struttura di cartelle pianificata con attenzione.

L’approccio e la struttura di denominazione delle cartelle scelti per memorizzare il contenuto sul Adobe Dynamic Media Classic dipende dalle esigenze della tua organizzazione. Di seguito sono riportati alcune strutture di cartelle di esempio:

**Basato su SKU** - Le cartelle vengono denominate in base agli SKU o ai numeri di elemento. Vengono ad esempio create cartelle separate per tutte le serie di numeri 0-, 20-, 30.

**Basato sul** marchio-per i produttori con più linee di marchio e rivenditori che mercato altri marchi di altre aziende, separare i file in cartelle di prodotti denominate per diversi marchi.

**Le cartelle basate su** progetto sono organizzate in base alla data di rollout/rilascio o al nome del progetto. Questa procedura è preferita dai clienti che si occupano principalmente della produzione di eCatalog. 

**Mirror della gerarchia** delle cartelle del sito Web: questa struttura di cartelle rispecchia la struttura della cartella del sito Web, con le cartelle denominate, ad esempio, per le categorie di prodotti.

## Informazioni sul caricamento dei file {#uploading-your-files}

Potete caricare singoli file dal desktop oppure caricare le cartelle mediante FTP. Per caricare più di 100 MB di file o intere cartelle e sottocartelle, selezionare **TRAMITE FTP** scheda.

Adobe Dynamic Media Classic ti invia un messaggio e-mail per confermare quando inizia e termina il processo di caricamento e per avvisarti di eventuali problemi.

Durante (o immediatamente dopo) un processo di caricamento di grandi dimensioni, alcuni nuovi elementi potrebbero visualizzare il messaggio &quot;Immagine non ancora ottimizzato&quot;. Questo messaggio viene visualizzato perché i file non sono ancora stati completamente elaborati e aggiunti a Adobe Systems Dynamic Media Classic. Potete ottimizzare questi file successivamente. Consultate [ ottimizzare i file ](application-setup.md#optimize_files) .

### Caricare i file utilizzando la scheda Da desktop {#upload-files-using-sps-desktop-application}

L&#39;applicazione Adobe Dynamic Media Classic Desktop consente di caricare file e cartelle trascinandoli.

1. Nell&#39;applicazione Adobe Dynamic Media Classic Desktop, nella barra di navigazione globale, selezionare **[!UICONTROL Carica]**.
1. Nella pagina Carica, seleziona la **[!UICONTROL Da desktop]** scheda.
1. Sul lato sinistro della pagina Carica, nella **[!UICONTROL Seleziona i file da caricare]** area, seleziona **[!UICONTROL Sfoglia]** per selezionare i file o le cartelle da caricare, quindi seleziona **[!UICONTROL Apri]**.
1. Sul lato destro della pagina Carica, nella **Scegliete la destinazione della cartella** , passare a una cartella di destinazione in cui si desidera aggiungere i file o le cartelle caricati.
1. (Facoltativo) Nella parte inferiore della pagina Carica, immetti il nuovo nome del processo di caricamento nel campo di testo Nome processo. In alternativa, è possibile utilizzare semplicemente il nome predefinito generato dal sistema fornito da Adobe Dynamic Media Classic. Il processo in corso e gli altri processi di caricamento e pubblicazione vengono registrati nella pagina Processi dove è possibile controllarne lo stato. Consultate [Verifica dei file di processo](checking-job-files.md#checking_job_files).
1. (Facoltativo) Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Pubblica dopo il caricamento]** per pubblicare automaticamente le risorse caricate.
Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. Facoltativo Nella parte inferiore della pagina di caricamento, seleziona **[!UICONTROL Sovrascrivi in qualsiasi cartella, stessa base risorsa nome, indipendentemente dall&#39;estensione]** , se desideri che i file caricati sostituiscano i file esistenti con gli stessi nomi. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni nella **[!UICONTROL configurazione]** dell&#39;applicazione > **[!UICONTROL Generale impostazioni]** > **[!UICONTROL upload to Application]** > **[!UICONTROL Sovrascrivi immagini]** .
1. Nell&#39;angolo in basso a destra della pagina di caricamento, seleziona **[!UICONTROL processo opzioni]** , quindi specifica le opzioni desiderate.

   Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

1. Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Salva]**.
1. Nell&#39;angolo in basso a destra della pagina di caricamento, selezionate **[!UICONTROL Invia caricamento]** .
Per visualizzare l&#39;avanzamento del caricamento, selezionate **[!UICONTROL i processi]** nella barra di navigazione globale. È possibile continuare a lavorare in Adobe Systems Dynamic Media Classic e tornare alla pagina processi in qualsiasi momento per rivedere un processo in corso. Per annullare un processo di caricamento in corso, fate clic sul pulsante **[!UICONTROL Annulla]** accanto alla durata.

### Caricate i file utilizzando il scheda VIA FTP {#upload-files-using-via-ftp}

1. Accedi al Adobe Systems Dynamic Media sito FTP classico specifico per la tua particolare area geografica. Utilizzate il nome utente e la password per FTP ricevuti dall’amministratore.
1. In Adobe Systems Dynamic Media Classic, nella barra di navigazione globale, seleziona **[!UICONTROL carica]** .
1. Nella pagina carica, selezionare la **[!UICONTROL scheda via FTP]** .
1. Nella parte sinistra della pagina di caricamento, nell&#39; **[!UICONTROL area scegli cartella FTP per il caricamento]** , scegliete una cartella FTP da cui caricare i file.
1. Nella parte destra della pagina di caricamento, nell&#39; **[!UICONTROL area scegli Adobe Systems Dynamic Media cartella destinazione]** , scegliete una cartella di destinazione in Adobe Systems Dynamic Media Classic.
1. Facoltativo Nella parte inferiore della pagina di caricamento, nel campo di testo nome processo, immettete il nuovo nome del processo di caricamento. Oppure, puoi semplicemente utilizzare il nome predefinito generato dal sistema che Adobe Systems fornisce Dynamic Media Classic. Il processo in corso e gli altri processi di caricamento e pubblicazione vengono registrati nella pagina Processi dove è possibile controllarne lo stato.
Consultate [Verifica dei file di processo](checking-job-files.md#checking_job_files).
1. Facoltativo Nella parte inferiore della pagina di caricamento, seleziona **[!UICONTROL Publish dopo il caricamento]** se desideri pubblicare automaticamente il risorse che carichi.
Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. La stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. (Facoltativo) Nella parte inferiore della pagina Carica, seleziona **[!UICONTROL Sovrascrivi in qualsiasi cartella, nome come risorsa base, ignora estensione]** se si desidera che i file caricati sostituiscano i file esistenti con gli stessi nomi. La stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali]** > **[!UICONTROL Carica nell&#39;applicazione]** > **[!UICONTROL Sovrascrivi immagini]**.
1. Facoltativo; disponibile solo se si è fatto clic su **[!UICONTROL TRAMITE FTP]** scheda. Nella parte inferiore della pagina di caricamento, seleziona **[!UICONTROL Annulla compressione zip o tar file al caricamento]** se desideri estrarre automaticamente tutti i file dal file zip o tar caricato. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. Nell&#39;angolo in basso a destra della pagina di caricamento, seleziona **[!UICONTROL processo opzioni]** , quindi specifica le opzioni desiderate.

   Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

1. Nella finestra di dialogo Opzioni processo di caricamento, selezionare **[!UICONTROL Salva]** .
1. Nell&#39;angolo in basso a destra della pagina di caricamento, selezionate **[!UICONTROL Invia caricamento]** .

   Per visualizzare l&#39;avanzamento del caricamento, nella barra di navigazione globale, selezionare **[!UICONTROL processi]** . Viene visualizzata la pagina Processi che mostra l’avanzamento del caricamento. È possibile continuare a lavorare in Adobe Systems Dynamic Media Classic e tornare alla pagina processi in qualsiasi momento per rivedere un processo in corso.

Per annullare un processo di caricamento in corso, fate clic sul pulsante **[!UICONTROL Annulla]** accanto alla durata.

## Finestra di dialogo Opzioni processo di caricamento {#upload-options}

Quando caricate dei file, potete scegliere una delle seguenti opzioni nella finestra di dialogo Opzioni processo di caricamento:

* **** Processo-seleziona **[!UICONTROL processo]** per scegliere le opzioni che influiscono sull&#39;intero processo di caricamento.

   È inoltre possibile scegliere *le opzioni predefinite* per il caricamento dei processi utilizzando la **[!UICONTROL finestra di dialogo Carica predefinita Opzioni]** in generale impostazioni. Vai a **[!UICONTROL configurazione]** > **[!UICONTROL impostazione applicazione]** > **[!UICONTROL Generale impostazioni]** > **[!UICONTROL Opzioni]** di caricamento predefinito, quindi imposta le opzioni predefinite desiderate.

   * **[!UICONTROL Quando]** - Questa opzione è disponibile solo se è stato selezionato il **[!UICONTROL TRAMITE FTP]** scheda.
      * **[!UICONTROL Una tantum]** : specifica un processo di caricamento che viene eseguito una volta. Le opzioni includono:
         * **[!UICONTROL Ora]** - Esegue il processo di caricamento subito dopo aver selezionato **[!UICONTROL Salva]** nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Invia caricamento]** nella pagina Carica.
         * **[!UICONTROL Pianifica per un momento successivo]** : seleziona l’anno, il mese, il giorno e l’ora (con incrementi di 15 minuti) in cui desideri eseguire il processo di caricamento.
      * **[!UICONTROL Periodico]** -specifica un processo di caricamento che viene eseguito quotidianamente, settimanalmente o mensilmente. In alternativa, Personalizza il processo di caricamento secondo le tue specifiche.
         * **[!UICONTROL Giornaliero]** -consente di regolare l&#39;ora in cui si desidera eseguire il processo ogni giorno. Se desideri che il processo venga eseguito solo dal lunedì al venerdì, seleziona **[!UICONTROL solo]** i giorni feriali.
         * **[!UICONTROL Settimanale]** -Scegli un giorno specifico della settimana e dell&#39;ora in cui desideri eseguire il processo.
         * **[!UICONTROL Mensile]** -Scegli un giorno specifico del mese o del giorno della settimana, compreso l&#39;ora di inizio, in cui desideri eseguire il processo.
         * **[!UICONTROL Personalizzato]** : personalizza l’intervallo di tempo di un processo di caricamento o pubblicazione in base alle tue specifiche. Consulta [Creare un intervallo di tempo del processo di caricamento o pubblicazione personalizzato](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **[!UICONTROL Pubblica dopo il caricamento]** - Disponibile se è stata selezionata l&#39;opzione **[!UICONTROL DAL DESKTOP]** scheda o **[!UICONTROL TRAMITE FTP]** scheda. Selezionate questa opzione per pubblicare automaticamente le risorse caricate. Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa opzione è disponibile anche nella pagina di caricamento.

   * **[!UICONTROL Sovrascrivi in qualsiasi cartella, stessa base risorsa nome, indipendentemente dall&#39;estensione]** , disponibile se hai selezionato la **[!UICONTROL scheda da desktop]** o **[!UICONTROL via FTP]** scheda. Selezionate questa opzione per sostituire i file esistenti con quelli caricati mantenendo gli stessi nomi. Questa opzione è disponibile anche nella pagina di caricamento. Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali]** > **[!UICONTROL Carica nell&#39;applicazione]** > **[!UICONTROL Sovrascrivi immagini]**.

   * **[!UICONTROL Decomprimi file Zip o Tar al caricamento]** - Disponibile se è stata selezionata l&#39;opzione **[!UICONTROL DAL DESKTOP]** scheda o **[!UICONTROL TRAMITE FTP]** scheda.
Seleziona questa opzione se desideri estrarre automaticamente tutti i file dal file ZIP o TAR caricato. La stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.

   * **[!UICONTROL Includi sottocartelle]** - Disponibile solo se è stata selezionata la **[!UICONTROL TRAMITE FTP]** scheda.
Selezionate questa opzione per caricare le sottocartelle della cartella che intendete caricare. I nomi della cartella e delle relative sottocartelle caricate vengono immessi automaticamente in Adobe Dynamic Media Classic.

   * **[!UICONTROL Elabora file di metadati]** - Disponibile solo se è stata selezionata l&#39;opzione **[!UICONTROL TRAMITE FTP]** scheda. Selezionate questa opzione se desiderate caricare un file delimitato da tabulazioni o XML per aggiungere metadati a più risorse. Consultate [Importare metadati (tramite FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **Opzioni di ritaglio** - Per ritagliare automaticamente i pixel dello spazio bianco da un&#39;immagine, aprire **[!UICONTROL Ritaglio]** menu, seleziona **[!UICONTROL Manuale]**, e immettere le misure in pixel nei campi di testo In alto, A destra, In basso e A sinistra per ritagliare i dati dai lati. Puoi anche selezionare **[!UICONTROL Rifila]** scegliere le opzioni seguenti dal menu Ritaglia:

   * **[!UICONTROL Rifila basato su]** -Scegli se ritagliare in base al colore o alla trasparenza:
      * **[!UICONTROL Colore]** -scegliete l&#39;opzione colore. Dal menu Angolo scegliete quindi l’angolo dell’immagine con il colore che rappresenta meglio quello dello spazio bianco da ritagliare.
Rifilatura in base al colore: specificate 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell&#39;angolo dell&#39;immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 
      * **[!UICONTROL Trasparenza]** -scegliete l&#39; **[!UICONTROL opzione trasparenza]** .
Ritaglio in base alla trasparenza: specificare 0 per ritagliare i pixel solo se sono trasparenti; i numeri più vicini a 1 consentono una maggiore trasparenza.
      * **[!UICONTROL Tolleranza]** - Trascinate il cursore per specificare una tolleranza da 0 a 1.

* **Opzioni profilo colore** : scegli una conversione colore quando crei file ottimizzati utilizzati per la distribuzione dinamica di Adobe Dynamic Media Classic:

   * **[!UICONTROL Conservazione]** colore predefinita-mantiene i colori dell&#39;immagine sorgente ogni volta che le immagini contengono informazioni sullo spazio colore; non c&#39;è conversione colore. In quasi tutte le immagini è incorporato il relativo profilo colore. Tuttavia, se un’immagine sorgente CMYK non contiene un profilo colore incorporato, i colori vengono convertiti nello spazio colore sRGB. sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.
   * **[!UICONTROL Mantieni Spazio cromatico]** originale-mantiene i colori originali senza alcuna conversione di colore nel punto di ingestione in Adobe Systems Dynamic Media Classic. Per le immagini prive di un profilo colore incorporato, qualsiasi conversione di colore necessaria per elaborare le richieste per l&#39;immagine viene effettuata utilizzando i profili colore predefiniti come configurato nelle impostazioni di Publish. Questi profili colore non sempre vengono allineati con il colore nei file creati con questa opzione. Si consiglia quindi di utilizzare l’opzione Mantenimento colore predefinito.
   * **[!UICONTROL Personalizzato da]** > **[!UICONTROL a]** -apre i menu in modo da poter scegliere uno **[!UICONTROL spazio di conversione da]** e **[!UICONTROL convertire in]** colore. Questa opzione avanzata ha priorità rispetto a eventuali informazioni di colore incorporate nel file sorgente. Selezionate questa opzione solo quando tutte le immagini che state inviando contengono dati di profilo colore errati o mancanti.

* **Immagine opzioni** di modifica-potete mantenere le maschere di ritaglio &lt;> nelle immagini e scegliere un profilo colore.
Consultate [ immagine opzioni di regolazione fine al caricamento ](image-editing-options-upload.md#image-editing-options-at-upload) .

* **Opzioni PostScript®** - È possibile rasterizzare i file di PostScript®, ritagliare i file, mantenere sfondi trasparenti, scegliere una risoluzione e scegliere uno spazio colore.
Consulta [Utilizzare i file PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Opzioni Photoshop** - Potete creare modelli da file Adobe® Photoshop®, gestire i livelli, specificare il nome dei livelli, estrarre il testo e specificare come le immagini vengono ancorate ai modelli.
Consultate [Opzioni di caricamento PSD](psd-files.md#psd_upload_options).

* **Opzioni PDF** - È possibile rasterizzare i file, estrarre parole di ricerca e collegamenti, generare automaticamente un eCatalog, impostare la risoluzione e scegliere uno spazio colore.
Consultate [Opzioni di caricamento PDF](pdfs.md#pdf_upload_options).

* **Illustrator opzioni** -potete rasterizzare Adobe Illustrator file®, mantenere sfondi trasparenti, scegliere una risoluzione e scegliere uno spazio colore.
Consultate [ lavorare con file ](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files) PostScript e Illustrator.

* **Opzioni** EVIDEO-potete transcodificare un file video scegliendo un video predefinito.
Consultate [ utilizzare i predefiniti ](uploading-encoding-videos.md#working_with_video_encoding_presets) di codifica video.

* **Metadati** aggiuntivi-immettete le parole chiave che descrivono i file che intendete caricare. Separate le parole chiave con una virgola. Le parole chiave consentono di effettuare ricerche di risorse in modo semplificato. Consulta [Eseguire una ricerca avanzata](searching-assets.md#conducting_an_advanced_search). Consultate anche [ caricare le parole chiave ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) training video.

* **Batch set Predefiniti** -se desideri creare un set di immagine, un set 360 gradi o un set di campioni dai file caricati, seleziona la **[!UICONTROL colonna attiva]** per il predefinito da utilizzare. Potete selezionare più di un predefinito. Potete creare i predefiniti nella pagina Impostazione applicazione/Predefiniti set di batch. Consultate [Predefiniti per set di batch](application-setup.md#batch_set_presets).

* **Avanzate** -vedere [ seguire un caricamento con un altro processo ](uploading-files.md#follow-an-upload-with-another-job) .

## Avviare un altro processo al termine di un caricamento {#follow-an-upload-with-another-job}

Quando caricate gli elementi tramite FTP, potete programmare un processo successivo per iniziare al termine del caricamento. Se altri processi sono programmati per iniziare, il processo che si programmare qui viene messo in coda dopo di loro.

Il nuovo processo Invia un notifica all&#39;indirizzo specificato in modo che possa essere attivato il codice in tale posizione. Questo processo di pubblicazione sequenziale usa lo stesso nome del processo di caricamento, con l’aggiunta del testo *Pub_* all’inizio.

**Per avviare un altro processo al termine di un caricamento:**

1. Seleziona **[!UICONTROL carica]** , quindi seleziona l&#39; **[!UICONTROL scheda via FTP]** .
1. Nell&#39;angolo in basso a destra della pagina di caricamento, selezionate **[!UICONTROL Job opzioni]** .
1. Nella finestra di dialogo Opzioni processo di caricamento, espandi **[!UICONTROL AVANZATE]** sezione.
1. Scegliete una delle seguenti opzioni dalla **[!UICONTROL Dopo il caricamento, continua con un altro processo]** elenco a discesa:

   * Nessuno
   * Richiesta HTTP
   * Pubblicazione da Image Server
   * Pubblicazione da Image Rendering
   * Pubblicazione video

1. Specificate l’indirizzo HTTP.
1. Specifica se si desidera eseguire solo se i file sono stati caricati.
1. Specificate se la richiesta deve essere eseguita ogni volta che termina il processo oppure solo quando i file sono stati pubblicati. 

   >[!NOTE]
   >
   >I processi pianificati regolarmente possono talvolta impedire la pubblicazione di file.

>[!MORELIKETHIS]
>
>* [Utilizzare le cartelle di risorse](asset-folders.md#working_with_asset_folders)
>* [Gestire i processi di caricamento e pubblicare ricorrenti](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Utilizzare un processo di caricamento o pubblicare come attivatore](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

