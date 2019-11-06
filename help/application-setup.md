---
title: Impostazione applicazione
seo-title: Impostazione applicazione
description: Scopri come impostare l’area dell’applicazione di Dynamic Media Classic.
seo-description: Scopri come impostare l’area dell’applicazione di Dynamic Media Classic.
uuid: 3e2f1d30-8f33-4a9d-bbe4-e8c3dbc968f8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/Categories/setup
discoiquuid: ae2d1895-a437-4463-bface-3960c8027551
translation-type: tm+mt
source-git-commit: 917ba4469b5ef22e62c572f80008e470dccdebe4

---


# Impostazione applicazione{#application-setup}

Potete usare le pagine Impostazione applicazione per specificare le impostazioni generali, creare predefiniti per immagini, predefiniti di codifica video, predefiniti per visualizzatori o per definire visualizzatori predefiniti e metadati. Potete anche impostare i predefiniti di set di batch per automatizzare la generazione di set 360 gradi 2D, le impostazioni di pubblicazione e le impostazioni video SEO.

>[!NOTE]
>
>Solo gli amministratori di Scene7 Publishing System possono modificare le impostazioni delle pagine di Impostazione applicazione.

## Impostazioni generali {#general-settings}

To open the Application General Settings page, on the Global Navigation bar, click **[!UICONTROL Setup &gt; Application Setup &gt; General Settings]**.

### Server

Al momento della creazione dell’account, Dynamic Media Classic fornisce automaticamente i server assegnati alla società. I server vengono utilizzati per generare stringhe URL per il proprio sito Web e le applicazioni. Tali chiamate URL sono specifiche dell’account utente.

