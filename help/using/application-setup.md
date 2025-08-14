---
title: Impostazione applicazione
description: Scopri come impostare e configurare l’area Applicazione di Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
topic: Administration
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '10899'
ht-degree: 29%

---

# Impostazione applicazione{#application-setup}

È possibile utilizzare le pagine Impostazione applicazione per immettere Impostazioni generali, creare predefiniti immagine, predefiniti codifica video, predefiniti visualizzatore o definire visualizzatori predefiniti e metadati. Puoi impostare i predefiniti per set di batch in modo che automatizzino la generazione di set 360 gradi 2D (ad esempio), le impostazioni di pubblicazione e le impostazioni Video SEO (Search Engine Optimization).

>[!NOTE]
>
>Solo gli amministratori di Adobe Dynamic Media Classic possono modificare le impostazioni in Impostazione applicazione.

## Impostazioni generali {#general-settings}

Per aprire la pagina Impostazioni generali applicazione, nella barra di navigazione globale passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Impostazioni generali]**.

### Server

Al momento della creazione dell’account, Adobe Dynamic Media Classic fornisce automaticamente i server assegnati alla tua azienda. Questi server vengono utilizzati per creare stringhe URL per il sito Web e le applicazioni. Tali chiamate URL sono specifiche dell’account utente.

Vedere anche [Test del servizio di test protetto](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL Nome server pubblicato]**: questo server è il server Live CDN (Content Deliver Network) utilizzato in tutte le chiamate URL generate dal sistema e specifiche per il tuo account. Modificare il nome del server solo se un tecnico del supporto tecnico Adobe Dynamic Media Classic ti ha richiesto di farlo.

* **[!UICONTROL Nome server di origine]**: questo server viene utilizzato solo per i test di controllo qualità. Modificare il nome del server solo se un tecnico del supporto tecnico Adobe Dynamic Media Classic ti ha richiesto di farlo.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Nome server Test&amp;Target]**: URL di Test&amp;Target, incluso `.com`. Per istruzioni su come ottenere questo URL, vedere Integrazione di [!DNL Adobe Dynamic Media Classic] con [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL Nome server di streaming iOS]**: l&#39;URL del server di streaming iOS [!DNL Adobe Dynamic Media Classic]. Questo server distribuisce video in streaming a dispositivi basati su iOS utilizzando il protocollo HTTP.

* **[!UICONTROL Nome server video progressivo]**: l&#39;URL del server video progressivo [!DNL Adobe Dynamic Media Classic]. Questo server distribuisce video progressivi utilizzando il protocollo HTTP.

