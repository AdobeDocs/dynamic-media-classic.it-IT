---
title: Caricamento dei file
seo-title: Caricamento dei file
description: 'null'
seo-description: Scoprite come caricare i file.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
translation-type: tm+mt
source-git-commit: d5dcc67200b636cafcf1c87b2ecdfb2271b7b9a2
workflow-type: tm+mt
source-wordcount: '3867'
ht-degree: 52%

---


# Caricamento dei file{#uploading-files}

Prima di caricare i file di risorse su Scene7 Publishing System, assicuratevi che presentino i nomi corretti e che la struttura delle cartelle sia impostata e organizzata come desiderato. Potete caricare i file da un sito FTP fornito da Dynamic Media Classic o direttamente dal computer o dalla rete. Dynamic Media Classic offre opzioni per l’ottimizzazione dei file durante il caricamento. Se è stata installata l’applicazione desktop di Adobe Scene7 Publishing System, potete caricare i file e le cartelle trascinandoli direttamente dal desktop. Consultate [Impostazioni generali dell’applicazione](application-setup.md#general_settings).

## Preparazione delle risorse e delle cartelle per il caricamento {#preparing-your-assets-and-folders-for-uploading}

Prima di caricare le risorse in Scene7 Publishing System, assicuratevi che siano nel formato e con le dimensioni appropriati. Dovete inoltre rispettare le regole Dynamic Media Classic per la denominazione delle risorse. È anche utile organizzare e disporre i file in una cartella per semplificarne l’individuazione e l’utilizzo. 

### Formati di file di risorse supportati {#supported-asset-file-formats}

In questa tabella sono elencati i formati di file di risorse supportati in Scene7 Publishing System. For information on supported Camera Raw files, see [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| Formati di file di risorse | Descrizione |
|--- |--- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Cascading Style Sheet | CSS |
| Profili colore | ICC, ICM |
| Font | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Immagini | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (solo Windows), TIF, TIFF |
| InDesign | INDD, INDT |
| MS Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG e Camera Raw |
| PostScript | EPS, PS |
| Dynamic Media Classic Image Authoring | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Video | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

Il supporto per il caricamento di file TAR e ZIP comprende una casella di controllo per selezionare la decompressione dei file.

### Formati immagine non supportati in Dynamic Media {#unsupported-image-formats-dynamic-media}

Nell&#39;elenco seguente sono descritti i sottotipi di formati di file immagine raster *non* supportati in Contenuti multimediali dinamici.

Consultate anche [Rilevamento di formati di file non supportati per gli elementi multimediali](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html)dinamici.

* File PNG con dimensioni blocco IDAT superiori a 100 MB.
* File PSB.
* I file PSD con uno spazio colore diverso da CMYK, RGB, Scala di grigio o Bitmap non sono supportati. Gli spazi colore DuoTone, Lab e Indexed non sono supportati.
* File PSD con una profondità di bit maggiore di 16.
* File TIFF con dati a virgola mobile.
* file TIFF con spazio colore Lab.

### Tipi di risorse {#asset-types}

Per ottenere risultati ottimali con la piattaforma Dynamic Media Classic, utilizzate i formati e le dimensioni file consigliati. Nella tabella seguente sono elencati i tipi di risorse con i formati e le dimensioni di file consigliati per le risorse usate comunemente.

| Tipo di risorsa | Descrizione/Consigli |
|--- |--- |
| Audio | I formati per l’input di risorse audio comprendono AAC, HE-AAC, AC3, WAV, WMA, AIFF e MP3. Potete transcodificare l’audio nei seguenti formati: MP3, AAC e HE-AAC. |
| Immagini (per Ridimensionamento immagini, Zoom, Set immagini, Set 360 gradi) | Le immagini devono avere il lato più lungo pari ad almeno 2000 pixel; le dimensioni delle immagini sono in genere comprese tra 1500 e 2500 pixel per il lato più lungo. Si consiglia di usare formati immagine senza perdita di dati, come i formati TIFF e PNG. Per le immagini JPEG, usate le impostazioni di qualità massima. I file GIF animati vengono gestiti come altri contenuti statici. |
| eCatalog | Usate i file PDF ad alta risoluzione creati in Adobe® Acrobat® o in un’applicazione Creative Suite salvati come “pronta per la stampa”. I file PDF includono tutti i font, le immagini, le maschere e gli elementi grafici di riferimento necessari nel formato a pagina singola, a due pagine affiancate o a più pagine. Ordinate le pagine assegnando ai file nomi in ordine alfanumerico. Salvate tutti i file PDF dell’eCatalog in un’unica cartella per semplificarne il caricamento. Potete selezionare le opzioni di ritaglio al momento del caricamento per rimuovere l’area di ritaglio dai file PDF, inclusi gli indicatori di taglio, i crocini di registro o le barre colore. La maggior parte dei file PDF pronti per la usano lo spazio cromatico CMYK; è quindi importante ottenere il profilo colore ICC CMYK usato con i file PDF. |
| Modelli | Un’immagine con livelli o un layout può includere testo, immagini e livelli. I livelli immagine, le stringhe di testo e gli attributi, quali il colore e le dimensioni, possono essere parametrizzati in modo da personalizzare i dati variabili. I requisiti delle immagini da usare nei modelli sono gli stessi delle altre immagini. Preparate gli elementi grafici in Photoshop o in un altro programma di modifica delle immagini. Salvate ogni elemento grafico come file trasparente a livello unico nel formato TIFF o PNG. Assicuratevi che la risoluzione delle immagini sia appropriata all’uso previsto. Le immagini da stampare devono essere a 300 ppi. |
| Video | Dynamic Media Classic supporta i file video salvati in formato OGV e MP4. Potete transcodificare i file in formato MP4 al momento del caricamento. Consultate Formati [di file di risorse](#supported-static-file-formats)supportati. |
| Font | Font TrueType, Type1 (solo Windows), OpenType caricati e PhotoFonts caricati |
| Immagini | Immagini e file immagine con più livelli. |
| Set di immagini e set di campioni | Set di immagini correlate che possono essere visualizzate in un visualizzatore. |
| Profili ICC | Profilo colore che potete usare per convertire un’immagine caricata dallo spazio colore di origine in un altro spazio colore. |
| Vignettature | Immagini create con il programma Image Authoring e i file correlati. |
| File contenuto | File di contenuto Adobe InDesign, Illustrator o Photoshop. |
| File FXG | File di formato grafico indipendenti dalla risoluzione che potete usare per creare modelli personalizzabili per la stampa, il Web, l’e-mail, il desktop e i dispositivi.  |
| File SVG | File di grafica vettoriale scalabile che possono essere sottoposti a rendering sui server Image Server.  |
| File XML | File che definiscono le regole di pre-elaborazione usate per modificare il percorso e le porzioni di query delle richieste.  |
| File Cascading Style Sheet. | Potete caricare interfacce CSS per personalizzare i visualizzatori HTML5. |
| File JavaScript | Nei file JavaScript vengono memorizzate le informazioni account durante la scrittura del codice per il visualizzatore. Adobe Security consiglia di usarli solo per gli account di clienti con un dominio separato per la consegna (per evitare il rischio di scripting attraverso più siti). |

>[!NOTE]
>
>quando caricate file immagine e file PDF in SPS, questi file sorgente vengono convertiti nel formato P-TIFF (TIFF piramidale). Questi file P-TIFF sono i file che verranno pubblicati successivamente sui server di immagini per file multimediali dinamici. Dynamic Media Classic utilizza il formato di file Tiff piramidale, in quanto contiene vari rapporti di zoom che consentono di eseguire rapidamente lo zoom quando viene visualizzato con un visualizzatore zoom dinamico Media Classic.

### Formati di file statici supportati {#supported-static-file-formats}

Dynamic Media Classic supporta diversi formati di file statici. Per contenuto statico si intende qualsiasi risorsa pubblicata &quot;così com’è&quot;, ad esempio CSS, PDF, SVG, XML e così via.

È possibile pubblicare i seguenti tipi di file:

* GIF animata
* File audio
* CSS
* JavaScript (se la società è configurata con un proprio dominio)
* Video Master
* PDF (se il file PDF è specificatamente contrassegnato per la pubblicazione dopo il caricamento, per evitare la distribuzione di tutti i file PDF per il flusso di lavoro eCatalog/PDF esistente)
* Video PrX
* SVG
* XML
* ZIP

Dynamic Media Classic non fornisce l&#39;opzione per generare un URL di anteprima del contenuto statico.

### Requisiti per i nomi di file {#filename-requirements}

Poiché nelle estensioni viene rimosso il nome del file durante il processo di caricamento, nel sistema non sono consentiti file con lo stesso nome radice. Nel sistema Dynamic Media Classic, il nome del file della risorsa meno l’estensione diventa l’ID della risorsa. Per questo motivo non sono consentite due risorse con lo stesso nome.

Assicuratevi che le seguenti regole di denominazione dei file vengano comprese da tutti gli utenti della società:

* Non sono consentiti nel sistema ID di risorse con lo stesso identico nome.
* I nomi ID delle risorse seguono la distinzione tra maiuscole e minuscole.
* Come procedura consigliata assicuratevi che gli ID delle risorse non contengano spazi vuoti, ad esempio evitate di usare nomi come giacca nera.tif o giacca blu.jpg. L’ASCII Dynamic Media Classic codifica gli spazi vuoti nei nomi delle risorse quando utilizza i nomi delle risorse per creare le stringhe URL. Poiché questi codici ASCII sono difficili da leggere, la lettura degli URL può risultare più complicata.
* I nomi file possono contenere caratteri specifici per particolari lingue. Tuttavia, non possono contenere i seguenti caratteri:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; { } %

   Se il nome del file contiene uno o più di questi caratteri, questi vengono eliminati dal nome del file al momento del caricamento.

Nella maggior parte dei casi, il nome file di una risorsa può essere uguale al relativo numero di elemento, allo SKU del prodotto o a un altro nome. Ad esempio:

| Elemento | Nome file | ID risorsa |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organizzazione e struttura delle cartelle {#folder-organization-and-structure}

Prima di caricare il contenuto sul sistema, organizzate e strutturate appositamente le cartelle e le sottocartelle di Scene7 Publishing System. La pianificazione preventiva di questa procedura presenta i due grandi vantaggi seguenti:

* Quando caricate il contenuto su SPS mediante FTP, potete specificare di replicare nel sistema la struttura delle cartelle durante il caricamento. In questo modo, il contenuto verrà organizzato nelle stesse cartelle e sottocartelle sia in SPS sia sul computer o sulla rete. Per replicare la struttura delle cartelle in SPS, selezionate l’opzione Includi sottocartelle durante il caricamento delle risorse mediante FTP.
* Riorganizzare le cartelle all’interno del sistema dopo il caricamento dei file è molto più difficile rispetto a iniziare la procedura con una struttura di cartelle pianificata con attenzione.

Il sistema di denominazione delle cartelle e la struttura selezionata per l’archiviazione del relativo contenuto in Scene7 Publishing System dipende dalle esigenze dell’organizzazione. Di seguito sono riportati alcune strutture di cartelle di esempio:

**Le cartelle basate** su SKU vengono denominate in base ai numeri SKU o agli elementi. Vengono ad esempio create cartelle separate per tutte le serie di numeri 0-, 20-, 30.

**Basato** sul marchio Per i produttori con più brand line e rivenditori che commercializzano altri marchi di altre aziende, separare i file in cartelle di prodotti denominate per marchi diversi.

**Le cartelle basate** sul progetto sono organizzate in base alla data di implementazione/rilascio o al nome del progetto. Questa procedura è preferita dai clienti che si occupano principalmente della produzione di eCatalog. 

**Mirror della gerarchia** delle cartelle del sito Web Questa struttura di cartelle riflette la struttura delle cartelle del sito Web, con le cartelle denominate, ad esempio, per le categorie di prodotti.

## Informazioni sul caricamento dei file {#uploading-your-files}

Potete caricare singoli file dal desktop oppure caricare le cartelle mediante FTP. If you want to upload more than 100 MB of files or upload entire folders and subfolders, select the **VIA FTP** tab.

Se avete installato l’applicazione desktop Scene7 Publishing System, potete trascinare i file e le cartelle direttamente dal desktop nella cartella di destinazione.

Da Scene7 Publishing System vengono inviati messaggi e-mail di conferma dell’inizio e della fine del processo di caricamento e che riportano eventuali problemi riscontrati.

Durante, o subito dopo, un grande processo di caricamento, per alcuni elementi nuovi può venire visualizzato il messaggio “Immagine non ancora ottimizzata”. Questo messaggio viene visualizzato perché i file non sono ancora stati elaborati completamente e aggiunti a SPS. Potete ottimizzare questi file successivamente. Consultate [Ottimizzare i file](application-setup.md#optimize_files).

### Caricamento di file tramite la scheda FROM DESKTOP {#upload-files-using-sps-desktop-application}

La versione desktop di Scene7 Publishing System consente di caricare i file e le cartelle semplicemente trascinandoli.

1. In Scene7 Publishing System fate clic sul pulsante **Carica** nella barra di navigazione globale.
1. On the Upload page, click the **FROM DESKTOP** tab.
1. Sul lato sinistro della pagina Carica, nell’area **Seleziona file da caricare** , fate clic su **Sfoglia** per selezionare i file o le cartelle da caricare, quindi fate clic su **Apri**.
1. Sul lato destro della pagina Carica, nell’area **Scegli destinazione** cartella, individuate la cartella di destinazione in cui desiderate aggiungere i file o le cartelle caricati.
1. (Facoltativo) Nella parte inferiore della pagina Carica, nel campo Nome **** processo, specificate il nuovo nome del processo di caricamento. Oppure potete semplicemente utilizzare il nome predefinito generato dal sistema fornito da SPS. Il processo in corso e gli altri processi di caricamento e pubblicazione vengono registrati nella pagina Processi dove è possibile controllarne lo stato.
Consultate [Verifica dei file di processo](checking-job-files.md#checking_job_files).
1. (Facoltativo) Nella parte inferiore della pagina Carica, selezionate **Pubblica dopo il caricamento** se desiderate pubblicare automaticamente le risorse caricate.
Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. (Facoltativo) Nella parte inferiore della pagina Carica, selezionate **Sovrascrivi in qualsiasi cartella, nome della stessa risorsa di base, indipendentemente dall’estensione** , se desiderate che i file caricati sostituiscano quelli esistenti con gli stessi nomi. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

1. Nella finestra di dialogo Opzioni processo di caricamento, fate clic su **Salva**.
1. Nell’angolo inferiore destro della pagina Carica, fate clic su **Invia caricamento**.
Per visualizzare l’avanzamento del caricamento, fate clic su **Processi** nella barra di navigazione globale. Potete continuare a usare Scene7 Publishing System e tornare alla pagina Processi in qualsiasi momento per controllare un processo in corso di elaborazione. Per annullare un processo di caricamento in corso, fate clic sul pulsante **Annulla** accanto alla durata.

### Caricamento di file tramite la scheda VIA FTP {#upload-files-using-via-ftp}

1. Accedete al sito FTP Dynamic Media Classic specifico per la vostra area geografica. Utilizzate il nome utente e la password per FTP ricevuti dall’amministratore.
1. In Dynamic Media Classic, nella barra di navigazione globale, fate clic su **Carica**.
1. On the Upload page, click the **VIA FTP** tab.
1. Sul lato sinistro della pagina Carica, nell’area **Scegli cartella FTP da caricare** , scegliete una cartella FTP da cui caricare i file.
1. Sul lato destro della pagina Carica, nell’area **Scegliete la destinazione** della cartella SPS, scegliete una cartella di destinazione in Scene7 Publishing System.
1. (Facoltativo) Nella parte inferiore della pagina Carica, nel campo Nome **** processo, specificate il nuovo nome del processo di caricamento. Oppure potete semplicemente utilizzare il nome predefinito generato dal sistema fornito da SPS. Il processo in corso e gli altri processi di caricamento e pubblicazione vengono registrati nella pagina Processi dove è possibile controllarne lo stato.
Consultate [Verifica dei file di processo](checking-job-files.md#checking_job_files).
1. (Facoltativo) Nella parte inferiore della pagina Carica, selezionate **Pubblica dopo il caricamento** se desiderate pubblicare automaticamente le risorse caricate.
Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. (Facoltativo) Nella parte inferiore della pagina Carica, selezionate **Sovrascrivi in qualsiasi cartella, nome della stessa risorsa di base, indipendentemente dall’estensione** , se desiderate che i file caricati sostituiscano quelli esistenti con gli stessi nomi. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.
1. (Facoltativo; disponibile solo se avete fatto clic sulla scheda **VIA FTP** ) Nella parte inferiore della pagina di caricamento, selezionate **Rimuovi compressione file ZIP o Tar al caricamento** se desiderate estrarre automaticamente tutti i file dal file ZIP o TAR caricato. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

1. Nella finestra di dialogo Opzioni processo di caricamento, fate clic su **Salva**.
1. Nell’angolo inferiore destro della pagina Carica, fate clic su **Invia caricamento**.

   Per visualizzare l’avanzamento del caricamento, nella barra di navigazione globale fate clic su **Processi**. Viene visualizzata la pagina Processi che mostra l’avanzamento del caricamento. Potete continuare a usare Scene7 Publishing System e tornare alla pagina Processi in qualsiasi momento per controllare un processo in corso di elaborazione. 

Per annullare un processo di caricamento in corso, fate clic sul pulsante **Annulla** accanto alla durata.

## Opzioni processo di caricamento, finestra di dialogo {#upload-options}

Quando caricate dei file, potete scegliere tra le seguenti opzioni nella finestra di dialogo Opzioni processo di caricamento:

* **LAVORO** — Fate clic su **PROCESSO** per scegliere le opzioni che interessano l’intero processo di caricamento.

   Potete anche scegliere le opzioni *predefinite* per il caricamento dei processi mediante la finestra di dialogo Opzioni **di caricamento** predefinite in Impostazioni generali. Fate clic su **Configurazione > Impostazione applicazione > Impostazioni generali > Opzioni** di caricamento predefinite, quindi impostate le opzioni predefinite desiderate.

   * **Quando** — L&#39;opzione **Quando** è disponibile solo se è stata selezionata la scheda **VIA FTP** .
      * **Una tantum** — Specificate un processo di caricamento da eseguire una volta. Le opzioni disponibili sono:
         * **Ora** — Esegue il processo di caricamento immediatamente dopo aver fatto clic su **Salva** nella finestra di dialogo Opzioni processo di caricamento, quindi fate clic su **Invia caricamento** nella pagina Carica.
         * **Pianificazione per un periodo successivo** — Selezionate l’anno, il mese, il giorno e l’ora (in incrementi di 15 minuti) in cui desiderate eseguire il processo di caricamento.
      * **Periodico** — Specificate un processo di caricamento che venga eseguito giornalmente, settimanalmente o mensilmente. In alternativa, potete personalizzare il processo di caricamento in base alle vostre specifiche.
         * **Giornaliero** — Impostate l’ora in cui desiderate che il processo venga eseguito ogni giorno. Se desiderate che il processo venga eseguito solo dal lunedì al venerdì, selezionate Solo **giorni** feriali.
         * **Settimanale** — Scegliete un giorno specifico della settimana e dell’ora in cui eseguire il processo.
         * **Mensile** — Scegliete un giorno specifico del mese o del giorno della settimana, incluso l’ora di inizio, in cui eseguire il processo.
         * **Personalizzato** — Potete personalizzare un intervallo di tempo per il processo di caricamento o pubblicazione in base alle vostre specifiche. Consultate [Creazione di un intervallo personalizzato per un processo di caricamento o pubblicazione](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **Pubblica dopo il caricamento** — Disponibile se avete selezionato la scheda **FROM DESKTOP** o **VIA FTP** . Selezionate questa opzione per pubblicare automaticamente le risorse caricate. Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa opzione è disponibile anche nella pagina di caricamento.

   * **Sovrascrivi in qualsiasi cartella, nome della stessa risorsa base, indipendentemente dall’estensione** — Disponibile se avete selezionato la scheda **FROM DESKTOP** o **VIA FTP** . Selezionate questa opzione per sostituire i file esistenti con quelli caricati mantenendo gli stessi nomi. Questa opzione è disponibile anche nella pagina di caricamento. The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.

   * **Decomprimete i file Zip o Tar durante il caricamento** — Disponibile se avete selezionato la scheda **FROM DESKTOP** o **VIA FTP** .
Selezionate questa opzione se desiderate estrarre automaticamente tutti i file dal file ZIP o TAR caricato. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.

   * **Includi sottocartelle** — Disponibile solo se è stata selezionata la scheda **VIA FTP** .
Selezionate questa opzione per caricare le sottocartelle della cartella che intendete caricare. I nomi della cartella e delle relative sottocartelle caricate vengono inseriti automaticamente in SPS. 

   * **Elabora file** di metadati — Disponibile solo se è stata selezionata una delle schede **VIA FTP** . Selezionate questa opzione se desiderate caricare un file delimitato da tabulazioni o XML per aggiungere metadati a più risorse. Consultate [Importare metadati (tramite FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **OPZIONI** DI RITAGLIO — Per ritagliare automaticamente i pixel dello spazio bianco da un’immagine, aprite il menu Ritaglio, scegliete Manuale e immettete i valori in pixel nei campi In alto, A destra, In basso e A sinistra per ritagliare dai lati. Potete inoltre scegliere Rifila dal menu Ritaglia e selezionare le seguenti opzioni:

   * **Rifila in base** a: Scegliete se ritagliare in base al colore o alla trasparenza:

      * **Colore** — Scegliete l’opzione Colore. Dal menu Angolo scegliete quindi l’angolo dell’immagine con il colore che rappresenta meglio quello dello spazio bianco da ritagliare.

         Ritaglio in base al colore: L’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo dell’immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

      * **Trasparenza** —  Scegliete l’opzione Trasparenza.

         Per rifilare in base alla trasparenza, l’impostazione 0 ritaglia i pixel solo se sono completamente trasparenti. Con valori più vicini a 1 viene invece tollerata una minore trasparenza. 

      * **Tolleranza** — Trascinate il cursore per specificare una tolleranza da 0 a 1.

* **OPZIONI** PROFILO COLORE — Quando create file ottimizzati per la distribuzione dinamica di Dynamic Media Classic, scegliete una conversione del colore:

   * **Mantenimento** colore predefinito — mantiene i colori dell’immagine sorgente ogni volta che le immagini contengono informazioni sullo spazio colore; non esiste alcuna conversione del colore. In quasi tutte le immagini è incorporato il relativo profilo colore. Tuttavia, se un’immagine sorgente CMYK non contiene un profilo colore incorporato, i colori vengono convertiti nello spazio colore sRGB. sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

   * **Mantieni spazio** colore originale Mantiene i colori originali senza alcuna conversione colore al momento dell’assimilazione in Scene7 Publishing System. Per le immagini senza un profilo colore incorporato, l’eventuale conversione colore per le richieste di elaborazione viene effettuata utilizzando i profili colore predefiniti in base alla configurazione delle impostazioni di pubblicazione. Tali profili colore potrebbero non essere allineati al colore nei file creati con questa opzione. Si consiglia quindi di utilizzare l’opzione Mantenimento colore predefinito.

   * **Personalizzato Da > A** — Consente di aprire i menu per scegliere uno spazio colore Converti da e Converti in. Questa opzione avanzata ha priorità rispetto a eventuali informazioni di colore incorporate nel file sorgente. Selezionate questa opzione solo quando tutte le immagini che state inviando contengono dati di profilo colore errati o mancanti.

* **OPZIONI** DI MODIFICA DELLE IMMAGINI — Potete mantenere le &lt;> maschere di ritaglio nelle immagini e scegliere un profilo colore.
Consultate [Opzioni di modifica delle immagini al caricamento](image-editing-options-upload.md#image-editing-options-at-upload).

* **OPZIONI** POSTSCRIPT — Potete rasterizzare i file PostScript®, ritagliare i file, mantenere lo sfondo trasparente, scegliere una risoluzione e uno spazio colore.
Consultate [Utilizzo dei file PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **OPZIONI** PHOTOSHOP — Potete creare modelli da file di Adobe® Photoshop®, mantenere i livelli, specificare i nomi dei livelli, estrarre del testo e specificare il modo in cui le immagini vengono ancorate ai modelli.
Consultate [Opzioni di caricamento PSD](psd-files.md#psd_upload_options).

* **OPZIONI** PDF — Potete rasterizzare i file, estrarre parole di ricerca e collegamenti, generare automaticamente un eCatalog, impostare la risoluzione e scegliere uno spazio colore.
Consultate [Opzioni di caricamento PDF](pdfs.md#pdf_upload_options).

* **OPZIONI** ILLUSTRATOR — Potete rasterizzare i file Adobe Illustrator®, conservare gli sfondi trasparenti, scegliere una risoluzione e uno spazio colore.
Consultate [Utilizzo dei file PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **OPZIONI** EVIDEO — Potete transcodificare un file video scegliendo un predefinito per video.
Consultate [Utilizzo dei predefiniti di codifica video](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **METADATI** AGGIUNTIVI — Inserite le parole chiave che descrivono i file da caricare. Separate le parole chiave con una virgola. Le parole chiave consentono di effettuare ricerche di risorse in modo semplificato. Consultate [Eseguire una ricerca avanzata](searching-assets.md#conducting_an_advanced_search).

* **PREDEFINITI** PER SET DI BATCH — Per creare un set di immagini, un set 360 gradi con più assi o un set di campioni dai file caricati, fate clic sulla colonna Attivo per il predefinito che desiderate usare. Potete selezionare più di un predefinito. Potete creare i predefiniti nella pagina Impostazione applicazione/Predefiniti set di batch. Consultate [Predefiniti per set di batch](application-setup.md#batch_set_presets).

* **AVANZATE** — Consultate [Seguire un caricamento con un altro processo](uploading-files.md#follow-an-upload-with-another-job).

## Avviare un altro processo al termine di un caricamento {#follow-an-upload-with-another-job}

Quando caricate elementi mediante FTP, potete pianificare l’inizio di un altro processo subito dopo il completamento del caricamento. Se all’ora specificata è pianificato l’inizio di altri processi, il processo impostato in questo campo verrà messo in coda.

Il nuovo processo invia una notifica all’indirizzo specificato per poter attivare il codice nella posizione esatta. Questo processo di pubblicazione sequenziale usa lo stesso nome del processo di caricamento, con l’aggiunta del testo *Pub_* all’inizio.

**Per avviare un altro processo al termine di un caricamento**

1. Click **Upload**, then click the **VIA FTP** tab.
1. In the lower-right corner of the Upload page, click **Job Options**.
1. Nella finestra di dialogo Opzioni processo di caricamento, espandete la sezione **AVANZATE** .
1. Scegliete una delle seguenti opzioni dall’elenco a discesa **Dopo il caricamento, con un altro processo** :

   * Nessuno
   * Richiesta HTTP
   * Pubblicazione da Image Server
   * Pubblicazione da Image Rendering
   * Pubblicazione video

1. Specificate l’indirizzo HTTP.
1. Specificate se eseguire solo se i file sono stati caricati.
1. Specificate se la richiesta deve essere eseguita ogni volta che termina il processo oppure solo quando i file sono stati pubblicati. 

   >[!NOTE]
   >
   >è possibile che i processi pianificati regolarmente non comportino la pubblicazione di alcun file.

>[!MORELIKETHIS]
>
>* [Utilizzo delle cartelle di risorse](asset-folders.md#working_with_asset_folders)
>* [Gestione di processi di caricamento e pubblicazione periodici](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Utilizzo di un processo di caricamento o pubblicazione come trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

