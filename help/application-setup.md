---
title: Impostazione applicazione
description: Scopri come configurare e configurare l’area Applicazione di Adobe Dynamic Media Classic. L’area Applicazione consente di specificare le impostazioni generali, creare predefiniti per la codifica di immagini, visualizzatori e video, definire visualizzatori e metadati predefiniti, le impostazioni di pubblicazione e le impostazioni SEO video. È inoltre possibile utilizzare l’area per impostare i predefiniti per set di batch per automatizzare la generazione di set 360 gradi 2D.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '11299'
ht-degree: 41%

---

# Impostazione applicazione{#application-setup}

Puoi utilizzare le pagine Impostazione applicazione per specificare le impostazioni generali, creare predefiniti per immagini, predefiniti di codifica video, predefiniti visualizzatore o per definire visualizzatori predefiniti e metadati. Puoi impostare i predefiniti per set di batch per automatizzare anche la generazione di set 360 gradi 2D (ad esempio), le impostazioni di pubblicazione e le impostazioni SEO video.

>[!NOTE]
>
>Solo gli amministratori di Adobe Dynamic Media Classic possono modificare le impostazioni nelle pagine Configurazione applicazione.

## Impostazioni generali {#general-settings}

Per aprire la pagina Impostazioni generali applicazione, nella barra di navigazione globale passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali]**.

### Server

Al momento della creazione dell’account, Adobe Dynamic Media Classic fornisce automaticamente i server assegnati all’azienda. I server vengono utilizzati per generare stringhe URL per il proprio sito Web e le applicazioni. Tali chiamate URL sono specifiche dell’account utente.

Vedi anche [Test del servizio Secure Testing](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL Nome server pubblicato]** - Questo server è il server CDN (Content Deliver Network) live utilizzato in tutte le chiamate URL generate dal sistema specifiche per il tuo account. Non modificare il nome del server a meno che non venga richiesto da un tecnico del supporto Adobe Dynamic Media Classic.

* **[!UICONTROL Nome server di origine]** - Questo server viene utilizzato solo per i test di controllo della qualità. Non modificare il nome del server a meno che non venga richiesto da un tecnico del supporto Adobe Dynamic Media Classic.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Nome server Test&amp;Target]** - L’URL di Test&amp;Target, fino a .com incluso. Per istruzioni su come ottenere questo URL, consulta Integrazione [!DNL Adobe Dynamic Media Classic] con [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL Nome server di streaming iOS]** - L’URL della [!DNL Adobe Dynamic Media Classic] Server di streaming iOS. Questo server distribuisce i video in streaming ai dispositivi basati su iOS utilizzando il protocollo HTTP.

* **[!UICONTROL Nome server video progressivo]** - L’URL della [!DNL Adobe Dynamic Media Classic] server video progressivo. Questo server distribuisce i video progressivi mediante il protocollo HTTP.