* **[!UICONTROL Mostra URL per risorse non pubblicate]**: seleziona questa opzione se vuoi che [!DNL Adobe Dynamic Media Classic] visualizzi un URL quando visualizzi l&#39;anteprima di una risorsa, pubblicata o meno. Se la risorsa non è pubblicata, l’URL non funziona. Tuttavia, potete utilizzare l’URL a scopo di progettazione o organizzazione.

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the Web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL Modello di annullamento validità CDN]**: specifica il modello utilizzato per annullare la validità della cache CDN (Content Delivery Network).

  Si supponga, ad esempio, di immettere un URL immagine (inclusi predefiniti o modificatori immagine) che fa riferimento a `<ID>`, anziché un ID immagine specifico come nell&#39;esempio seguente:

  `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

  Se il modello contiene solo `<ID>`, Adobe Dynamic Media Classic compila `https://<server>/is/image`, dove `<server>` è il nome del server di pubblicazione definito in Impostazioni generali.

  Se si imposta il modello di annullamento validità CDN, selezionare un&#39;immagine denominata Backpack_B, quindi passare a **[!UICONTROL File]** > **[!UICONTROL Annulla validità CDN]**, nell&#39;interfaccia di annullamento validità CDN verrà restituito il seguente URL generato:

  `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

  Nella casella di riepilogo URL, seleziona **[!UICONTROL Continua]** per cancellare la cache per quella chiamata URL immagine specifica. È inoltre possibile aggiungere URL digitandoli o incollandoli nella casella di riepilogo URL, senza dover impostare il modello in precedenza.

  Dopo aver selezionato il modello di annullamento validità CDN e aver effettuato una richiesta di annullamento validità CDN, nell’interfaccia utente viene visualizzato un indicatore. Fornisce una stima del tempo necessario per cancellare la cache.

  Quando fai clic su **[!UICONTROL File]** > **[!UICONTROL Annulla validità CDN]**, nell&#39;URL del modello salvato viene fatto riferimento a ogni immagine se in Dynamic Media Classic sono selezionate più immagini. Pertanto, puoi definire un Modello di annullamento validità CDN facendo riferimento a ciascun URL a cui viene fatto riferimento nel sito web (ad esempio i dettagli del prodotto e i risultati della ricerca). Quindi, quando selezioni una o più immagini per l’annullamento della validità dalla cache, gli URL compilano automaticamente l’interfaccia.

  Consultate [Memorizzazione dei contenuti nella cache](dmc-platform-overview.md#content_caching).

  Consultate [Risorse ripubblicate e ritardi CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Sfoglia

* **[!UICONTROL Mostra progetti]**: determina se i progetti sono disponibili per organizzare le risorse di Adobe Dynamic Media Classic. Consulta [Organizzare il lavoro con i progetti](/help/using/organizing-projects.md).

* **[!UICONTROL Mostra contenuto eVideo di esempio]**: attiva o disattiva la visualizzazione del contenuto di esempio eVideo.

* **[!UICONTROL Mostra contenuto generato]**: nelle cartelle viene visualizzato il contenuto generato da una risorsa. Ad esempio, quando un file PDF viene rasterizzato durante il caricamento, Adobe Dynamic Media Classic crea un&#39;immagine per ogni pagina del PDF originale. Se è selezionata l&#39;opzione Mostra contenuto generato, viene visualizzata ogni immagine generata al caricamento del PDF originale. Viene visualizzato insieme al PDF nella cartella in cui è stato caricato PDF.

* **[!UICONTROL Mostra video codificati]**: disattivato per impostazione predefinita.

  Puoi cercare e sfogliare rapidamente i video in Adobe Dynamic Media Classic senza dover navigare attraverso numerosi derivati codificati dello stesso video. Lascia deselezionata questa opzione (impostazione predefinita). Vengono visualizzate solo la miniatura del video principale (il video sorgente caricato e utilizzato per creare i derivati) e la miniatura del set video adattivo &quot;principale&quot; (che contiene i derivati &quot;secondari&quot; del set video codificato).

  È comunque possibile accedere ai singoli video codificati dal video principale o dal set di video adattivi. A questo scopo, fate doppio clic sulla miniatura del video per aprire la visualizzazione Dettagli. Quindi seleziona **[!UICONTROL Video codificati]** nel pannello a destra per accedere a tutti i video &quot;secondari&quot;.

  Puoi anche passare a **[!UICONTROL File]** > **[!UICONTROL Rielabora]** per creare altri video &quot;secondari&quot; codificati direttamente da un set di video adattivi. Adobe Dynamic Media Classic trova automaticamente il video principale &quot;principale&quot; del set di video adattivi e lo utilizza come video sorgente per la transcodifica. Quando salvate i nuovi video codificati, tuttavia, questi non vengono visti nelle operazioni di ricerca o navigazione. Sono comunque accessibili dalla scheda Video codificati in visualizzazione Dettagli.

  Vedi [Caricare e transcodificare video](uploading-encoding-videos.md#uploading_and_encoding_videos).

  Per poter accedere a tutte le versioni derivate codificate durante la ricerca e la navigazione, selezionate **[!UICONTROL Mostra video codificati]**.

  Alcune azioni nel menu Genera funzionano solo o eventualmente con singoli video. Questa funzionalità rende necessaria la visualizzazione di tutte le versioni derivate di video codificati disponibili per la selezione, a prescindere dall’impostazione di **[!UICONTROL Mostra video codificati]**. Le azioni di compilazione che superano l&#39;impostazione **[!UICONTROL Mostra video codificati]** includono **[!UICONTROL set di video adattivi]** e **[!UICONTROL eCatalog]**.

  >[!NOTE]
  >
  >Se non hai utilizzato Adobe Dynamic Media Classic per caricare e codificare le risorse video, Adobe Dynamic Media Classic mostra tutti i singoli video codificati, anche se questa opzione è deselezionata.

* **[!UICONTROL Pulsante Aggiorna sottocartelle]**: attiva o disattiva la visualizzazione del pulsante Aggiorna sottocartelle.

### Account FTP Adobe Dynamic Media Classic

* **[!UICONTROL Server]**: elenca il server dell&#39;account FTP.

* **[!UICONTROL Nome utente]**: elenca il nome utente dell&#39;account FTP.

### Carica nell’applicazione

Vedi anche il video di formazione [Opzioni per processi di caricamento](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS).

* **[!UICONTROL Sovrascrivi immagini]**: Adobe Dynamic Media Classic non consente a due file di avere lo stesso nome. L&#39;ID Adobe Dynamic Media Classic di ogni elemento (il nome immagine meno l&#39;estensione del nome file) deve essere univoco. In virtù di questa regola, nella finestra di dialogo Carica è disponibile l’opzione Sovrascrivi. Il risultato effettivo di questa opzione dipende dal valore impostato per l’opzione Sovrascrivi immagini. È possibile specificare come caricare le immagini sostitutive, ossia se devono sostituire le immagini originali o diventare duplicati di tali immagini. Le immagini duplicate vengono rinominate con un &quot;-1&quot; (ad esempio, chair.tif viene rinominato chair-1.tif). Queste opzioni interessano le immagini caricate in una cartella diversa da quella degli originali o le immagini con una diversa estensione file (ad esempio, JPG, TIF o PNG). Vedere [Utilizzare l&#39;opzione Sovrascrivi immagini](#using-the-overwrite-images-option).

   * **[!UICONTROL Sovrascrivi nella cartella corrente, nome immagine di base o estensione uguali]**: questa opzione è la regola più rigorosa per la sostituzione. Richiede che l’immagine sostitutiva sia caricata nella stessa cartella dell’immagine originale e che abbia la stessa estensione del nome file dell’originale. Se entrambi i requisiti non vengono soddisfatti, viene creata una copia dell’immagine.

   * **[!UICONTROL Sovrascrivi nella cartella corrente, nome come risorsa base, indipendentemente dall&#39;estensione]**: richiede che l&#39;immagine sostitutiva venga caricata nella stessa cartella dell&#39;originale, ma l&#39;estensione del nome file può essere diversa dall&#39;originale. Ad esempio, sedia.tif sostituisce sedia.jpg.

   * **[!UICONTROL Sovrascrivi in qualsiasi cartella, nome risorsa base o estensione]**: richiede che l&#39;immagine sostitutiva abbia la stessa estensione del nome file dell&#39;immagine originale. Ad esempio, chair.jpg deve sostituire chair.jpg, non chair.tif). Tuttavia, è possibile caricare l’immagine sostitutiva in una cartella diversa da quella dell’originale. L’immagine aggiornata sarà contenuta nella nuova cartella e il file verrà rimosso dal percorso originale.

   * **[!UICONTROL Sovrascrivi in qualsiasi cartella, nome come risorsa base, indipendentemente dall&#39;estensione]**: questa opzione è la regola di sostituzione più inclusiva. L’immagine sostitutiva può essere caricata in una cartella diversa da quella dell’originale, con una diversa estensione file, e sostituire il file originale. Se il file originale si trova in un’altra cartella, l’immagine sostitutiva sarà contenuta nella nuova cartella nella quale è stata caricata.

* **[!UICONTROL Mantieni pubblicazione]**: specifica se un&#39;immagine sostitutiva caricata in Adobe Dynamic Media Classic mantiene l&#39;impostazione Pronto per la pubblicazione dell&#39;immagine da sostituire. Oppure, l’impostazione viene specificata al momento del caricamento.

* **[!UICONTROL Profili colore predefiniti]**: specifica i profili colore applicati come parte delle opzioni dei profili colore predefiniti quando si aggiungono immagini CMYK.

* **[!UICONTROL Opzioni di caricamento predefinite]**: apre la finestra di dialogo Opzioni processo di caricamento, in cui è possibile specificare le opzioni di caricamento predefinite. Per informazioni su queste opzioni, consultate [Opzioni di caricamento](/help/using/uploading-files.md#upload_options).

### Editor mappa immagine (su applicazione)

* **[!UICONTROL Mappatura immagine predefinita HREF]**: definisce l&#39;URL predefinito utilizzato per la colonna HREF nella mappatura immagine. Questo URL è l&#39;URL predefinito visualizzato quando crei mappe immagine.

* **[!UICONTROL Modello mappatura immagine predefinito]**: definisce il JavaScript predefinito per il modello HREF nella mappatura immagine. Puoi impostare un codice personalizzato da eseguire ogni volta che selezioni una mappa immagine.

### Altre impostazioni (su applicazione)

* **[!UICONTROL Avvertenze per la pulizia del cestino]**: Assets nel cestino viene rimosso automaticamente entro sette giorni. Seleziona &quot;Invia e-mail prima dell’eliminazione automatica degli elementi dal cestino&quot; per inviare notifiche agli amministratori della società quando le risorse presenti nel cestino sono a quattro giorni dall’eliminazione definitiva. Vedi [Gestione cartella cestino](/help/using/trash-folder.md).

## Utilizzare l’opzione Sovrascrivi immagini {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic non consente a due file di avere lo stesso nome. L&#39;ID Adobe Dynamic Media Classic di ogni elemento (il nome immagine meno l&#39;estensione del nome file) deve essere univoco. In virtù di questa regola, nella finestra di dialogo Carica è disponibile l’opzione Sovrascrivi immagini. L’effetto esatto di questa opzione dipende da un’impostazione per le impostazioni interne di Adobe Dynamic Media Classic di ogni azienda.

Se in precedenza avete caricato le immagini e quindi modificato i file originali (o li avete sostituiti), l&#39;opzione di sovrascrittura selezionata specifica in che modo Adobe Dynamic Media Classic sostituisce le immagini. I dati relativi all’immagine non vengono modificati, ma la nuova immagine sostituisce la precedente. Se la cartella contiene anche immagini che non sono già presenti in Adobe Dynamic Media Classic, queste immagini vengono aggiunte.

Utilizza questa opzione se le immagini caricate sono cambiate in qualche modo (l’immagine è stata modificata) ma il riferimento all’immagine rimane lo stesso. La sovrascrittura è utile anche per il caricamento e la copia da CD di Adobe®. Puoi ottimizzare il modo in cui Adobe Dynamic Media Classic *copia* l&#39;immagine. Potete anche regolare le opzioni del profilo colore ICC nella finestra di dialogo Carica (Upload) e ricaricarle utilizzando la funzione di sovrascrittura.

Gli ID Adobe Dynamic Media Classic utilizzati per accedere alle immagini dai server di produzione derivano dai nomi dei file immagine. L’utilizzo di caratteri maiuscoli e minuscoli nel nome del file è importante, sia per la sostituzione dei file esistenti che per gli ID Adobe Dynamic Media Classic utilizzati per accedere all’immagine. L’utilizzo di nomi di file con caratteri maiuscoli e minuscoli è corretto prima del caricamento in Adobe Dynamic Media Classic per evitare Adobe Dynamic Media Classic ID che differiscono solo per la stessa immagine.

Se deselezionate questa opzione, tutte le immagini con lo stesso nome file delle immagini esistenti vengono considerate copie e non vengono aggiunte.

## Predefiniti immagine {#image-presets}

Nella schermata Predefiniti immagine è possibile creare e modificare i predefiniti per le immagini. I predefiniti per immagini consentono a Adobe Dynamic Media Classic di distribuire immagini in modo dinamico a dimensioni diverse dalla stessa immagine principale. Ogni predefinito immagine rappresenta una raccolta predefinita di comandi di ridimensionamento e formattazione per la visualizzazione delle immagini. Quando crei un predefinito immagine, selezioni una dimensione per la consegna delle immagini. È inoltre possibile selezionare i comandi di formattazione per ottimizzare l&#39;aspetto dell&#39;immagine quando questa viene distribuita per la visualizzazione.

Gli amministratori possono creare predefiniti per l’esportazione delle risorse. Gli utenti possono scegliere un predefinito al momento dell&#39;esportazione delle immagini, che consente anche di riformattarle in base alle specifiche specificate dall&#39;amministratore.

Per aprire la schermata Predefinito immagine, sulla barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**.

Consulta [Smart imaging](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

### Creare e modificare i predefiniti immagine {#creating-and-editing-image-presets}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**.
1. Crea un predefinito o inizia da uno esistente:

   * **Crea un predefinito immagine**: seleziona **[!UICONTROL Aggiungi]**.
   * **Crea un predefinito immagine da un predefinito esistente**: seleziona il predefinito immagine più simile a quello che desideri creare, quindi seleziona **[!UICONTROL Modifica]**.

1. Nella pagina Aggiungi (o Modifica) predefinito, inserisci un nome per il predefinito.
1. Impostate le opzioni desiderate. 

   Consultate [Opzioni dei predefiniti immagine](application-setup.md#image_preset_options).

1. Seleziona **[!UICONTROL Salva]** oppure, se hai iniziato da un predefinito esistente, seleziona **[!UICONTROL Salva con nome]**.
1. Per visualizzare in anteprima il predefinito con la tua immagine, seleziona **[!UICONTROL Sfoglia]**, quindi seleziona un&#39;immagine. Per visualizzare l&#39;anteprima con l&#39;immagine predefinita, selezionare **[!UICONTROL Reimposta]**.

È possibile modificare un predefinito immagine selezionandone il nome nella schermata Predefiniti immagine e selezionando **[!UICONTROL Modifica]**. Per eliminare un predefinito immagine, selezionarlo, quindi selezionare **[!UICONTROL Elimina]**.

### Opzioni dei predefiniti immagine {#image-preset-options}

Nelle schermate Aggiungi predefinito e Modifica predefinito sono disponibili le seguenti opzioni per creare e modificare i predefiniti immagine:

* **[!UICONTROL Nome predefinito]**: immettere un nome descrittivo senza spazi vuoti. Per aiutare gli utenti a identificare questo predefinito immagine, includi nel nome la specifica della dimensione dell’immagine.

* **[!UICONTROL Larghezza e altezza]**: immetti la dimensione in pixel dell&#39;immagine trasmessa.

* **[!UICONTROL Formato]**: selezionare un formato dal menu. La scelta del formato GIF, JPEG, PDF o TIFF offre più opzioni:

   * Opzioni Quantizzazione colore GIF

      * **[!UICONTROL Tipo]**: selezionare Adattivo (impostazione predefinita), Web o Mac. Se si seleziona **[!UICONTROL GIF With Alpha]**, l&#39;opzione Mac non è disponibile.

      * **[!UICONTROL Dithering]**: Selezionare Diffondi o Disattivato.

      * **[!UICONTROL Numero di colori]**: trascina il cursore per immettere 2-255.

      * **[!UICONTROL Elenco colori]**: immettere un elenco separato da virgole. Ad esempio, per bianco, grigio e nero, immettere `000000,888888,ffffff`.

   * Opzioni JPEG

      * **[!UICONTROL Qualità]**: controlla il livello di compressione di JPEG. Questa impostazione interessa sia le dimensioni del file che la qualità dell’immagine. La scala per la qualità dei file JPEG va da 1 a 100.

      * **[!UICONTROL Attiva downsampling crominanza JPG]**: poiché l&#39;occhio è meno sensibile alle informazioni di colore ad alta frequenza rispetto alla luminanza ad alta frequenza, le immagini JPEG dividono le informazioni dell&#39;immagine in componenti di luminanza e colore. Quando un’immagine JPEG viene compressa, il componente della luminanza viene lasciato alla massima risoluzione, mentre per i componenti colore viene eseguito il downsampling calcolando la media di gruppi di pixel. Il downsampling riduce il volume dei dati della metà o di un terzo senza alcun impatto sulla qualità percepita. Non è possibile eseguire il downsampling sulle immagini in scala di grigio. Questa tecnica riduce il fattore di compressione ed è utile per le immagini ad alto contrasto (ad esempio, immagini con testo sovrapposto).

   * Opzioni PDF e TIFF

      * **[!UICONTROL Compressione]**: selezionare un algoritmo di compressione.

* **[!UICONTROL Spazio colore]**: selezionare uno spazio colore.

* **[!UICONTROL Nitidezza]**: selezionare l&#39;opzione Attiva nitidezza semplice per applicare un filtro di nitidezza di base all&#39;immagine dopo il ridimensionamento. La nitidezza contribuisce a compensare la sfocatura che può prodursi quando si visualizza un’immagine in dimensioni diverse.

  Per ulteriori informazioni sulla nitidezza, sulle modalità di ricampionamento e sulla maschera di contrasto, vedere [Contrassegnare un&#39;immagine](sharpening-image.md#sharpening_an_image). Vedi anche il video di formazione [Nitidezza](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS).

* **[!UICONTROL Modalità ricampionamento]**: selezionare un&#39;opzione per la modalità ricampionamento. Queste opzioni aumentano la nitidezza quando si esegue il downsampling dell’immagine:

* **[!UICONTROL B-Lineare]**: metodo di ricampionamento più veloce. Alcuni artefatti di aliasing sono visibili.

* **[!UICONTROL Bicubico]**: aumenta l&#39;utilizzo di CPU nel server immagini, ma genera immagini più nitide con artefatti di alias meno evidenti.

* **[!UICONTROL `Sharp 2`]**: può produrre risultati leggermente più nitidi rispetto all&#39;opzione Bicubico, ma a un costo CPU ancora più elevato sul server immagini.

* **[!UICONTROL Trilineare]**: utilizza risoluzioni più alte e più basse, se disponibili; consigliato solo quando l&#39;alias è un problema. Questo metodo riduce le dimensioni JPEG grazie a una minore quantità di dati ad alta frequenza.

* **[!UICONTROL Maschera di contrasto]**: scegli queste opzioni per ottimizzare la nitidezza:

* **[!UICONTROL Importo]**: controlla la quantità di contrasto applicata ai pixel del bordo. Il valore predefinito è 1,0. Per le immagini ad alta risoluzione, è possibile aumentare questo valore fino a 5,0. Il fattore può essere interpretato come una misura dell’intensità del filtro.

* **[!UICONTROL Raggio]**: determina il numero di pixel attorno ai pixel del bordo che influiscono sulla nitidezza. Per immagini ad alta risoluzione, inserite un valore da 1 a 2. Con un valore basso si agisce solo sui pixel del bordo; con un valore più elevato si agisce su una fascia più ampia di pixel. Il valore più adatto dipende dalle dimensioni dell’immagine.

* **[!UICONTROL Soglia]**: determina l&#39;intervallo di contrasto da ignorare quando viene applicato il filtro Maschera di contrasto. In altre parole, può aiutare a stabilire quanto devono differire i pixel resi più nitidi dall’area circostante prima che vengano considerati pixel del bordo e più nitidi. Per evitare di introdurre disturbi, provare con valori compresi tra `.02` e `0.2`. Il valore predefinito 6 applica la nitidezza a tutti i pixel dell&#39;immagine.

* **[!UICONTROL Spazio colore]**: determina se l&#39;immagine utilizza lo spazio in cui è stata creata, in genere RGB (Originale) o uno spazio di luminanza (Intensità).

* **[!UICONTROL Colore]** Scegliere le opzioni seguenti:

* **[!UICONTROL Profilo colore di output]**: selezionare **[!UICONTROL Usa predefinito]** o uno dei profili colore ICC disponibili in Adobe Dynamic Media Classic.

  Consultate anche [Profili ICC](icc-profiles.md#icc_profiles).

* **[!UICONTROL Intento di rendering]**: selezionare un&#39;opzione se si desidera ignorare l&#39;intento di rendering predefinito del profilo colore. Utilizzare questa opzione quando uno dei profili ICC predefiniti è lo spazio colore di destinazione di una conversione colore. In alternativa, questo profilo caratterizza la periferica di output (stampante o monitor) e l&#39;intento di rendering specificato è valido per questo profilo.

* **[!UICONTROL Incorpora profilo]**: selezionare questa opzione in modo che, se si apre l&#39;immagine in Adobe® Photoshop®, il profilo venga utilizzato.

* **[!UICONTROL Risoluzione di stampa]**: selezionare una risoluzione per la stampa dell&#39;immagine. Il valore predefinito è 72 pixel.

* **[!UICONTROL Modificatori URL]**: se preferisci specificare i modificatori URL che definiscono il predefinito immagine, anziché le impostazioni, immetti i modificatori qui.

* **[!UICONTROL URL immagine di esempio]**: elenca la stringa URL &quot;raw&quot; utilizzata dal server immagini Dynamic Media per distribuire le immagini con il predefinito immagine che si sta aggiungendo o modificando. Questa stringa URL codifica tutte le impostazioni di formato selezionate nella schermata Aggiungi predefinito o Modifica predefinito.

### Modificare, rimuovere o disattivare un predefinito immagine {#editing-removing-or-deactivating-an-image-preset}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**.
1. Nella schermata Predefiniti immagine, selezionate un predefinito nella tabella ed effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Modifica]** e quindi specificare nuove opzioni nella finestra di dialogo Modifica predefinito.
   * Selezionare **[!UICONTROL Elimina]** per rimuovere il predefinito dall&#39;elenco.
   * Deselezionare la casella di controllo **[!UICONTROL Attivo]** accanto al nome di un predefinito se si desidera rimuoverlo dall&#39;intera interfaccia utente di Adobe Dynamic Media Classic per gli utenti MediaPortal.

## Attivare o disattivare i predefiniti per video adattivi {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic offre predefiniti di codifica video adattiva. Si tratta di un elenco principale di predefiniti che combina in un unico gruppo sia 16:9 predefiniti video adattivi che 4:3 predefiniti video adattivi. Tali predefiniti riflettono le impostazioni di codifica più comuni e sono ottimizzati per la riproduzione su dispositivi mobili, tablet e computer desktop.

Per impostazione predefinita, sono attivati solo i predefiniti di codifica &quot;Video adattivo&quot; (abilitati o &quot;attivati&quot;). Se necessario, potete disattivarli. I predefiniti per video adattivi non attivati non vengono visualizzati come opzione selezionabile nella sezione eVideo della finestra di dialogo Opzioni processo di caricamento.

Consulta [Caricare e codificare video](uploading-encoding-videos.md#uploading_and_encoding_videos).

Vedere anche [Video predefiniti](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) video di formazione.

**Per attivare o disattivare i predefiniti per video adattivi:**

1. Nell&#39;angolo superiore destro di Adobe Dynamic Media Classic, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Predefiniti video]** > **[!UICONTROL Predefiniti video adattivi]**.
1. Nella pagina Predefiniti video adattati, deselezionate la casella di controllo accanto al nome di un predefinito per eliminarlo dall’elenco Opzioni eVideo nella finestra di dialogo Opzioni processo di caricamento.
1. Seleziona **[!UICONTROL Chiudi]**.

## Predefiniti video per la codifica di file video {#video-presets-for-encoding-video-files}

Per selezionare un predefinito di codifica, seleziona **[!UICONTROL Opzioni processo]** nell&#39;angolo inferiore destro della pagina Carica. Nella finestra di dialogo Opzioni processo di caricamento, espandi Opzioni eVideo e seleziona i predefiniti di codifica video desiderati.

>[!NOTE]
>
>Ad eccezione di &quot;Video adattivo&quot;, che è abilitato per impostazione predefinita, non è possibile visualizzare tutti gli altri predefiniti di codifica video adattivo o video singolo nella finestra di dialogo Opzioni processo di caricamento. Gli amministratori di Adobe Dynamic Media Classic determinano quali predefiniti di codifica video sono visibili nella finestra di dialogo Opzioni processo di caricamento.

* Seleziona uno dei seguenti predefiniti di codifica video adattiva o a codifica singola:

   * **[!UICONTROL 16:9 video adattivo]**: crea video con proporzioni 16:9 da distribuire a desktop, dispositivi mobili (iPhone, iPad, Android™) e tablet (iPad, Android™), ottimizzati con la risoluzione e la velocità bit che più si adattano alla velocità di connessione del visualizzatore.

   * **[!UICONTROL 4:3 video adattivo]**: creazione di video con proporzioni 4:3 da distribuire a desktop, dispositivi mobili (iPhone, iPad, Android™) e tablet (iPad, Android™), ottimizzati con la risoluzione e la velocità bit che meglio corrispondono alla velocità di connessione del visualizzatore.

   * **[!UICONTROL Video adattivo]**: predefinito a codifica singola che funziona con qualsiasi proporzione per creare video da distribuire su dispositivi mobili, tablet e desktop. I video sorgente caricati e codificati con questo predefinito sono impostati su un’altezza specifica. Tuttavia, la larghezza viene ridimensionata automaticamente per mantenere le proporzioni del video.

     Questa flessibilità di scalabilità automatica è disponibile anche per impostazione predefinita quando crei un predefinito di codifica video personalizzato.

     Consulta [Aggiungere o modificare un predefinito di codifica video](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL Codifica video adattivo (16:9 o 4:3)]**: crea video con proporzioni 16:9 e 4:3 da consegnare a desktop, dispositivi mobili (iPhone, iPad, Android™) e tablet (iPad, Android™). Il tutto ottimizzato con la risoluzione e il bit rate che più si adattano alla velocità di connessione dell&#39;utente.

     Consulta [Predefiniti video per codifica video adattiva (16:9 o 4:3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   * **[!UICONTROL Predefiniti codifica singola]**

     >[!NOTE]
     >
     >Per inviare video agli iPad, puoi selezionare un predefinito di codifica Mobile o un predefinito di codifica Tablet PC. I predefiniti Tablet sono stati creati appositamente per gli iPad, generalmente con risoluzione e qualità più alta per usufruire delle dimensioni delle schermo e della connessione di banda più elevata. La visualizzazione di file video codificati con un predefinito Tablet richiede di includere un codice di rilevamento dispositivi al sito mobile o all’applicazione. questo codice è disponibile per i video visualizzati su iPhone o iPad, a seconda del dispositivo di riproduzione. Se si sceglie un predefinito Mobile per la consegna dei file video ad iPad, il flusso di lavoro risulta semplificato poiché potete scegliere lo stesso file video sia per iPhone che per iPad. Tuttavia, la qualità viene standardizzata all’esperienza iPhone con risoluzione ridotta.

      * Nell&#39;elenco a discesa Ordina predefiniti codifica del gruppo Predefiniti di codifica selezionare Nome o Dimensione per ordinare i predefiniti in base al nome o alla dimensione della risoluzione.
      * Seleziona un predefinito di codifica in base alle dimensioni di risoluzione e alla larghezza di banda con cui intendi riprodurre il video.
      * È possibile selezionare Codifica video adattiva e uno o più predefiniti di codifica per video. Ad esempio, potete codificare un file per desktop e dispositivo mobile in un unico processo di caricamento.

Dopo aver selezionato **[!UICONTROL Avvia caricamento]**, il file video principale originale viene caricato e i file codificati vengono generati dal file principale.

### Le opzioni dei predefiniti di codifica {#about-encoding-preset-options}

I parametri delle opzioni dei predefiniti di codifica sono i seguenti:

* **[!UICONTROL Velocità di connessione di destinazione]**: velocità di connessione Internet dell&#39;utente finale di destinazione.

* **[!UICONTROL Suffisso file codificato]**: il suffisso allegato al file video codificato a scopo di identificazione.

* **[!UICONTROL Velocità bit video (velocità dati)]**: quantità di dati codificati per creare un singolo secondo di riproduzione video (in kilobit al secondo).

* **[!UICONTROL Larghezza/altezza pixel]**: dimensione della larghezza dell&#39;immagine sullo schermo, in pixel; dimensione dell&#39;altezza dell&#39;immagine sullo schermo (in pixel).

* **[!UICONTROL Frame al secondo (fps)]**: numero di fotogrammi, o immagini fisse, per ogni secondo del video. Negli Stati Uniti e in Giappone, i video sono solitamente ripresi a 29,97 fps; in Europa e in Asia (escluso il Giappone), sono invece ripresi a 25 fps. Il film viene girato a 24 fps.

* **[!UICONTROL Velocità in bit audio]**: quantità di dati codificati per costituire un singolo secondo di riproduzione audio, in kilobit al secondo.

Le tabelle di seguito indicano le procedure ottimali per la scelta dei predefiniti per video e le convenzioni di denominazione utilizzate per designare i file codificati.

### Video adattivo (predefinito) {#adaptive-video-default}

Per creare video da distribuire a dispositivi mobili, tablet e computer desktop; predefinito di codifica che funziona con qualsiasi proporzione. I video sorgente caricati codificati con questo predefinito (impostazione predefinita e best practice) vengono impostati su un’altezza fissa, mentre la larghezza viene ridimensionata automaticamente per mantenere le proporzioni del video.

**Video adattivo (predefinito)**

|  | Nome predefinito di codifica/Descrizione | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Valore fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto × 360, 800 Kbps | _Mobile_Auto×360p_800K | 800 | Auto×360 | Come sorgente | 64 | Per dispositivi mobili (iPhone, iPad, Android™) |
| 2 | Auto × 480, 1400 Kbps | _Tablet_Auto×480p_1400K | 1400 | Auto×480 | Come sorgente | 96 | Per tablet (iPad, Android™) |
| 3 | Auto × 720, 2600 Kbps | _Desktop_Auto×720p_2600K | 2600 | Auto×720 | Come sorgente | 128 | Per desktop |

### Predefiniti codifica video adattiva (16:9 o 4:3) {#adaptive-video-encoding-or-video-presets}

Questi predefiniti di codifica video adattiva combinano una serie di singoli predefiniti di codifica selezionati automaticamente in base alle proporzioni del video caricato. Ad esempio, se carichi un video 4:3, viene codificato automaticamente utilizzando tutti e cinque i predefiniti 4:3 presenti nell&#39;elenco dei predefiniti principali nell&#39;opzione **Codifica video adattivo (16:9 o 4:3)**.

Per informazioni sui parametri delle opzioni di codifica, consultate [Le opzioni dei predefiniti di codifica](application-setup.md#about_encoding_preset_options).

**Predefiniti di codifica video adattiva (16:9 o 4:3)**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Valore fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512x288 | Come sorgente | 64 | Risoluzione Medium, 3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_384x288_600 | 600 | 384x288 | Come sorgente | 64 | Risoluzione Medium, 3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640x360 | Come sorgente | 80 | Risoluzione Medium, WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640x480 | Come sorgente | 80 | Risoluzione Medium, WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbps | _iPad_768x432_1200K | 1200 | 768x432 | Come sorgente | 96 | Alta risoluzione, WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | Come sorgente | 96 | Alta risoluzione, WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Come sorgente | 128 | Widescreen ad alta definizione |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3,0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | Come sorgente | 128 | Alta definizione |

### Predefiniti di codifica video per computer desktop {#desktop-video-encoding-presets}

Predefiniti di codifica video per MP4 e OGV su computer desktop.

Per informazioni sui parametri delle opzioni di codifica, consultate [Le opzioni dei predefiniti di codifica](application-setup.md#about_encoding_preset_options).

**H264 Principale 3.2: Audio AAC, estensione file MP4**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Valore fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | Come sorgente | 64 | Widescreen a bassa risoluzione |
| 2 | 16:9, 640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640x360 | Come sorgente | 80 | Widescreen a risoluzione media |
| 3 | 16:9, 800x450 (1200 Kbps) | 1,5 Mbps | _800x450_1200K | 1200 | 800x450 | Come sorgente | 96 | Risoluzione medio-alta |
| 4 | 16:9, 1280x720 (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Come sorgente | 128 | Widescreen ad alta definizione |
| 5 | 4:3, 320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | Come sorgente | 64 | Bassa risoluzione |
| 6 | 4:3, 480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | Come sorgente | 80 | Risoluzione media |
| 7 | 4:3, 640x480 (1200 Kbps) | 1,5 Mbps | _640x480_1200K | 1200 | 640x480 | Come sorgente | 96 | Risoluzione medio-alta |
| 8 | 4:3, 1280x960 (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 | 1280x960 | Come sorgente | 128 | Alta definizione |

**OGG Theora Vorbis: estensione file OGV**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Valore fps | Bitrate audio (Kbps) | Consigli |
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

Come fps sorgente. Predefiniti di codifica video per dispositivi mobili iPhone, iPad e Android™.

Per informazioni sui parametri delle opzioni di codifica, consultate [Le opzioni dei predefiniti di codifica](application-setup.md#about_encoding_preset_options).

**H264 Baseline 2.1: Audio AAC, estensione file MP4**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Bitrate video (Kbps) | Larghezza/Altezza in pixel | Valore fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, dispositivi mobili (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 2 | 16:9, 512x288, dispositivi mobili (600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512x288 | Come sorgente | 64 | Risoluzione Medium, 3G |
| 3 | 16:9, 512x288, dispositivi mobili (800 Kbps) | 900 | _Mobile_512x288_800K | 800 | 512x288 | Come sorgente | 80 | Risoluzione Medium, Wi-Fi |
| 4 | 16:9, 512x288, dispositivi mobili (1000 Kbps) | 1,2 Mbps | _Mobile_512x288_1000K | 1000 | 512x288 | Come sorgente | 80 | Alta risoluzione, Wi-Fi |
| 5 | 16:9, 512x288, dispositivi mobili (1200 Kbps) | 1,5 Mbps | _Mobile_512x288_1200K | 1200 | 512x288 | Come sorgente | 96 | Alta risoluzione, Wi-Fi |
| 6 | 4:3, 384x288, dispositivi mobili (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 7 | 4:3, 384x288, dispositivi mobili (600 Kbps) | 700 | _Mobile_384x288_600K | 600 | 384x288 | Come sorgente | 64 | Risoluzione Medium, 3G |
| 8 | 4:3, 448x336, dispositivi mobili (800 Kbps) | 900 | _Mobile_448x336_800K | 800 | 448x336 | Come sorgente | 80 | Risoluzione Medium, Wi-Fi |
| 9 | 4:3, 448x336, dispositivi mobili (1000 Kbps) | 1,2 Mbps | _Mobile_448x336_1000K | 1000 | 448x336 | Come sorgente | 80 | Alta risoluzione, Wi-Fi |
| 10 | 4:3, 448x336, dispositivi mobili (1200 Kbps) | 1,5 Mbps | _Mobile_448x336_1200K | 1200 | 448x336 | Come sorgente | 96 | Alta risoluzione, Wi-Fi |

## Predefiniti per visualizzatori {#viewer-presets}

>[!NOTE]
>
>**Avviso di fine del ciclo di vita dei visualizzatori Flash**: a partire dal 31 gennaio 2017, Adobe Dynamic Media Classic ha ufficialmente terminato il supporto per la piattaforma di visualizzazione Flash.

Un *predefinito per visualizzatori* è un gruppo di impostazioni con cui viene definito in che modo le risorse multimediali verranno visualizzate sullo schermo del computer e sui dispositivi mobili dell’utente. In qualità di amministratore, potete creare dei predefiniti per visualizzatori. Sono disponibili impostazioni per un’ampia gamma di opzioni di configurazione dei visualizzatori. Ad esempio, è possibile modificare le dimensioni dello schermo del visualizzatore, il comportamento dello zoom, gli schemi di colori, i bordi e i font.

Come best practice, utilizza i visualizzatori video Adobe Dynamic Media Classic HTML5. I predefiniti utilizzati nei visualizzatori video HTML5 sono lettori video affidabili.

Combinando in un singolo lettore quanto segue:

* Possibilità di progettare i componenti di riproduzione utilizzando HTML5 e CSS.
* Avere la riproduzione incorporata.
* Utilizza lo streaming adattivo e progressivo a seconda delle funzionalità del browser.

È possibile estendere la portata dei contenuti rich media agli utenti desktop, tablet e mobili e garantire un&#39;esperienza video semplificata.

Consulta [Informazioni sui visualizzatori HTML5](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) nella Guida di riferimento dei visualizzatori Adobe.

Vedere [Matrice di compatibilità del predefinito visualizzatore Adobe Dynamic Media Classic](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Consultate [Procedura ottimale: utilizzo del visualizzatore video HTML5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

In base al visualizzatore, potete aggiungere delle funzioni per community. e comprendono i pulsanti Incorpora, E-mail, Collega e Visita. Questi pulsanti consentono agli utenti che utilizzano i visualizzatori di condividere il visualizzatore con altri utenti o aprire il sito Web Adobe Dynamic Media Classic.

Vedi anche [Esempi della libreria di riferimento visualizzatori Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Supporto del visualizzatore per pagine Web dinamiche {#viewer-support-for-responsive-designed-web-pages}

Pagine Web diverse hanno esigenze diverse. Talvolta è necessario creare una pagina Web contenente un collegamento che consenta di aprire HTML5 Viewer in una finestra del browser separata. In altri casi, è necessario incorporare il visualizzatore HTML5 direttamente nella pagina di hosting. In quest&#39;ultimo caso, è probabile che la pagina Web abbia un layout statico. Oppure è &quot;reattivo&quot; e viene visualizzato in modo diverso su dispositivi diversi o per diverse dimensioni della finestra del browser. Per soddisfare queste esigenze, i visualizzatori HTML5 forniti con Adobe Dynamic Media Classic supportano sia pagine Web statiche che pagine Web dinamiche.

Per ulteriori informazioni su come incorporare i visualizzatori reattivi nelle pagine Web, vedere [Informazioni sulla libreria di immagini reattive](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library#image-serving-api), [Utilizzare la libreria di immagini reattive](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#image-serving-api) e [Riferimento comando: Attributi comando](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#responsive-static-image-library).

### Tipi di predefiniti per visualizzatori {#viewer-preset-types}

Gli amministratori possono creare e personalizzare i seguenti tipi di predefiniti per visualizzatori.

* **[!UICONTROL Visualizzatore eCatalog]**: simula la lettura di un catalogo stampato. È possibile spostarsi da una pagina all&#39;altra, ingrandire e ridurre gli elementi di una pagina, utilizzare le mappe immagine per visualizzare ulteriori informazioni sugli elementi della pagina o eseguire ricerche nel catalogo. Potete inoltre includere un pannello Info per visualizzare informazioni dettagliate e un elemento mappato da un&#39;immagine se l&#39;area della mappa ha un attributo rollover_key valido. Per includere un pannello Info, specificate un URL di Information Server nel pannello Impostazioni del pannello Info della finestra Predefinito visualizzatore eCatalog.

* **[!UICONTROL Visualizzatore set campioni]**: visualizza un&#39;immagine con un colore, un materiale, una trama, una finitura o un&#39;infrastruttura diversi. Gli utenti selezionano una miniatura per visualizzare le varianti nell’immagine.

* **[!UICONTROL Visualizzatore set di file multimediali diversi]**: visualizza diversi tipi di file multimediali in un solo visualizzatore. Potete includere set di campioni, set 360 gradi, immagini e video. È possibile impostare le schede in modo che contengano diversi tipi di contenuto, ad esempio una scheda per i set di immagini e una scheda per i video. I video riprodotti da un set di file multimediali diversi utilizzano un visualizzatore video standard con una timeline e controlli video quali Stop, Pause, Rewind e Play. Quando imposti un predefinito visualizzatore set di file multimediali diversi, specifica quali visualizzatori desideri utilizzare per i diversi tipi di risorse nel set di file multimediali diversi. Per visualizzare un set di file multimediali diversi potete anche usare il visualizzatore Griglia o Carosello.

* **[!UICONTROL Visualizzatore set 360 gradi]**: fornisce più visualizzazioni di un&#39;immagine in modo che gli utenti possano ruotare l&#39;oggetto per esaminare i diversi lati e angoli.

* **Visualizzatore video**: visualizza i video utilizzando le dimensioni di risoluzione del file di origine o una dimensione personalizzata. In Adobe Dynamic Media Classic sono disponibili molti predefiniti visualizzatore predefiniti per la riproduzione di video e, se sei un amministratore, puoi creare predefiniti visualizzatore video personalizzati. Sono disponibili più di 12 impostazioni diverse per la configurazione del Visualizzatore video. Puoi configurare i relativi:

   * dimensione
   * colore di primo piano e di sfondo
   * controlli video e audio
   * barra di avanzamento
   * interfaccia utente - interfaccia utente
   * funzioni social
   * e Aiuto

* **[!UICONTROL Visualizzatori zoom]**: offre la possibilità di scegliere tra tre tipi di visualizzatori zoom:

* **[!UICONTROL Visualizzatore zoom]**: consente agli utenti di ingrandire l&#39;area selezionandola. È possibile selezionare i controlli per ingrandire, ridurre e ripristinare le dimensioni predefinite dell&#39;immagine.

* **[!UICONTROL Visualizzatore zoom: a comparsa]**: visualizza una seconda immagine dell&#39;area ingrandita accanto all&#39;immagine originale. Non vi sono controlli; gli utenti devono semplicemente spostare la selezione sull’area da visualizzare.

Quando calcolate l’utilizzo di larghezza di banda totale per questo visualizzatore, tenete presente che nel visualizzatore vengono caricate sia l’immagine principale che l’immagine a comparsa. Le dimensioni dell’immagine principale (Larghezza e Altezza area visualizzazione) e il fattore di zoom determinano le dimensioni dell’immagine a comparsa. Per impedire che le dimensioni del file dell’immagine a comparsa diventino eccessive, bilanciate questi due valori: se le dimensioni dell’immagine principale sono grandi, riducete il fattore di zoom. I valori Larghezza a comparsa e Altezza comparsa determinano le dimensioni della finestra a comparsa ma non dell’immagine a comparsa caricata nel visualizzatore.

Ad esempio, se le dimensioni dell’immagine principale sono 350 x 350 pixel, con un fattore di zoom pari a 3 l’immagine a comparsa risultante sarà di 1050 x 1050 pixel. Se le dimensioni dell’immagine principale sono 300 x 300 pixel, con un fattore di zoom pari a 4 l’immagine a comparsa risultante sarà di 1200 x 1200 pixel. In base alla qualità JPEG impostata (impostazioni consigliate: 80-90), potete ridurre sensibilmente le dimensioni del file. I fattori di zoom consigliati sono i valori compresi tra 2,5 e 4, a seconda delle dimensioni dell’immagine principale.

### Matrice di compatibilità del predefinito per visualizzatori Adobe Dynamic Media Classic {#scene-viewer-preset-compatibility-matrix}

**Avviso di fine del ciclo di vita dei visualizzatori Flash**: a partire dal 31 gennaio 2017, Adobe Dynamic Media Classic ha ufficialmente terminato il supporto per la piattaforma di visualizzazione Flash.

La tabella seguente identifica i predefiniti visualizzatore Adobe Dynamic Media Classic attualmente disponibili. La tabella specifica anche la compatibilità del visualizzatore con i dispositivi desktop e mobili e la tecnologia utilizzata per ogni visualizzatore specificato.

Vedi anche [Esempi della libreria di riferimento visualizzatori Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Per informazioni sulle versioni supportate del browser Web e del sistema operativo per i visualizzatori, consulta le Note sulla versione dei visualizzatori.

Consulta le [Note sulla versione di riferimento per visualizzatori Adobe](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources).

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori zoom |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori set immagini |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori set campioni |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori eCatalog |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Include il supporto per i social media e la ricerca nel catalogo.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Include il supporto per i social media e la ricerca nel catalogo.) | HTML5 | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori 360 gradi |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**Visualizzatori per eVideo**

Adobe Dynamic Media Classic supporta la riproduzione di video per dispositivi mobili per video MP4 H.264.

* I dispositivi BlackBerry® che supportano questo formato video sono disponibili nei seguenti percorsi: [Formati video supportati in BlackBerry®](https://developers.blackberry.com/us/en)
* È inoltre possibile trovare i dispositivi Windows® che supportano questo formato video nei seguenti: [Formati video supportati in Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet | Smartphone BlackBerry® | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Include il supporto per i sottotitoli.) Consulta [Best practice: utilizzo del visualizzatore video Universal HTML5.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Include il supporto per sottotitoli e social media.) | HTML5 | X | X | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori set di file multimediali diversi |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Matrice dei gesti supportati dai visualizzatori per dispositivi mobili {#supported-mobile-viewers-gestures-matrix}

La tabella seguente identifica i movimenti del visualizzatore mobile supportati sui dispositivi iOS, Android™ 2.x e Android™ 3.x.

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori set immagini |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### La schermata Predefiniti visualizzatore {#about-the-viewer-preset-screen}

Potete creare e gestire i predefiniti per visualizzatori nella schermata Predefiniti per visualizzatore. Per aprire questa schermata, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.

La schermata Predefiniti visualizzatore offre strumenti che consentono di eseguire le seguenti attività:

* **Aggiungi un predefinito**: seleziona **[!UICONTROL Aggiungi]** e effettua le scelte desiderate nella finestra di dialogo Aggiungi predefinito visualizzatore.

      Vedere [Aggiungi e modifica predefiniti visualizzatore](application-setup.md#adding_and_editing_viewer_presets).
  
* **Modificare un predefinito**: selezionare un predefinito, quindi selezionare **[!UICONTROL Modifica]**.

      Vedere [Aggiungi e modifica predefiniti visualizzatore](application-setup.md#adding_and_editing_viewer_presets).
  
* **Eliminare un predefinito**: selezionare un predefinito, quindi selezionare **[!UICONTROL Elimina]**.

* **Esportare un predefinito**: selezionare un predefinito visualizzatore HTML5. Quindi fai clic su **[!UICONTROL Esporta]** per scaricare l&#39;interfaccia del visualizzatore in modo da poterla utilizzare come base per la creazione e l&#39;aggiunta di un altro predefinito visualizzatore.

      Vedere [Esportare un predefinito visualizzatore HTML5](application-setup.md#export_an_html5_viewer_preset).
  
* **Filtra l&#39;elenco dei predefiniti visualizzatore**: utilizzare questi strumenti per filtrare l&#39;elenco:

      * Aprire l&#39;elenco a discesa **Attivo/Inattivo** e selezionare un&#39;opzione per visualizzare i predefiniti attivi, i predefiniti inattivi o tutti i predefiniti.
     * Aprire l&#39;elenco a discesa **Viewer** e selezionare un&#39;opzione per visualizzare solo i visualizzatori di un determinato tipo. Seleziona **[!UICONTROL Tutti i visualizzatori]** per visualizzare tutti i visualizzatori.
  
* **Predefiniti di ordinamento**: selezionare un&#39;intestazione di colonna (**[!UICONTROL Active]**, **[!UICONTROL Type]**, **[!UICONTROL Preset]** o **[!UICONTROL Platform]**) per ordinare l&#39;elenco in una colonna. Selezionare un&#39;intestazione di colonna una seconda volta per ordinare l&#39;elenco in ordine decrescente o crescente.

* **Attiva e disattiva i predefiniti**: seleziona un predefinito, quindi seleziona l&#39;opzione Attivo per attivarlo o disattivarlo.

      Vedere [Attivare o disattivare i predefiniti visualizzatore](application-setup.md#activating_or_deactivating_viewer_presets).
  
>[!NOTE]
>
>Seleziona **[!UICONTROL Anteprima]** sul lato destro della pagina Predefiniti visualizzatore per visualizzare l&#39;aspetto di una risorsa nel predefinito visualizzatore selezionato. Per visualizzare una risorsa diversa, seleziona **[!UICONTROL Sfoglia]** nella pagina Predefiniti visualizzatore e seleziona un&#39;altra risorsa nella finestra di dialogo Seleziona anteprima risorsa.

### Aggiungere e modificare i predefiniti per visualizzatori {#adding-and-editing-viewer-presets}

Oltre ad aggiungere i predefiniti visualizzatore utilizzando **[!UICONTROL Aggiungi]** nell&#39;interfaccia utente, puoi anche utilizzare **[!UICONTROL Esporta]** per aggiungere un predefinito visualizzatore. È sufficiente esportare un predefinito visualizzatore HTML5 esistente e utilizzarlo come base per il nuovo predefinito.

Consulta [Esportazione predefinito visualizzatore HTML5](application-setup.md#exporting_an_html5_viewer_preset).

Guarda anche il video di formazione [Predefiniti visualizzatore](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

**Per aggiungere e modificare i predefiniti visualizzatore:**

1. Nell&#39;angolo superiore destro di Adobe Dynamic Media Classic, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.

   Potete filtrare l’elenco dei predefiniti. Ad esempio, per visualizzare soltanto i predefiniti per i visualizzatori video, selezionate Visualizzatore video dall’elenco a discesa Visualizzatori nella barra degli strumenti che si trova appena sopra la tabella.

1. Nella pagina Predefiniti visualizzatore, aggiungi o modifica il Predefinito visualizzatore nella schermata Predefiniti visualizzatore.

   * **Aggiungi**: sulla barra degli strumenti, seleziona **[!UICONTROL Aggiungi]**. Nella finestra di dialogo Aggiungi predefinito visualizzatore, seleziona una piattaforma e fai clic su un tipo di risorsa multimediale avanzato.

         Selezionare **[!UICONTROL Salva con nome]** al termine della creazione del predefinito visualizzatore.
     
   * **Aggiungi partendo da un predefinito visualizzatore esistente**: nella tabella, seleziona un predefinito visualizzatore video, quindi seleziona **[!UICONTROL Modifica]** sulla barra degli strumenti.

         Dopo aver riconfigurato il Visualizzatore video, seleziona **[!UICONTROL Salva con nome]** per salvare il predefinito utilizzando un nome diverso nel campo di testo Nome predefinito.
     
   * **Modifica**: seleziona un predefinito visualizzatore esistente, quindi seleziona **[!UICONTROL Modifica]**.

1. Nella pagina Configurazione del visualizzatore, immetti o modifica il nome del predefinito nel campo Nome predefinito.
1. Impostate le opzioni rimanenti in base alle vostre esigenze.

   >[!NOTE]
   >
   >Selezionare **[!UICONTROL Come Source]** per ridimensionare automaticamente il Visualizzatore video in base alle dimensioni di risoluzione del video codificato. Se si seleziona questa opzione, non è possibile immettere le opzioni Larghezza stage e Altezza stage. e tali valori verranno invece determinati dal video stesso. Se si seleziona **[!UICONTROL Come Source]**, impostare l&#39;opzione Dimensione margine in modo che rifletta le dimensioni dell&#39;interfaccia al di fuori dell&#39;area di riproduzione video. Le dimensioni del margine corrispondono all’altezza e alla larghezza in pixel dei controlli video. Per determinare le dimensioni dei margini desiderate, è possibile utilizzare l&#39;immagine seguente.*

   ![Configurazione del margine del visualizzatore video](assets/vs_video_viewer_configure_margin.png)

1. Effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Salva con nome]** se hai aggiunto un predefinito visualizzatore partendo da un predefinito esistente.
   * Seleziona **[!UICONTROL Salva]** se hai aggiunto o modificato un predefinito visualizzatore.

### Esportare un predefinito visualizzatore HTML5 {#exporting-an-html-viewer-preset}

È possibile esportare un predefinito visualizzatore HTML5 esistente da utilizzare come base per la creazione di un predefinito visualizzatore HTML5. In questo modo si evita di dover creare un visualizzatore da zero. Se esportate un predefinito con aspetto e comportamento simili a quelli desiderati, potrete usarlo come base di partenza per apportare le regolazioni necessarie.

Tutti i file CSS predefiniti del predefinito visualizzatore in Adobe Dynamic Media Classic utilizzano percorsi relativi di gestione delle immagini che puntano alle risorse in `Scene7SharedAssets`. Ad esempio, il percorso relativo di una risorsa immagine in un file CSS del predefinito per visualizzatori in

`Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

