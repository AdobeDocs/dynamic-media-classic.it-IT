---
title: Creazione di un documento PDF
seo-title: Creazione di un documento PDF
description: 'null'
seo-description: Come creare un documento PDF utilizzando il processo Web-stampa in Dynamic Media Classic.
uuid: 274 fb 06 b -320 b -40 fa -8 b 61-c 224 d 8 aceaa 1
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/template-publishing
discoiquuid: 87 e 91 e 8 e -10 a 2-4 fba -87 c 7-aad 2 bd 798146
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Creazione di un documento PDF {#creating-a-pdf-document}

Il passaggio finale del processo Web-stampa consiste nella generazione del PDF personalizzato. Dopo che l’utente finale ha personalizzato il modello con l’applicazione Web che avete creato, può creare il documento PDF finale. Il PDF finale viene in genere inviato a un provider di servizi di stampa per la stampa professionale. Per garantire la corretta stampa del PDF finale, gli sviluppatori devono usare il file joboptions corretto e impostano correttamente font, indicatori di stampa e colori.

## Configurazione dei predefiniti PDF {#setting-up-pdf-presets}

Per specificare il livello di compatibilità PDF e le impostazioni della stampante, creare e caricare un file joboptions PDF in Dynamic Media Classic Server. Ad esempio, potete scegliere l’output PDF conforme con le specifiche PDF/X-4 (consigliato per flussi di lavoro PDF per la stampa editoriale). Potete creare il file joboptions con il vostro software di authoring (ad esempio, Adobe Illustrator) oppure in Acrobat. Consultate sempre lo stampatore, che potrà consigliarvi le impostazioni di processo corrette il lavoro di stampa in oggetto.

Per ulteriori informazioni sulla creazione di file joboptions e sulla creazione di un file joboptions in Acrobat, consultate la guida di Adobe Acrobat.

Per creare un file joboptions in Illustrator:

1. Scegliete Modifica &gt; Predefiniti Adobe PDF.
1. Nella finestra di dialogo, selezionate il predefinito che desiderate usare.

   Le seguenti impostazioni Opzioni processo sono supportate da Dynamic Media Classic:

   | Opzione processo | Descrizione |
   |--- |--- |
   | Generali | <ul><li>Compatibilità </li><li>Compressione a livello di oggetto</li><li>Miniature incorporate</li><li>Ottimizzazione per accesso rapido sul Web</li></ul> |
   | Immagini | <ul><li>Downsampling</li><li>Risoluzione</li><li>Soglia</li><li>Compressione per colore, grigio e mono</li></ul> |
   | Font | <ul><li>Incorporazione di tutti i font (i font vengono incorporati per impostazione predefinita)</li><li>Incorporazione dei font OpenType</li><li>Creazione di sottoinsiemi di font incorporati quando la percentuale di caratteri usati è minore di un determinato valore</li><li>Elenco dei font da incorporare sempre</li><li>Elenco dei font da non incorporare mai</li></ul> |
   | Colore | <ul><li>Strategia colore (Tag per sole immagini viene trattato come Tag per tutto)</li><li>Intento di rendering del documento</li><li>Per 4.2.5 sono supportati solo i seguenti spazi di lavoro. 4.3 consentirà di usare anche eventuali profili caricati dall’utente in IPS.</li><li>Per ovviare a questo limite, potete specificare lo spazio colore di destinazione per la grafica da convertire mediante i profili colore predefiniti per la società.</li></ul> |
   | RGB | <ul><li>e-sRGB </li><li>scRGB with encoding range [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>Flat XYZ</li><li>ROMM-RGB lineare</li><li>ROMM-RGB</li><li>sYCC a 8 bit</li><li>e-sYCC a 8 bit</li></ul> |
   | Grigio | <ul><li>Grigio gamma 1,8</li><li>Grigio gamma 2,2</li><li>Ingrossamento punti 10%</li><li>Ingrossamento punti 15%</li><li>Ingrossamento punti 20%</li><li>Ingrossamento punti 25%</li><li>Ingrossamento punti 30%</li><li>sGray</li></ul> |
   | Mantenimento dei valori CMYK per spazi colore CMYK calibrati |  |
   | Avanzate | Mantenimento dei commenti OPI sempre attivo |
   | Standard | Standard di conformità |

   >[!NOTE]
   >
   >Dynamic Media Classic ignora le impostazioni dei segni di stampa nel file joboptions. Gli indicatori di stampa sono invece configurati mediante l'uso di comandi URL Classic Classic.

1. Fate clic su Esporta, specificate nome e percorso e fate clic su Salva.
1. Caricate il file joboptions come una risorsa in Scene7 Publishing System.

   Utilizzate il file joboptions con il modello pubblicato inserendo i relativi riferimenti nell’URL. Ad esempio:

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## Preparazione del PDF per la stampa {#preparing-the-pdf-for-print}

Prima di finalizzare il PDF per la stampa, seguite le linee guida riportate in questa sezione.

**Immagini**

Accertatevi che tutte le immagini del processo di pubblicazione siano state caricate sul server Dynamic Media Classic e pubblicate.

**Font**

Accertatevi che tutti i font nel processo di pubblicazione siano stati caricati in Dynamic Media Server e pubblicati. Accertatevi di disporre dei diritti legali per l’hosting dei font, se intendete consentire agli utenti finali di modificarli.

**Risoluzione delle immagini (pixel per pollice)**

La risoluzione delle immagini bitmap viene mantenuta dal server Dynamic Media Classic nei PDF generati pronti per la stampa. Se necessario, Media Classic viene ridimensionata in scala di immagini. Per risultati ottimali, lasciate la risoluzione impostata con il valore predefinito (in genere 72 dpi) per l’anteprima sul Web. La risoluzione predefinita per tutte le immagini della società viene impostata nella finestra Impostazioni di pubblicazione di Image Server nella sezione Risoluzione predefinita di stampa. Valori di risoluzione elevati (ad esempio, 300 dpi) possono comportare tempi di elaborazione lunghi e devono essere usati solo per i PDF destinati alla stampa. Usate il comando imageRes= nell’URL per ignorare manualmente la risoluzione predefinita per i processi PDF.

**Gestione colore**

Il documento e le immagini possono usare i modelli di colore scala di grigio, CMYK, tinte piatte denominate, RGB o Lab, che possono essere non calibrati oppure calibrati mediante un profilo colore ICC. Per risultati ottimali, incorporate il profilo nel file PDF generato pronto per la stampa, Per impostazione predefinita, il server Dynamic Media Classic esegue questa operazione. Accertatevi che tutti i profili colore richiesti siano stati caricati nella piattaforma Dynamic Media Classic. Preferibilmente, accertatevi che le opzioni di gestione del colore impostate nell'applicazione grafica corrispondano a quelle impostate in Dynamic Media Classic Server:

**Impostazioni di gestione del colore impostate nell’applicazione grafica:** nelle impostazioni colore dell’applicazione grafica (ad esempio in Adobe Illustrator), specificate i profili colore RGB e CMYK nella sezione degli spazi di lavoro.

**Impostazioni di gestione colore Dynamic Media Classic:** In genere, le impostazioni di gestione del colore nell'applicazione grafica devono corrispondere ai profili colore predefiniti nel server Dynamic Media Classic. Le impostazioni si trovano nella finestra Impostazione pubblicazione/Image Server.

## Visualizzazione degli indicatori di stampa {#displaying-printer-marks}

Potete creare un PDF per uno dei seguenti casi:

* Documento finito
* Documento intermedio, ad esempio una pellicola o lastra da inviare a uno stampatore per la produzione

Un documento intermedio può contenere alcune caratteristiche aggiuntive necessarie per la produzione, ad esempio margini di pagina al vivo, indicatori di stampa e così via. Queste vengono solitamente visualizzate al di fuori dei limiti della pagina finita.

Sono supportati tutti gli indicatori disponibili nella schermata “Aggiungi indicatori di stampa” di Acrobat. Gli indicatori di stampa sono controllati dal parametro `printerMark`. È richiesta la seguente sintassi `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`.

* indicatori di rifilo = 0|1
* indicatori di pagina al vivo = 0|1
* crocini di registro = 0|1
* barre colori = 0|1
* informazioni pagina = 0|1
* stile = Illustrator | IllustratorJ | QuarkXPress
* spessore linea = 0.125 | 0.25 | 0.50
* incorpora in livello = 0|1

Quando si prepara un documento per la produzione di stampe, potrebbe essere necessario inserire degli indicatori di stampa con cui il service possa allineare le pellicole delle selezioni colore per la produzione di prove colore, misurare la pellicola per la corretta calibrazione e la densità degli inchiostri, rifilare le pellicole alle dimensioni desiderate e così via. Gli indicatori di stampa indicano i limiti del documento, come ad esempio i limiti di rifilo e di pagina al vivo. I contenuti per la produzione possono includere:

**Casella** File multimediali I limiti del supporto fisico su cui verrà stampata la pagina. Eventuali contenuti all’esterno del riquadro MediaBox possono essere eliminati senza alterare i contenuti del documento finale.

**Casella** al vivo L'area in cui viene ritagliato il contenuto della pagina in un ambiente di produzione. In questa area può rientrare lo spazio necessario in base alle limitazioni fisiche dei dispositivi di taglio, piega e rifilo. Il valore predefinito corrisponde al riquadro di ritaglio della pagina.

**Trimbox Le** dimensioni desiderate per la pagina finale dopo il rifilo. Il limite di rifilo può essere più piccolo del limite del supporto, per consentire la stampa di contenuti necessari alla produzione quali istruzioni di stampa, indicatori di taglio e barre dei colori. Il valore predefinito corrisponde al riquadro di ritaglio della pagina.

**Casella** grafica L'estensione del contenuto significativo della pagina (inclusa l'eventuale spazio bianco) come previsto dall'autore della pagina. Il valore predefinito corrisponde al riquadro di ritaglio della pagina.

Per riprodurre gli indicatori di stampa disponibili in Adobe Illustrator, InDesign e Acrobat, potete usare i modificatori riportati in questa tabella:

| Modificatore/Valori | Descrizione |
|--- |--- |
| bleedMargin=top,left,bottom,right | Specificato in Acrobat con l’opzione di impostazione dei riquadri di pagina. Selezionate BleedBox, quindi specificate i margini mediante l’opzione Controlli margine.<br><br>I valori rappresentano la distanza dai bordi superiore, sinistro, inferiore e destro rispetto ai bordi originali della grafica (il limite del supporto), verso l’interno. I valori (0-1000) sono espressi in punti.<br><br>Nuova altezza = altezza originale - (margine superiore + margine inferiore)<br><br>Nuova larghezza = larghezza originale - (sinistra + destra) |
| mediaMargin=top,left,bottom,right | Specificato in Acrobat con l’opzione di impostazione dei riquadri di pagina. Modificate le dimensioni di pagina personalizzate, per l’opzione Modifica dimensioni pagina.<br><br>I valori rappresentano la distanza dai bordi superiore, sinistro, inferiore e destro rispetto ai bordi originali della grafica (il limite del supporto), verso l’esterno. I valori (0-1000) sono espressi in punti.<br><br>Nuova altezza = margine superiore + margine inferiore + heightnuovo<br><br>larghezza = Larghezza superiore + margine inferiore + widget:<br><br>i nuovi valori di altezza e larghezza determinano le nuove dimensioni della pagina del PDF generato.<br><br>Una volta definito il nuovo riquadro MediaBox, tutti i calcoli per i margini di ritaglio e di pagina al vivo devono considerare come bordo della grafica il nuovo riquadro MediaBox. |
| trimMargin=top,left,bottom,right | Specificato in Acrobat con l’opzione di impostazione dei riquadri di pagina. Selezionate TrimBox, quindi specificate i margini mediante l’opzione Controlli margine.<br><br>I valori rappresentano la distanza dai bordi superiore, sinistro, inferiore e destro rispetto ai bordi originali della grafica (il limite del supporto), verso l’interno. I valori (0-1000) sono espressi in punti.<br><br>Nuova altezza = altezza originale - (margine superiore + margine inferiore)<br><br>Nuova larghezza = larghezza originale - (sinistra + destra) |
| printerMark= indicatori di rifilo, indicatori pagina al vivo, crocini di registro, barre colori, informazioni pagina, stile, spessore linea, incorpora in livello | I valori sono i seguenti:<br><br>indicatori di rifilo = 0,1 (il valore predefinito è 0)<br><br>indicatori pagina al vivo = 0,1 (il valore predefinito è 0)<br><br>crocini di registro = 0,1 (<br><br>il valore predefinito è 0) bars bars = 0,1 (predefinito è 0)<br><br>le informazioni di pagina = 0,1 (predefinito è 0)<br><br>, quelle predefinite = 1 (impostazione predefinita: 0.25) Stile =<br><br>Valore predefinito: 2 (impostazione predefinita:) Stile = Valore predefinito: Spessore riga; il valore predefinito è.<br><br>incorpora in livello = 0, 1, con 1 creazione di un nuovo livello contenente tutti gli indicatori di stampa (il valore predefinito è 1)<br><br>a seconda dello stile utilizzato, gli indicatori e le barre di colore appaiono diversi e corrispondono ai relativi stili usati da Acrobat. |

Note sugli indicatori di stampa:

* Quando specificate gli indicatori di stampa, specificate i margini di pagina al vivo, di rifilo e del supporto mediante chiamate URL. Se si specificano gli indicatori di stampa senza specificare questi margini, gli indicatori di stampa cadranno al di fuori dell’area visibile del file PDF generato. Inoltre, gli indicatori di rifilo e di pagina al vivo si sovrapporranno.
* Se si specificano gli stessi valori di margine per il margine di rifilo e quello della pagina al vivo, gli indicatori di rifilo e di pagina al vivo si sovrappongono se entrambi i flag sono impostati su 1 in `&printerMark`.
* Se si specifica fmt=formati swf/immagine tramite chiamate URL, nell’output non saranno presenti indicatori di stampa o margini perché questa funzione è specifica per l’output PDF.
* Specifying `&printerMark=`through the URL results in default values being used for all parameters. Specifying `&printerMark=1` results in trim marks being set to 1 and default values for other parameters. Tuttavia, per impostare l’ennesimo elemento su Attivato, è necessario specificare nell’URL anche tutti i parametri precedenti (n-1).
* Specifying only one value for `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in that value being applied to all the top, bottom, left, and right margins of the original artwork.
* Specifying only the top and left values through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the top value being assigned to the bottom value and the left value being equal to the right.
* Not specifying the right value through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the left value being assigned to the right.
* Per un PDF con più pagine, gli indicatori di stampa o i margini vengono applicati a tutte le pagine (in Acrobat, gli utenti possono selezionare degli intervalli di pagine per gli indicatori di stampa o i margini).
* L’output di un file PDF con indicatori di stampa o margini corrisponde esattamente a quello di Acrobat X, a meno che non venga specificato diversamente.

Se intendete creare un file PDF conforme con PDF/X-4 utilizzando il modificatore &amp;joboption nell’URL, tenete presente i limiti relativi agli indicatori di stampa specificati nel documento ISO_15930-7-2008.pdf:

* Ogni oggetto Page di un file PDF deve includere i parametri MediaBox. Ogni oggetto Page in un file conforme con PDF/X-4 deve includere parametri TrimBox o ArtBox, ma non entrambi. Il riquadro MediaBox può essere ereditato.
* Se è presente un riquadro BleedBox, il riquadro ArtBox o TrimBox non può estendersi oltre i limiti del riquadro BleedBox. Se è presente un riquadro CropBox, i riquadri ArtBox, TrimBox o BleedBox non possono estendersi oltre i limiti del riquadro CropBox.
* I riquadri ArtBox, TrimBox, CropBox o BleedBox devono estendersi oltre i limiti del riquadro MediaBox.
* In alcuni settori l’inclusione di riquadri BleedBox è obbligatoria. Seguite sempre le linee guida degli specifici settori.
* Si consiglia di usare il riquadro TrimBox anziché ArtBox.
* Tutte le annotazioni diverse da TrapNet e PrinterMark devono disporre di un valore Rect tale da essere completamente all’esterno del riquadro BleedBox (oppure TrimBox o ArtBox, in assenza di BleedBox). Tutte le annotazioni PrinterMark devono disporre di un valore Rect tale da essere completamente all’esterno del riquadro TrimBox o ArtBox. Un lettore conforme con le specifiche PDF/X-4 potrebbe ignorare completamente le annotazioni eccetto le annotazioni PDF TrapNet.
* Un parametro Rect viene considerato completamente all’esterno di un riquadro se tutte le sue coordinate si trovano all’esterno del riquadro o sul suo bordo e se l’intersezione dei due rettangoli è pari a zero.
* Se il dizionario ViewerPreferences contiene le chiavi ViewArea, ViewClip, PrintArea o PrintClip, ciascuna di queste deve disporre di un valore MediaBox oppure (se è presente un riquadro BleedBox in tutti gli oggetti Page del file) BleedBox.