Consultate anche [Verifica del servizio di verifica protetta](testing-assets-making-them-public.md#testing_the_secure_testing_service).

**Nome** server pubblicato Questo server è il server CDN attivo utilizzato in tutte le chiamate URL generate dal sistema specifiche per l’account. Non modificate il nome del server a meno che non venga richiesto espressamente da un tecnico del supporto per Dynamic Media Classic.

**Nome** server origine Questo server viene utilizzato solo per il controllo qualità. Non modificate il nome del server a meno che non venga richiesto da un tecnico del supporto per Dynamic Media Classic.

**Nome** server AGM Questo server viene utilizzato per i modelli Web-stampa. ed è impostato a livello di società. Non modificate il nome del server a meno che non venga richiesto da un tecnico del supporto per Dynamic Media Classic.

**Nome** server Test&amp;Target L’URL Test&amp;Target, fino a .com incluso. Per istruzioni su come ottenere questo URL, consultate Integrazione di Dynamic Media Classic con Target Classic.

**Nome** server di streaming iOS L’URL del server di streaming iOS Dynamic Media Classic. Questo server distribuisce i video in streaming ai dispositivi basati su iOS utilizzando il protocollo HTTP.

**Nome** server video progressivo L’URL del server video progressivo Dynamic Media Classic. Questo server distribuisce i video progressivi mediante il protocollo HTTP.

**Mostra URL per risorse** non pubblicate Selezionate questa opzione se desiderate che Dynamic Media Classic visualizzi un URL per l’anteprima di una risorsa, pubblicata o meno. Se la risorsa non è pubblicata, l’URL non funziona. Tuttavia, potete utilizzare l’URL a scopo di progettazione o organizzazione.

**Consenti installazione** AIR Selezionate questa opzione per consentire agli utenti di scaricare la versione desktop di Scene7 Publishing System nei propri dischi rigidi locali. Gli utenti installano queste applicazioni dall’area Versione Desktop della schermata Configurazione personale.

Gli utenti AIR devono disinstallare manualmente l’app esistente e reinstallarla dalla versione Web di Scene7 Publishing System (in Impostazioni personali). Dopo questa reinstallazione una tantum, viene richiesto di effettuare l’aggiornamento ogni volta che nel server viene rilevata una nuova versione di Scene7 Publishing System AIR. Scene7 Publishing System è integrato con Application Update Framework, che semplifica il processo di aggiornamento.

**Modello** di annullamento validità CDN Specifica il modello utilizzato per annullare la validità della cache CDN (Content Delivery Network).

For example, suppose you enter an image URL (including image presets or modifiers) referencing `<ID>`, instead of a specific image ID as in the following example:

`https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

If the Template just contains `<ID>`, then SPS fills in the `https://<server>/is/image`, where `<server>` is the Publish Server Name that is defined in General Settings.

Se si imposta il modello per Annulla validità CDN, si seleziona un’immagine denominata Backpack_B e si fa clic su **File** &gt; **Annulla validità CDN**, il seguente URL viene generato nell’interfaccia di Annulla validità CDN:

`https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

Nella casella di riepilogo URL, fate clic su **Continua** per cancellare la cache per questa specifica chiamata di URL immagine. Potete anche aggiungere gli URL digitandoli o incollandoli nella casella di riepilogo URL; non è necessario impostare precedentemente il modello.

Dopo aver selezionato il modello di annullamento validità CDN e aver inviato una richiesta per annullare la validità del CDN, nell’interfaccia utente compare un indicatore con una stima del tempo necessario per cancellare la cache.

Analogamente, se sono selezionate più immagini in SPS quando fate clic su **File** &gt; **Annulla validità CDN**, viene inserito un riferimento a ogni immagine nell’URL del modello salvato. Di conseguenza, è possibile definire un modello per Annulla validità CDN con riferimento a ciascun URL al quale viene fatto riferimento nel sito Web (ad esempio dettagli prodotti, risultati della ricerca, e così via). Quindi, quando selezionate una o più immagini di cui annullare la validità della cache, gli URL vengono automaticamente inseriti nell’interfaccia.

Consultate [Memorizzazione dei contenuti nella cache](scene7-platform-overview.md#content_caching).

Consultate [Risorse ripubblicate e ritardi CDN](publishing-files.md#republished_assets_and_cdn_delays).

**Sfoglia**

**Mostra progetti** Consente di determinare se i progetti sono disponibili come mezzo per organizzare le risorse Dynamic Media Classic. Consultate Organizzazione del lavoro mediante i progetti.

**Mostra contenuto** eVideo campione Attivate o disattivate la visualizzazione del contenuto di esempio eVideo.

**Mostra contenuto** generato Nelle cartelle, mostra il contenuto generato da una risorsa. Ad esempio, quando un file PDF viene rasterizzato durante il caricamento, Dynamic Media Classic crea un’immagine per ciascuna pagina del PDF originale. Se l’opzione Mostra contenuto generato è selezionata, ogni immagine generata durante il caricamento del PDF originale viene visualizzata insieme al PDF nella cartella in cui questo è stato caricato.

**Mostra video** codificati deselezionati (disattivati) per impostazione predefinita.

Per cercare e sfogliare rapidamente i video in Scene7 Publishing System senza dover navigare attraverso numerosi derivati codificati dello stesso video, lascia deselezionata questa opzione (impostazione predefinita). Nell’interfaccia utente vengono visualizzate solo l’anteprima Video principale, ossia il video sorgente caricato e utilizzato per creare tutte le versioni derivate, e nell’interfaccia utente viene visualizzata solo l’anteprima del set video adattivo "padre", che contiene tutte le versioni derivate "figlio" del set video codificato.

Tuttavia, potete comunque accedere ai singoli video codificati a partire dal video principale o dal set video adattivo. A questo scopo, fate doppio clic sulla miniatura del video per aprire la visualizzazione Dettagli. Fate clic su **Video codificati** nel pannello a destra per accedere ai video secondari.

Potete inoltre scegliere **File &gt; Rielabora** per creare altri video codificati secondari direttamente da un set di video adattivi. Scene7 Publishing System individua automaticamente il video principale padre del set di video adattivi e lo utilizza come video sorgente per la transcodifica. Quando salvate i nuovi video codificati, tuttavia, questi non vengono visti nelle operazioni di ricerca o navigazione. Sono comunque accessibili dalla scheda Video codificati in visualizzazione Dettagli.

Consultate [Caricamento e transcodifica di video](uploading-encoding-videos.md#uploading_and_encoding_videos).

Per poter accedere a tutte le versioni derivate codificate durante la ricerca e la navigazione, selezionate **Mostra video codificati**.

Alcune azioni nel menu Genera funzionano solo o eventualmente con singoli video. Questa funzionalità rende necessaria la visualizzazione di tutte le versioni derivate di video codificati disponibili per la selezione, a prescindere dall’impostazione di **Mostra video codificati**. The Build actions that over-ride the **Show Encoded Videos** setting include **Adaptive Video Sets**, and **eCatalogs**.

>[Nota]
>
>Se non avete usato Scene7 Publishing System per caricare e codificare le risorse video, Dynamic Media Classic mostra tutti i singoli video codificati, anche se questa opzione è deselezionata.

**Pulsante** Aggiorna sottocartelle Attiva o disattiva la visualizzazione del pulsante Aggiorna delle sottocartelle.

**Account FTP Dynamic Media Classic**

**Server** Elenca il server account FTP.

**Nome** utente Elenca il nome utente dell'account FTP.

**Carica nell’applicazione**

**Sovrascrivi immagini** Dynamic Media Classic non consente a due file di avere lo stesso nome. Ciascun elemento deve avere un ID Scene7 Publishing System (il nome immagine senza l’estensione del nome file) univoco. In virtù di questa regola, nella finestra di dialogo Carica è disponibile l’opzione Sovrascrivi. Il risultato effettivo di questa opzione dipende dal valore impostato per l’opzione Sovrascrivi immagini. È possibile specificare come caricare le immagini sostitutive, ossia se devono sostituire le immagini originali o diventare duplicati di tali immagini. Le immagini duplicate vengono rinominate con il suffisso “-1” (ad esempio, il file sedia.tif viene rinominato sedia-1.tif). Queste opzioni interessano le immagini caricate in una cartella diversa da quella degli originali o le immagini con una diversa estensione file (ad esempio, JPG, TIF o PNG). Consultate Utilizzo dell’opzione Sovrascrivi immagini.

**Sovrascrivi in cartella corrente, nome/estensione come risorsa base**

Questa opzione rappresenta la regola di sostituzione più restrittiva. Richiede che l’immagine sostitutiva sia caricata nella stessa cartella dell’immagine originale e che abbia la stessa estensione del nome file dell’originale. Se entrambi i requisiti non vengono soddisfatti, viene creata una copia dell’immagine.

**Sovrascrivi in cartella corrente, nome come risorsa base, ignora estensione**

Questa opzione richiede che l’immagine sostitutiva sia caricata nella stessa cartella dell’originale, ma l’estensione file può anche essere diversa. Ad esempio, sedia.tif sostituisce sedia.jpg.

**Sovrascrivi in qualsiasi cartella, nome/estensione come risorsa base**

Questa opzione richiede che l’immagine sostitutiva abbia la stessa estensione dell’originale (ad esempio, sedia.jpg sostituisce sedia.jpg ma non sedia.tif). Tuttavia, è possibile caricare l’immagine sostitutiva in una cartella diversa da quella dell’originale. L’immagine aggiornata sarà contenuta nella nuova cartella e il file verrà rimosso dal percorso originale.

**Sovrascrivi in qualsiasi cartella, nome come risorsa base, ignora estensione**

Questa opzione rappresenta la regola di sostituzione meno restrittiva. L’immagine sostitutiva può essere caricata in una cartella diversa da quella dell’originale, con una diversa estensione file, e sostituire il file originale. Se il file originale si trova in un’altra cartella, l’immagine sostitutiva sarà contenuta nella nuova cartella nella quale è stata caricata.

**Mantieni pubblicazione** Consente di specificare se un’immagine sostitutiva caricata in Dynamic Media Classic deve mantenere l’impostazione Pronto per la pubblicazione dell’immagine sostituita oppure se deve essere specificata al momento del caricamento.

**Profili** colore predefiniti Specifica i profili colore applicati come parte delle opzioni di profilo colore predefinito per l’aggiunta di immagini CMYK.

**Opzioni** di caricamento predefinite Apre la finestra di dialogo Opzioni processo di caricamento, in cui potete specificare le opzioni di caricamento predefinite. Per informazioni su queste opzioni, consultate Opzioni di caricamento.

**Editor mappa immagine, su applicazione**

**HREF** mappatura immagine predefinita Definisce l’URL predefinito utilizzato per la colonna HREF della mappatura immagine. Si tratta dell’URL predefinito visibile quando vengono create nuove mappe immagine.

**Modello** di mappatura immagine predefinito Definisce il codice JavaScript predefinito per il modello HREF di mappatura immagine. Potete impostare un codice personalizzato da eseguire quando si fa clic su una mappa immagine.

**Altre impostazioni, su applicazione**

**Il cestino può ripulire le risorse degli avvisi** nel cestino vengono automaticamente rimosse entro sette giorni. Selezionate “Invia e-mail prima che gli elementi nel cestino siano eliminati automaticamente” se desiderate che vengano inviate notifiche agli amministratori dell’azienda quattro giorni prima che le risorse nel cestino vengano definitivamente eliminate. Consultate Gestione della cartella Cestino.

## Utilizzo dell’opzione Sovrascrivi immagini {#using-the-overwrite-images-option}

Dynamic Media Classic non consente a due file di avere lo stesso nome. Ciascun elemento deve avere un ID Scene7 Publishing System (il nome immagine senza l’estensione del nome file) univoco. In virtù di questa regola, nella finestra di dialogo Carica è disponibile l’opzione Sovrascrivi immagini. Il risultato effettivo di questa opzione dipende dalla configurazione delle impostazioni interne di Scene7 Publishing System definita per ciascuna società.

Se avete precedentemente caricato delle immagini e quindi modificato i file originali (o li avete sostituiti), l’opzione Sovrascrivi selezionata specifica in che modo Dynamic Media Classic sostituisce le immagini. I dati relativi all’immagine non vengono modificati, ma la nuova immagine sostituisce la precedente. Se la cartella contiene anche immagini che non sono già presenti in Dynamic Media Classic, queste vengono aggiunte.

Usate questa opzione se le immagini caricate sono state modificate (l’immagine è stata manipolata) ma il riferimento all’immagine è rimasto inalterato. L’opzione Sovrascrivi è utile anche quando si caricano e si estraggono dati da file Adobe® PDF. To fine-tune how Dynamic Media Classic *rips* the image, adjust the ICC color profile options in the Upload dialog box and re-upload using the Overwrite feature.

Gli ID Dynamic Media Classic utilizzati per accedere alle immagini dai server di produzione sono derivati dai nomi dei file immagine. L’uso di caratteri maiuscoli e minuscoli nel nome del file è importante, sia per la sostituzione dei file esistenti che per gli ID Dynamic Media Classic utilizzati per accedere all’immagine. Accertatevi che i caratteri maiuscoli e minuscoli nei nomi dei file siano corretti prima di caricarli in Dynamic Media Classic, per evitare che gli ID di Dynamic Media Classic siano diversi solo per la stessa immagine.

Se deselezionate questa opzione, tutte le immagini con lo stesso nome file delle immagini esistenti vengono considerate copie e non vengono aggiunte.

## Predefiniti immagine {#image-presets}

Nella schermata Predefiniti immagine è possibile creare e modificare i predefiniti per le immagini. I predefiniti per immagini consentono a Dynamic Media Classic di distribuire dinamicamente immagini di diverse dimensioni dalla stessa immagine principale. Ogni predefinito immagine rappresenta una raccolta predefinita di comandi di ridimensionamento e formattazione per la visualizzazione delle immagini. Quando create un predefinito per immagini, dovete scegliere una dimensione da usare per la distribuzione delle immagini. È inoltre necessario scegliere dei comandi di formattazione con cui ottimizzare l’aspetto delle immagini per la distribuzione.

Gli amministratori possono creare predefiniti per l’esportazione delle risorse. Gli utenti possono scegliere un predefinito durante l’esportazione di immagini, per riformattarle in base alle specifiche definite dall’amministratore.

To open the Image Preset screen, on the Global Navigation bar, click **Setup** &gt; **Image Presets**.

Consultate [Smart imaging](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html).

### Creazione e modifica dei predefiniti per visualizzatori {#creating-and-editing-image-presets}

1. Fate clic su **Configurazione** &gt; **Predefiniti immagini**.
1. Create un nuovo predefinito o iniziate da uno esistente: 
   * **Creazione di un predefinito** per immagini - Fate clic su **Aggiungi**.
   * **Creazione di un predefinito per immagini da un predefinito** esistente - Selezionate il predefinito per immagini più simile a quello che desiderate creare, quindi fate clic su Modifica.

1. Nella schermata Aggiungi predefinito o Modifica predefinito, specificate il nome del predefinito.
1. Impostate le opzioni desiderate. 

   Consultate [Opzioni dei predefiniti immagine](application-setup.md#image_preset_options).

1. Click **Save**, or if you started from an existing preset, click **Save As**.
1. To preview the preset with your own image, click **Browse** and then select an image. To preview with the default image, click **Reset**.

Per modificare un predefinito immagine, selezionatene il nome nella schermata Predefiniti immagine e fate clic su Modifica. Per eliminare un predefinito immagine, selezionatelo e fate clic su Elimina.

### Opzioni dei predefiniti immagine {#image-preset-options}

Nelle schermate Aggiungi predefinito e Modifica predefinito sono disponibili le seguenti opzioni per creare e modificare i predefiniti immagine:

**Nome** predefinito Immettete un nome descrittivo senza spazi vuoti. Se includete nel nome l’indicazione delle dimensioni dell’immagine, gli utenti potranno identificarlo più facilmente.

**Larghezza e altezza** Specificate in pixel le dimensioni in base alle quali l’immagine viene trasmessa.

**Formato** Scegliere un formato dal menu. Quando si sceglie il formato GIF, JPEG, PDF o TIFF vengono visualizzate le seguenti opzioni:

* Opzioni Quantizzazione colore GIF

   **Tipo**

   Scegli Adattivo (il valore predefinito), Web o Macintosh. Se scegli GIF con Alfa, l'opzione Macintosh® non è disponibile.

   **Dithering**

   Scegliete Diffondi o Disattivato.

   **Numero di colori**

   Trascinate il cursore per inserire 2-255.

   **Elenco colori**

   Inserite un elenco di voci separate da virgola. Ad esempio, per bianco, grigio e nero inserite 000000,888888,ffffff.

* Opzioni JPEG

   **Qualità**

   Controlla il livello di compressione JPEG. Questa impostazione interessa sia le dimensioni del file che la qualità dell’immagine. La scala di qualità JPEG va da 1 a 100.

   **Attiva il downsampling per la crominanza JPG**

   Poiché l’occhio è meno sensibile alle informazioni sul colore ad alta frequenza che alla luminanza ad alta frequenza, le immagini JPEG dividono le informazioni sull’immagine nelle componenti luminanza e colore. Quando un’immagine JPEG viene compressa, il componente della luminanza viene lasciato alla massima risoluzione, mentre per i componenti colore viene eseguito il downsampling calcolando la media di gruppi di pixel. Il downsampling riduce di metà o un terzo il volume di dati, con impatto trascurabile sulla qualità percepita. Non è possibile eseguire il downsampling sulle immagini in scala di grigio. Questa tecnica riduce il fattore di compressione ed è utile per le immagini ad alto contrasto (ad esempio, immagini con testo sovrapposto).

* Opzioni PDF e TIFF

   **Compressione**

   Scegliete un algoritmo di compressione.

**Spazio colore** Scegliere uno spazio colore.

**Nitidezza** Selezionate l’opzione Attiva nitidezza semplice per applicare un filtro di nitidezza di base all’immagine al termine del ridimensionamento. La nitidezza contribuisce a compensare la sfocatura che può prodursi quando si visualizza un’immagine in dimensioni diverse.

Per ulteriori informazioni sulla nitidezza, le modalità di ricampionamento e la maschera di contrasto, consultate [Applicazione della nitidezza a un’immagine](sharpening-image.md#sharpening_an_image).

**Modalità** di ricampionamento Scegliete un’opzione della modalità di ricampionamento. Queste opzioni aumentano la nitidezza quando si esegue il downsampling dell’immagine:

**B-Lineare** Il metodo di ricampionamento più veloce; alcuni artefatti di alias sono visibili.

**Bicubico** Aumenta l’utilizzo della CPU sul server immagini, ma produce immagini più nitide con meno artefatti di alias.

**Sharp2** Può produrre risultati leggermente più nitidi rispetto all’opzione Bicubico, ma con una CPU ancora più elevata sul server immagini.

**Tri-Lineare** utilizza risoluzioni più elevate e più basse, se disponibili; consigliato solo quando l'aliasing è un problema. Questo metodo riduce le dimensioni JPEG grazie a una minore quantità di dati ad alta frequenza.

**Maschera di contrasto** Scegliete le seguenti opzioni per regolare la nitidezza:

**Fattore** Controlla la quantità di contrasto applicata ai pixel lungo i bordi. Il valore predefinito è 1,0. Per le immagini ad alta risoluzione, è possibile aumentare questo valore fino a 5,0. Il fattore può essere interpretato come una misura dell’intensità del filtro.

**Raggio** Determina il numero di pixel attorno ai pixel del bordo che influiscono sulla nitidezza. Per immagini ad alta risoluzione, inserite un valore da 1 a 2. Con un valore basso si agisce solo sui pixel del bordo; con un valore più elevato si agisce su una fascia più ampia di pixel. Il valore più adatto dipende dalle dimensioni dell’immagine.

**Soglia** Determina l’intervallo di contrasto da ignorare quando viene applicato il filtro maschera di contrasto. In altre parole, questa opzione specifica quale deve essere il grado di differenza dei pixel da rendere più nitidi rispetto all’area circostante, affinché vengano considerati pixel di un bordo e quindi resi più nitidi. Per evitare la comparsa di disturbi, provate con valori compresi tra 0,02 e 0,2. Con il valore predefinito 6 la nitidezza viene applicata a tutti i pixel nell’immagine.

**Spazio** colore Determina se l’immagine utilizza lo spazio in cui è stata creata, in genere RGB (Originale) o uno spazio di luminanza (Intensità).

**Colore** Scegliere le seguenti opzioni:

**Profilo** colore di output Selezionate Usa predefinito o uno dei profili colore ICC disponibili in Scene7 Publishing System.

Consultate anche [Profili ICC](icc-profiles.md#icc_profiles).

**Intento** di rendering Selezionate un'opzione se desiderate ignorare l'intento di rendering predefinito del profilo colore. Usate questa opzione quando uno dei profili ICC predefiniti è lo spazio colore di destinazione di una conversione colore, un dispositivo di output (stampante o monitor) è caratterizzato da tale profilo e l’intento di rendering è valido per questo profilo.

**Incorpora profilo** Selezionate questa opzione affinché, se aprite l'immagine in Adobe® Photoshop®, venga utilizzato questo profilo.

**Risoluzione** di stampa Scegliere una risoluzione per la stampa dell'immagine; Il valore predefinito è 72 pixel.

**Modificatori** URL Se preferite specificare i modificatori URL che definiscono il predefinito per immagini, anziché le impostazioni, inserite qui i modificatori.

**URL** immagine campione Mostra la stringa URL "non elaborata" usata dal server immagini per distribuire le immagini con il predefinito per immagini che si sta aggiungendo o modificando. Nella stringa URL vengono codificate tutte le impostazioni di formattazione selezionate nella schermata Aggiungi predefinito o Modifica predefinito.

### Modifica, rimozione o disattivazione di un predefinito immagine {#editing-removing-or-deactivating-an-image-preset}

1. Fate clic su **Configurazione** &gt; **Predefiniti immagini**.
1. Nella schermata Predefiniti immagine, selezionate un predefinito nella tabella ed effettuate una delle seguenti operazioni:

   * Click **Edit** and then specify new options in the Edit Preset dialog box.
   * Click **Delete** to remove the preset from the list.
   * Deselezionate la casella di controllo Attivo accanto al nome di un predefinito per rimuoverlo dall’interfaccia utente di Scene7 Publishing System per gli utenti di Media Portal.

## Attivazione o disattivazione dei predefiniti video adattivi {#activating-or-deactivating-adaptive-video-presets}

Dynamic Media Classic offre predefiniti di codifica per video adattivi. Si tratta di un elenco di predefiniti in cui sono raggruppati i predefiniti per video adattivi da 16:9 e da 4:3. Tali predefiniti riflettono le impostazioni di codifica più comuni e sono ottimizzati per la riproduzione su dispositivi mobili, tablet e computer desktop.

Solo i predefiniti di codifica video adattiva sono attivati (o “abilitati”) per impostazione predefinita. Se necessario, potete disattivarli. I predefiniti per video adattivi non attivati non vengono visualizzati come opzione selezionabile nella sezione eVideo della finestra di dialogo Opzioni processo di caricamento.

Consultate [Caricamento e codifica dei video](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Per attivare o disattivare i predefiniti video adattivi**

1. Nell’angolo in alto a destra di Scene7 Publishing System, fate clic su **Configurazione** &gt; **Impostazione applicazione** &gt; **Predefiniti video** &gt; **Predefiniti video adattati**.
1. Nella pagina Predefiniti video adattati, deselezionate la casella di controllo accanto al nome di un predefinito per eliminarlo dall’elenco Opzioni eVideo nella finestra di dialogo Opzioni processo di caricamento.
1. Fate clic su **Chiudi**.

## Predefiniti video per la codifica di file video {#video-presets-for-encoding-video-files}

Per scegliere un predefinito di codifica, fate clic su Opzioni processo nell’angolo in basso a destra della pagina Carica. Nella finestra di dialogo Opzioni processo di caricamento, espandete le opzioni eVideo e scegliete i predefiniti di codifica desiderati.

>[!NOTE]
>
>Con l’eccezione di “Video adattivo”, abilitato per impostazione predefinita, non tutti gli altri predefiniti di codifica singola o adattiva sono visualizzati nella finestra di dialogo Opzioni processo di caricamento. Gli amministratori di Dynamic Media Classic determinano quali predefiniti di codifica video sono visibili nella finestra di dialogo Opzioni processo di caricamento.

* Scegliete uno dei seguenti predefiniti di codifica per video adattivi o per codifica singola:

   **Video adattivo 16:9**

   Per creare video con proporzioni 16:9 da distribuire a computer desktop, dispositivi mobili (iPhone, iPad, Android) e tablet (iPad, Android), ottimizzati con risoluzione e bitrate in base alla velocità di connessione dell’utente.

   **Video adattivo 4:3**

   Per creare video con proporzioni 4:3 da distribuire a computer desktop, dispositivi mobili (iPhone, iPad, Android) e tablet (iPad, Android), ottimizzati con risoluzione e bitrate in base alla velocità di connessione dell’utente.

   **Video adattivo**

   Per creare video da distribuire a dispositivi mobili, tablet e computer desktop; predefinito codifica singola che funziona con qualsiasi proporzione. I video sorgente caricati e codificati con questo predefinito sono impostati su un’altezza specifica. Tuttavia, il valore della larghezza viene ridimensionato automaticamente per mantenere le proporzioni del video.

   La flessibilità di questo ridimensionamento automatico è disponibile anche per impostazione predefinita quando create un predefinito di codifica video personalizzato.

   Consultate [Aggiunta o modifica di un predefinito di codifica video](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset)

   **Codifica video adattiva (16:9 o 4:3)**

   Create video con proporzioni 16:9 e 4:3 da distribuire a computer desktop, dispositivi mobili (iPhone, iPad, Android) e tablet (iPad, Android), ottimizzati con risoluzione e bitrate in base alla velocità di connessione dell’utente.

   Consultate [Predefiniti per codifica video adattiva (16:9 o 4:3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   **Predefiniti codifica singola**

   >[NOTA]
   >
   >per visualizzare un video sull’iPad, potete scegliere un predefinito di codifica Mobile o Tablet. I predefiniti Tablet sono stati creati appositamente per gli iPad, generalmente con risoluzione e qualità più alta per usufruire delle dimensioni delle schermo e della connessione di banda più elevata. La visualizzazione di file video codificati con un predefinito Tablet richiede di includere un codice di rilevamento dispositivi al sito mobile o all’applicazione. questo codice è disponibile per i video visualizzati su iPhone o iPad, a seconda del dispositivo di riproduzione. Se si sceglie un predefinito Mobile per la consegna dei file video ad iPad, il flusso di lavoro risulta semplificato poiché potete scegliere lo stesso file video sia per iPhone che per iPad. Tuttavia, la qualità viene standardizzata all’esperienza iPhone con risoluzione ridotta.

   * Nel gruppo Predefiniti di codifica, nell’elenco a discesa Ordina predefiniti codifica, selezionate Nome o Dimensioni per ordinare i predefiniti per nome o per dimensione di risoluzione.
   * Scegliete un predefinito di codifica basato sulla dimensione di risoluzione e sulla larghezza di banda con la quale intendete riprodurre il video.
   * Per ogni video potete scegliere un predefinito per codifica video adattiva e uno o più predefiniti di codifica. Ad esempio, potete codificare un file per desktop e dispositivo mobile in un unico processo di caricamento.

Dopo aver fatto clic sul pulsante **Avvia caricamento**, il file video principale originale viene caricato e da tale file vengono generati file codificati.

### Le opzioni dei predefiniti di codifica {#about-encoding-preset-options}

I parametri delle opzioni dei predefiniti di codifica sono i seguenti:

**Velocità** di connessione di destinazione La velocità di connessione Internet dell’utente finale di destinazione.

**Suffisso** del file codificato Il suffisso associato al file video codificato a scopo di identificazione.

**Bitrate video (velocità dati)** La quantità di dati codificati per creare un secondo di riproduzione video (in kilobit al secondo).

**Larghezza/Altezza** pixel La dimensione della larghezza dell’immagine sullo schermo, in pixel; l’altezza dell’immagine sullo schermo (in pixel).

**Fotogramma al secondo (fps)** Il numero di fotogrammi o immagini fisse per ogni secondo di video. Negli Stati Uniti e in Giappone, i video sono solitamente ripresi a 29,97 fps; in Europa e in Asia (escluso il Giappone), sono invece ripresi a 25 fps. I film sono ripresi a 24 fps.

**Bitrate** audio La quantità di dati codificati per creare un secondo di riproduzione audio, espressa in kilobit al secondo.

Le tabelle di seguito indicano le procedure ottimali per la scelta dei predefiniti per video e le convenzioni di denominazione utilizzate per designare i file codificati.

### Video adattivo (predefinito) {#adaptive-video-default}

Per creare video da distribuire a dispositivi mobili, tablet e computer desktop; predefinito di codifica che funziona con qualsiasi proporzione. I video sorgente caricati e codificati con questo predefinito (per impostazione predefinita e procedura ottimale) sono impostati su un’altezza specifica, ma il valore della larghezza viene ridimensionato automaticamente per mantenere le proporzioni del video.

**Video adattivo (predefinito)**

|  | Nome predefinito di codifica/Descrizione | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto x360, 800 Kbps | _Mobile_Autox360p_800K | 800 | Auto x360 | Come sorgente | 64 | Per dispositivi mobili (iPhone, iPad, Android) |
| 2 | Auto x480, 1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Auto x480 | Come sorgente | 96 | Per tablet (iPad, Android) |
| 3 | Auto x720, 2600 Kbps | _Desktop_Autox720p_2600K | 2600 | Auto x720 | Come sorgente | 128 | Per desktop |

### Predefiniti per codifica video adattiva (16:9 o 4:3){#adaptive-video-encoding-or-video-presets}

Di seguito sono elencati i predefiniti di codifica disponibili per video adattivi; combinano una serie di singoli predefiniti di codifica selezionati automaticamente in base alle proporzioni del video caricato. Ad esempio, se caricate un video da 4:3, questo viene codificato automaticamente utilizzando i cinque predefiniti da 4:3 inclusi nell’elenco dei predefiniti principali per l’opzione **Codifica video adattiva (16:9 o 4:3)**.

Per informazioni sui parametri delle opzioni di codifica, consultate [Le opzioni dei predefiniti di codifica](application-setup.md#about_encoding_preset_options).

**Predefiniti per codifica video adattiva (16:9 o 4:3)**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, Mobile (iPhone, iPad, Android), (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 2 | 4:3, 384x288 px, Mobile (iPhone, iPad, Android), (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 3 | 16:9, 512x288, Mobile (iPhone, iPad, Android), (600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512x288 | Come sorgente | 64 | Risoluzione media, 3G |
| 4 | 4:3, 384x288, Mobile (iPhone, iPad, Android), (600 Kbps) | 700 | _Mobile_384x288_600 | 600 | 384x288 | Come sorgente | 64 | Risoluzione media, 3G |
| 5 | 16:9, 640x360, Tablet (iPad, Android), (800 Kbps) | 900 | _iPad_640x360_800K | 800 | 640x360 | Come sorgente | 80 | Risoluzione media, WiFi |
| 6 | 4:3, 640x480, Tablet (iPad, Android), (800 Kbps) | 900 | _iPad_640x480_800K | 800 | 640x480 | Come sorgente | 80 | Risoluzione media, WiFi |
| 7 | 16:9, 768x432, Tablet (iPad, Android), (1200 Kbps) | 1,5 Mbps | _iPad_768x432_1200K | 1200 | 768x432 | Come sorgente | 96 | Alta risoluzione, WiFi |
| 8 | 4:3, 768x576, Tablet (iPad, Android), (1200 Kbps) | 1,5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | Come sorgente | 96 | Alta risoluzione, WiFi |
| 9 | 16:9, 1280x720, Desktop, (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Come sorgente | 128 | Widescreen ad alta definizione |
| 10 | 4:3, 1280x960, Desktop, (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | Come sorgente | 128 | Alta definizione |

### Predefiniti di codifica video per computer desktop {#desktop-video-encoding-presets}

Predefiniti di codifica video per MP4 e OGV su computer desktop.

Per informazioni sui parametri delle opzioni di codifica, consultate [Le opzioni dei predefiniti di codifica](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2 - Audio AAC - Estensione MP4**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | Come sorgente | 64 | Widescreen a bassa risoluzione |
| 2 | 16:9, 640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640x360 | Come sorgente | 80 | Widescreen a risoluzione media |
| 3 | 16:9, 800x450 (1200 Kbps) | 1,5 Mbps | _800x450_1200K | 1200 | 800x450 | Come sorgente | 96 | Risoluzione medio-alta |
| 4 | 16:9, 1280x720 (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Come sorgente | 128 | Widescreen ad alta definizione |
| 5 | 4:3, 320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | Come sorgente | 64 | Bassa risoluzione |
| 6 | 4:3, 480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | Come sorgente | 80 | Risoluzione media |
| 7 | 4:3, 640x480 (1200 Kbps) | 1,5 Mbps | _640x480_1200K | 1200 | 640x480 | Come sorgente | 96 | Risoluzione medio-alta |
| 8 | 4:3, 1280x960 (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 | 1280x960 | Come sorgente | 128 | Alta definizione |

**OGG Vorbis Theora - Estensione OGV**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps), OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | Come sorgente | 64 | Widescreen a bassa risoluzione |
| 2 | 16:9, 640x360 (800 Kbps), OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | Come sorgente | 80 | Widescreen a risoluzione media |
| 3 | 16:9, 800x450 (1200 Kbps), OGG | 1,5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | Come sorgente | 96 | Risoluzione medio-alta |
| 4 | 16:9, 1280x720 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x720_2000K | 2000 | 1280x720 | Come sorgente | 128 | Widescreen ad alta definizione |
| 5 | 4:3, 320x240 (400 Kbps), OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | Come sorgente | 64 | Bassa risoluzione |
| 6 | 4:3, 480x360 (800 Kbps), OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | Come sorgente | 80 | Risoluzione media |
| 7 | 4:3, 640x480 (1200 Kbps), OGG | 1,5 Mbps | _OGG_640x480_1200K | 1200 | 640x480 | Come sorgente | 96 | Risoluzione medio-alta |
| 8 | 4:3, 1280x960 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x960_2000K | 2000 | 1280x960 | Come sorgente | 128 | Alta definizione |

### Predefiniti di codifica per video per dispositivi mobili {#mobile-video-encoding-presets}

Come fps sorgente. Predefiniti di codifica video per iPhone, iPad e dispositivi mobili Android.

Per informazioni sui parametri delle opzioni di codifica, consultate [Le opzioni dei predefiniti di codifica](application-setup.md#about_encoding_preset_options).

**H264 Baseline 2.1 - Audio AAC - Estensione MP4**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Bitrate video (Kbps) | Larghezza/Altezza in pixel | Fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, Mobile (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 2 | 16:9, 512x288, Mobile (600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512x288 | Come sorgente | 64 | Risoluzione media, 3G |
| 3 | 16:9, 512x288, Mobile (800 Kbps) | 900 | _Mobile_512x288_800K | 800 | 512x288 | Come sorgente | 80 | Risoluzione media, Wi-Fi |
| 4 | 16:9, 512x288, Mobile (1000 Kbps) | 1,2 Mbps | _Mobile_512x288_1000K | 1000 | 512x288 | Come sorgente | 80 | Alta risoluzione, Wi-Fi |
| 5 | 16:9, 512x288, Mobile (1200 Kbps) | 1,5 Mbps | _Mobile_512x288_1200K | 1200 | 512x288 | Come sorgente | 96 | Alta risoluzione, Wi-Fi |
| 6 | 4:3, 384x288, Mobile (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 7 | 4:3, 384x288, Mobile (600 Kbps) | 700 | _Mobile_384x288_600K | 600 | 384x288 | Come sorgente | 64 | Risoluzione media, 3G |
| 8 | 4:3, 448x336, Mobile (800 Kbps) | 900 | _Mobile_448x336_800K | 800 | 448x336 | Come sorgente | 80 | Risoluzione media, Wi-Fi |
| 9 | 4:3, 448x336, Mobile (1000 Kbps) | 1,2 Mbps | _Mobile_448x336_1000K | 1000 | 448x336 | Come sorgente | 80 | Alta risoluzione, Wi-Fi |
| 10 | 4:3, 448x336, Mobile (1200 Kbps) | 1,5 Mbps | _Mobile_448x336_1200K | 1200 | 448x336 | Come sorgente | 96 | Alta risoluzione, Wi-Fi |

## Predefiniti per visualizzatori {#viewer-presets}

>[!NOTE]
>
>**Avviso** di fine del ciclo di vita dei visualizzatori Flash - A partire dal 31 gennaio 2017, Adobe Scene7 Publishing System ha dichiarato ufficialmente terminato il supporto per la piattaforma di visualizzatori Flash. Per ulteriori informazioni su questa importante modifica, consulta il seguente sito Web sulle domande frequenti: [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html).

Un *predefinito per visualizzatori* è un gruppo di impostazioni con cui viene definito in che modo le risorse multimediali verranno visualizzate sullo schermo del computer e sui dispositivi mobili dell’utente. In qualità di amministratore, potete creare dei predefiniti per visualizzatori. Sono disponibili impostazioni per un’ampia gamma di opzioni di configurazione dei visualizzatori. Ad esempio, è possibile modificare le dimensioni dello schermo del visualizzatore, il comportamento dello zoom, gli schemi di colori, i bordi e i font.

Come procedura ottimale, usate i visualizzatori per video HTML5 Dynamic Media Classic. I predefiniti utilizzati nei visualizzatori Video HTML5 sono lettori video affidabili. Combinando in un singolo lettore la possibilità di progettare i componenti di riproduzione in HTML5 e CSS, usufruire di riproduzione incorporata e utilizzare lo streaming adattativo e progressivo a seconda delle caratteristiche del browser, i contenuti multimediali potranno essere visti dagli utenti con computer desktop, tablet e dispositivi mobili. Potrete così offrire ai visitatori un’esperienza di streaming video ottimizzata.

Consultate [I visualizzatori](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) HTML5 nella guida di riferimento dei visualizzatori Adobe.

Consultate Matrice [di compatibilità dei predefiniti per visualizzatori](application-setup.md#scene7_viewer_preset_compatibility_matrix)Dynamic Media Classic.

Consultate [Procedura ottimale: utilizzo del visualizzatore video HTML5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

In base al visualizzatore, potete aggiungere delle funzioni per community. e comprendono i pulsanti Incorpora, E-mail, Collega e Visita. Questi pulsanti consentono agli utenti che utilizzano i visualizzatori di condividerli con altri utenti o di aprire il sito Web di Dynamic Media Classic.

Consultate anche gli esempi della libreria di riferimento dei visualizzatori Adobe [qui](/help/assets/vlist/vlist.html) e [qui](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Supporto nei visualizzatori per pagine Web reattive {#viewer-support-for-responsive-designed-web-pages}

Diversi tipi di pagine Web hanno esigenze differenti. In una pagina Web può essere necessario un collegamento che apre il visualizzatore HTML5 in una seconda finestra del browser. In altri casi, potrebbe essere necessario incorporare il visualizzatore HTML5 direttamente nella pagina. In quest’ultimo caso, la pagina Web potrebbe avere un layout statico oppure essere “reattiva” e assumere un aspetto diverso su dispositivi diversi o per diverse dimensioni della finestra del browser. Per soddisfare queste esigenze, i visualizzatori HTML5 forniti con Dynamic Media Classic supportano sia le pagine Web statiche che quelle reattive.

See [Responsive Static Image library](https://marketing.adobe.com.com/resources/help/en_US/s7/is_ir_api/is_api/c_about_responsive_static_image_library.html)in the *Adobe Image Serving API Help* for more information on how to embed responsive viewers onto your web pages.

### Tipi di predefiniti per visualizzatori {#viewer-preset-types}

Gli amministratori possono creare e personalizzare i seguenti tipi di predefiniti per visualizzatori.

**Visualizzatore** eCatalog Simula la lettura di un catalogo stampato. Potete spostarvi da una pagina all’altra, ingrandire e ridurre gli elementi di una pagina, usare le mappe immagine per visualizzare ulteriori informazioni sugli elementi della pagina o per cercare nel catalogo. Potete inoltre includere un pannello Info con le informazioni dettagliate su un articolo collegato a una mappa, se all’area della mappa è assegnato un attributo rollover_key valido. Per includere un pannello Info, specificate l’URL di un server informazioni nel riquadro Impostazioni pannello Info, nella finestra Predefinito visualizzatore eCatalog.

**Visualizzatore** set di campioni Consente di visualizzare un’immagine con un colore, un materiale, una texture, una finitura o un tessuto diverso. Per visualizzare l’immagine con le varianti desiderate, gli utenti del sito potranno fare clic sulla relativa miniatura.

**Visualizzatore** set di file multimediali diversi Consente di visualizzare diversi tipi di file multimediali in un visualizzatore. Potete includere set di campioni, set 360 gradi, immagini e video. Potete configurare schede per diversi tipi di contenuto, ad esempio una scheda per i set di immagini e una scheda per i video. Per la riproduzione dei video da un set di file multimediali diversi viene usato un visualizzatore standard con un indicatore temporale e controlli per interrompere, mettere in pausa, riavvolgere e riprodurre il video. Quando configurate il predefinito per visualizzatori di un set di file multimediali diversi, specificate i visualizzatori da usare per i diversi tipi di risorse del set. Per visualizzare un set di file multimediali diversi potete anche usare il visualizzatore Griglia o Carosello.

**Visualizzatore** di set 360 gradi Consente di visualizzare più visualizzazioni di un’immagine per consentire agli utenti di ruotare l’oggetto in modo da esaminare i diversi lati e angolazioni.

**Visualizzatore** video Consente di visualizzare i video usando le dimensioni di risoluzione del file sorgente o una dimensione personalizzata. Dynamic Media Classic viene fornito con diversi predefiniti per visualizzatori per la riproduzione di video; inoltre, se siete un amministratore, potete creare predefiniti per visualizzatori video personalizzati. Sono disponibili oltre dodici diverse impostazioni per la configurazione del visualizzatore video. Potete configurare la relativa dimensione, il colore di primo piano e di sfondo, i controlli audio e video, la barra di avanzamento, l’interfaccia utente, le funzioni per social networking e l’Aiuto.

**Visualizzatori** zoom Offre tre tipi di visualizzatori zoom:

**Visualizzatore** zoom Consente agli utenti di ingrandire l’area facendo clic su di essa. Sono disponibili controlli per ingrandire/ridurre la visualizzazione e reimpostare le dimensioni predefinite dell’immagine.

**Visualizzatore zoom: A comparsa** Visualizza una seconda immagine dell’area ingrandita accanto all’immagine originale. Non vi sono controlli; gli utenti devono semplicemente spostare la selezione sull’area da visualizzare.

Quando calcolate l’utilizzo di larghezza di banda totale per questo visualizzatore, tenete presente che nel visualizzatore vengono caricate sia l’immagine principale che l’immagine a comparsa. Le dimensioni dell’immagine principale (Larghezza e Altezza area visualizzazione) e il fattore di zoom determinano le dimensioni dell’immagine a comparsa. Per impedire che le dimensioni del file dell’immagine a comparsa diventino eccessive, bilanciate questi due valori: se le dimensioni dell’immagine principale sono grandi, riducete il fattore di zoom. I valori Larghezza a comparsa e Altezza comparsa determinano le dimensioni della finestra a comparsa ma non dell’immagine a comparsa caricata nel visualizzatore.

Ad esempio, se le dimensioni dell’immagine principale sono 350 x 350 pixel, con un fattore di zoom pari a 3 l’immagine a comparsa risultante sarà di 1050 x 1050 pixel. Se le dimensioni dell’immagine principale sono 300 x 300 pixel, con un fattore di zoom pari a 4 l’immagine a comparsa risultante sarà di 1200 x 1200 pixel. In base alla qualità JPEG impostata (impostazioni consigliate: 80-90), potete ridurre sensibilmente le dimensioni del file. I fattori di zoom consigliati sono i valori compresi tra 2,5 e 4, a seconda delle dimensioni dell’immagine principale.

### Matrice di compatibilità dei predefiniti per visualizzatori Dynamic Media Classic {#scene-viewer-preset-compatibility-matrix}

**Avviso** di fine del ciclo di vita dei visualizzatori Flash: A partire dal 31 gennaio 2017, Adobe Scene7 Publishing System ha dichiarato ufficialmente terminato il supporto per la piattaforma di visualizzatori Flash.

Per ulteriori informazioni su questa importante modifica, consulta il seguente sito Web sulle domande frequenti: [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html).

Nella tabella seguente sono elencati i predefiniti per visualizzatori Dynamic Media Classic attualmente disponibili. Viene inoltre specificata la compatibilità con dispositivi desktop e mobili nonché la tecnologia utilizzata per ciascun visualizzatore.

Consultate anche gli esempi della libreria di riferimento dei visualizzatori Adobe [qui](/help/assets/vlist/vlist.html) e [qui](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Per informazioni sui browser Web e sulle versioni del sistema operativo supportati per i visualizzatori, consultate le relative Note sulla versione.

Consultate [Note](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/)sulla versione di riferimento dei visualizzatori Adobe.

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori zoom |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori per set di immagini |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
|  Visualizzatori per set di campioni |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori eCatalog |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Include il supporto per social media e la ricerca di cataloghi) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Include il supporto per social media e la ricerca di cataloghi) | HTML5 | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori per set 360 gradi |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**Visualizzatori per eVideo**

Dynamic Media Classic supporta la riproduzione di video mobile per video MP4 H.264.

* Per un elenco dei dispositivi BlackBerry che supportano questo formato video, consultate: Formati video [supportati su Blackberry](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* Per un elenco dei dispositivi Windows che supportano questo formato video, consultate i seguenti:Formati video[supportati su Windows Phone](https://docs.microsoft.com/en-us/previous-versions/windows/apps/ff462087(v=vs.105)?redirectedfrom=MSDN)

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android | Smartphone Blackberry | Windows Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Include il supporto per sottotitoli codificati). Consultate [Procedura consigliata: utilizzo del visualizzatore universale per video HTML5.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Comprende il supporto per sottotitoli codificati e social media.) | HTML5 | X | X | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Set di file multimediali diversi |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Matrice dei gesti supportati dai visualizzatori per dispositivi mobili {#supported-mobile-viewers-gestures-matrix}

Nella tabella seguente sono descritti i gesti per visualizzatori mobili supportati su dispositivi iOS, Android 2.x e Android 3.x.

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori per set di immagini |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Informazioni sulla schermata Preimpostazioni visualizzatore {#about-the-viewer-preset-screen}

Potete creare e gestire i predefiniti per visualizzatori nella schermata Predefiniti per visualizzatore. Per aprire questa schermata, fate clic su **Configurazione** &gt; **Predefiniti visualizzatore**.

La schermata Predefiniti visualizzatore offre strumenti che consentono di eseguire le seguenti attività:

**Aggiunta di un predefinito** Fate clic su Aggiungi e selezionate le opzioni desiderate nella finestra di dialogo Aggiungi predefinito per visualizzatore.

Consultate [Aggiunta e modifica dei predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets).

**Modifica di un predefinito** Selezionate un predefinito, quindi fate clic su **Modifica**.

Consultate [Aggiunta e modifica dei predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets).

**Eliminazione di un predefinito** Selezionate un predefinito, quindi fate clic su **Elimina**.

**Esportazione di un predefinito** Selezionate un predefinito per visualizzatori HTML5, quindi fate clic su Esporta per scaricare l’interfaccia del visualizzatore in modo da poterlo usare come base per creare e aggiungere un nuovo predefinito per visualizzatori.

Consultate [Esportazione di un predefinito](application-setup.md#exporting_an_html5_viewer_preset)per visualizzatori HTML5.

**Applicazione di filtri all’elenco** Predefiniti visualizzatore Utilizzate questi strumenti per filtrare l’elenco:

* Aprite l’elenco a discesa **Attivo/Inattivo** e scegliete un’opzione per mostrare i predefiniti attivi, i predefiniti inattivi o tutti i predefiniti.
* Aprite l’elenco a discesa **Visualizzatore** e scegliete un’opzione per visualizzare soltanto alcuni visualizzatori specifici. Scegliete **Tutti i visualizzatori** per visualizzare tutti i visualizzatori.

**Ordinamento dei predefiniti** Fate clic sull’intestazione di una colonna (Attivo, Tipo, Predefinito o Piattaforma) per ordinare l’elenco in base a una colonna. Fate clic sul titolo di una colonna una seconda volta per ordinare l’elenco in ordine decrescente (o crescente).

**Attivazione e disattivazione dei predefiniti** Selezionate un predefinito e fate clic sull’opzione Attivo per attivarlo o disattivarlo.

Consultate [Attivazione o disattivazione dei predefiniti per visualizzatori](application-setup.md#activating_or_deactivating_viewer_presets).

>[!NOTE]
>
>Fate clic su Anteprima sul lato destro della schermata Predefiniti visualizzatore per verificare l’aspetto di una risorsa in base al predefinito per visualizzatore selezionato. Per visualizzare un’altra risorsa, fate clic su Sfoglia nella schermata Predefiniti visualizzatore e selezionate una risorsa diversa nella finestra di dialogo Seleziona anteprima risorsa.

### Aggiunta e modifica dei predefiniti per visualizzatori {#adding-and-editing-viewer-presets}

Oltre ad aggiungere i predefiniti visualizzatore tramite Aggiungi nell’interfaccia utente, potete anche usare Esporta per aggiungere un predefinito visualizzatore. Potete semplicemente esportare un predefinito per visualizzatori HTML5 esistente e usarlo come base per il nuovo predefinito.

Consultate [Esportazione di un predefinito](application-setup.md#exporting_an_html5_viewer_preset)per visualizzatori HTML5.

**Per aggiungere o modificare dei predefiniti per visualizzatori**

1. Nell’angolo in alto a destra di Scene7 Publishing System, fate clic su **Configurazione** &gt; **Predefiniti visualizzatore**.

   Potete filtrare l’elenco dei predefiniti. Ad esempio, per visualizzare soltanto i predefiniti per i visualizzatori video, selezionate Visualizzatore video dall’elenco a discesa Visualizzatori nella barra degli strumenti che si trova appena sopra la tabella.

1. Nella schermata Predefiniti visualizzatore, aggiungete o modificate il predefinito per visualizzatori.

   **Aggiunta** Fare clic su Aggiungi sulla barra degli strumenti. Nella finestra di dialogo Aggiungi predefinito per visualizzatore, scegliete una piattaforma e un tipo di risorsa multimediale avanzata. 

   Al termine, fate clic su **Salva con nome**.

   **Aggiungendo i dati da un predefinito** per visualizzatori esistente Nella tabella, selezionate un predefinito per visualizzatori video e fate clic su Modifica nella barra degli strumenti.

   Dopo aver configurato il visualizzatore video, fate clic su **Salva con nome** per salvare il predefinito specificando un altro nome nel campo Nome predefinito.

   **Modifica** Selezionate un predefinito per visualizzatori esistente e fate clic su **Modifica**.

1. Nella schermata Configura visualizzatore, immettete o modificate il nome del predefinito nel campo Nome predefinito.
1. Impostate le opzioni rimanenti in base alle vostre esigenze.

   >[NOTA]
   >
   >scegliete Come sorgente per ridimensionare automaticamente il visualizzatore video nella dimensione di risoluzione del video codificato stesso. Se scegliete questa opzione, non potete specificare i valori di larghezza e altezza dell’area di visualizzazione e tali valori verranno invece determinati dal video stesso. Se scegliete Come sorgente, impostate le opzioni relative alle dimensioni dei margini per riflettere le dimensioni dell’interfaccia fuori dall’area di riproduzione del video. Le dimensioni del margine corrispondono all’altezza e alla larghezza in pixel dei controlli video. La figura di seguito illustra come determinare le dimensioni dei margini da usare.*

   ![](assets/vs_video_viewer_configure_margin.png)

1. Effettuate una delle seguenti operazioni:

   * Fate clic su **Salva con nome** se avete aggiunto un predefinito per visualizzatori a partire da un predefinito esistente.
   * Fate clic su **Salva** se avete aggiunto o modificato un predefinito per visualizzatori.

### Esportazione di un predefinito per visualizzatori HTML5 {#exporting-an-html-viewer-preset}

Potete esportare un predefinito per visualizzatori HTML5 esistente da usare come base per la creazione di un nuovo predefinito per visualizzatori HTML5. In questo modo si evita di dover creare un visualizzatore da zero. Se esportate un predefinito con aspetto e comportamento simili a quelli desiderati, potrete usarlo come base di partenza per apportare le regolazioni necessarie.

Tenete presente che tutti i file CSS predefiniti per visualizzatori in SPS usano percorsi di trasmissione delle immagini relativi che puntano alle risorse presenti in `Scene7SharedAssets`. Ad esempio, di seguito è riportato un percorso relativo a una risorsa immagine in un file CSS predefinito per visualizzatori presente in `Scene7SharedAsset`: Se `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`invece ospitate file CSS per visualizzatori sul vostro sito, dovete risolvere il percorso relativo dell’immagine utilizzando un percorso esplicito del server immagini nel vostro ambiente. A scopo illustrativo, se devi aggiornare il percorso relativo sopra a un percorso esplicito, potrebbe essere simile al seguente, dove `https://s7d1.scene7.com` è il percorso diretto del server immagini: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Per esportare un predefinito per visualizzatori HTML5**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Fate clic su **Configurazione** &gt; **Predefiniti visualizzatore**.
1. On the Viewer Presets toolbar, in the second drop-down list from the left, select **HTML5**.
1. Selezionate **Tutti i visualizzatori** nel terzo elenco a discesa da sinistra.
1. Selezionate il predefinito per visualizzatori da usare come base per la creazione di un nuovo predefinito per visualizzatori HTML5.
1. Nella barra degli strumenti, fate clic su **Esporta**.
1. Nella finestra di dialogo Esporta risorse selezionate, fate clic su **Invia esportazione**.

   Dopo l’esportazione, ottenete un file CSS. Scaricate e decomprimete il file.

1. Aprite il file CSS in un Editor CSS, apportate le modifiche e salvate il file.
1. Caricate il file CSS in Scene7 Publishing System.

   Consultate [Caricamento dei file](uploading-files.md#uploading_files).

1. Pubblicate il file CSS sul server immagini per file multimediali dinamici.

   Consultate [Pubblicazione dei file](publishing-files.md#publishing_files).

1. Aggiungete il nuovo predefinito per visualizzatori seguendo la procedura standard. Selezionate il file CSS del visualizzatore caricato.

   Consultate [Aggiunta e modifica dei predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets).

### Attivazione o disattivazione dei predefiniti per visualizzatori {#activating-or-deactivating-viewer-presets}

Per creare un URL per la visualizzazione delle risorse, gli utenti aprono l’elenco a discesa Predefiniti nella finestra di dialogo Anteprima, selezionano un predefinito per visualizzatore e fanno clic su Copia URL (consultate [Copia dell’URL di un predefinito per visualizzatori](application-setup.md#copying_the_url_of_a_viewer_preset)). Questo elenco di predefiniti offre i predefiniti per visualizzatori aggiunti e gestiti dagli amministratori nella schermata Predefiniti per visualizzatore. Ad esempio, tutti i predefiniti per visualizzatori eCatalog attivi vengono visualizzati nell’elenco a discesa Predefiniti nella finestra di dialogo Anteprima quando un utente esegue l’anteprima di un eCatalog.

Se i predefiniti per visualizzatori non vengono disattivati nella schermata Predefiniti per visualizzatore, nell’elenco a discesa Predefiniti nella finestra di dialogo Anteprima potrebbero accumularsi troppi predefiniti. 

**Per attivare o disattivare i predefiniti per visualizzatori**

1. Choose **Setup** &gt; **Viewer Presets** to open the Viewer Presets screen.
1. Selezionate o deselezionate l’opzione Attivo per attivare o disattivare i predefiniti per visualizzatori.

### Copia dell’URL di un predefinito per visualizzatori {#copying-the-url-of-a-viewer-preset}

Una volta pubblicata una risorsa, potete copiare un URL per visualizzare la risorsa con le impostazioni di un predefinito per visualizzatore.

L’URL viene copiato negli Appunti. Potete utilizzarlo come desiderate nel codice HTML di una pagina Web, in un dispositivo mobile o in un’applicazione.

**Per copiare l’URL di un predefinito per visualizzatori**

1. Selezionate la risorsa nel pannello Sfoglia.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, fate clic su **Copia URL** a destra del visualizzatore desiderato.
   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, sotto la miniatura, fate clic su **Anteprima** &gt; **Elenco visualizzatori**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**.

   * Fate clic su **Visualizzazione elenco**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, a destra della miniatura, fate clic su **Anteprima** &gt; **Elenco visualizzatori**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**.

   * Fate clic su **Visualizzazione griglia**, **Visualizzazione elenco** o **Visualizzazione dettagli**. Nella stessa barra degli strumenti, fate clic su **Anteprima** &gt; **Elenco visualizzatori**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**.

### Copiare il codice da incorporare di un predefinito per visualizzatori {#copying-the-embed-code-of-a-viewer-preset}

La funzione Incorpora codice permette di analizzare il codice visualizzatore del predefinito per visualizzatori selezionato. Potete anche copiare il codice negli Appunti per poi incollarlo nelle pagine Web su cui verrà distribuito il visualizzatore. 

La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

**Per copiare il codice da incorporare di un predefinito per visualizzatori**

1. Selezionate la risorsa nel pannello delle risorse.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL a destra, fate clic su **Incorpora codice**.
   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, sotto la miniatura, fate clic su **Anteprima** &gt; **Elenco visualizzatori**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**.

   * Fate clic su **Visualizzazione elenco**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, a destra della miniatura, fate clic su **Anteprima** &gt; **Elenco visualizzatori**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**.

   * Fate clic su **Visualizzazione griglia**, **Visualizzazione elenco** o **Visualizzazione dettagli**. Nella stessa barra degli strumenti, fate clic su **Anteprima** &gt; **Elenco visualizzatori**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**.

1. Nella finestra di dialogo Codice da incorporare, fate clic su **Copia negli Appunti**.
1. Fate clic su **Chiudi**.

## Configurazione dei visualizzatori predefiniti {#configuring-default-viewers}

Quando utilizzate la funzione Anteprima in Scene7 Publishing System, potete usare i visualizzatori predefiniti per configurare il visualizzatore predefinito associato a una risorsa. Potete impostare l’esperienza di anteprima predefinita per i seguenti tipi di risorse:

* Immagine
* Video
* Set 360 gradi
* Catalogo
* Set di immagini
* Set di campioni
* Set file multimediali

**Per configurare i visualizzatori predefiniti**

1. In the Setup drop-down list, click **Application Setup**.
1. In the Setup window, in the left pane, expand **Application Setup** &gt; **Viewers**
1. Click **Default Viewers**.
1. Nella finestra Visualizzatori predefiniti, nell’elenco a discesa per ogni tipo di risorsa, selezionate il visualizzatore da associare all’anteprima della risorsa.
1. In the lower-right corner of the Default Viewers window, click **Save Settings**.
1. In the lower-right corner of the Setup window, click **Close** to return to the Asset window.

## Visualizzazione metadati {#metadata-views}

I *metadati* sono informazioni standardizzate su una risorsa. Potete utilizzare i metadati per semplificare il flusso di lavoro, organizzare le risorse e migliorare le ricerche. Dynamic Media Classic supporta lo standard IPTC (International Press Telecommunications Council) e XMP (Extensible metadata platform). Prima che gli utenti possano vedere o immettere i metadati di una risorsa in visualizzazione Dettagli, possono aprire il menu Visualizzazioni metadati e scegliere il set di campi di metadati che desiderano visualizzare o utilizzare per descrivere la risorsa.

Dynamic Media Classic viene fornito con visualizzazioni di metadati predefinite e gli amministratori possono creare visualizzazioni di metadati personalizzate che gli utenti possono scegliere quando immettono i metadati.

### Creazione di una visualizzazione metadati {#creating-a-metadata-view}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Views**.
1. Fate clic su **Aggiungi**.
1. Nel campo di testo Nome predefinito, inserite un nome per la visualizzazione.
1. (Optional) Check **Make Default** to make this view the one that users see when they open the Metadata panel in Detail View.
1. (Optional) Select **Include UDF** to include user-defined fields in the view. Questi vengono presentati nella parte superiore del pannello Metadati in visualizzazione Dettagli.
1. Select the fields you want for the view (click **Select All** to select all the fields).
1. Fate clic su **Salva**.

   Le categorie e i campi selezionati per la visualizzazione vengono visualizzati nel pannello Anteprima.

### Gestione di visualizzazioni metadati {#managing-metadata-views}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Views**.
1. Effettuate una delle seguenti operazioni:

   * Per visualizzare un’anteprima di una visualizzazione, selezionatela. I campi della visualizzazione vengono visualizzati nel pannello Anteprima.
   * To edit a view, select it and then click **Edit**. Then select or deselect field names on the Preview panel, and select or deselect the **Include UDF** option.
   * To delete a view, select it and then click **Delete**.
   * To make a view the default, select it and then click **Make Default**. La visualizzazione predefinita è quella che gli utenti vedono non appena aprono una risorsa in visualizzazione Dettagli e passano al pannello Metadati.

## Predefiniti per metadati {#metadata-presets}

I predefiniti per metadati consentono agli amministratori di controllare e modificare i metadati assegnati alle risorse. In visualizzazione Dettagli, un utente può specificare i metadati relativi a una risorsa nei campi forniti a tale scopo. Ad esempio, un utente può inserire un nome proprietario, una descrizione del copyright e un indirizzo. Per verificare che gli utenti inseriscano queste informazioni in modo preciso e completo, potete creare predefiniti per metadati. Scegliendo un predefinito per metadati in visualizzazione Dettagli, i campi metadati vengono compilati automaticamente con valori predefiniti. Ad esempio, il nome proprietario, la descrizione del copyright e l’indirizzo vengono inseriti automaticamente.

Create un predefinito per metadati per ciascun set di valori per metadati che desiderate vengano inseriti automaticamente per gli utenti in visualizzazione Dettagli per descrivere una risorsa.

### Creazione o modifica di un predefinito per metadati {#creating-or-editing-a-metadata-preset}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Presets** .
1. Nella schermata Predefiniti metadati, effettuate una delle seguenti operazioni:

   * To create a preset, click **Add**. Nel campo di testo Nome modello metadati, digitate un nome per il predefinito, quindi fate clic su Visualizzazione **** metadati e scegliete una visualizzazione dall’elenco a discesa (consultate Visualizzazione [](application-setup.md#metadata_views)metadati).
   * To edit an existing preset, select the preset from the Metadata Presets list and then click **Edit**.

1. Espandete i titoli che desiderate includere nel predefinito e inserite i valori nei diversi campi da includere nel predefinito.
1. Fate clic su **Salva**.

   Le categorie e i campi selezionati per il predefinito vengono visualizzati nel pannello dell’anteprima.

### Gestione di predefiniti per metadati {#managing-metadata-presets}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Presets**.
1. Effettuate una delle seguenti operazioni:

   * Per visualizzare l’anteprima di un predefinito, selezionate il predefinito. Le informazioni sul predefinito (categorie e campi) vengono visualizzate nella schermata Anteprima.
   * To delete a preset, select the preset, and then click **Delete**.

## Campi definiti dall’utente {#user-defined-fields}

I campi metadati definiti dall’utente possono essere creati solo da un amministratore di Media Portal o un amministratore società. I campi personalizzati possono essere utili per organizzare le risorse in Scene7 Publishing System. Se necessario, potete contrassegnare i campi come Attivo. Se attivati, i nomi di tali campi di metadati personalizzati compaiono nella visualizzazione Dettagli del pannello Metadati. Nei campi di metadati definiti dall’utente gli utenti possono immettere informazioni per descrivere le risorse. Gli utenti possono inoltre utilizzare tali campi di metadati come criteri di ricerca.

I campi metadati definiti dall’utente sono utili ad esempio per ritardare il momento di attivazione di una risorsa per un lancio o una promozione. È possibile definire un campo di attivazione in base al tipo *Data*. Then, using the **Metadata** panel in **Detail** view or **File** &gt; **Edit Info**, you can specify when the asset is activated. Scene7 Publishing System verifica lo stato di pubblicazione di una risorsa e la cronologia delle modifiche. Se non rientra nel tempo di attivazione, lo stato di pubblicazione è "Non pubblicato".

>[!NOTE]
>
>per rendere i campi definiti dall’utente disponibili nel pannello Metadati in visualizzazione Dettagli, è necessario includere tali campi in Visualizzazioni metadati. Nella schermata Visualizzazioni metadati, selezionate l’opzione Includi UDF (User-Defined Fields, campi definiti dall’utente). Per ulteriori informazioni, consultate [Visualizzazione metadati](application-setup.md#metadata_views).

>[!NOTE]
>
>per cercare le risorse utilizzando i campi definiti dall’utente, fate clic su **Configurazione** &gt; **Configurazione personale** e selezionate **Includi UDF nella ricerca**. Consultate [Configurazione personale](personal-setup.md#personal_setup).

### Creazione di un campo di metadati definito dall’utente {#creating-a-user-defined-metadata-field}

1. Fate clic su **Configurazione** &gt; **Impostazione applicazione** &gt; **Metadati** &gt; **Campi definiti dall’utente**.
1. Fate clic su **Aggiungi**.
1. Nella finestra di dialogo Campo personalizzato, impostate le opzioni desiderate.

   **Nome** Immettere un nome per il campo di metadati.

   **Tipo** Scegliete un’opzione per definire il tipo di informazioni che gli utenti possono immettere nel campo di metadati:

   **Stringa** Una stringa di testo.

   **Int** Un numero intero.

   **Mobile** Un numero a virgola mobile.

   **Sì/No** Un valore booleano sì/no.

   **Data** Una data. Il formato consentito è GG/MM/AAAA.

   **Nome** file Il nome di un file.

   **Colore** Il nome di un colore.

   **Dimensione** Larghezza e altezza della risorsa.

   **Senza tipo** Per compatibilità con versioni precedenti. Non selezionate questa opzione.

   **Valore** predefinito (facoltativo) Immettete il valore che verrà immesso dagli utenti nel campo. Il valore immesso diventa il valore predefinito per il nuovo campo creato.

   **Applicabile a** (facoltativo), scegliete un tipo di risorsa se desiderate che il campo di metadati sia applicabile solo a un tipo specifico di risorsa.

   ***Note**: Choose an **Applies To** option carefully because you cannot change the **Applies To** option after you create a user-defined field. Dynamic Media Classic lets you edit the name, type, and default value of a user-defined field, but not the **Applies To** setting. *

1. Al termine della creazione del campo di metadati, fate clic su **Salva**.

### Gestire i campi definiti dall’utente {#manage-user-defined-fields}

Nella schermata Campi definiti dall’utente sono disponibili i comandi necessari per gestire i campi di metadati personalizzati, definiti dall’utente. 

I campi definiti dall’utente possono essere gestiti solo da un amministratore di Media Portal o un amministratore società.

Per aprire questa schermata, fate clic su **Configurazione** &gt; **Impostazione applicazione** &gt; **Metadati** &gt; **Campi definiti dall’utente**.

**Modifica di un campo** Selezionare il campo, quindi fare clic su **Modifica**.

**Eliminazione di un campo** Selezionare il campo, quindi fare clic su **Elimina**.

**Attiva campo** Fare clic per selezionare o deselezionare l'opzione Attivo accanto al nome di un campo. Se rivestite un ruolo di amministratore società, questa opzione potrebbe non essere disponibile. Poiché questa opzione è correlata a Media Portal, per visualizzare i campi di attivazione è necessario selezionare (attivare) Mostra funzioni di Media Portal in Configurazione personale.

## Ottimizzare i file {#optimize-files}

Quando si caricano dei file in Scene7 Publishing System, questi vengono ottimizzati per l’archiviazione e la pubblicazione. Tuttavia, se il processo di caricamento viene interrotto, alcune immagini potrebbero non essere ottimizzate. In questo caso viene visualizzato il messaggio “Immagine non ancora ottimizzata”. Tali file possono comunque essere ottimizzati dagli utenti con ruolo di amministratore.

Scene7 Publishing System analizza i file e ottimizza solo le immagini di cui non è stata completata l’ottimizzazione.

1. Scegliete **Configurazione** &gt; Impostazione **** applicazione, quindi selezionate **Ottimizza file**.
1. Enter information for the optimization job and click **Submit**.

   Se lavorate con più società, ottimizzate separatamente i file appartenenti a società diverse.

## Predefiniti per set di batch {#batch-set-presets}

Usate i predefiniti per set di batch per creare automaticamente set di immagini o set 360 gradi mentre un processo è in esecuzione per caricare delle risorse in Scene7 Publishing System.

Gli amministratori della società definiscono innanzi tutto le convenzioni di denominazione delle risorse che desiderano riunire in un set. Potete quindi creare un predefinito per set di batch che faccia riferimento a tali immagini. Ogni predefinito ha un nome univoco ed è un set autonomo di istruzioni che definisce come comporre il set con le immagini in base alle convenzioni di denominazione specificate con le opzioni del predefinito.

Tutti i predefiniti per set di batch attivi di una società sono riportati nella finestra di dialogo Opzioni processo di caricamento e potete quindi specificare il predefinito da applicare per ogni sessione di caricamento. Per gli amministratori di società vengono visualizzati tutti i predefiniti per set di batch, attivi e inattivi. Quando caricate dei file, Dynamic Media Classic crea automaticamente un set con tutti i file che corrispondono alla convenzione di denominazione definita nei predefiniti attivi.

### Denominazione predefinita {#default-naming}

L’amministratore della società può creare una convenzione di denominazione predefinita, da usare in qualsiasi predefinito per set di batch. Questa impostazione può rappresentare l’unica impostazione effettivamente necessaria per generare i set in batch per tutti i siti Web della società. Per usare la convenzione di denominazione predefinita, è necessario creare un predefinito per set di batch. Per gestire eventuali eccezioni alla denominazione predefinita stabilita per la società, potete creare altri predefiniti per set di batch con convenzioni di denominazione personalizzate, da applicare a particolari set di contenuti.

Benché la configurazione di una convenzione di denominazione predefinita non sia obbligatoria per definire i predefiniti per set di batch, è comunque consigliabile usarla: consente infatti di specificare tutti gli elementi di denominazione che possono essere raggruppati in un set, semplificando così la creazione di set di batch.

1. Fate clic su **Configurazione** &gt; **Impostazione applicazione** &gt; **Predefiniti set di batch** &gt; **Denominazione predefinita**.
1. Selezionate **Visualizza modulo** o **Visualizza codice** per specificare la modalità di visualizzazione e di inserimento delle informazioni relative a ciascun elemento.

   Selezionate la casella di controllo Visualizza codice per visualizzare i valori delle espressioni regolari che vengono generati mano a mano che selezionate le opzioni del modulo. Qualora la visualizzazione modulo presenti delle limitazioni, potete inserire o modificare tali valori per definire meglio gli elementi di denominazione. Se i valori che avete immesso non possono essere analizzati nella visualizzazione modulo, i campi del modulo corrispondenti vengono disattivati.

   >[!NOTE]
   i campi del modulo disattivati non indicano che l’espressione regolare non è valida. Non è disponibile una funzione di convalida delle espressioni regolari generate. I risultati dell’espressione regolare generata verranno visualizzati per ogni elemento dopo la riga Risultato. L’espressione regolare completa è riportata nella parte inferiore della pagina.

1. Espandete ciascun elemento come opportuno e inserite le convenzioni di denominazione da usare.
1. Se necessario, fate clic su **Aggiungi** per aggiungere un’altra convenzione di denominazione a un elemento. Per eliminare la convenzione di denominazione per un elemento, fate clic su **Rimuovi**.
1. Fate clic su **Salva con nome** e specificate il nome del predefinito. Se invece state modificando un predefinito esistente, fate clic su **Salva**.

In alternativa, potete usare l’opzione Visualizza codice, senza campi del modulo. In questa visualizzazione potete creare definizioni complete delle convenzioni di denominazione mediante espressioni regolari.

Per la definizione sono disponibili due elementi, Corrispondenza e Nome base. Questi campi consentono di definire tutti gli elementi di una convenzione di denominazione e identificare la porzione della convenzione usata per denominare il set in cui sono contenuti. Una singola convenzione di denominazione di una società può usare una o più righe di definizione per ognuno di questi elementi. Potete usare tutte le righe necessarie a creare una definizione univoca e raggrupparle in elementi distinti, ad esempio per l’immagine principale, l’elemento colore, l’elemento visualizzazione alternativa e l’elemento campione.

### Creazione di un predefinito per set di batch {#creating-a-batch-set-preset}

Dynamic Media Classic utilizza i predefiniti per set di batch per organizzare le risorse che condividono informazioni o contenuti in set di immagini da visualizzare nei visualizzatori. Le definizioni dei predefiniti per set di batch vengono eseguite automaticamente insieme ai processi di importazione delle risorse programmati in Dynamic Media Classic.

Usate la schermata Predefinito set di batch per creare, modificare e gestire i predefiniti per set di batch. Potete creare tutti i predefiniti per set di batch necessari per i processi di inserimento delle risorse. Sono disponibili due moduli per la definizione dei predefiniti per set di batch: uno per la convenzione di denominazione eventualmente configurata e uno per le convenzioni di denominazione generate al momento.

Potete definire un predefinito per set di batch usando i campi modulo o un codice, per la generazione di espressioni regolari. Come per la denominazione predefinita, potete scegliere di visualizzare il codice mentre inserite le informazioni nel modulo e creare le definizione tramite l’uso di espressioni regolari. In alternativa, potete deselezionare una delle due visualizzazioni e usare solo l’altra.

Consultate anche [Creazione di un predefinito per set di batch per la generazione automatica di un set 360 gradi 2D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**Per creare un predefinito per set di batch**

1. Fate clic su **Configurazione** &gt; **Impostazione applicazione** &gt; **Predefiniti set di batch** &gt; **Predefinito set di batch**. La vista predefinita e **Visualizza modulo**, come impostato nell’angolo in alto a destra della pagina Dettagli.
1. Nel pannello Elenco predefiniti, fate clic su **Aggiungi** per attivare i campi delle definizioni nel pannello Dettagli nella parte destra della schermata.
1. Nel pannello Dettagli, digitate nel campo Nome predefinito il nome da assegnare al predefinito.
1. Selezionate il tipo di predefinito dal menu Tipo set di batch.

   Per generare automaticamente un set 360 gradi, selezionate **Set 360 gradi con asse multiplo** dall’elenco a discesa Tipo set di batch.

1. Effettuate una delle seguenti operazioni:

   * Se usate una convenzione di denominazione predefinita precedentemente impostata in Impostazione applicazione &gt; Predefiniti per set di batch &gt; Denominazione predefinita, espandete **Convenzioni di denominazione delle risorse** e, dall’elenco a discesa Denominazione file, scegliete **Impostazione predefinita**.
   * Per definire una convenzione di denominazione durante l’impostazione del predefinito, espandete **Convenzioni di denominazione delle risorse** e scegliete **Personale** dall’elenco Denominazione file.

1. Per l’ordine della sequenza, definite l’ordine delle immagini dopo che il set è stato raggruppato in Dynamic Media Classic. Per impostazione predefinita le risorse sono elencate in ordine alfabetico. Tuttavia, potete definirne l’ordine utilizzando un elenco separato da virgole delle espressioni regolari.
1. Per Imposta convenzione di denominazione e creazione, specificate il suffisso o il prefisso da aggiungere al nome di base definito nella convenzione di denominazione della risorsa. Definite inoltre la posizione in cui verrà creato il set di immagini nella struttura di cartelle di Dynamic Media Classic.

   Se definite un numero elevato di set di immagini, è consigliabile tenerli separati dalle cartelle contenenti le risorse. Molti clienti creano una cartella con i set di immagini e reindirizzano l’applicazione in modo che memorizzi in tale cartella i set di batch generati.

1. Fate clic su **Salva** nel pannello Dettagli.

### Creazione di un predefinito per set di batch per la generazione automatica di un set 360 gradi 2D {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Potete usare il tipo di set di batch **Set 360 gradi con asse multiplo** per creare una definizione che automatizza la generazione di set 360 gradi 2D. Il raggruppamento delle immagini utilizza espressioni regolari per riga e colonna per il corretto allineamento delle risorse di immagini nella posizione corrispondente nell’array multidimensionale.

Consultate anche [Creazione di un predefinito per set di batch](application-setup.md#creating_a_batch_set_preset).

Per i set 360 gradi 2D non è previsto alcun limite minimo o massimo di righe o colonne.

Ad esempio, supponiamo che dobbiate creare un set 360 gradi con più assi denominato *spin-2dspin*. Disponete di una serie di immagini per set 360 gradi che contengono tre righe con 12 immagini per riga. Le immagini sono denominate come segue:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Con queste informazioni, la definizione per il tipo di set di batch potrebbe essere come segue:

![](assets/se_batch_set_recipe.png)

Il raggruppamento per la parte condivisa del nome delle risorse del set 360 gradi viene aggiunto al campo **Corrispondenza** (evidenziato). La porzione variabile del nome delle risorse contenente la riga e la colonna viene aggiunta rispettivamente ai campi **Riga** e **Colonna**.

Quando il set 360 gradi viene caricato e pubblicato, potete attivare il nome della descrizione set 360 gradi 2D elencato in **Predefiniti per set di batch** nella finestra di dialogo **Opzioni processo di caricamento**.

**Per creare un predefinito per set di batch per la generazione automatica di un set 360 gradi 2D**

1. Scegliete **Configurazione** &gt; **Impostazione applicazione** &gt; **Predefiniti set di batch** &gt; **Predefinito set di batch**. La vista predefinita e **Visualizza modulo**, come impostato nell’angolo in alto a destra della pagina Dettagli.
1. Nel pannello Elenco predefiniti, fate clic su **Aggiungi** per attivare i campi delle definizioni nel pannello Dettagli nella parte destra della schermata.
1. Nel pannello Dettagli, digitate nel campo Nome predefinito il nome da assegnare al predefinito.
1. Selezionate **Set risorse** dal menu a discesa Tipo set di batch.
1. Nell’elenco a discesa Sottotipo, selezionate **Set 360 gradi con asse multiplo**.
1. Espandete **Convenzioni di denominazione delle risorse** e scegliete **Personale** dal menu a discesa Denominazione file.
1. Utilizzate gli attributi **Corrispondenza** e, facoltativamente, **Nome base** per definire un’espressione regolare per la denominazione delle risorse di immagine che compongono il gruppo.

   Esempio di espressione regolare letterale Corrispondenza:

   `(\w+)-\w+-\w+`

1. Espandete **Posizione colonna riga** e definite il formato del nome per la posizione della risorsa di immagine nell’array set 360 gradi 2D.

   Usate le parentesi per racchiudere la posizione di riga o colonna nel nome file.

   Esempio di espressione regolare per riga:

   `\w+-R([0-9]+)-\w+`

   Oppure

   `\w+-(\d+)-\w+`

   Esempio di espressione regolare per colonna:

   `\w+-\w+-C([0-9]+)`

   Oppure

   `\w+-\w+-C(\d+)`

   Tenete presente che questi sono solo esempi. Potete creare le espressioni regolari in base alle vostre esigenze.

   >[!NOTE]
   se la combinazione di espressioni regolari per riga e colonna non è in grado di determinare la posizione della risorsa all’interno dell’array del set 360 gradi multidimensionale, la risorsa non viene aggiunta al set e viene registrato un errore.

1. Per Imposta convenzione di denominazione e creazione, specificate il suffisso o il prefisso da aggiungere al nome di base definito nella convenzione di denominazione della risorsa. Definite inoltre la posizione in cui verrà creato il set di immagini nella struttura di cartelle di Dynamic Media Classic.

   Se definite un numero elevato di set di immagini, è consigliabile tenerli separati dalle cartelle contenenti le risorse. Molti clienti creano una cartella con i set di immagini e reindirizzano l’applicazione in modo che memorizzi in tale cartella i set di batch generati.

1. Fate clic su **Salva** nel pannello Dettagli.
1. Caricate e pubblicate normalmente il set 360 gradi, assicurandovi di attivare il nome del set 360 gradi 2D nella finestra di dialogo Opzioni processo di caricamento, nella sezione Predefiniti per set di batch.

>[!MORELIKETHIS]
* [Anteprima di una risorsa](previewing-asset.md#previewing_an_asset)
* [Configurazione dei predefiniti immagine](setting-image-presets.md#setting_up_image_presets)
* [Visualizzazione, aggiunta ed esportazione di metadati](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
* [Verifica dei file di processo](checking-job-files.md#checking_job_files)