Tuttavia, se ospiti i file CSS del visualizzatore sul tuo sito, devi risolvere questi percorsi immagine relativi utilizzando un percorso esplicito al server immagini nel tuo ambiente. Ad esempio, se hai aggiornato il percorso relativo precedente a un percorso esplicito, potrebbe essere simile al seguente, dove `https://s7d1.scene7.com` è il percorso diretto del server immagini: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Per esportare un predefinito visualizzatore HTML5:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Sulla barra degli strumenti Predefiniti visualizzatore, nel secondo elenco a discesa da sinistra, selezionare **[!UICONTROL HTML5]**.
1. Selezionate **[!UICONTROL Tutti i visualizzatori]** nel terzo elenco a discesa da sinistra.
1. Selezionare il predefinito visualizzatore da utilizzare come base per un nuovo predefinito visualizzatore HTML5.
1. Nella barra degli strumenti, seleziona **[!UICONTROL Esporta]**.
1. Nella finestra di dialogo Esporta Assets selezionato, seleziona **[!UICONTROL Invia esportazione]**.

   Dopo l’esportazione, ottieni un file CSS. Scaricate e decomprimete il file.

1. Aprite il file CSS in un Editor CSS, apportate le modifiche e salvate il file.
1. Carica il file CSS in Adobe Dynamic Media Classic.

   Vedi [Carica file](uploading-files.md#uploading_files).

1. Pubblica il file CSS sul server immagini Dynamic Media.

   Vedi [File di pubblicazione](publishing-files.md#publishing_files).

1. Aggiungi normalmente il nuovo predefinito visualizzatore. Seleziona il file CSS del visualizzatore caricato.

   Consulta [Aggiungere e modificare i predefiniti visualizzatore](application-setup.md#adding_and_editing_viewer_presets).

### Attivare o disattivare i predefiniti visualizzatore {#activating-or-deactivating-viewer-presets}

Per creare un URL per la visualizzazione delle risorse, gli utenti aprono l&#39;elenco a discesa Predefiniti nella finestra di dialogo Anteprima, selezionano un predefinito visualizzatore, quindi selezionano **[!UICONTROL Copia URL]** (vedi [Copia l&#39;URL di un predefinito visualizzatore](application-setup.md#copying_the_url_of_a_viewer_preset)). Questo elenco di predefiniti offre i predefiniti per visualizzatori aggiunti e gestiti dagli amministratori nella schermata Predefiniti per visualizzatore. Ad esempio, tutti i predefiniti visualizzatore eCatalog attivi vengono visualizzati nell&#39;elenco a discesa Predefiniti nella finestra di dialogo Anteprima quando un utente visualizza l&#39;anteprima di un eCatalog.

Se i predefiniti per visualizzatori non vengono disattivati nella schermata Predefiniti per visualizzatore, nell’elenco a discesa Predefiniti nella finestra di dialogo Anteprima potrebbero accumularsi troppi predefiniti. 

**Per attivare o disattivare i predefiniti visualizzatore:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Nella pagina Predefiniti visualizzatore, seleziona o deseleziona le opzioni **[!UICONTROL Attivo]** per attivare o disattivare i Predefiniti visualizzatore.

### Copiare l’URL di un predefinito per visualizzatori {#copying-the-url-of-a-viewer-preset}

Una volta pubblicata una risorsa, potete copiare un URL per visualizzare la risorsa con le impostazioni di un predefinito per visualizzatore.

L’URL viene copiato negli Appunti. È possibile utilizzarlo in base alle esigenze nel codice HTML della pagina Web, del dispositivo mobile o dell&#39;applicazione.

**Per copiare l&#39;URL di un predefinito visualizzatore:**

1. Seleziona la risorsa nel pannello Sfoglia.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e Codice di incorporamento a destra, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato.
   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]** sotto l&#39;immagine di anteprima.

   Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

   * Selezionare **[!UICONTROL Vista elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell&#39;immagine di anteprima passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

   Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

   * Selezionare **[!UICONTROL Visualizzazione griglia]**, **[!UICONTROL Visualizzazione elenco]** o **[!UICONTROL Visualizzazione dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

   Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

### Copiare il codice di incorporamento di un predefinito visualizzatore {#copying-the-embed-code-of-a-viewer-preset}

La funzione Incorpora codice permette di analizzare il codice visualizzatore del predefinito per visualizzatori selezionato. È inoltre possibile copiare il codice negli Appunti in modo da poterlo incollare nelle pagine Web per la distribuzione del visualizzatore.

La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

**Per copiare il codice di incorporamento di un predefinito visualizzatore:**

1. Seleziona la risorsa nel pannello Sfoglia risorse.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL a destra, seleziona **[!UICONTROL Incorpora codice]**.
   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]** sotto l&#39;immagine di anteprima.

   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Vista elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell&#39;immagine di anteprima passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Visualizzazione griglia]**, **[!UICONTROL Visualizzazione elenco]** o **[!UICONTROL Visualizzazione dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

1. Nella finestra di dialogo Incorpora codice, seleziona **[!UICONTROL Copia negli Appunti]**.
1. Seleziona **[!UICONTROL Chiudi]**.

## Configurare i visualizzatori predefiniti {#configure-default-viewers}

Puoi utilizzare i visualizzatori predefiniti per configurare il visualizzatore predefinito associato a una risorsa quando utilizzi Anteprima in Adobe Dynamic Media Classic. Potete impostare l’esperienza di anteprima predefinita per i seguenti tipi di risorse:

* Immagine
* Video
* Set 360 gradi
* Catalogo
* Set di immagini
* Set di campioni
* Set file multimediali

**Per configurare i visualizzatori predefiniti:**

1. Nell&#39;elenco a discesa Configurazione selezionare **[!UICONTROL Configurazione applicazione]**.
1. Nel riquadro a sinistra della finestra Configurazione, vai a **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Visualizzatori]**
1. Seleziona **[!UICONTROL Visualizzatori predefiniti]**.
1. Nella finestra Visualizzatori predefiniti, seleziona nell’elenco a discesa per ciascun tipo di risorsa il visualizzatore da associare all’anteprima della risorsa.
1. Nell&#39;angolo inferiore destro della finestra Visualizzatori predefiniti, selezionare **[!UICONTROL Salva impostazioni]**.
1. Nell&#39;angolo inferiore destro della finestra di installazione, selezionare **[!UICONTROL Chiudi]** per tornare alla finestra Risorsa.

## Visualizzazione metadati {#metadata-views}

I *metadati* sono informazioni standardizzate su una risorsa. Potete utilizzare i metadati per semplificare il flusso di lavoro, organizzare le risorse e migliorare le ricerche. Adobe Dynamic Media Classic supporta lo standard IPTC (International Press Telecommunications Council) e lo standard XMP (Extensible Metadata Platform). Prima che gli utenti possano visualizzare o immettere i metadati di una risorsa in Vista dettagli, possono aprire il menu Visualizzazioni metadati. Da qui, può selezionare il set di campi di metadati che desidera visualizzare o utilizzare per descrivere la risorsa.

In Adobe Dynamic Media Classic sono disponibili visualizzazioni metadati predefinite; gli amministratori possono creare visualizzazioni metadati personalizzate che gli utenti possono scegliere quando immettere i metadati.

### Creazione di una visualizzazione metadati {#creating-a-metadata-view}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Visualizzazioni metadati]**.
1. Seleziona **[!UICONTROL Aggiungi]**.
1. Nel campo di testo Nome predefinito immettere un nome per la visualizzazione.
1. (Facoltativo) Selezionare **[!UICONTROL Rendi predefinita]** per impostare questa visualizzazione come quella visualizzata dagli utenti all&#39;apertura del pannello Metadati in Visualizzazione dettagli.
1. (Facoltativo) Selezionare **[!UICONTROL Includi UDF]** per includere nella visualizzazione i campi definiti dall&#39;utente. Questi vengono presentati nella parte superiore del pannello Metadati in visualizzazione Dettagli.
1. Selezionare i campi desiderati per la visualizzazione (selezionare **[!UICONTROL Seleziona tutto]** per selezionare tutti i campi).
1. Seleziona **[!UICONTROL Salva]**.

   Le categorie e i campi selezionati per la visualizzazione vengono visualizzati nel pannello Anteprima.

### Gestione delle visualizzazioni metadati {#managing-metadata-views}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Visualizzazioni metadati]**.
1. Effettuate una delle seguenti operazioni:

   * Per visualizzare un’anteprima di una visualizzazione, selezionatela. I campi della visualizzazione vengono visualizzati nel pannello Anteprima.
   * Per modificare una visualizzazione, selezionarla, quindi selezionare **[!UICONTROL Modifica]**. Selezionare o deselezionare i nomi dei campi nel pannello Anteprima, quindi selezionare o deselezionare l&#39;opzione **[!UICONTROL Includi UDF]**.
   * Per eliminare una visualizzazione, selezionarla, quindi selezionare **[!UICONTROL Elimina]**.
   * Per impostare una visualizzazione come predefinita, selezionarla, quindi selezionare **[!UICONTROL Imposta come predefinita]**. La vista predefinita è quella che gli utenti visualizzano quando aprono una risorsa in Vista dettagli e passano al pannello Metadati.

## Predefiniti per metadati {#metadata-presets}

I predefiniti di metadati consentono agli amministratori di controllare e regolare i metadati assegnati alle risorse. Nella Vista dettagli, un utente può immettere i metadati di una risorsa nei campi forniti a tale scopo. Ad esempio, un utente può inserire un nome proprietario, una descrizione del copyright e un indirizzo. Per fare in modo che gli utenti immettano queste informazioni in modo accurato e completo, puoi creare predefiniti di metadati. Quando si sceglie un predefinito di metadati nella vista Dettaglio, i campi di metadati vengono compilati con valori predefiniti. Ad esempio, il nome proprietario, la descrizione del copyright e l’indirizzo vengono inseriti automaticamente.

Crea un predefinito di metadati per ogni set di valori di metadati che desideri che gli utenti possano immettere automaticamente nella Vista dettagli per descrivere una risorsa.

### Creazione o modifica di un predefinito per metadati {#creating-or-editing-a-metadata-preset}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Predefiniti metadati]**.
1. Nella schermata Predefiniti metadati, effettuate una delle seguenti operazioni:

   * Per creare un predefinito, selezionare **[!UICONTROL Aggiungi]**. Nel campo di testo Nome modello metadati, digita un nome per il predefinito. Selezionare **[!UICONTROL Visualizzazioni metadati]**, quindi selezionare una visualizzazione dall&#39;elenco a discesa (vedere [Visualizzazioni metadati](application-setup.md#metadata_views)).
   * Per modificare un predefinito esistente, selezionarlo dall&#39;elenco Predefiniti metadati, quindi selezionare **[!UICONTROL Modifica]**.

1. Espandere le intestazioni che si desidera includere nel predefinito e immettere i valori nei diversi campi che si desidera includere nel predefinito.
1. Seleziona **[!UICONTROL Salva]**.

   Le categorie e i campi selezionati per il predefinito vengono visualizzati nel pannello dell’anteprima.

### Gestione dei predefiniti per metadati {#managing-metadata-presets}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Predefiniti metadati]**.
1. Effettuate una delle seguenti operazioni:

   * Per visualizzare l’anteprima di un predefinito, selezionate il predefinito. Le informazioni sul predefinito (categorie e campi) vengono visualizzate nella schermata Anteprima.
   * Per eliminare un predefinito, selezionarlo, quindi selezionare **[!UICONTROL Elimina]**.

## Campi definiti dall’utente {#user-defined-fields}

I campi metadati definiti dall’utente possono essere creati solo da un amministratore di Media Portal o un amministratore società. I campi personalizzati consentono di organizzare le risorse in Adobe Dynamic Media Classic. Se necessario, puoi contrassegnare i campi come Attivi. Quando questa opzione è attivata, i nomi di questi campi di metadati personalizzati vengono visualizzati nel pannello Metadati in Vista dettagli. Nei campi di metadati definiti dall’utente gli utenti possono immettere informazioni per descrivere le risorse. Gli utenti possono inoltre utilizzare tali campi di metadati come criteri di ricerca.

I campi metadati definiti dall’utente sono utili ad esempio per ritardare il momento di attivazione di una risorsa per un lancio o una promozione. Definisci un campo &quot;attivazione&quot; in base al tipo *Data*. Quindi, utilizzando il pannello **[!UICONTROL Metadati]** in Visualizzazione dettagli o **[!UICONTROL File]** > **[!UICONTROL Modifica informazioni]**, puoi specificare quando attivare la risorsa. Adobe Dynamic Media Classic controlla lo stato di pubblicazione di una risorsa e la cronologia delle pubblicazioni. Se non rientra nel tempo di attivazione, lo stato di pubblicazione sarà &quot;Non pubblicato&quot;.

>[!NOTE]
>
>Per fare in modo che i campi definiti dall&#39;utente vengano visualizzati nel pannello Metadati in Visualizzazione dettagli, includete i campi definiti dall&#39;utente nelle Visualizzazioni metadati. Nella schermata Visualizzazioni metadati, selezionate l’opzione Includi UDF (User-Defined Fields, campi definiti dall’utente). Per ulteriori informazioni, consultate [Visualizzazione metadati](application-setup.md#metadata_views).

>[!NOTE]
>
>Per cercare le risorse utilizzando campi personalizzati definiti dall&#39;utente, passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**, quindi selezionare **[!UICONTROL Includi UDF nella ricerca]**. Consultate [Configurazione personale](personal-setup.md#personal_setup).

### Creare un campo di metadati definito dall&#39;utente {#creating-a-user-defined-metadata-field}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Campi definiti dall&#39;utente]**.
1. Seleziona **[!UICONTROL Aggiungi]**
1. Nella finestra di dialogo Campo personalizzato, impostate le opzioni desiderate.

   * **[!UICONTROL Nome]**: immettere un nome per il campo metadati.

   * **[!UICONTROL Tipo]**: selezionare un&#39;opzione che definisca il tipo di informazioni che gli utenti possono immettere nel campo metadati:

   * **[!UICONTROL Stringa]**: una stringa di testo.

   * **[!UICONTROL Intero]**: un numero intero.

   * **[!UICONTROL Mobile]**: numero a virgola mobile.

   * **[!UICONTROL Sì/No]**: un valore booleano sì/no.

   * **[!UICONTROL Data]**: una data. Il formato consentito è GG/MM/AAAA.

   * **[!UICONTROL Nome file]**: nome di un file.

   * **[!UICONTROL Colore]**: nome di un colore.

   * **[!UICONTROL Dimension]**: larghezza e altezza della risorsa.

   * **[!UICONTROL Non tipizzato]**: per compatibilità con le versioni precedenti. Non selezionate questa opzione.

   * **[!UICONTROL Valore predefinito]**: facoltativo. Immetti il valore che gli utenti immetteranno con maggiore probabilità nel campo. Il valore immesso diventa il valore predefinito per il nuovo campo creato.

   * **[!UICONTROL Si Applica A]**: Facoltativo. Seleziona un tipo di risorsa se desideri che il campo metadati sia applicabile solo a un tipo specifico di risorsa.

     >[!NOTE]
     >
     >Selezionare attentamente un&#39;opzione **[!UICONTROL Si applica a]** perché non è possibile modificare l&#39;opzione **[!UICONTROL Si applica a]** dopo aver creato un campo definito dall&#39;utente. Adobe Dynamic Media Classic consente di modificare il nome, il tipo e il valore predefinito di un campo definito dall&#39;utente, ma non l&#39;impostazione **[!UICONTROL Si applica a]**. *

1. Seleziona **[!UICONTROL Salva]** al termine della creazione del campo metadati.

### Gestire i campi definiti dall’utente {#manage-user-defined-fields}

Nella schermata Campi definiti dall’utente sono disponibili i comandi necessari per gestire i campi di metadati personalizzati, definiti dall’utente. 

I campi definiti dall’utente possono essere gestiti solo da un amministratore di Media Portal o un amministratore società.

Per aprire questa schermata, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Campi definiti dall&#39;utente]**.

* **Modifica campo**: selezionare il campo, quindi selezionare **[!UICONTROL Modifica]**.

* **Elimina campo**: selezionare il campo, quindi selezionare **[!UICONTROL Elimina]**.

* **Attiva campo**: seleziona o deseleziona l&#39;opzione **[!UICONTROL Attivo]** accanto al nome di un campo. Se hai il ruolo di amministrazione aziendale, questa opzione non viene visualizzata. Poiché questa opzione è correlata a Media Portal, è necessario selezionare (attivare) Mostra funzionalità Media Portal in Impostazione personale per visualizzare i campi attivati.

## Ottimizzare i file {#optimize-files}

Quando si caricano i file in Adobe Dynamic Media Classic, il sistema li ottimizza per l&#39;archiviazione e la pubblicazione. Tuttavia, se il processo di caricamento viene interrotto, alcune immagini potrebbero non essere ottimizzate. In questo caso, viene visualizzato il messaggio &quot;Immagine non ancora ottimizzata&quot;. Tali file possono comunque essere ottimizzati dagli utenti con ruolo di amministratore.

Adobe Dynamic Media Classic esegue la ricerca nei file e ottimizza solo le immagini che non erano state completamente ottimizzate in precedenza.

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]**, quindi seleziona **[!UICONTROL Ottimizza file]**.
1. Immettere le informazioni per il processo di ottimizzazione e selezionare **[!UICONTROL Invia]**.

   Se lavorate con più società, ottimizzate separatamente i file appartenenti a società diverse.

## Predefiniti per set di batch {#batch-set-presets}

Utilizza i predefiniti per set di batch per creare automaticamente set di immagini o set 360 gradi mentre è in esecuzione un processo per caricare le risorse in Adobe Dynamic Media Classic.

Gli amministratori aziendali definiscono innanzitutto le convenzioni di denominazione per le risorse che desiderano raggruppare in un set. È quindi possibile creare un predefinito per set di batch per fare riferimento a queste immagini. Ogni predefinito ha un nome univoco ed è un set autonomo di istruzioni che definisce come comporre il set con le immagini in base alle convenzioni di denominazione specificate con le opzioni del predefinito.

Tutti i predefiniti per set di batch attivi per una società sono elencati nella finestra di dialogo Opzioni processo di caricamento, che consente di specificare il predefinito da applicare durante ogni sessione di caricamento. Gli amministratori della società visualizzano tutti i predefiniti per set di batch attivi e inattivi. Quando caricate i file, Adobe Dynamic Media Classic crea automaticamente un set con tutti i file che corrispondono alla convenzione di denominazione definita nei predefiniti attivi.

### Denominazione predefinita {#default-naming}

L’amministratore della società crea una convenzione di denominazione predefinita che viene utilizzata in qualsiasi composizione di predefiniti per set di batch. La convenzione di denominazione predefinita selezionata nella definizione del predefinito per set di batch può essere tutto ciò che la società deve generare in batch set per tutti i siti web. Un predefinito per set di batch viene creato per utilizzare la convenzione di denominazione predefinita definita. È possibile creare un numero illimitato di predefiniti per set di batch con convenzioni di denominazione alternative e personalizzate necessarie per un particolare set di contenuti nei casi in cui vi sia un’eccezione alla denominazione predefinita definita dall’azienda.

Per utilizzare la funzionalità Predefinito per set di batch non è necessario impostare una convenzione di denominazione predefinita. Tuttavia, in base alle best practice di Adobe, è consigliabile utilizzare una convenzione di denominazione predefinita per definire tutti gli elementi della convenzione di denominazione che si desidera raggruppare in un set. In questo modo è possibile semplificare la creazione di set di batch.

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Predefiniti set di batch]** > **[!UICONTROL Denominazione predefinita]**.
1. Selezionate **[!UICONTROL Visualizza modulo]** o **[!UICONTROL Visualizza codice]** per specificare la modalità di visualizzazione e di inserimento delle informazioni relative a ciascun elemento.

   È possibile selezionare la casella di controllo **[!UICONTROL Visualizza codice]** per visualizzare la creazione del valore dell&#39;espressione regolare insieme alle selezioni del modulo. È possibile immettere o modificare questi valori per definire gli elementi della convenzione di denominazione, se per qualsiasi motivo la visualizzazione Maschera vi limita. Se non è possibile analizzare i valori nella visualizzazione Maschera, i campi del modulo diventano inattivi.

   >[!NOTE]
   >
   >i campi del modulo disattivati non indicano che l’espressione regolare non è valida. Non è disponibile una funzione di convalida delle espressioni regolari generate. Vedrai i risultati dell’espressione regolare che stai creando per ogni elemento dopo la riga Risultato. L’espressione regolare completa è riportata nella parte inferiore della pagina.

