---
title: Caricamento dei file
seo-title: Caricamento dei file
description: 'null'
seo-description: Scoprite come caricare i file.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '3855'
ht-degree: 44%

---


# Caricamento dei file{#uploading-files}

Prima di caricare i file di risorse in Dynamic Media Classic, accertatevi che i nomi dei file di risorse siano corretti e che la struttura delle cartelle sia impostata e organizzata nel modo desiderato. Potete caricare i file da un sito FTP fornito da Dynamic Media Classic o direttamente dal computer o dalla rete. Dynamic Media Classic offre opzioni per ottimizzare i file mentre li caricate. Se avete installato ’applicazione desktop Dynamic Media Classic Adobe, potete caricare file e cartelle trascinandoli direttamente dal desktop. Consultate [Impostazioni generali dell’applicazione](application-setup.md#general_settings).

## Preparazione delle risorse e delle cartelle per il caricamento  {#preparing-your-assets-and-folders-for-uploading}

Prima di caricare le risorse in Dynamic Media Classic, assicuratevi che siano nel formato e nelle dimensioni appropriati. Dovete inoltre rispettare le regole di Dynamic Media Classic per la denominazione delle risorse. È anche utile organizzare e disporre i file in una cartella per semplificarne l’individuazione e l’utilizzo. 

### Formati di file di risorse supportati  {#supported-asset-file-formats}

In questa tabella sono elencati i formati di file di risorse supportati da Dynamic Media Classic. Per informazioni sui file Camera Raw supportati, vedere [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

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

L&#39;elenco seguente descrive i sottotipi di formati di file immagine raster *non* supportati in Dynamic Media.

Vedere anche [Rilevamento di formati di file non supportati per Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

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
| Video | Dynamic Media Classic supporta i file video salvati in formato OGV e MP4. Potete transcodificare i file in formato MP4 al momento del caricamento.Consultate [Formati di file di risorse supportati](#supported-static-file-formats). |
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
>Quando caricate file immagine e PDF in Dynamic Media Classic, il sistema converte questi file sorgente in file P-TIFF (TIFF piramidale). Questi file P-TIFF sono i file che verranno pubblicati successivamente sui server di immagini Dynamic Media. Dynamic Media Classic utilizza il formato di file Tiff piramidale perché contiene vari rapporti di zoom che consentono di eseguire rapidamente lo zoom quando viene visualizzato con un visualizzatore zoom Dynamic Media Classic.

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

Poiché nelle estensioni viene rimosso il nome del file durante il processo di caricamento, nel sistema non sono consentiti file con lo stesso nome radice. Nel sistema Dynamic Media Classic, il nome del file della risorsa meno l’estensione del nome del file diventa l’ID della risorsa. Per questo motivo non sono consentite due risorse con lo stesso nome.

Assicuratevi che le seguenti regole di denominazione dei file vengano comprese da tutti gli utenti della società:

* Non sono consentiti nel sistema ID di risorse con lo stesso identico nome.
* I nomi ID delle risorse seguono la distinzione tra maiuscole e minuscole.
* Come procedura consigliata assicuratevi che gli ID delle risorse non contengano spazi vuoti, ad esempio evitate di usare nomi come giacca nera.tif o giacca blu.jpg. In Dynamic Media Classic ASCII gli spazi vuoti nei nomi delle risorse vengono codificati quando vengono usati i nomi delle risorse per creare stringhe URL. Poiché questi codici ASCII sono difficili da leggere, la lettura degli URL può risultare più complicata.
* I nomi file possono contenere caratteri specifici per particolari lingue. Tuttavia, non possono contenere i seguenti caratteri:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; { } %

   Se il nome del file contiene uno o più di questi caratteri, questi vengono eliminati dal nome del file al momento del caricamento.

Nella maggior parte dei casi, il nome file di una risorsa può essere uguale al relativo numero di elemento, allo SKU del prodotto o a un altro nome. Ad esempio:

| Elemento | Nome file | ID risorsa |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organizzazione e struttura delle cartelle  {#folder-organization-and-structure}

Organizzate e strutturate le cartelle e sottocartelle per il contenuto in Dynamic Media Classic prima di caricare il contenuto nel sistema. La pianificazione preventiva di questa procedura presenta i due grandi vantaggi seguenti:

* Quando caricate il contenuto in Dynamic Media Classic tramite FTP, potete indicare al sistema di replicare la struttura delle cartelle durante il caricamento. In questo modo, il contenuto viene organizzato nelle stesse cartelle e sottocartelle di Dynamic Media Classic che si trova sul computer o sulla rete. Per replicare la struttura delle cartelle in Dynamic Media Classic, selezionate l’opzione Includi sottocartelle quando caricate le risorse tramite FTP.
* Riorganizzare le cartelle all’interno del sistema dopo il caricamento dei file è molto più difficile rispetto a iniziare la procedura con una struttura di cartelle pianificata con attenzione.

L’approccio e la struttura di denominazione delle cartelle scelti per memorizzare il contenuto in Dynamic Media Classic dipende dalle esigenze dell’organizzazione. Di seguito sono riportati alcune strutture di cartelle di esempio:

**Le cartelle** basate su SKU vengono denominate in base agli SKU o ai numeri di elemento. Vengono ad esempio create cartelle separate per tutte le serie di numeri 0-, 20-, 30.

**Marca:** per i produttori con più brand line e rivenditori che commercializzano altri marchi di altre aziende, separa i file in cartelle di prodotti denominate per marchi diversi.

**Le cartelle** basate sul progetto sono organizzate in base alla data di implementazione/rilascio o al nome del progetto. Questa procedura è preferita dai clienti che si occupano principalmente della produzione di eCatalog. 

**Mirror della** gerarchia di cartelle del sito WebQuesta struttura di cartelle riflette la struttura di cartelle del sito Web, con le cartelle denominate, ad esempio, per le categorie di prodotti.

## Informazioni sul caricamento di file {#uploading-your-files}

Potete caricare singoli file dal desktop oppure caricare le cartelle mediante FTP. Se desiderate caricare più di 100 MB di file o caricare intere cartelle e sottocartelle, selezionate la scheda **VIA FTP**.

Dynamic Media Classic invia un messaggio e-mail di conferma dell’inizio e della fine del processo di caricamento e di notifica di eventuali problemi.

Durante, o subito dopo, un grande processo di caricamento, per alcuni elementi nuovi può venire visualizzato il messaggio “Immagine non ancora ottimizzata”. Questo messaggio viene visualizzato perché i file non sono ancora stati elaborati completamente e aggiunti ad Dynamic Media Classic. Potete ottimizzare questi file successivamente. Consultate [Ottimizzare i file](application-setup.md#optimize_files).

### Caricamento di file tramite la scheda DESKTOP FROM {#upload-files-using-sps-desktop-application}

L’applicazione Dynamic Media Classic Desktop consente di caricare file e cartelle mediante trascinamento.

1. Nell’applicazione Dynamic Media Classic Desktop, nella barra di navigazione globale, fate clic su **Carica**.
1. Nella pagina Carica, fate clic sulla scheda **FROM DESKTOP**.
1. Sul lato sinistro della pagina Carica, nell&#39;area **Seleziona file da caricare**, fate clic su **Sfoglia** per selezionare i file o le cartelle da caricare, quindi fate clic su **Apri**.
1. Sul lato destro della pagina Carica, nell&#39;area **Scegli destinazione cartella**, individuate la cartella di destinazione in cui desiderate aggiungere i file o le cartelle caricati.
1. (Facoltativo) Nella parte inferiore della pagina Carica, specificate il nuovo nome del processo di caricamento nel campo **Nome processo**. Oppure, potete semplicemente utilizzare il nome predefinito generato dal sistema fornito da Dynamic Media Classic. Il processo in corso e gli altri processi di caricamento e pubblicazione vengono registrati nella pagina Processi dove è possibile controllarne lo stato.
Consultate [Verifica dei file di processo](checking-job-files.md#checking_job_files).
1. (Facoltativo) Nella parte inferiore della pagina Carica, selezionate **Pubblica dopo il caricamento** per pubblicare automaticamente le risorse caricate.
Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. (Facoltativo) Nella parte inferiore della pagina di caricamento, selezionate **Sovrascrivi in qualsiasi cartella, stesso nome risorsa di base indipendentemente dall’estensione** se desiderate che i file caricati sostituiscano quelli esistenti con gli stessi nomi. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni in **Impostazione applicazione > Impostazioni generali > Carica nell&#39;applicazione > Sovrascrivi immagini**.
1. Nell’angolo inferiore destro della pagina Carica, fate clic su **Opzioni processo**, quindi specificate le opzioni desiderate.

   Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

1. Nella finestra di dialogo Opzioni processo di caricamento, fate clic su **Salva**.
1. Nell’angolo inferiore destro della pagina Carica, fate clic su **Invia caricamento**.
Per visualizzare l’avanzamento del caricamento, fate clic su **Processi** nella barra di navigazione globale. Potete continuare a utilizzare Dynamic Media Classic e tornare alla pagina Processi in qualsiasi momento per controllare un processo in corso di elaborazione. Per annullare un processo di caricamento in corso, fate clic sul pulsante **Annulla** accanto alla durata.

### Caricamento di file tramite la scheda VIA FTP {#upload-files-using-via-ftp}

1. Accedete al sito Dynamic Media Classic FTP specifico per la vostra area geografica. Utilizzate il nome utente e la password per FTP ricevuti dall’amministratore.
1. In Dynamic Media Classic, nella barra di navigazione globale, fate clic su **Carica**.
1. Nella pagina Carica, fai clic sulla scheda **VIA FTP**.
1. Sul lato sinistro della pagina di caricamento, nell&#39;area **Scegli cartella FTP da caricare**, scegliete una cartella FTP da cui caricare i file.
1. Sul lato destro della pagina Carica, nell&#39;area **Scegli  Adobe destinazione cartella Dynamic Media**, scegliete una cartella di destinazione in Dynamic Media Classic.
1. (Facoltativo) Nella parte inferiore della pagina Carica, specificate il nuovo nome del processo di caricamento nel campo **Nome processo**. Oppure, potete semplicemente utilizzare il nome predefinito generato dal sistema fornito da Dynamic Media Classic. Il processo in corso e gli altri processi di caricamento e pubblicazione vengono registrati nella pagina Processi dove è possibile controllarne lo stato.
Consultate [Verifica dei file di processo](checking-job-files.md#checking_job_files).
1. (Facoltativo) Nella parte inferiore della pagina Carica, selezionate **Pubblica dopo il caricamento** per pubblicare automaticamente le risorse caricate.
Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. (Facoltativo) Nella parte inferiore della pagina di caricamento, selezionate **Sovrascrivi in qualsiasi cartella, stesso nome risorsa di base indipendentemente dall’estensione** se desiderate che i file caricati sostituiscano quelli esistenti con gli stessi nomi. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni in **Impostazione applicazione > Impostazioni generali > Carica nell&#39;applicazione > Sovrascrivi immagini**.
1. (Facoltativo; disponibile solo se avete fatto clic sulla scheda **VIA FTP**) Nella parte inferiore della pagina di caricamento, selezionate **Rimuovi compressione file ZIP o Tar al caricamento** se desiderate estrarre automaticamente tutti i file dal file ZIP o TAR caricato. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.
1. Nell’angolo inferiore destro della pagina Carica, fate clic su **Opzioni processo**, quindi specificate le opzioni desiderate.

   Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

1. Nella finestra di dialogo Opzioni processo di caricamento, fate clic su **Salva**.
1. Nell’angolo inferiore destro della pagina Carica, fate clic su **Invia caricamento**.

   Per visualizzare l’avanzamento del caricamento, nella barra di navigazione globale fate clic su **Processi**. Viene visualizzata la pagina Processi che mostra l’avanzamento del caricamento. Potete continuare a utilizzare Dynamic Media Classic e tornare alla pagina Processi in qualsiasi momento per controllare un processo in corso di elaborazione.

Per annullare un processo di caricamento in corso, fate clic sul pulsante **Annulla** accanto alla durata.

## Opzioni processo di caricamento, finestra di dialogo {#upload-options}

Quando caricate dei file, potete scegliere tra le seguenti opzioni nella finestra di dialogo Opzioni processo di caricamento:

* **PROCESSO** — Fate clic su  **** PROCESSO per scegliere le opzioni che interessano l’intero processo di caricamento.

   È inoltre possibile scegliere le opzioni *default* per il caricamento dei processi mediante la finestra di dialogo **Opzioni di caricamento predefinite** in Impostazioni generali. Fate clic su **Configurazione > Impostazione applicazione > Impostazioni generali > Opzioni di caricamento predefinite**, quindi impostate le opzioni predefinite desiderate.

   * **Quando** — L&#39;opzione  **** Quando è disponibile solo se è stata selezionata la scheda  **VIA** FTP.
      * **Una tantum** — Specificate un processo di caricamento da eseguire una volta. Le opzioni disponibili sono:
         * **Ora** — Esegue il processo di caricamento immediatamente dopo aver fatto clic su  **** Salva nella finestra di dialogo Opzioni processo di caricamento, quindi fare clic su  **Invia** caricamento nella pagina Carica.
         * **Pianificazione per un successivo** — Selezionate l’anno, il mese, il giorno e l’ora (in incrementi di 15 minuti) in cui desiderate eseguire il processo di caricamento.
      * **Periodico** — Specificate un processo di caricamento che venga eseguito giornalmente, settimanalmente o mensilmente. In alternativa, potete personalizzare il processo di caricamento in base alle vostre specifiche.
         * **Giornaliero** — Impostate l’ora in cui desiderate che il processo venga eseguito ogni giorno. Se desiderate che il processo venga eseguito solo dal lunedì al venerdì, selezionate **Solo giorni feriali**.
         * **Settimanale** — Scegliete un giorno specifico della settimana e dell’ora in cui eseguire il processo.
         * **Mensile** — Scegliete un giorno specifico del mese o del giorno della settimana, incluso l’ora di inizio, in cui eseguire il processo.
         * **Personalizzato** — Potete personalizzare un intervallo di tempo per il processo di caricamento o pubblicazione in base alle vostre specifiche. Consultate [Creazione di un intervallo personalizzato per un processo di caricamento o pubblicazione](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **Pubblica Dopo Il Caricamento** — Disponibile se avete selezionato la scheda  **FROM** DESKTOP o  **VIA** FTP. Selezionate questa opzione per pubblicare automaticamente le risorse caricate. Quando pubblicate dei file, questi vengono inviati ai server dinamici. Gli URL di questi file possono essere utilizzati nei siti Web e nelle applicazioni esterni. Questa opzione è disponibile anche nella pagina di caricamento.

   * **Sovrascrivi in qualsiasi cartella, nome della stessa risorsa base, indipendentemente dall’estensione** : Disponibile se avete selezionato la scheda  **FROM** DESKTOP o  **VIA** FTP. Selezionate questa opzione per sostituire i file esistenti con quelli caricati mantenendo gli stessi nomi. Questa opzione è disponibile anche nella pagina di caricamento. Il nome di questa opzione potrebbe essere diverso, a seconda delle impostazioni in **Impostazione applicazione > Impostazioni generali > Carica nell&#39;applicazione > Sovrascrivi immagini**.

   * **Rimuovi compressione di file ZIP o Tar durante il caricamento** — Disponibile se avete selezionato la scheda  **FROM** DESKTOP o  **VIA** FTP.
Selezionate questa opzione se desiderate estrarre automaticamente tutti i file dal file ZIP o TAR caricato. Questa stessa opzione è disponibile anche nella finestra di dialogo Opzioni processo.

   * **Includi sottocartelle** — Disponibile solo se è stata selezionata la scheda  **VIA** FTP.
Selezionate questa opzione per caricare le sottocartelle della cartella che intendete caricare. I nomi della cartella e delle relative sottocartelle caricate vengono inseriti automaticamente in Dynamic Media Classic.

   * **Elabora file**  di metadati Disponibile solo se è stata selezionata una  **scheda** FTP VIA. Selezionate questa opzione se desiderate caricare un file delimitato da tabulazioni o XML per aggiungere metadati a più risorse. Consultate [Importare metadati (tramite FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **CROP  OPTIONS** — Per ritagliare automaticamente i pixel dello spazio bianco da un’immagine, aprite il menu Ritaglio, scegliete Manuale e immettete i valori in pixel nei campi In alto, A destra, In basso e A sinistra per ritagliare dai lati. Potete inoltre scegliere Rifila dal menu Ritaglia e selezionare le seguenti opzioni:

   * **Rifila in base**  a: Scegliete se ritagliare in base al colore o alla trasparenza:

      * **Colore** — Scegliete l’opzione Colore. Dal menu Angolo scegliete quindi l’angolo dell’immagine con il colore che rappresenta meglio quello dello spazio bianco da ritagliare.

         Ritaglio in base al colore: L’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo dell’immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

      * **Trasparenza** — Scegliete l’opzione Trasparenza.

         Per rifilare in base alla trasparenza, l’impostazione 0 ritaglia i pixel solo se sono completamente trasparenti. Con valori più vicini a 1 viene invece tollerata una minore trasparenza. 

      * **Tolleranza** — Trascinate il cursore per specificare una tolleranza da 0 a 1.

* **PROFILO COLORE  OPTIONS** — Scegliete una conversione del colore quando create file ottimizzati per la distribuzione dinamica di Dynamic Media Classic:

   * **Mantenimento colore predefinito** — mantiene i colori dell’immagine sorgente ogni volta che le immagini contengono informazioni sullo spazio colore; non esiste alcuna conversione del colore. In quasi tutte le immagini è incorporato il relativo profilo colore. Tuttavia, se un’immagine sorgente CMYK non contiene un profilo colore incorporato, i colori vengono convertiti nello spazio colore sRGB. sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

   * **Mantieni spazio**  colore originale Mantiene i colori originali senza alcuna conversione colore al momento dell’assimilazione in Dynamic Media Classic. Per le immagini senza un profilo colore incorporato, l’eventuale conversione colore per le richieste di elaborazione viene effettuata utilizzando i profili colore predefiniti in base alla configurazione delle impostazioni di pubblicazione. Tali profili colore potrebbero non essere allineati al colore nei file creati con questa opzione. Si consiglia quindi di utilizzare l’opzione Mantenimento colore predefinito.

   * **Personalizzato Da > A** — Consente di aprire i menu per scegliere uno spazio colore Converti da e Converti in. Questa opzione avanzata ha priorità rispetto a eventuali informazioni di colore incorporate nel file sorgente. Selezionate questa opzione solo quando tutte le immagini che state inviando contengono dati di profilo colore errati o mancanti.

* **MODIFICA IMMAGINE  OPTIONS** — Potete mantenere le  &lt;> maschere di ritaglio nelle immagini e scegliere un profilo colore.
Consultate [Opzioni di modifica delle immagini al caricamento](image-editing-options-upload.md#image-editing-options-at-upload).

* **OPTIONS**  POSTSCRIPT  Potete rasterizzare i file di PostScript®, ritagliare i file, mantenere lo sfondo trasparente, scegliere una risoluzione e uno spazio colore.
Consultate [Utilizzo dei file PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **OPTIONS**  Photoshop  Potete creare modelli da file  Adobe® Photoshop®, mantenere i livelli, specificare i nomi dei livelli, estrarre del testo e specificare il modo in cui le immagini vengono ancorate ai modelli.
Consultate [Opzioni di caricamento PSD](psd-files.md#psd_upload_options).

* **OPTIONS**   PDF Potete rasterizzare i file, estrarre parole di ricerca e collegamenti, generare automaticamente un eCatalog, impostare la risoluzione e scegliere uno spazio colore.
Consultate [Opzioni di caricamento PDF](pdfs.md#pdf_upload_options).

* **ILLUSTRATOR  OPTIONS** — Potete rasterizzare  file Adobe Illustrator®, mantenere lo sfondo trasparente, scegliere una risoluzione e uno spazio colore.
Consultate [Utilizzo dei file PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **OPTIONS**  EVIDEO  Potete transcodificare un file video scegliendo un predefinito per video.
Consultate [Utilizzo dei predefiniti di codifica video](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **METADATI**  AGGIUNTIVI Inserite le parole chiave che descrivono i file da caricare. Separate le parole chiave con una virgola. Le parole chiave consentono di effettuare ricerche di risorse in modo semplificato. Consultate [Eseguire una ricerca avanzata](searching-assets.md#conducting_an_advanced_search).

* **PREDEFINITI**  PER SET DI BATCH Per creare un set di immagini, un set 360 gradi con più assi o un set di campioni dai file caricati, fate clic sulla colonna Attivo per il predefinito che desiderate usare. Potete selezionare più di un predefinito. Potete creare i predefiniti nella pagina Impostazione applicazione/Predefiniti set di batch. Consultate [Predefiniti per set di batch](application-setup.md#batch_set_presets).

* **AVANZATO** — Consultate  [Seguire un caricamento con un altro processo](uploading-files.md#follow-an-upload-with-another-job).

## Avviare un altro processo al termine di un caricamento {#follow-an-upload-with-another-job}

Quando caricate elementi mediante FTP, potete pianificare l’inizio di un altro processo subito dopo il completamento del caricamento. Se all’ora specificata è pianificato l’inizio di altri processi, il processo impostato in questo campo verrà messo in coda.

Il nuovo processo invia una notifica all’indirizzo specificato per poter attivare il codice nella posizione esatta. Questo processo di pubblicazione sequenziale usa lo stesso nome del processo di caricamento, con l’aggiunta del testo *Pub_* all’inizio.

**Per avviare un altro processo al termine di un caricamento**

1. Fare clic su **Carica**, quindi fare clic sulla scheda **VIA FTP**.
1. Nell’angolo inferiore destro della pagina Carica, fate clic su **Opzioni processo**.
1. Nella finestra di dialogo Opzioni processo di caricamento, espandete la sezione **AVANZATE**.
1. Scegliete una delle seguenti opzioni dall&#39;elenco a discesa **Dopo il caricamento con un altro processo**:

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