* **[!UICONTROL Mostra URL per le risorse non pubblicate]** - Selezionare questa opzione se si desidera [!DNL Adobe Dynamic Media Classic] per visualizzare un URL durante l’anteprima di una risorsa, pubblicata o meno. Se la risorsa non è pubblicata, l’URL non funziona. Tuttavia, potete utilizzare l’URL a scopo di progettazione o organizzazione.

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL Modello di annullamento validità CDN]** - Specifica il modello utilizzato per annullare la validità della cache CDN (Content Delivery Network).

   Ad esempio, supponiamo di inserire un URL immagine (inclusi predefiniti immagine o modificatori) che fa riferimento a `<ID>`, invece di un ID immagine specifico come nell&#39;esempio seguente:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   Se il modello contiene solo `<ID>`, quindi Adobe Dynamic Media Classic compila il `https://<server>/is/image`, dove `<server>` è il nome del server di pubblicazione definito in Impostazioni generali.

   Impostare il modello di annullamento validità CDN, selezionare un&#39;immagine denominata Zaino_B, quindi passare a **[!UICONTROL File]** > **[!UICONTROL Annulla validità CDN]** si traduce nel seguente URL generato nell’interfaccia di annullamento validità CDN:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   Nella casella di riepilogo URL, seleziona **[!UICONTROL Continua]** per cancellare la cache per la chiamata URL immagine specifica. Puoi anche aggiungere URL digitandoli o incollandoli nella casella di riepilogo URL; non è necessario impostare il modello in anticipo.

   Dopo aver selezionato il modello di annullamento validità CDN e aver effettuato una richiesta di annullamento validità CDN, viene visualizzato un indicatore nell’interfaccia utente. Fornisce una stima di quanto tempo ci vuole per cancellare la cache.

   Analogamente, se in Adobe Dynamic Media Classic sono selezionate più immagini quando si passa a **[!UICONTROL File]** > **[!UICONTROL Annulla validità CDN]**, nell’URL del modello salvato viene fatto riferimento a ogni immagine. Di conseguenza, puoi definire un modello di annullamento validità CDN facendo riferimento a ciascun URL a cui si fa riferimento sul sito web (ad esempio dettagli del prodotto e risultati di ricerca). Quindi, quando selezioni una o più immagini della cache di cui annullare la validità, gli URL compilano automaticamente l’interfaccia.

   Consultate [Memorizzazione dei contenuti nella cache](dmc-platform-overview.md#content_caching).

   Consultate [Risorse ripubblicate e ritardi CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Sfoglia

* **[!UICONTROL Mostra progetti]** - Determina se i progetti sono disponibili come mezzo per organizzare le risorse Adobe Dynamic Media Classic. Vedi [Organizzare il lavoro con i progetti](/help/organizing-projects.md).

* **[!UICONTROL Mostra contenuti eVideo di esempio]** - Attivare o disattivare la visualizzazione dei contenuti di esempio eVideo.

* **[!UICONTROL Mostra contenuto generato]** - Nelle cartelle mostra il contenuto generato da una risorsa. Ad esempio, quando un file PDF viene rasterizzato durante il caricamento, Adobe Dynamic Media Classic crea un’immagine per ogni pagina del PDF originale. Se l’opzione Mostra contenuto generato è selezionata, ogni immagine generata durante il caricamento del PDF originale viene visualizzata insieme al PDF nella cartella in cui questo è stato caricato.

* **[!UICONTROL Mostra video codificati]** - Deselezionato (disattivato) per impostazione predefinita.

   Per cercare e sfogliare rapidamente i video in Adobe Dynamic Media Classic senza dover navigare attraverso numerosi derivati codificati dello stesso video, lascia deselezionata questa opzione (impostazione predefinita). Vengono visualizzate solo la miniatura del video principale (il video sorgente caricato e utilizzato per creare i derivati) e la miniatura del set video adattivo &quot;principale&quot; (che contiene i derivati &quot;secondari&quot; del set video codificato).

   Tuttavia, è comunque possibile accedere a singoli video codificati dal video principale o dal set video adattivo. A questo scopo, fate doppio clic sulla miniatura del video per aprire la visualizzazione Dettagli. Quindi seleziona **[!UICONTROL Video codificati]** nel pannello di destra per accedere a tutti i video &quot;secondari&quot;.

   Puoi anche andare a **[!UICONTROL File]** > **[!UICONTROL Rielaborazione]** per creare video &quot;figlio&quot; più codificati direttamente da un set video adattivo. Adobe Dynamic Media Classic trova automaticamente il video principale del set di video adattivi e lo utilizza come video sorgente per la transcodifica. Quando salvate i nuovi video codificati, tuttavia, questi non vengono visti nelle operazioni di ricerca o navigazione. Sono comunque accessibili dalla scheda Video codificati in visualizzazione Dettagli.

   Vedi [Caricare e transcodificare video](uploading-encoding-videos.md#uploading_and_encoding_videos).

   Per poter accedere a tutte le versioni derivate codificate durante la ricerca e la navigazione, selezionate **[!UICONTROL Mostra video codificati]**.

   Alcune azioni nel menu Genera funzionano solo o eventualmente con singoli video. Questa funzionalità rende necessaria la visualizzazione di tutte le versioni derivate di video codificati disponibili per la selezione, a prescindere dall’impostazione di **[!UICONTROL Mostra video codificati]**. Azioni di generazione che sovrascrivono il **[!UICONTROL Mostra video codificati]** impostazione **[!UICONTROL Set video adattivi]** e **[!UICONTROL eCatalogs]**.

   >[!NOTE]
   >
   >Se non hai utilizzato Adobe Dynamic Media Classic per caricare e codificare le risorse video, Adobe Dynamic Media Classic mostra tutti i singoli video codificati, anche se questa opzione è deselezionata.

* **[!UICONTROL Pulsante Visualizza sottocartelle]** - Attivare o disattivare la visualizzazione del pulsante Aggiorna sottocartelle.

### Account FTP Adobe Dynamic Media Classic

* **[!UICONTROL Server]** - Elenca il server account FTP.

* **[!UICONTROL Nome utente]** - Elenca il nome utente dell&#39;account FTP.

### Carica nell’applicazione

Vedi anche [Opzioni del processo di caricamento predefinite](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS) video di formazione.

* **[!UICONTROL Sovrascrivi immagini]** - Adobe Dynamic Media Classic non consente a due file di avere lo stesso nome. L’ID Adobe Dynamic Media Classic di ogni elemento (il nome dell’immagine meno l’estensione del nome del file) deve essere univoco. In virtù di questa regola, nella finestra di dialogo Carica è disponibile l’opzione Sovrascrivi. Il risultato effettivo di questa opzione dipende dal valore impostato per l’opzione Sovrascrivi immagini. È possibile specificare come caricare le immagini sostitutive, ossia se devono sostituire le immagini originali o diventare duplicati di tali immagini. Le immagini duplicate vengono rinominate con il suffisso “-1” (ad esempio, il file sedia.tif viene rinominato sedia-1.tif). Queste opzioni interessano le immagini caricate in una cartella diversa da quella degli originali o le immagini con una diversa estensione file (ad esempio, JPG, TIF o PNG). Vedi [Utilizzare l’opzione Sovrascrivi immagini](#using-the-overwrite-images-option).

   * **[!UICONTROL Sovrascrivi nella cartella corrente, nome/estensione dell&#39;immagine di base]** - Questa opzione è la regola più rigida per la sostituzione. Richiede che l’immagine sostitutiva sia caricata nella stessa cartella dell’immagine originale e che abbia la stessa estensione del nome file dell’originale. Se entrambi i requisiti non vengono soddisfatti, viene creata una copia dell’immagine.

   * **[!UICONTROL Sovrascrivi nella cartella corrente, lo stesso nome della risorsa di base indipendentemente dall&#39;estensione]** - Richiede di caricare l&#39;immagine sostitutiva nella stessa cartella dell&#39;originale, tuttavia l&#39;estensione del nome file può essere diversa dall&#39;originale. Ad esempio, sedia.tif sostituisce sedia.jpg.

   * **[!UICONTROL Sovrascrivi in qualsiasi cartella, stesso nome/estensione della risorsa di base]** - Richiede che l&#39;immagine sostitutiva abbia la stessa estensione del nome del file dell&#39;immagine originale (ad esempio, sedia.jpg deve sostituire sedia.jpg, non sedia.tif). Tuttavia, è possibile caricare l’immagine sostitutiva in una cartella diversa da quella dell’originale. L’immagine aggiornata sarà contenuta nella nuova cartella e il file verrà rimosso dal percorso originale.

   * **[!UICONTROL Sovrascrivi in qualsiasi cartella, lo stesso nome della risorsa di base indipendentemente dall’estensione]** - Questa opzione è la regola di sostituzione più inclusiva. L’immagine sostitutiva può essere caricata in una cartella diversa da quella dell’originale, con una diversa estensione file, e sostituire il file originale. Se il file originale si trova in un’altra cartella, l’immagine sostitutiva sarà contenuta nella nuova cartella nella quale è stata caricata.

* **[!UICONTROL Mantieni pubblicazione]** - Specifica se un&#39;immagine sostitutiva caricata in Adobe Dynamic Media Classic conserva l&#39;impostazione Ready to Publish dell&#39;immagine che sta sostituendo, oppure se l&#39;impostazione è specificata al momento del caricamento.

* **[!UICONTROL Profili colore predefiniti]** - Specifica i profili di colore applicati come parte delle Opzioni profilo colore predefinito quando si aggiungono immagini CMYK.

* **[!UICONTROL Opzioni di caricamento predefinite]** - Apre la finestra di dialogo Opzioni processo di caricamento, in cui è possibile specificare le opzioni di caricamento predefinite. Per informazioni su queste opzioni, consultate [Opzioni di caricamento](/help/uploading-files.md#upload_options).

### Editor mappa immagine, su applicazione

* **[!UICONTROL HREF di mappatura immagine predefinito]** - Definisce l&#39;URL predefinito utilizzato per la colonna HREF nel mapping delle immagini. Questo URL è l’URL predefinito visualizzato quando create le mappe immagine.

* **[!UICONTROL Modello di mappatura immagine predefinito]** - Definisce il JavaScript predefinito per il modello HREF nel mapping delle immagini. Puoi impostare un codice personalizzato da eseguire qui ogni volta che selezioni una mappa immagine.

### Altre impostazioni, su applicazione

* **[!UICONTROL Il Cestino Può Pulire Gli Avvisi]** - Le risorse nel cestino vengono rimosse automaticamente entro sette giorni. Selezionate “Invia e-mail prima che gli elementi nel cestino siano eliminati automaticamente” se desiderate che vengano inviate notifiche agli amministratori dell’azienda quattro giorni prima che le risorse nel cestino vengano definitivamente eliminate. Vedi [Gestire la cartella Cestino](/help/trash-folder.md).

## Utilizzare l’opzione Sovrascrivi immagini {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic non consente a due file di avere lo stesso nome. L’ID Adobe Dynamic Media Classic di ogni elemento (il nome dell’immagine meno l’estensione del nome del file) deve essere univoco. In virtù di questa regola, nella finestra di dialogo Carica è disponibile l’opzione Sovrascrivi immagini. L&#39;effetto esatto di questa opzione dipende da un&#39;impostazione per le impostazioni interne Adobe Dynamic Media Classic di ciascuna azienda.

Se in precedenza hai caricato le immagini e poi le hai modificate (o sostituite), l’opzione Sovrascrivi selezionata specifica in che modo Adobe Dynamic Media Classic sostituisce le immagini. I dati relativi all’immagine non vengono modificati, ma la nuova immagine sostituisce la precedente. Se la cartella contiene anche immagini che non sono già presenti in Adobe Dynamic Media Classic, queste vengono aggiunte.

Utilizza questa opzione se le immagini caricate sono cambiate in qualche modo (l’immagine è stata modificata) ma il riferimento all’immagine rimane lo stesso. L’opzione Sovrascrivi è utile anche quando si caricano e si estraggono dati da file Adobe® PDF. Ottimizzazione di Adobe Dynamic Media Classic *strisce* nell’immagine, regola le opzioni del profilo colore ICC nella finestra di dialogo Carica e ricarica utilizzando la funzione Sovrascrivi.

Gli ID Adobe Dynamic Media Classic utilizzati per accedere alle immagini dai server di produzione sono derivati dai nomi dei file immagine. L’utilizzo di caratteri maiuscoli e minuscoli nel nome file è importante sia per la sostituzione dei file esistenti che per gli ID Adobe Dynamic Media Classic utilizzati per accedere all’immagine. Assicurati che l’uso di caratteri maiuscoli e minuscoli nei nomi dei file sia corretto prima di caricarli in Adobe Dynamic Media Classic, per evitare ID Adobe Dynamic Media Classic che differiscono solo nel caso della stessa immagine.

Se deselezionate questa opzione, tutte le immagini con lo stesso nome file delle immagini esistenti vengono considerate copie e non vengono aggiunte.

## Predefiniti immagine {#image-presets}

Nella schermata Predefiniti immagine è possibile creare e modificare i predefiniti per le immagini. I predefiniti per immagini consentono a Adobe Dynamic Media Classic di distribuire le immagini in modo dinamico a diverse dimensioni rispetto alla stessa immagine primaria. Ogni predefinito immagine rappresenta una raccolta predefinita di comandi di ridimensionamento e formattazione per la visualizzazione delle immagini. Quando crei un predefinito per immagini, selezioni una dimensione per la distribuzione delle immagini. È inoltre possibile selezionare i comandi di formattazione in modo che l&#39;aspetto dell&#39;immagine sia ottimizzato quando l&#39;immagine viene consegnata per la visualizzazione.

Gli amministratori possono creare predefiniti per l’esportazione delle risorse. Gli utenti possono scegliere un predefinito al momento dell’esportazione delle immagini, che riformatta anche le immagini in base alle specifiche specificate dall’amministratore.

Per aprire la schermata Predefinito immagine, nella barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**.

Vedi [Smart imaging](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

### Creare e modificare i predefiniti immagine {#creating-and-editing-image-presets}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**.
1. Crea un predefinito o inizia da uno esistente:

   * **Creare un predefinito per immagini** - Seleziona **[!UICONTROL Aggiungi]**.
   * **Creare un predefinito per immagini da un predefinito esistente** - Seleziona il predefinito per immagini più simile a quello che desideri creare, quindi seleziona **[!UICONTROL Modifica]**.

1. Nella pagina Aggiungi (o Modifica) predefinito , immetti un nome per il predefinito.
1. Impostate le opzioni desiderate. 

   Consultate [Opzioni dei predefiniti immagine](application-setup.md#image_preset_options).

1. Seleziona **[!UICONTROL Salva]** oppure, se hai iniziato da un predefinito esistente, seleziona **[!UICONTROL Salva con nome]**.
1. Per visualizzare in anteprima il predefinito con la tua immagine, seleziona **[!UICONTROL Sfoglia]** quindi selezionate un&#39;immagine. Per visualizzare in anteprima l’immagine predefinita, seleziona **[!UICONTROL Reimposta]**.

Per modificare un predefinito immagine, selezionane il nome nella schermata Predefiniti immagine e seleziona **[!UICONTROL Modifica]**. Per eliminare un predefinito immagine, selezionalo e seleziona **[!UICONTROL Elimina]**.

### Opzioni dei predefiniti immagine {#image-preset-options}

Nelle schermate Aggiungi predefinito e Modifica predefinito sono disponibili le seguenti opzioni per creare e modificare i predefiniti immagine:

* **[!UICONTROL Nome predefinito]** - Immettere un nome descrittivo senza spazi vuoti. Per aiutare gli utenti a identificare questo predefinito per immagini, includi nel nome la specifica della dimensione dell’immagine.

* **[!UICONTROL Larghezza e altezza]** - Immettere in pixel le dimensioni in cui l&#39;immagine viene distribuita.

* **[!UICONTROL Formato]** - Selezionare un formato dal menu. La scelta del formato GIF, JPEG, PDF o TIFF offre ulteriori opzioni:

   * Opzioni Quantizzazione colore GIF

      * **[!UICONTROL Tipo]** - Selezionare Adattivo (il valore predefinito), Web o Macintosh. Se si seleziona **[!UICONTROL GIF con Alpha]**, l’opzione Macintosh non è disponibile.

      * **[!UICONTROL Dither]** - Selezionare Diffusa o Disattivata.

      * **[!UICONTROL Numero di colori]** - Trascinare il cursore per inserire 2-255.

      * **[!UICONTROL Elenco colori]** - Inserire un elenco separato da virgole. Ad esempio, per bianco, grigio e nero inserite `000000,888888,ffffff`.
   * Opzioni JPEG

      * **[!UICONTROL Qualità]** - Controlla il livello di compressione JPEG. Questa impostazione interessa sia le dimensioni del file che la qualità dell’immagine. La scala di qualità JPEG è 1-100.

      * **[!UICONTROL Abilita il downsampling della crominanza di JPG]** - Poiché l&#39;occhio è meno sensibile alle informazioni sui colori ad alta frequenza rispetto alla luminanza ad alta frequenza, le immagini JPEG dividono le informazioni sulle immagini in componenti luminanza e colore. Quando un’immagine JPEG viene compressa, il componente della luminanza viene lasciato alla massima risoluzione, mentre per i componenti colore viene eseguito il downsampling calcolando la media di gruppi di pixel. Il downsampling riduce di metà o un terzo il volume di dati, con impatto trascurabile sulla qualità percepita. Non è possibile eseguire il downsampling sulle immagini in scala di grigio. Questa tecnica riduce il fattore di compressione ed è utile per le immagini ad alto contrasto (ad esempio, immagini con testo sovrapposto).
   * Opzioni PDF e TIFF

      * **[!UICONTROL Compressione]** - Selezionare un algoritmo di compressione.



* **[!UICONTROL Spazio colore]** - Selezionare uno spazio colore.

* **[!UICONTROL Nitidezza]** - Selezionare l&#39;opzione Abilita nitidezza semplice per applicare un filtro di nitidezza di base all&#39;immagine dopo che è stata effettuata la modifica in scala. La nitidezza contribuisce a compensare la sfocatura che può prodursi quando si visualizza un’immagine in dimensioni diverse.

   Per ulteriori informazioni sulla nitidezza, le modalità di ricampionamento e la maschera di contrasto, consulta [Rendere più nitida un’immagine](sharpening-image.md#sharpening_an_image). Vedi anche [Nitidezza](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) video di formazione.

* **[!UICONTROL Modalità di campionamento]** - Selezionare un&#39;opzione in modalità di ricampionamento. Queste opzioni aumentano la nitidezza quando si esegue il downsampling dell’immagine:

* **[!UICONTROL B-Lineare]** - il metodo di ricampionamento più veloce; alcuni artefatti di aliasing sono evidenti.

* **[!UICONTROL Bi-Cubic]** - Aumenta l&#39;utilizzo della CPU sul server di immagini, ma produce immagini più nitide con artefatti di aliasing meno evidenti.

* **[!UICONTROL Sharp2]** - Può produrre risultati leggermente più nitidi rispetto all&#39;opzione Bi-Cubic, ma a costi di CPU ancora più elevati sul server di immagini.

* **[!UICONTROL Trilineare]** - utilizza risoluzioni sia superiori che inferiori, se disponibili; consigliato solo quando l’aliasing è un problema. Questo metodo riduce le dimensioni JPEG grazie a una minore quantità di dati ad alta frequenza.

* **[!UICONTROL Maschera definizione dettagli]** - Scegliere le seguenti opzioni per ottimizzare la nitidezza:

* **[!UICONTROL Importo]** - Controlla la quantità di contrasto applicata ai pixel del bordo. Il valore predefinito è 1,0. Per le immagini ad alta risoluzione, è possibile aumentare questo valore fino a 5,0. Il fattore può essere interpretato come una misura dell’intensità del filtro.

* **[!UICONTROL Raggio]** - Determina il numero di pixel intorno ai pixel del bordo che influiscono sulla nitidezza. Per immagini ad alta risoluzione, inserite un valore da 1 a 2. Con un valore basso si agisce solo sui pixel del bordo; con un valore più elevato si agisce su una fascia più ampia di pixel. Il valore più adatto dipende dalle dimensioni dell’immagine.

* **[!UICONTROL Soglia]** - Determina l&#39;intervallo di contrasto da ignorare quando viene applicato il filtro Maschera definizione dettagli. In altre parole, questa opzione specifica quale deve essere il grado di differenza dei pixel da rendere più nitidi rispetto all’area circostante, affinché vengano considerati pixel di un bordo e quindi resi più nitidi. Per evitare la comparsa di disturbi, provate con valori compresi tra 0,02 e 0,2. Con il valore predefinito 6 la nitidezza viene applicata a tutti i pixel nell’immagine.

* **[!UICONTROL Spazio colore]** - Determina se l&#39;immagine utilizza lo spazio in cui è stata creata, in genere RGB (Originale) o uno spazio di luminanza (Intensità).

* **[!UICONTROL Colore]** Scegli le seguenti opzioni:

* **[!UICONTROL Profilo colore di uscita]** - Seleziona **[!UICONTROL Usa predefinito]** o uno dei profili di colore ICC disponibili su Adobe Dynamic Media Classic.

   Consultate anche [Profili ICC](icc-profiles.md#icc_profiles).

* **[!UICONTROL Intento di rendering]** - Seleziona un’opzione se desideri ignorare l’intento di rendering predefinito del profilo colore. Utilizza questa opzione quando uno dei profili ICC predefiniti è lo spazio colore di destinazione di una conversione di colore. Oppure, una periferica di output (stampante o monitor) è caratterizzata da questo profilo e l&#39;intento di rendering specificato è valido per questo profilo.

* **[!UICONTROL Incorpora profilo]** - Selezionare questa opzione in modo che, se si apre questa immagine in Adobe® Photoshop®, utilizzi questo profilo.

* **[!UICONTROL Risoluzione di stampa]** - Selezionare una risoluzione per stampare l&#39;immagine; Il valore predefinito è 72 pixel.

* **[!UICONTROL Modificatori URL]** - Se preferisci specificare i modificatori URL che definiscono il predefinito immagine, anziché le impostazioni, immetti qui i modificatori .

* **[!UICONTROL URL immagine di esempio]** - Elenca la stringa URL &quot;grezza&quot; utilizzata da Dynamic Media Image Server per fornire le immagini con il predefinito immagine che si sta aggiungendo o modificando. Questa stringa URL codifica tutte le impostazioni di formato selezionate nella schermata Aggiungi predefinito o Modifica predefinito .

### Modificare, rimuovere o disattivare un predefinito immagine {#editing-removing-or-deactivating-an-image-preset}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**.
1. Nella schermata Predefiniti immagine, selezionate un predefinito nella tabella ed effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Modifica]** e quindi specificare nuove opzioni nella finestra di dialogo Modifica predefinito.
   * Seleziona **[!UICONTROL Elimina]** per rimuovere il predefinito dall&#39;elenco.
   * Deseleziona la **[!UICONTROL Attivo]** casella di controllo accanto a un nome predefinito se desideri rimuoverlo dall&#39;intera interfaccia utente di Adobe Dynamic Media Classic per gli utenti di MediaPortal.

## Attivare o disattivare i predefiniti video adattivi {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic offre predefiniti di codifica per video adattivi. Si tratta di un elenco principale di predefiniti che combina in un unico gruppo sia i predefiniti video adattivi 16:9 che i predefiniti video adattivi 4:3. Tali predefiniti riflettono le impostazioni di codifica più comuni e sono ottimizzati per la riproduzione su dispositivi mobili, tablet e computer desktop.

Solo i predefiniti di codifica video adattiva sono attivati (o “abilitati”) per impostazione predefinita. Se necessario, potete disattivarli. I predefiniti per video adattivi non attivati non vengono visualizzati come opzione selezionabile nella sezione eVideo della finestra di dialogo Opzioni processo di caricamento.

Vedi [Caricare e codificare video](uploading-encoding-videos.md#uploading_and_encoding_videos).

Vedi anche [Predefiniti video](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) video di formazione.

**Per attivare o disattivare i predefiniti video adattivi:**

1. Nell&#39;angolo in alto a destra di Adobe Dynamic Media Classic, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti video]** > **[!UICONTROL Predefiniti video adattivi]**.
1. Nella pagina Predefiniti video adattati, deselezionate la casella di controllo accanto al nome di un predefinito per eliminarlo dall’elenco Opzioni eVideo nella finestra di dialogo Opzioni processo di caricamento.
1. Seleziona **[!UICONTROL Chiudi]**.

## Predefiniti video per la codifica di file video {#video-presets-for-encoding-video-files}

Per selezionare un predefinito di codifica, seleziona nell’angolo inferiore destro della pagina Carica **[!UICONTROL Opzioni processo]**. Nella finestra di dialogo Opzioni processo di caricamento , espandi Opzioni eVideo e seleziona i predefiniti di codifica video desiderati.

>[!NOTE]
>
>Ad eccezione di &quot;Adaptive Video&quot;, che è abilitato per impostazione predefinita, non è possibile visualizzare tutti gli altri predefiniti di codifica video adattivo o video singolo nella finestra di dialogo Opzioni processo di caricamento. Gli amministratori di Adobe Dynamic Media Classic determinano quali predefiniti di codifica video sono visibili nella finestra di dialogo Opzioni processo di caricamento .

* Seleziona uno dei seguenti predefiniti di codifica video adattiva o di codifica singola:

   * **[!UICONTROL Video adattivo 16:9]** - Crea video con rapporto di formato 16:9 per la distribuzione su desktop, dispositivi mobili (iPhone, iPad, Android™) e tablet (iPad, Android™), ottimizzati con la risoluzione e il bit rate che meglio corrispondono alla velocità di connessione del visualizzatore.

   * **[!UICONTROL Video adattivo 4:3]** - Crea video con rapporto di formato 4:3 per la distribuzione su desktop, dispositivi mobili (iPhone, iPad, Android™) e tablet (iPad, Android™), ottimizzati con risoluzione e bit rate che corrispondano meglio alla velocità di connessione del visualizzatore.

   * **[!UICONTROL Video adattivo]** - Un singolo predefinito di codifica che funziona con qualsiasi proporzione per creare video da distribuire a dispositivi mobili, tablet e desktop. I video sorgente caricati e codificati con questo predefinito sono impostati su un’altezza specifica. Tuttavia, il valore della larghezza viene ridimensionato automaticamente per mantenere le proporzioni del video.

      La flessibilità di questo ridimensionamento automatico è disponibile anche per impostazione predefinita quando create un predefinito di codifica video personalizzato.

      Vedi [Aggiungere o modificare un predefinito di codifica video](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL Codifica video adattiva (16:9 o 4:3)]** - Crea video con rapporto di formato 16:9 e 4:3 per la distribuzione su desktop, dispositivi mobili (iPhone, iPad, Android™) e tablet (iPad, Android™). Tutto ottimizzato con la risoluzione e il bit rate che meglio corrispondono alla velocità di connessione del visualizzatore.

      Consultate [Predefiniti per codifica video adattiva (16:9 o 4:3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   * **[!UICONTROL Predefiniti codifica singola]**

      >[!NOTE]
      >
      >Per inviare un video agli iPad, puoi selezionare un predefinito di codifica Mobile o un predefinito di codifica Tablet . I predefiniti Tablet sono stati creati appositamente per gli iPad, generalmente con risoluzione e qualità più alta per usufruire delle dimensioni delle schermo e della connessione di banda più elevata. La visualizzazione di file video codificati con un predefinito Tablet richiede di includere un codice di rilevamento dispositivi al sito mobile o all’applicazione. questo codice è disponibile per i video visualizzati su iPhone o iPad, a seconda del dispositivo di riproduzione. Se si sceglie un predefinito Mobile per la consegna dei file video ad iPad, il flusso di lavoro risulta semplificato poiché potete scegliere lo stesso file video sia per iPhone che per iPad. Tuttavia, la qualità viene standardizzata all’esperienza iPhone con risoluzione ridotta.

      * Nel gruppo Predefiniti di codifica, nell’elenco a discesa Ordina predefiniti codifica, selezionate Nome o Dimensioni per ordinare i predefiniti per nome o per dimensione di risoluzione.
      * Seleziona un predefinito di codifica in base alle dimensioni della risoluzione e alla larghezza di banda con cui intendi riprodurre il video.
      * È possibile selezionare Codifica video adattiva e uno o più predefiniti di codifica per video. Ad esempio, potete codificare un file per desktop e dispositivo mobile in un unico processo di caricamento.

Dopo aver selezionato **[!UICONTROL Avvia caricamento]**, il file video principale originale viene caricato e i file codificati vengono generati dal file principale.

### Le opzioni dei predefiniti di codifica {#about-encoding-preset-options}

I parametri delle opzioni dei predefiniti di codifica sono i seguenti:

* **[!UICONTROL Velocità di connessione di destinazione]** - La velocità di connessione Internet dell&#39;utente finale di destinazione.

* **[!UICONTROL Suffisso file codificato]** - Il suffisso allegato al file video codificato a scopo di identificazione.

* **[!UICONTROL Bit rate video (velocità dati)]** - La quantità di dati codificati per creare un secondo di riproduzione video (in kilobit al secondo).

* **[!UICONTROL Larghezza/Altezza pixel]** - Dimensione della larghezza dell&#39;immagine dello schermo, in pixel; la dimensione in altezza dell’immagine dello schermo (in pixel).

* **[!UICONTROL Frame al secondo (fps)]** - Il numero di fotogrammi, o immagini fisse, per ogni secondo di video. Negli Stati Uniti e in Giappone, i video sono solitamente ripresi a 29,97 fps; in Europa e in Asia (escluso il Giappone), sono invece ripresi a 25 fps. I film sono ripresi a 24 fps.

* **[!UICONTROL Bit rate audio]** - La quantità di dati codificati per creare un secondo di riproduzione audio, espressa in kilobit al secondo.

Le tabelle di seguito indicano le procedure ottimali per la scelta dei predefiniti per video e le convenzioni di denominazione utilizzate per designare i file codificati.

### Video adattivo (predefinito) {#adaptive-video-default}

Per creare video da distribuire a dispositivi mobili, tablet e computer desktop; predefinito di codifica che funziona con qualsiasi proporzione. I video sorgente caricati e codificati con questo predefinito (per impostazione predefinita e procedura ottimale) sono impostati su un’altezza specifica, ma il valore della larghezza viene ridimensionato automaticamente per mantenere le proporzioni del video.

**Video adattivo (predefinito)**

|  | Nome predefinito di codifica/Descrizione | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto x360, 800 Kbps | _Mobile_Autox360p_800K | 800 | Auto x360 | Come sorgente | 64 | Per dispositivi mobili (iPhone, iPad, Android™) |
| 2 | Auto x480, 1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Auto x480 | Come sorgente | 96 | Per tablet (iPad, Android™) |
| 3 | Auto x720, 2600 Kbps | _Desktop_Autox720p_2600K | 2600 | Auto x720 | Come sorgente | 128 | Per desktop |

### Predefiniti per codifica video adattiva (16:9 o 4:3) {#adaptive-video-encoding-or-video-presets}

Di seguito sono elencati i predefiniti di codifica disponibili per video adattivi; combinano una serie di singoli predefiniti di codifica selezionati automaticamente in base alle proporzioni del video caricato. Ad esempio, se carichi un video 4:3, questo viene codificato automaticamente utilizzando tutti e cinque i predefiniti 4:3 presenti nell’elenco dei predefiniti principali nel **Codifica video adattiva (16:9 o 4:3)** opzione .

Per informazioni sui parametri delle opzioni di codifica, consultate [Le opzioni dei predefiniti di codifica](application-setup.md#about_encoding_preset_options).

**Predefiniti per codifica video adattiva (16:9 o 4:3)**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512x288 | Come sorgente | 64 | Risoluzione media, 3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_384x288_600 | 600 | 384 x 288 | Come sorgente | 64 | Risoluzione media, 3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640x360 | Come sorgente | 80 | Risoluzione media, WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640x480 | Come sorgente | 80 | Risoluzione media, WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android™), (1200 Kbps)` | 1,5 Mbps | _iPad_768x432_1200K | 1200 | 768x432 | Come sorgente | 96 | Alta risoluzione, WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android™), (1200 Kbps)` | 1,5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | Come sorgente | 96 | Alta risoluzione, WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Come sorgente | 128 | Widescreen ad alta definizione |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3,0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | Come sorgente | 128 | Alta definizione |

### Predefiniti di codifica video per computer desktop {#desktop-video-encoding-presets}

Predefiniti di codifica video per MP4 e OGV su computer desktop.

Per informazioni sui parametri delle opzioni di codifica, consultate [Le opzioni dei predefiniti di codifica](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2 - Audio AAC - Estensione MP4**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | Come sorgente | 64 | Widescreen a bassa risoluzione |
| 2 | 16:9, 640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640 x 360 | Come sorgente | 80 | Widescreen a risoluzione media |
| 3 | 16:9, 800x450 (1200 Kbps) | 1,5 Mbps | _800x450_1200K | 1200 | 800x450 | Come sorgente | 96 | Risoluzione medio-alta |
| 4 | 16:9, 1280x720 (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Come sorgente | 128 | Widescreen ad alta definizione |
| 5 | 4:3, 320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | Come sorgente | 64 | Bassa risoluzione |
| 6 | 4:3, 480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | Come sorgente | 80 | Risoluzione media |
| 7 | 4:3, 640x480 (1200 Kbps) | 1,5 Mbps | _640x480_1200K | 1200 | 640 x 480 | Come sorgente | 96 | Risoluzione medio-alta |
| 8 | 4:3, 1280x960 (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 | 1280x960 | Come sorgente | 128 | Alta definizione |

**OGG Vorbis Theora - Estensione OGV**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps), OGG | 500 | _OGG_480x270_400K | 400 | 480 x 270 | Come sorgente | 64 | Widescreen a bassa risoluzione |
| 2 | 16:9, 640x360 (800 Kbps), OGG | 900 | _OGG_640x360_800K | 800 | 640 x 360 | Come sorgente | 80 | Widescreen a risoluzione media |
| 3 | 16:9, 800x450 (1200 Kbps), OGG | 1,5 Mbps | _OGG_800x450_1200K | 1200 | 800 x 450 | Come sorgente | 96 | Risoluzione medio-alta |
| 4 | 16:9, 1280x720 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x720_2000K | 2000 | 1280x720 | Come sorgente | 128 | Widescreen ad alta definizione |
| 5 | 4:3, 320x240 (400 Kbps), OGG | 500 | _OGG_320X240_400K | 400 | 320 x 240 | Come sorgente | 64 | Bassa risoluzione |
| 6 | 4:3, 480x360 (800 Kbps), OGG | 900 | _OGG_480x360_800K | 800 | 480 x 360 | Come sorgente | 80 | Risoluzione media |
| 7 | 4:3, 640x480 (1200 Kbps), OGG | 1,5 Mbps | _OGG_640x480_1200K | 1200 | 640 x 480 | Come sorgente | 96 | Risoluzione medio-alta |
| 8 | 4:3, 1280x960 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x960_2000K | 2000 | 1280x960 | Come sorgente | 128 | Alta definizione |

### Predefiniti di codifica per video per dispositivi mobili {#mobile-video-encoding-presets}

Come fps sorgente. Predefiniti di codifica video per dispositivi mobili iPhone, iPad e Android™.

Per informazioni sui parametri delle opzioni di codifica, consultate [Le opzioni dei predefiniti di codifica](application-setup.md#about_encoding_preset_options).

**H264 Baseline 2.1 - Audio AAC - Estensione MP4**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Bitrate video (Kbps) | Larghezza/Altezza in pixel | Fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, Mobile (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 2 | 16:9, 512x288, Mobile (600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512x288 | Come sorgente | 64 | Risoluzione media, 3G |
| 3 | 16:9, 512x288, Mobile (800 Kbps) | 900 | _Mobile_512x288_800K | 800 | 512x288 | Come sorgente | 80 | Risoluzione media, Wi-Fi |
| 4 | 16:9, 512x288, Mobile (1000 Kbps) | 1,2 Mbps | _Mobile_512x288_1000K | 1000 | 512x288 | Come sorgente | 80 | Alta risoluzione, Wi-Fi |
| 5 | 16:9, 512x288, Mobile (1200 Kbps) | 1,5 Mbps | _Mobile_512x288_1200K | 1200 | 512x288 | Come sorgente | 96 | Alta risoluzione, Wi-Fi |
| 6 | 4:3, 384x288, Mobile (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 7 | 4:3, 384x288, Mobile (600 Kbps) | 700 | _Mobile_384x288_600K | 600 | 384 x 288 | Come sorgente | 64 | Risoluzione media, 3G |
| 8 | 4:3, 448x336, Mobile (800 Kbps) | 900 | _Mobile_448x336_800K | 800 | 448x336 | Come sorgente | 80 | Risoluzione media, Wi-Fi |
| 9 | 4:3, 448x336, Mobile (1000 Kbps) | 1,2 Mbps | _Mobile_448x336_1000K | 1000 | 448 x 336 | Come sorgente | 80 | Alta risoluzione, Wi-Fi |
| 10 | 4:3, 448x336, Mobile (1200 Kbps) | 1,5 Mbps | _Mobile_448x336_1200K | 1200 | 448 x 336 | Come sorgente | 96 | Alta risoluzione, Wi-Fi |

## Predefiniti per visualizzatori {#viewer-presets}

>[!NOTE]
>
>**Avviso sulla fine del ciclo di vita dei visualizzatori di Flash** - Dal 31 gennaio 2017, Adobe Dynamic Media Classic ha ufficialmente terminato il supporto per la piattaforma di visualizzazione dei Flash.

Un *predefinito per visualizzatori* è un gruppo di impostazioni con cui viene definito in che modo le risorse multimediali verranno visualizzate sullo schermo del computer e sui dispositivi mobili dell’utente. In qualità di amministratore, potete creare dei predefiniti per visualizzatori. Sono disponibili impostazioni per un’ampia gamma di opzioni di configurazione dei visualizzatori. Ad esempio, è possibile modificare le dimensioni dello schermo del visualizzatore, il comportamento dello zoom, gli schemi di colori, i bordi e i font.

Come best practice, utilizza i visualizzatori video Adobe Dynamic Media Classic HTML5. I predefiniti utilizzati nei visualizzatori Video HTML5 sono lettori video affidabili.

Combinando in un singolo player quanto segue:

* La possibilità di progettare i componenti per la riproduzione utilizzando HTML5 e CSS.
* Riproduzione incorporata.
* Utilizza lo streaming adattivo e progressivo a seconda delle funzionalità del browser.

Estendi la portata dei contenuti rich media agli utenti desktop, tablet e dispositivi mobili e assicurati un’esperienza video semplificata.

Vedi [Informazioni sui visualizzatori HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) nella Guida di riferimento visualizzatori di Adobi.

Vedi [Matrice di compatibilità dei predefiniti per visualizzatori Adobe Dynamic Media Classic](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Consultate [Procedura ottimale: utilizzo del visualizzatore video HTML5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

In base al visualizzatore, potete aggiungere delle funzioni per community. e comprendono i pulsanti Incorpora, E-mail, Collega e Visita. Questi pulsanti consentono agli utenti che utilizzano i visualizzatori di condividere il visualizzatore con altri utenti o di aprire il sito web Adobe Dynamic Media Classic.

Vedi anche [Esempi della libreria di riferimento visualizzatori di Adobi](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Supporto visualizzatore per pagine web reattive {#viewer-support-for-responsive-designed-web-pages}

Diversi tipi di pagine Web hanno esigenze differenti. A volte si desidera una pagina web che fornisca un collegamento che apre il visualizzatore HTML5 in una finestra separata del browser. In altri casi, è necessario incorporare il visualizzatore HTML5 direttamente nella pagina di hosting. In quest&#39;ultimo caso, la pagina web ha probabilmente un layout statico. Oppure, è &quot;reattivo&quot; e viene visualizzato in modo diverso su diversi dispositivi o per diverse dimensioni della finestra del browser. Per soddisfare queste esigenze, i visualizzatori HTML5 forniti con Adobe Dynamic Media Classic supportano sia le pagine web statiche che le pagine web reattive.

Per ulteriori informazioni su come incorporare i visualizzatori reattivi nelle pagine web, consulta [Informazioni sulla libreria di immagini reattive](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api), [Utilizzare la libreria di immagini reattive](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api)e [Riferimento comando - Attributi comando](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library).

### Tipi di predefiniti per visualizzatori {#viewer-preset-types}

Gli amministratori possono creare e personalizzare i seguenti tipi di predefiniti per visualizzatori.

* **[!UICONTROL Visualizzatore eCatalog]** - Simula l&#39;esperienza di lettura di un catalogo stampato. È possibile spostarsi da una pagina all’altra, ingrandire e ridurre gli elementi di una pagina, utilizzare mappe immagine per visualizzare ulteriori informazioni sugli elementi della pagina o cercare nel catalogo. Potete inoltre includere un pannello Info con le informazioni dettagliate su un articolo collegato a una mappa, se all’area della mappa è assegnato un attributo rollover_key valido. Per includere un pannello Info, specificate l’URL di un server informazioni nel riquadro Impostazioni pannello Info, nella finestra Predefinito visualizzatore eCatalog.

* **[!UICONTROL Visualizzatore set di campioni]** - Visualizza un&#39;immagine in un colore, materiale, texture, finitura o tessuto diverso. Per visualizzare le varianti dell’immagine, gli utenti selezionano una miniatura.

* **[!UICONTROL Visualizzatore set di file multimediali diversi]** - Visualizza diversi tipi di contenuti multimediali in un visualizzatore. Potete includere set di campioni, set 360 gradi, immagini e video. Potete configurare schede per diversi tipi di contenuto, ad esempio una scheda per i set di immagini e una scheda per i video. Per la riproduzione dei video da un set di file multimediali diversi viene usato un visualizzatore standard con un indicatore temporale e controlli per interrompere, mettere in pausa, riavvolgere e riprodurre il video. Quando configurate il predefinito per visualizzatori di un set di file multimediali diversi, specificate i visualizzatori da usare per i diversi tipi di risorse del set. Per visualizzare un set di file multimediali diversi potete anche usare il visualizzatore Griglia o Carosello.

* **[!UICONTROL Visualizzatore set 360 gradi]** - Fornisce più viste di un&#39;immagine in modo che gli utenti possano ruotare l&#39;oggetto per esaminare i diversi lati e angoli.

* **Visualizzatore video** - Visualizza i video utilizzando le dimensioni di risoluzione del file sorgente o una dimensione personalizzata. Adobe Dynamic Media Classic viene fornito con molti predefiniti per visualizzatori per la riproduzione di video e, se siete amministratori, potete creare predefiniti per visualizzatori video personalizzati. Sono disponibili più di 12 diverse impostazioni per la configurazione del visualizzatore video. Potete configurare la relativa dimensione, il colore di primo piano e di sfondo, i controlli audio e video, la barra di avanzamento, l’interfaccia utente, le funzioni per social networking e l’Aiuto.

* **[!UICONTROL Visualizzatori zoom]** - Offre tre tipi di visualizzatori zoom:

* **[!UICONTROL Visualizzatore zoom]** - Consente agli utenti di ingrandire l’area selezionandola. È possibile selezionare i controlli per ingrandire, ridurre e ripristinare le dimensioni predefinite dell&#39;immagine.

* **[!UICONTROL Visualizzatore zoom: Uscita rapida]** - Visualizza una seconda immagine dell&#39;area ingrandita accanto all&#39;immagine originale. Non vi sono controlli; gli utenti devono semplicemente spostare la selezione sull’area da visualizzare.

Quando calcolate l’utilizzo di larghezza di banda totale per questo visualizzatore, tenete presente che nel visualizzatore vengono caricate sia l’immagine principale che l’immagine a comparsa. Le dimensioni dell’immagine principale (Larghezza e Altezza area visualizzazione) e il fattore di zoom determinano le dimensioni dell’immagine a comparsa. Per impedire che le dimensioni del file dell’immagine a comparsa diventino eccessive, bilanciate questi due valori: se le dimensioni dell’immagine principale sono grandi, riducete il fattore di zoom. I valori Larghezza a comparsa e Altezza comparsa determinano le dimensioni della finestra a comparsa ma non dell’immagine a comparsa caricata nel visualizzatore.

Ad esempio, se le dimensioni dell’immagine principale sono 350 x 350 pixel, con un fattore di zoom pari a 3 l’immagine a comparsa risultante sarà di 1050 x 1050 pixel. Se le dimensioni dell’immagine principale sono 300 x 300 pixel, con un fattore di zoom pari a 4 l’immagine a comparsa risultante sarà di 1200 x 1200 pixel. In base alla qualità JPEG impostata (impostazioni consigliate: 80-90), potete ridurre sensibilmente le dimensioni del file. I fattori di zoom consigliati sono i valori compresi tra 2,5 e 4, a seconda delle dimensioni dell’immagine principale.

### Matrice di compatibilità dei predefiniti per visualizzatori Adobe Dynamic Media Classic {#scene-viewer-preset-compatibility-matrix}

**Avviso sulla fine del ciclo di vita dei visualizzatori di Flash**: Dal 31 gennaio 2017, Adobe Dynamic Media Classic ha ufficialmente terminato il supporto per la piattaforma di visualizzazione dei Flash.

Nella tabella seguente sono elencati i predefiniti per visualizzatori Adobe Dynamic Media Classic attualmente disponibili. Viene inoltre specificata la compatibilità con dispositivi desktop e mobili nonché la tecnologia utilizzata per ciascun visualizzatore.

Vedi anche [Esempi della libreria di riferimento visualizzatori di Adobi](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Per informazioni sui browser Web e sulle versioni del sistema operativo supportati per i visualizzatori, consultate le relative Note sulla versione.

Vedi [Note sulla versione di riferimento per i visualizzatori di Adobi](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori zoom |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori per set di immagini |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
|  Visualizzatori per set di campioni |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori eCatalog |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Include il supporto per i social media e la ricerca nel catalogo). | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(include il supporto per social media e la ricerca nel catalogo). | HTML5 | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori per set 360 gradi |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**Visualizzatori per eVideo**

Adobe Dynamic Media Classic supporta la riproduzione video mobile per video MP4 H.264.

* I dispositivi BlackBerry® che supportano questo formato video sono disponibili nel seguente sito: [Formati video supportati su BlackBerry®](https://developers.blackberry.com/us/en)
* È inoltre possibile trovare i dispositivi Windows® che supportano questo formato video nel seguente percorso: [Formati video supportati su Windows® Phone](https://docs.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ | Smartphone BlackBerry® | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video (include il supporto per sottotitoli codificati) Consultate [Procedura consigliata: utilizzo del visualizzatore universale per video HTML5.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social (include il supporto per sottotitoli codificati e social media) | HTML5 | X | X | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Set di file multimediali diversi |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Matrice dei gesti supportati dai visualizzatori per dispositivi mobili {#supported-mobile-viewers-gestures-matrix}

La tabella seguente identifica i movimenti dei visualizzatori mobili supportati sui dispositivi iOS, Android™ 2.x e Android™ 3.x.

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori per set di immagini |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Informazioni sulla schermata Preimpostazioni visualizzatore {#about-the-viewer-preset-screen}

Potete creare e gestire i predefiniti per visualizzatori nella schermata Predefiniti per visualizzatore. Per aprire questa schermata, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.

La schermata Predefiniti visualizzatore offre strumenti che consentono di eseguire le seguenti attività:

* **Aggiungi un predefinito** - Seleziona **[!UICONTROL Aggiungi]** ed effettua le relative scelte nella finestra di dialogo Aggiungi predefinito visualizzatore .

       Consulta [Aggiungere e modificare i predefiniti visualizzatore](application-setup.md#adding_and_editing_viewer_presets).
   
* **Modificare un predefinito** - Selezionare un predefinito, quindi selezionare **[!UICONTROL Modifica]**.

       Consulta [Aggiungere e modificare i predefiniti visualizzatore](application-setup.md#adding_and_editing_viewer_presets).
   
* **Eliminare un predefinito** - Selezionare un predefinito, quindi selezionare **[!UICONTROL Elimina]**.

* **Esportare un predefinito** - Selezionare un predefinito visualizzatore HTML5, quindi selezionare **[!UICONTROL Esporta]** per scaricare lo skin del visualizzatore in modo da poterlo utilizzare come base per creare e aggiungere un altro predefinito per visualizzatori.

       Consulta [Esportare un predefinito visualizzatore HTML5](application-setup.md#export_an_html5_viewer_preset).
   
* **Filtrare l’elenco Predefiniti visualizzatore** - Utilizzare questi strumenti per filtrare l&#39;elenco:

       * Apri l’elenco a discesa **Attivo/Inattivo** e seleziona un’opzione per mostrare i predefiniti attivi, inattivi o tutti i predefiniti.
       * Apri l’elenco a discesa **Visualizzatore** e seleziona un’opzione per visualizzare solo i visualizzatori di un determinato tipo. Seleziona **[!UICONTROL Tutti i visualizzatori]** per visualizzare tutti i visualizzatori.
   
* **Ordina predefiniti** - Seleziona un’intestazione di colonna (**[!UICONTROL Attivo]**, **[!UICONTROL Tipo]**, **[!UICONTROL Predefinito]** oppure **[!UICONTROL Piattaforma]**) per ordinare l’elenco in una colonna. Seleziona un’intestazione di colonna una seconda volta per ordinare l’elenco in ordine decrescente (o crescente).

* **Attivare e disattivare i predefiniti** - Selezionare un predefinito, quindi selezionare l&#39;opzione Attivo per attivarlo o disattivarlo.

       Consultate [Attivare o disattivare i predefiniti visualizzatore](application-setup.md#activating_or_deactivating_viewer_presets).
   
>[!NOTE]
>
>Seleziona **[!UICONTROL Anteprima]** sul lato destro della pagina Predefiniti visualizzatore per verificare l’aspetto di una risorsa nel predefinito visualizzatore selezionato. Per visualizzare una risorsa diversa, seleziona **[!UICONTROL Sfoglia]** nella pagina Predefiniti visualizzatore e selezionate una risorsa diversa nella finestra di dialogo Seleziona anteprima risorsa .

### Aggiungere e modificare i predefiniti visualizzatore {#adding-and-editing-viewer-presets}

Oltre ad aggiungere i predefiniti visualizzatore utilizzando **[!UICONTROL Aggiungi]** nell’interfaccia utente, puoi anche utilizzare **[!UICONTROL Esporta]** per aggiungere un predefinito visualizzatore. È sufficiente esportare un predefinito visualizzatore HTML5 esistente e utilizzarlo come base per il nuovo predefinito.

Vedi [Esportare un predefinito visualizzatore HTML5](application-setup.md#exporting_an_html5_viewer_preset).

Vedi anche [Predefiniti visualizzatore](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) video di formazione.

**Per aggiungere o modificare dei predefiniti per visualizzatori:**

1. Nell&#39;angolo in alto a destra di Adobe Dynamic Media Classic, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.

   Potete filtrare l’elenco dei predefiniti. Ad esempio, per visualizzare soltanto i predefiniti per i visualizzatori video, selezionate Visualizzatore video dall’elenco a discesa Visualizzatori nella barra degli strumenti che si trova appena sopra la tabella.

1. Nella pagina Predefiniti visualizzatore , aggiungi o modifica il predefinito visualizzatore nella schermata Predefiniti visualizzatore .

   * **Aggiungi** - Nella barra degli strumenti, seleziona **[!UICONTROL Aggiungi]**. Nella finestra di dialogo Aggiungi predefinito visualizzatore , seleziona una piattaforma e un tipo di risorsa rich media.

          Seleziona **[!UICONTROL Salva con nome]** al termine della creazione del predefinito visualizzatore.
      
   * **Aggiungi a partire da un predefinito visualizzatore esistente** - Nella tabella, seleziona un predefinito per visualizzatori video, quindi seleziona **[!UICONTROL Modifica]** sulla barra degli strumenti.

          Dopo aver riconfigurato il visualizzatore video, seleziona **[!UICONTROL Salva con nome]** per salvare il predefinito utilizzando un nome diverso nel campo di testo Nome predefinito.
      
   * **Modifica** - Seleziona un predefinito per visualizzatori esistente, quindi seleziona **[!UICONTROL Modifica]**.

1. Nella schermata Configura visualizzatore, immetti o modifica il nome del predefinito nel campo Nome predefinito .
1. Impostate le opzioni rimanenti in base alle vostre esigenze.

   >[!NOTE]
   >
   >Seleziona **[!UICONTROL Come origine]** per ridimensionare automaticamente il visualizzatore video alle dimensioni di risoluzione del video codificato stesso. Se si seleziona questa opzione, non è possibile immettere la larghezza e l&#39;altezza dello stage. e tali valori verranno invece determinati dal video stesso. Se si seleziona **[!UICONTROL Come origine]**, impostate l’opzione Dimensione margine in modo che rifletta le dimensioni dell’interfaccia all’esterno dell’area di riproduzione del video. Le dimensioni del margine corrispondono all’altezza e alla larghezza in pixel dei controlli video. L’immagine seguente consente di determinare le dimensioni del margine da utilizzare.*

   ![Configurazione del margine del visualizzatore video](assets/vs_video_viewer_configure_margin.png)

1. Effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Salva con nome]** se hai aggiunto un predefinito visualizzatore a partire da un predefinito esistente.
   * Seleziona **[!UICONTROL Salva]** se hai aggiunto o modificato un predefinito visualizzatore.

### Esportare un predefinito per visualizzatori HTML5 {#exporting-an-html-viewer-preset}

È possibile esportare un predefinito per visualizzatori HTML5 esistente da utilizzare come base per la creazione di un predefinito per visualizzatori HTML5. In questo modo si evita di dover creare un visualizzatore da zero. Se esportate un predefinito con aspetto e comportamento simili a quelli desiderati, potrete usarlo come base di partenza per apportare le regolazioni necessarie.

Tutti i file CSS predefiniti del visualizzatore in Adobe Dynamic Media Classic utilizzano percorsi di trasmissione delle immagini relativi che puntano alle risorse su `Scene7SharedAssets`. Ad esempio, il seguente è un percorso relativo a una risorsa immagine in un file CSS predefinito per visualizzatori su

`Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

Tuttavia, se si ospitano file CSS del visualizzatore sul proprio sito, è necessario risolvere questi percorsi immagine relativi utilizzando un percorso esplicito del server immagini nel proprio ambiente. Ad esempio, se devi aggiornare il percorso relativo sopra a un percorso esplicito, potrebbe essere simile al seguente, dove `https://s7d1.scene7.com` è il percorso diretto del server di immagini: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Per esportare un predefinito visualizzatore HTML5:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Nella barra degli strumenti Predefiniti visualizzatore, seleziona il secondo elenco a discesa a sinistra **[!UICONTROL HTML5]**.
1. Selezionate **[!UICONTROL Tutti i visualizzatori]** nel terzo elenco a discesa da sinistra.
1. Selezionare il predefinito visualizzatore da utilizzare come base per un nuovo predefinito visualizzatore HTML5.
1. Nella barra degli strumenti, seleziona **[!UICONTROL Esporta]**.
1. Nella finestra di dialogo Esporta risorse selezionate, seleziona **[!UICONTROL Invia esportazione]**.

   Dopo l’esportazione, ottieni un file CSS. Scaricate e decomprimete il file.

1. Aprite il file CSS in un Editor CSS, apportate le modifiche e salvate il file.
1. Carica il file CSS in Adobe Dynamic Media Classic.

   Vedi [Caricare file](uploading-files.md#uploading_files).

1. Pubblica il file CSS sul server di immagini Dynamic Media.

   Vedi [Pubblicare i file](publishing-files.md#publishing_files).

1. Aggiungete il nuovo predefinito per visualizzatori seguendo la procedura standard. Seleziona il file CSS del visualizzatore caricato.

   Vedi [Aggiungere e modificare i predefiniti visualizzatore](application-setup.md#adding_and_editing_viewer_presets).

### Attivare o disattivare i predefiniti visualizzatore {#activating-or-deactivating-viewer-presets}

Per creare un URL per la visualizzazione delle risorse, gli utenti aprono l’elenco a discesa Predefiniti nella finestra di dialogo Anteprima, selezionano un predefinito visualizzatore e quindi selezionano **[!UICONTROL Copia URL]** (vedi [Copiare l’URL di un predefinito per visualizzatori](application-setup.md#copying_the_url_of_a_viewer_preset)). Questo elenco di predefiniti offre i predefiniti per visualizzatori aggiunti e gestiti dagli amministratori nella schermata Predefiniti per visualizzatore. Ad esempio, tutti i predefiniti per visualizzatori eCatalog attivi vengono visualizzati nell’elenco a discesa Predefiniti nella finestra di dialogo Anteprima quando un utente esegue l’anteprima di un eCatalog.

Se i predefiniti per visualizzatori non vengono disattivati nella schermata Predefiniti per visualizzatore, nell’elenco a discesa Predefiniti nella finestra di dialogo Anteprima potrebbero accumularsi troppi predefiniti. 

**Per attivare o disattivare i predefiniti per visualizzatori:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Nella pagina Predefiniti visualizzatore , seleziona o deseleziona **[!UICONTROL Attivo]** opzioni per attivare o disattivare i predefiniti visualizzatore.

### Copiare l’URL di un predefinito per visualizzatori {#copying-the-url-of-a-viewer-preset}

Una volta pubblicata una risorsa, potete copiare un URL per visualizzare la risorsa con le impostazioni di un predefinito per visualizzatore.

L’URL viene copiato negli Appunti. Potete utilizzarlo come desiderate nel codice HTML di una pagina Web, in un dispositivo mobile o in un’applicazione.

**Per copiare l’URL di un predefinito per visualizzatori:**

1. Selezionate la risorsa nel pannello Sfoglia.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Vista a griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato.
   * Seleziona **[!UICONTROL Vista a griglia]**. Nel pannello delle risorse, seleziona una singola risorsa, quindi, sotto la miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Copia URL]**.

   * Seleziona **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse , seleziona una singola risorsa, quindi, a destra della miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Copia URL]**.

   * Seleziona **[!UICONTROL Vista a griglia]**, **[!UICONTROL Vista a elenco]** oppure **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Copia URL]**.

### Copiare il codice di incorporamento di un predefinito per visualizzatori {#copying-the-embed-code-of-a-viewer-preset}

La funzione Incorpora codice permette di analizzare il codice visualizzatore del predefinito per visualizzatori selezionato. Potete anche copiare il codice negli Appunti per poi incollarlo nelle pagine Web su cui verrà distribuito il visualizzatore. 

La modifica del codice non è consentita nella finestra di dialogo Incorpora codice.

**Per copiare il codice da incorporare di un predefinito per visualizzatori:**

1. Selezionate la risorsa nel pannello delle risorse.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Vista a griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL a destra, seleziona **[!UICONTROL Codice di incorporamento]**.
   * Seleziona **[!UICONTROL Vista a griglia]**. Nel pannello delle risorse, seleziona una singola risorsa, quindi, sotto la miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**.

   * Seleziona **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse , seleziona una singola risorsa, quindi, a destra della miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**.

   * Seleziona **[!UICONTROL Vista a griglia]**, **[!UICONTROL Vista a elenco]** oppure **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**.

1. Nella finestra di dialogo Incorpora codice selezionare **[!UICONTROL Copia negli Appunti]**.
1. Seleziona **[!UICONTROL Chiudi]**.

## Configurare i visualizzatori predefiniti {#configuring-default-viewers}

Puoi utilizzare i visualizzatori predefiniti per configurare il visualizzatore predefinito associato a una risorsa quando utilizzi Anteprima in Adobe Dynamic Media Classic. Potete impostare l’esperienza di anteprima predefinita per i seguenti tipi di risorse:

* Immagine
* Video
* Set 360 gradi
* Catalogo
* Set di immagini
* Set di campioni
* Set file multimediali

**Per configurare i visualizzatori predefiniti:**

1. Nell’elenco a discesa Configurazione , seleziona **[!UICONTROL Impostazione applicazione]**.
1. Nella finestra Configurazione, nel riquadro a sinistra, passare a **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Visualizzatori]**
1. Seleziona **[!UICONTROL Visualizzatori predefiniti]**.
1. Nella finestra Visualizzatori predefiniti, nell’elenco a discesa per ogni tipo di risorsa, selezionate il visualizzatore da associare all’anteprima della risorsa.
1. Nell’angolo in basso a destra della finestra Visualizzatori predefiniti, seleziona **[!UICONTROL Salva impostazioni]**.
1. Nell&#39;angolo inferiore destro della finestra Configurazione, selezionare **[!UICONTROL Chiudi]** per tornare alla finestra Risorsa.

## Visualizzazione metadati {#metadata-views}

I *metadati* sono informazioni standardizzate su una risorsa. Potete utilizzare i metadati per semplificare il flusso di lavoro, organizzare le risorse e migliorare le ricerche. Adobe Dynamic Media Classic supporta lo standard IPTC (International Press Telecommunications Council) e lo standard XMP (Extensible Metadata Platform). Prima che gli utenti visualizzino o immettano i metadati di una risorsa in Vista dettagli, possono aprire il menu Visualizzazioni metadati . Da qui, possono selezionare il set di campi di metadati che desiderano visualizzare o utilizzare per descrivere la risorsa.

Adobe Dynamic Media Classic viene fornito con visualizzazioni metadati predefinite e gli amministratori possono creare visualizzazioni metadati personalizzate che gli utenti possono scegliere quando inserire i metadati.

### Creazione di una visualizzazione metadati {#creating-a-metadata-view}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Visualizzazioni metadati]**.
1. Seleziona **[!UICONTROL Aggiungi]**.
1. Nel campo di testo Nome predefinito , immetti un nome per la visualizzazione.
1. (Facoltativo) Controllo **[!UICONTROL Imposta come predefinito]** per impostare questa visualizzazione come visualizzata dagli utenti all’apertura del pannello Metadati in Vista dettagli.
1. (Facoltativo) Seleziona **[!UICONTROL Includi UDF]** per includere nella visualizzazione i campi definiti dall’utente. Questi vengono presentati nella parte superiore del pannello Metadati in visualizzazione Dettagli.
1. Selezionare i campi desiderati per la visualizzazione (selezionare **[!UICONTROL Seleziona tutto]** per selezionare tutti i campi).
1. Seleziona **[!UICONTROL Salva]**.

   Le categorie e i campi selezionati per la visualizzazione vengono visualizzati nel pannello Anteprima.

### Gestione delle visualizzazioni metadati {#managing-metadata-views}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Visualizzazioni metadati]**.
1. Effettuate una delle seguenti operazioni:

   * Per visualizzare un’anteprima di una visualizzazione, selezionatela. I campi della visualizzazione vengono visualizzati nel pannello Anteprima.
   * Per modificare una visualizzazione, selezionala e seleziona **[!UICONTROL Modifica]**. Quindi seleziona o deseleziona i nomi dei campi nel pannello Anteprima e seleziona o deseleziona la **[!UICONTROL Includi UDF]** opzione .
   * Per eliminare una visualizzazione, selezionala e seleziona **[!UICONTROL Elimina]**.
   * Per impostare una visualizzazione predefinita, selezionarla, quindi selezionare **[!UICONTROL Imposta come predefinito]**. La visualizzazione predefinita è quella che gli utenti visualizzano quando aprono una risorsa in Vista dettagli e accedono al pannello Metadati.

## Predefiniti per metadati {#metadata-presets}

I predefiniti per metadati consentono agli amministratori di controllare e modificare i metadati assegnati alle risorse. Nella Vista dettagli, un utente può immettere i metadati di una risorsa nei campi forniti a tal fine. Ad esempio, un utente può inserire un nome proprietario, una descrizione del copyright e un indirizzo. Per fare in modo che gli utenti inseriscano queste informazioni in modo accurato e completo, puoi creare i predefiniti per metadati. Quando si sceglie un predefinito per metadati nella visualizzazione dettagli, i campi di metadati vengono compilati con valori predefiniti. Ad esempio, il nome proprietario, la descrizione del copyright e l’indirizzo vengono inseriti automaticamente.

Crea un predefinito per metadati per ogni set di valori di metadati che desideri che gli utenti siano in grado di immettere automaticamente in Vista dettagli per descrivere una risorsa.

### Creazione o modifica di un predefinito per metadati {#creating-or-editing-a-metadata-preset}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Predefiniti metadati]**.
1. Nella schermata Predefiniti metadati, effettuate una delle seguenti operazioni:

   * Per creare un predefinito, seleziona **[!UICONTROL Aggiungi]**. Nel campo di testo Nome modello metadati , digita un nome per il predefinito. Seleziona **[!UICONTROL Visualizzazioni metadati]**, quindi seleziona una visualizzazione dall’elenco a discesa (vedi [Visualizzazioni metadati](application-setup.md#metadata_views)).
   * Per modificare un predefinito esistente, selezionalo dall’elenco Predefiniti metadati , quindi seleziona **[!UICONTROL Modifica]**.

1. Espandi le intestazioni da includere nel predefinito e inserisci i valori nei diversi campi che desideri includere nel predefinito.
1. Seleziona **[!UICONTROL Salva]**.

   Le categorie e i campi selezionati per il predefinito vengono visualizzati nel pannello dell’anteprima.

### Gestione dei predefiniti per metadati {#managing-metadata-presets}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Predefiniti metadati]**.
1. Effettuate una delle seguenti operazioni:

   * Per visualizzare l’anteprima di un predefinito, selezionate il predefinito. Le informazioni sul predefinito (categorie e campi) vengono visualizzate nella schermata Anteprima.
   * Per eliminare un predefinito, selezionalo e seleziona **[!UICONTROL Elimina]**.

## Campi definiti dall’utente {#user-defined-fields}

I campi metadati definiti dall’utente possono essere creati solo da un amministratore di Media Portal o un amministratore società. I campi personalizzati possono essere utili per organizzare le risorse in Adobe Dynamic Media Classic. Se necessario, è possibile contrassegnare i campi come Attivo. Quando sono attivati, i nomi di questi campi di metadati personalizzati vengono visualizzati nel pannello Metadati in Vista dettagli. Nei campi di metadati definiti dall’utente gli utenti possono immettere informazioni per descrivere le risorse. Gli utenti possono inoltre utilizzare tali campi di metadati come criteri di ricerca.

I campi metadati definiti dall’utente sono utili ad esempio per ritardare il momento di attivazione di una risorsa per un lancio o una promozione. Puoi definire un campo &quot;attivazione&quot; in base al tipo *Data*. Quindi, utilizzando **[!UICONTROL Metadati]** pannello in Vista dettagli o **[!UICONTROL File]** > **[!UICONTROL Modifica informazioni]**, puoi specificare quando la risorsa viene attivata. Adobe Dynamic Media Classic controlla lo stato di pubblicazione di una risorsa e la cronologia di pubblicazione. Se non rientra nel tempo di attivazione, lo stato di pubblicazione è indicato come &quot;Non pubblicato&quot;.

>[!NOTE]
>
>Per visualizzare i campi definiti dall’utente nel pannello Metadati in Vista dettagli, includi i campi definiti dall’utente in Visualizzazioni metadati. Nella schermata Visualizzazioni metadati, selezionate l’opzione Includi UDF (User-Defined Fields, campi definiti dall’utente). Per ulteriori informazioni, consultate [Visualizzazione metadati](application-setup.md#metadata_views).

>[!NOTE]
>
>Per cercare le risorse utilizzando campi personalizzati definiti dall’utente, passa a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**, quindi seleziona **[!UICONTROL Includi UDF nella ricerca]**. Consultate [Configurazione personale](personal-setup.md#personal_setup).

### Creare un campo di metadati definito dall’utente {#creating-a-user-defined-metadata-field}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Campi definiti dall’utente]**.
1. Seleziona **[!UICONTROL Aggiungi]**
1. Nella finestra di dialogo Campo personalizzato, impostate le opzioni desiderate.

   * **[!UICONTROL Nome]** - Immettere un nome per il campo metadati.

   * **[!UICONTROL Tipo]** - Selezionare un’opzione che definisce il tipo di informazioni che gli utenti possono immettere nel campo metadati:

   * **[!UICONTROL Stringa]** - Una stringa di testo.

   * **[!UICONTROL Int]** - Un numero intero.

   * **[!UICONTROL Mobile]** - Un numero a virgola mobile.

   * **[!UICONTROL Sì/No]** - Un valore booleano sì/no.

   * **[!UICONTROL Data]** - Una data. Il formato consentito è GG/MM/AAAA.

   * **[!UICONTROL Nome file]** - Il nome di un file.

   * **[!UICONTROL Colore]** - Il nome di un colore.

   * **[!UICONTROL Dimension]** - Larghezza e altezza della risorsa.

   * **[!UICONTROL Non digitato]** - Compatibilità con le versioni precedenti. Non selezionate questa opzione.

   * **[!UICONTROL Valore predefinito]** - È possibile immettere il valore che gli utenti avranno più probabilità di immettere nel campo. Il valore immesso diventa il valore predefinito per il nuovo campo creato.

   * **[!UICONTROL Si applica a]** - Se si desidera che il campo metadati sia applicato solo a un tipo specifico di risorsa, è possibile selezionare un tipo di risorsa.

      >[!NOTE]
      >
      >Seleziona un **[!UICONTROL Si applica a]** questa opzione è stata selezionata con attenzione perché non è possibile modificare **[!UICONTROL Si applica a]** dopo aver creato un campo definito dall’utente. Adobe Dynamic Media Classic consente di modificare il nome, il tipo e il valore predefinito di un campo definito dall’utente, ma non il **[!UICONTROL Si applica a]** impostazione. *

1. Seleziona **[!UICONTROL Salva]** al termine della creazione del campo metadati.

### Gestire i campi definiti dall’utente {#manage-user-defined-fields}

Nella schermata Campi definiti dall’utente sono disponibili i comandi necessari per gestire i campi di metadati personalizzati, definiti dall’utente. 

I campi definiti dall’utente possono essere gestiti solo da un amministratore di Media Portal o un amministratore società.

Per aprire questa schermata, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Campi definiti dall’utente]**.

* **Modificare un campo** - Selezionare il campo, quindi selezionare **[!UICONTROL Modifica]**.

* **Eliminare un campo** - Selezionare il campo, quindi selezionare **[!UICONTROL Elimina]**.

* **Attiva campo** - Seleziona o deseleziona la **[!UICONTROL Attivo]** accanto al nome di un campo. Se hai un ruolo di amministrazione aziendale, questa opzione non viene visualizzata. Poiché questa opzione è correlata a MediaPortal, è necessario selezionare (attivare) Mostra funzionalità MediaPortal in Configurazione personale per visualizzare i campi di attivazione.

## Ottimizzare i file {#optimize-files}

Quando carichi i file in Adobe Dynamic Media Classic, il sistema li ottimizza per l’archiviazione e la pubblicazione. Tuttavia, se il processo di caricamento viene interrotto, alcune immagini potrebbero non essere ottimizzate. In questo caso viene visualizzato il messaggio “Immagine non ancora ottimizzata”. Tali file possono comunque essere ottimizzati dagli utenti con ruolo di amministratore.

Adobe Dynamic Media Classic esegue ricerche nei file e ottimizza solo le immagini che non erano completamente ottimizzate in precedenza.

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]**, quindi seleziona **[!UICONTROL Ottimizzare i file]**.
1. Immetti le informazioni per il processo di ottimizzazione e seleziona **[!UICONTROL Invia]**.

   Se lavorate con più società, ottimizzate separatamente i file appartenenti a società diverse.

## Predefiniti per set di batch {#batch-set-presets}

Utilizza i predefiniti per set di batch per creare automaticamente set di immagini o set 360 gradi mentre un processo è in esecuzione per caricare le risorse in Adobe Dynamic Media Classic.

Gli amministratori della società definiscono innanzitutto le convenzioni di denominazione per le risorse che desiderano raggruppare in un set. Puoi quindi creare un Batch Set Preset per fare riferimento a queste immagini. Ogni predefinito ha un nome univoco ed è un set autonomo di istruzioni che definisce come comporre il set con le immagini in base alle convenzioni di denominazione specificate con le opzioni del predefinito.

Tutti i predefiniti per set di batch attivi di una società sono riportati nella finestra di dialogo Opzioni processo di caricamento e potete quindi specificare il predefinito da applicare per ogni sessione di caricamento. Per gli amministratori di società vengono visualizzati tutti i predefiniti per set di batch, attivi e inattivi. Quando carichi dei file, Adobe Dynamic Media Classic crea automaticamente un set con tutti i file che corrispondono alla convenzione di denominazione definita nei predefiniti attivi.

### Denominazione predefinita {#default-naming}

L’amministratore della società può creare una convenzione di denominazione predefinita, da usare in qualsiasi predefinito per set di batch. La convenzione di denominazione predefinita selezionata nella definizione del predefinito del set di batch può essere tutto ciò che è necessario per la tua azienda per generare set in batch per tutti i siti web. Per usare la convenzione di denominazione predefinita, è necessario creare un predefinito per set di batch. Per gestire eventuali eccezioni alla denominazione predefinita stabilita per la società, potete creare altri predefiniti per set di batch con convenzioni di denominazione personalizzate, da applicare a particolari set di contenuti.

Non è necessario impostare una convenzione di denominazione predefinita per utilizzare la funzionalità Batch Set Preset. Tuttavia, Adobe di best practice consiglia di utilizzare una convenzione di denominazione predefinita per definire tutti gli elementi della convenzione di denominazione che si desidera raggruppare in un set. In questo modo è possibile semplificare la creazione dei set di batch.

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti set di batch]** > **[!UICONTROL Denominazione predefinita]**.
1. Per specificare come visualizzare e immettere le informazioni di ciascun elemento, seleziona **[!UICONTROL Visualizza modulo]** o **[!UICONTROL Visualizza codice]**.

   È possibile selezionare la **[!UICONTROL Visualizza codice]** casella di controllo per visualizzare la creazione del valore dell’espressione regolare accanto alle selezioni del modulo. Qualora la visualizzazione modulo presenti delle limitazioni, potete inserire o modificare tali valori per definire meglio gli elementi di denominazione. Se i valori non possono essere analizzati nella visualizzazione modulo, i campi modulo diventano inattivi.

   >[!NOTE]
   >
   >i campi del modulo disattivati non indicano che l’espressione regolare non è valida. Non è disponibile una funzione di convalida delle espressioni regolari generate. I risultati dell’espressione regolare generata verranno visualizzati per ogni elemento dopo la riga Risultato. L’espressione regolare completa è riportata nella parte inferiore della pagina.

1. Espandete ciascun elemento come opportuno e inserite le convenzioni di denominazione da usare.
1. Se necessario, seleziona **[!UICONTROL Aggiungi]** per aggiungere un’altra convenzione di denominazione per un elemento. Oppure, seleziona **[!UICONTROL Rimuovi]** per eliminare una convenzione di denominazione per un elemento.
1. Seleziona **[!UICONTROL Salva con nome]** e digita un nome per il predefinito. Oppure, seleziona **[!UICONTROL Salva]** se stai modificando un predefinito esistente.

In alternativa, potete usare l’opzione Visualizza codice, senza campi del modulo. In questa visualizzazione puoi creare le definizioni delle convenzioni di denominazione utilizzando esclusivamente espressioni regolari.

Per la definizione sono disponibili due elementi, Corrispondenza e Nome base. Questi campi consentono di definire tutti gli elementi di una convenzione di denominazione e identificare la porzione della convenzione usata per denominare il set in cui sono contenuti. Una convenzione di denominazione individuale di un’azienda può utilizzare una o più righe di definizione per ciascuno di questi elementi. Potete usare tutte le righe necessarie a creare una definizione univoca e raggrupparle in elementi distinti, ad esempio per l’immagine principale, l’elemento colore, l’elemento visualizzazione alternativa e l’elemento campione.

### Creare un predefinito per set di batch {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic utilizza i predefiniti per set di batch per organizzare le risorse che condividono informazioni o contenuti comuni in set di immagini da visualizzare nei visualizzatori. Le ricette predefinite per set di batch vengono eseguite automaticamente insieme ai processi di importazione delle risorse programmati in Adobe Dynamic Media Classic.

Usate la schermata Predefinito set di batch per creare, modificare e gestire i predefiniti per set di batch. Puoi creare tutti i predefiniti necessari per coprire tutti i processi di inserimento delle risorse necessari. Esistono due forme di definizioni di predefiniti per set di batch: uno per una convenzione di denominazione predefinita configurata e uno per le convenzioni di denominazione personalizzata create in tempo reale.

È possibile utilizzare il metodo campo modulo per definire un predefinito per set di batch o il metodo del codice, che consente di utilizzare espressioni regolari. Come in **[!UICONTROL Denominazione predefinita]**, puoi selezionare **[!UICONTROL Vista Codice]** allo stesso tempo, definisci nella visualizzazione modulo e utilizza espressioni regolari per creare le tue definizioni. In alternativa, potete deselezionare una delle due visualizzazioni e usare solo l’altra.

Vedi anche [Crea un set di batch predefinito per la generazione automatica di un set 360 gradi 2D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

Vedi anche [Set 360 gradi 2D](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS) video di formazione.

**Per creare un predefinito per set di batch:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti set di batch]** > **[!UICONTROL Preimpostazione set di batch]**. La vista predefinita e **[!UICONTROL Visualizza modulo]**, come impostato nell’angolo in alto a destra della pagina Dettagli.
1. Nel pannello Elenco predefiniti, seleziona **[!UICONTROL Aggiungi]** per attivare i campi di definizione nel pannello Dettagli sul lato destro della pagina.
1. Nel pannello Dettagli, digitate nel campo Nome predefinito il nome da assegnare al predefinito.
1. Selezionate il tipo di predefinito dal menu Tipo set di batch.

   Per generare automaticamente un set 360 gradi, selezionate **[!UICONTROL Set 360 gradi con asse multiplo]** dall’elenco a discesa Tipo set di batch.

1. Effettuate una delle seguenti operazioni:

   * Se utilizzi una convenzione di denominazione predefinita impostata in precedenza in **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti set di batch]** > **[!UICONTROL Denominazione predefinita]**, espandi **[!UICONTROL Convenzioni di denominazione delle risorse]**, quindi seleziona **[!UICONTROL Predefinito]**.
   * Per definire una convenzione di denominazione durante la configurazione del predefinito, espandi **[!UICONTROL Convenzioni di denominazione delle risorse]**, quindi seleziona **[!UICONTROL Personalizzato]**.

1. Per Ordine di sequenza, definite l&#39;ordine delle immagini dopo il raggruppamento del set in Adobe Dynamic Media Classic. Per impostazione predefinita le risorse sono elencate in ordine alfabetico. Tuttavia, potete definirne l’ordine utilizzando un elenco separato da virgole delle espressioni regolari.
1. Per Imposta convenzione di denominazione e creazione, specificate il suffisso o il prefisso da aggiungere al nome di base definito nella convenzione di denominazione della risorsa. Definisci anche dove viene creato il set di immagini nella struttura di cartelle di Adobe Dynamic Media Classic.

   Se definisci un numero elevato di set di immagini, mantieni questi set separati dalle cartelle contenenti le risorse stesse. Molti clienti creano una cartella con i set di immagini e reindirizzano l’applicazione in modo che memorizzi in tale cartella i set di batch generati.

1. Seleziona **[!UICONTROL Salva]** nel pannello Dettagli.

### Crea un set di batch predefinito per la generazione automatica di un set 360 gradi 2D {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Potete usare il tipo di set di batch **Set 360 gradi con asse multiplo** per creare una definizione che automatizza la generazione di set 360 gradi 2D. Il raggruppamento delle immagini utilizza espressioni regolari per riga e colonna per il corretto allineamento delle risorse di immagini nella posizione corrispondente nell’array multidimensionale.

Vedi anche [Creare un predefinito per set di batch](application-setup.md#creating_a_batch_set_preset).

Non esiste un numero minimo o massimo di righe o colonne che è necessario avere in un set 360 gradi a più assi.

Ad esempio, supponi di voler creare un set 360 gradi con più assi denominato *spin-2dspin*. Disponete di una serie di immagini per set 360 gradi che contengono tre righe con 12 immagini per riga. Le immagini sono denominate come segue:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Con queste informazioni, la ricetta Tipo set di batch può essere creata come segue:

![Immagine ricetta set di batch](assets/se_batch_set_recipe.png)

Il raggruppamento per la parte del nome della risorsa condivisa del set 360 gradi viene aggiunto al campo Match (Corrispondenza) (come evidenziato). La parte variabile del nome della risorsa, contenente la riga e la colonna, viene aggiunta rispettivamente ai campi Riga e Colonna.

Quando il set 360 gradi viene caricato e pubblicato, puoi attivare il nome della definizione del set 360 gradi 2D che è riportato in **[!UICONTROL Predefiniti set di batch]**, nella finestra di dialogo Opzioni processo di caricamento.

**Per creare un predefinito per set di batch per la generazione automatica di un set 360 gradi 2D:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti set di batch]** > **[!UICONTROL Preimpostazione set di batch]**. La vista predefinita e **[!UICONTROL Visualizza modulo]**, come impostato nell’angolo in alto a destra della pagina Dettagli.
1. Nel pannello Elenco predefiniti, seleziona **[!UICONTROL Aggiungi]** per attivare i campi di definizione nel pannello Dettagli sul lato destro della pagina.
1. Nel pannello Dettagli, digitate nel campo Nome predefinito il nome da assegnare al predefinito.
1. Nel menu a discesa Tipo set di batch, seleziona **[!UICONTROL Set risorse]**.
1. Nell’elenco a discesa Sottotipo, selezionate **[!UICONTROL Set 360 gradi con asse multiplo]**.
1. Espandi **[!UICONTROL Convenzioni di denominazione delle risorse]**, quindi seleziona **[!UICONTROL Personalizzato]**.
1. Utilizza gli attributi **[!UICONTROL Match (Corrispondenza)]** e, facoltativamente, **[!UICONTROL Nome base]** per definire un’espressione regolare per la denominazione delle risorse dell’immagine che compongono il raggruppamento.

   Ad esempio, l’espressione regolare Corrispondenza letterale potrebbe avere l’aspetto seguente:

   `(\w+)-\w+-\w+`

1. Espandete **[!UICONTROL Posizione colonna riga]** e definite il formato del nome per la posizione della risorsa di immagine nell’array set 360 gradi 2D.

   Usate le parentesi per racchiudere la posizione di riga o colonna nel nome file.

   Ad esempio, per l’espressione regolare riga, potrebbe essere simile al seguente:

   `\w+-R([0-9]+)-\w+`

   Oppure

   `\w+-(\d+)-\w+`

   Per l’espressione regolare della colonna, potrebbe essere simile al seguente:

   `\w+-\w+-C([0-9]+)`

   Oppure

   `\w+-\w+-C(\d+)`

   Tieni presente che queste espressioni sono solo esempi. Potete creare le espressioni regolari in base alle vostre esigenze.

   >[!NOTE]
   >
   >Se la combinazione di espressioni regolari in righe e colonne non è in grado di determinare la posizione della risorsa all’interno della matrice del set 360 gradi multidimensionale, la risorsa non viene aggiunta al set e viene registrato un errore.

1. Per Imposta convenzione di denominazione e creazione, specificate il suffisso o il prefisso da aggiungere al nome di base definito nella convenzione di denominazione della risorsa. Definisci anche dove viene creato il set di immagini nella struttura di cartelle di Adobe Dynamic Media Classic.

   Se definisci un numero elevato di set di immagini, mantieni questi set separati dalle cartelle contenenti le risorse stesse. Molti clienti creano una cartella con i set di immagini e reindirizzano l’applicazione in modo che memorizzi in tale cartella i set di batch generati.

1. Seleziona **[!UICONTROL Salva]** nel pannello Dettagli.
1. Caricate e pubblicate normalmente il set 360 gradi, assicurandovi di attivare il nome del set 360 gradi 2D nella finestra di dialogo Opzioni processo di caricamento, nella sezione Predefiniti per set di batch.

>[!MORELIKETHIS]
>
>* [Visualizzare un&#39;anteprima di una risorsa](previewing-asset.md#previewing_an_asset)
>* [Impostazione dei predefiniti per immagini](setting-image-presets.md#setting_up_image_presets)
>* [Visualizzare, aggiungere ed esportare metadati](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Controllare i file di processo](checking-job-files.md#checking_job_files)