1. Espandete ciascun elemento come opportuno e inserite le convenzioni di denominazione da usare.
1. Se necessario, selezionare **[!UICONTROL Aggiungi]** per aggiungere un&#39;altra convenzione di denominazione per un elemento. In alternativa, selezionare **[!UICONTROL Rimuovi]** per eliminare una convenzione di denominazione per un elemento.
1. Selezionare **[!UICONTROL Salva con nome]** e digitare un nome per il predefinito. Oppure, seleziona **[!UICONTROL Salva]** se stai modificando un predefinito esistente.

In alternativa, potete usare l’opzione Visualizza codice, senza campi del modulo. In questa vista puoi creare le definizioni delle convenzioni di denominazione interamente utilizzando espressioni regolari.

Per la definizione sono disponibili due elementi, Corrispondenza e Nome base. Questi campi sono tutti gli elementi definiti per una convenzione di denominazione. Possono aiutare a identificare la parte della convenzione utilizzata per denominare l’insieme in cui sono contenuti. La convenzione di denominazione individuale di un’azienda può utilizzare una o più righe di definizione per ciascuno di questi elementi. È possibile utilizzare tutte le righe per la definizione univoca e raggrupparle in elementi distinti, ad esempio per l&#39;immagine principale, l&#39;elemento Colore, l&#39;elemento Visualizzazione alternativa e l&#39;elemento Campione.

### Creare un predefinito per set di batch {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic utilizza i predefiniti per set di batch per organizzare le risorse che condividono alcune informazioni o contenuti comuni in set di immagini da visualizzare nei visualizzatori. Le composizioni del predefinito per set di batch vengono eseguite automaticamente insieme ai processi di importazione risorse pianificati in Adobe Dynamic Media Classic.

Utilizzare Predefinito set di batch per creare, modificare e gestire i predefiniti set di batch. Puoi creare tutti i predefiniti necessari per coprire tutti i processi di acquisizione risorse necessari. Esistono due forme di definizioni dei predefiniti per set di batch: una per una convenzione di denominazione predefinita che hai impostato e una per le convenzioni di denominazione personalizzate che crei al volo.

È possibile utilizzare il metodo campo modulo per definire un predefinito per set di batch o il metodo di codice, che consente di utilizzare espressioni regolari. Come in **[!UICONTROL Denominazione predefinita]**, è possibile selezionare **[!UICONTROL Visualizzazione codice]** contemporaneamente alla definizione nella visualizzazione Maschera e utilizzare espressioni regolari per generare le definizioni. In alternativa, potete deselezionare una delle due visualizzazioni e usare solo l’altra.

Vedi anche [Creare un predefinito per set di batch per la generazione automatica di un set 360 gradi 2D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

Guarda anche il video di formazione [Set 360 gradi 2D](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS).

**Per creare un predefinito per set di batch:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Predefiniti set di batch]** > **[!UICONTROL Predefinito set di batch]**. La vista predefinita e **[!UICONTROL Visualizza modulo]**, come impostato nell’angolo in alto a destra della pagina Dettagli.
1. Nel pannello Elenco predefiniti, seleziona **[!UICONTROL Aggiungi]** per attivare i campi di definizione nel pannello Dettagli sul lato destro della pagina.
1. Nel pannello Dettagli, digitate nel campo Nome predefinito il nome da assegnare al predefinito.
1. Selezionate il tipo di predefinito dal menu Tipo set di batch.

   Per generare automaticamente un set 360 gradi, selezionate **[!UICONTROL Set 360 gradi con asse multiplo]** dall’elenco a discesa Tipo set di batch.

1. Effettuate una delle seguenti operazioni:

   * Se utilizzi una convenzione di denominazione predefinita che hai impostato in precedenza in **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Predefiniti set di batch]** > **[!UICONTROL Denominazione predefinita]**, espandi **[!UICONTROL Convenzioni di denominazione risorse]**, quindi seleziona **[!UICONTROL Predefinito]** nell&#39;elenco a discesa Denominazione file.
   * Per definire una convenzione di denominazione durante la configurazione del predefinito, espandi **[!UICONTROL Convenzioni di denominazione delle risorse]**, quindi seleziona **[!UICONTROL Personalizzato]** nell&#39;elenco a discesa Denominazione file.

1. Per Ordine sequenza, definisci l’ordine delle immagini dopo che il set è stato raggruppato in Adobe Dynamic Media Classic. Per impostazione predefinita le risorse sono elencate in ordine alfabetico. Tuttavia, potete definirne l’ordine utilizzando un elenco separato da virgole delle espressioni regolari.
1. Per Imposta convenzione di denominazione e creazione, specificate il suffisso o il prefisso del nome base definito nella convenzione di denominazione delle risorse. Definisci anche dove viene creato il set di immagini nella struttura di cartelle di Adobe Dynamic Media Classic.

   Se definisci un numero elevato di Set di immagini, mantieni questi set separati dalle cartelle che contengono le risorse stesse. Molti clienti creano una cartella Set di immagini e reindirizzano l’applicazione per inserire qui i set generati da set di batch.

1. Seleziona **[!UICONTROL Salva]** nel pannello Dettagli.

### Creare un predefinito per set di batch per la generazione automatica di un set 360 gradi 2D {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

È possibile utilizzare il tipo di set di batch **Set 360 gradi a più assi** per creare una &quot;ricetta&quot; che automatizza la generazione di set 360 gradi 2D. Il raggruppamento delle immagini utilizza espressioni regolari per riga e colonna per il corretto allineamento delle risorse di immagini nella posizione corrispondente nell’array multidimensionale.

Vedere anche [Creare un predefinito per set di batch](application-setup.md#creating_a_batch_set_preset).

In un set 360 gradi multiasse non è necessario disporre di un numero minimo o massimo di righe o colonne.

Ad esempio, si supponga di voler creare un set 360 gradi multiasse denominato *spin-2dspin*. Hai un set di immagini Set 360 gradi che contengono tre righe, con 12 immagini per riga. Le immagini sono denominate come segue:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Con queste informazioni, la composizione del tipo di set di batch può essere creata come segue:

![Immagine ricetta set di batch](assets/se_batch_set_recipe.png)

Il raggruppamento per la parte del nome della risorsa condivisa del set 360 gradi viene aggiunto al campo Match (Corrispondenza) (come evidenziato). La parte variabile del nome della risorsa contenente la riga e la colonna viene aggiunta rispettivamente ai campi Riga e Colonna.

Quando il set 360 gradi viene caricato e pubblicato, puoi attivare il nome della definizione del set 360 gradi 2D che è elencato in **[!UICONTROL Predefiniti set di batch]** nella finestra di dialogo Opzioni processo di caricamento.

**Per creare un predefinito per set di batch per la generazione automatica di un set 360 gradi 2D:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Predefiniti set di batch]** > **[!UICONTROL Predefinito set di batch]**. La vista predefinita e **[!UICONTROL Visualizza modulo]**, come impostato nell’angolo in alto a destra della pagina Dettagli.
1. Nel pannello Elenco predefiniti, seleziona **[!UICONTROL Aggiungi]** per attivare i campi di definizione nel pannello Dettagli sul lato destro della pagina.
1. Nel pannello Dettagli, digitate nel campo Nome predefinito il nome da assegnare al predefinito.
1. Selezionate **[!UICONTROL Set risorse]** dal menu a discesa Tipo set di batch.
1. Nell&#39;elenco a discesa Sottotipo selezionare **[!UICONTROL Set 360 gradi con asse multiplo]**.
1. Espandi **[!UICONTROL Convenzioni di denominazione risorse]**, quindi seleziona **[!UICONTROL Personalizzato]** nell&#39;elenco a discesa Denominazione file.
1. Utilizzate gli attributi **[!UICONTROL Corrispondenza]** e, facoltativamente, **[!UICONTROL Nome base]** per definire un’espressione regolare per la denominazione delle risorse di immagine che compongono il gruppo.

   Ad esempio, l’espressione regolare Match letterale potrebbe avere l’aspetto seguente:

   `(\w+)-\w+-\w+`

1. Espandete **[!UICONTROL Posizione colonna riga]** e definite il formato del nome per la posizione della risorsa di immagine nell’array set 360 gradi 2D.

   Usate le parentesi per racchiudere la posizione di riga o colonna nel nome file.

   Ad esempio, per l’espressione regolare della riga, potrebbe essere simile alla seguente:

   `\w+-R([0-9]+)-\w+`

   Oppure

   `\w+-(\d+)-\w+`

   Per l’espressione regolare della colonna, potrebbe avere l’aspetto seguente:

   `\w+-\w+-C([0-9]+)`

   Oppure

   `\w+-\w+-C(\d+)`

   Ricorda che queste espressioni sono solo esempi. Potete creare le espressioni regolari in base alle vostre esigenze.

   >[!NOTE]
   >
   >Se la combinazione di espressioni regolari in righe e colonne non è in grado di determinare la posizione della risorsa all’interno della matrice del set 360 gradi multidimensionale, tale risorsa non viene aggiunta al set. Errore registrato.

1. Per Imposta convenzione di denominazione e creazione, specificate il suffisso o il prefisso del nome base definito nella convenzione di denominazione delle risorse. Definisci anche dove viene creato il set di immagini nella struttura di cartelle di Adobe Dynamic Media Classic.

   Se definisci un numero elevato di Set di immagini, mantieni questi set separati dalle cartelle che contengono le risorse stesse. Molti clienti creano una cartella Set di immagini e reindirizzano l’applicazione per inserire qui i set generati da set di batch.

1. Seleziona **[!UICONTROL Salva]** nel pannello Dettagli.
1. Carica e pubblica il set 360 gradi come di consueto, assicurandoti di attivare il nome del set 360 gradi 2D nella finestra di dialogo Opzioni caricamento processo, in Predefiniti set di batch.

>[!MORELIKETHIS]
>
>* [Anteprima di una risorsa](previewing-asset.md#previewing_an_asset)
>* [Configura predefiniti immagine](setting-image-presets.md#setting_up_image_presets)
>* [Visualizzare, aggiungere ed esportare i metadati](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Verifica file di processo](checking-job-files.md#checking_job_files)
