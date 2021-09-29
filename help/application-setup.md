---
title: Impostazione applicazione
description: Scopri come impostare e configurare l’area Applicazione di Adobe Dynamic Media Classic. L’area Applicazione consente di specificare le impostazioni generali, creare predefiniti per la codifica di immagini, visualizzatori e video, definire visualizzatori e metadati predefiniti, le impostazioni di pubblicazione e le impostazioni SEO video. È inoltre possibile utilizzare l’area per impostare i predefiniti per set di batch per automatizzare la generazione di set 360 gradi 2D.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
source-git-commit: 0e2271924f49edd6ac424bb7cbd56af1e6afd817
workflow-type: tm+mt
source-wordcount: '11003'
ht-degree: 44%

---

# Impostazione applicazione{#application-setup}

Puoi utilizzare le pagine Impostazione applicazione per specificare le impostazioni generali, creare predefiniti per immagini, predefiniti di codifica video, predefiniti visualizzatore o per definire visualizzatori predefiniti e metadati. Puoi impostare i predefiniti per set di batch per automatizzare anche la generazione di set 360 gradi 2D (ad esempio), le impostazioni di pubblicazione e le impostazioni SEO video.

>[!NOTE]
>
>Solo gli amministratori di Dynamic Media Classic di Adobe possono modificare le impostazioni nelle pagine Impostazione applicazione.

## Impostazioni generali {#general-settings}

Per aprire la pagina Impostazioni generali applicazione, nella barra di navigazione globale passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Impostazioni generali]**.

### Server

Al momento della creazione dell’account, Adobe Dynamic Media Classic fornisce automaticamente i server assegnati all’azienda. I server vengono utilizzati per generare stringhe URL per il proprio sito Web e le applicazioni. Tali chiamate URL sono specifiche dell’account utente.

Vedere anche [Test del servizio di test Secure](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL Nome server pubblicato]** : questo server è il server CDN (Live Content Delivery Network) utilizzato in tutte le chiamate URL generate dal sistema specifiche per il tuo account. Non modificare il nome del server a meno che non venga richiesto da un tecnico di supporto Adobe Dynamic Media Classic.

* **[!UICONTROL Nome server di origine]** : questo server viene utilizzato solo per il test del controllo qualità. Non modificare il nome del server a meno che non venga richiesto da un tecnico del supporto Dynamic Media Classic di Adobe.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Nome server Test&amp;Target]** : l’URL di Test&amp;Target, fino a .com incluso. Per istruzioni su come ottenere questo URL, consulta Integrazione di [!DNL Adobe Dynamic Media Classic] con [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL Nome server di streaming iOS]** : l’URL del server di streaming  [!DNL Adobe Dynamic Media Classic] iOS. Questo server distribuisce i video in streaming ai dispositivi basati su iOS utilizzando il protocollo HTTP.

* **[!UICONTROL Nome server video progressivo]** : l’URL del server video  [!DNL Adobe Dynamic Media Classic] progressivo. Questo server distribuisce i video progressivi mediante il protocollo HTTP.

* **[!UICONTROL Mostra URL per risorse non pubblicate]** : seleziona questa opzione se desideri  [!DNL Adobe Dynamic Media Classic] visualizzare un URL quando visualizzi l’anteprima di una risorsa, pubblicata o meno. Se la risorsa non è pubblicata, l’URL non funziona. Tuttavia, potete utilizzare l’URL a scopo di progettazione o organizzazione.

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL Modello di annullamento validità CDN]**  - Specifica il modello utilizzato per annullare la validità della cache CDN (Content Delivery Network).

   Ad esempio, supponiamo di inserire un URL immagine (inclusi predefiniti immagine o modificatori) che fa riferimento a `<ID>`, invece di un ID immagine specifico come nell&#39;esempio seguente:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   Se il modello contiene solo `<ID>`, Adobe Dynamic Media Classic si riempie nel `https://<server>/is/image`, dove `<server>` è il Nome del server di pubblicazione definito in Impostazioni generali.

   Imposta il modello di annullamento validità CDN, seleziona un&#39;immagine denominata Zaino_B, quindi vai a **[!UICONTROL File]** > **[!UICONTROL Annulla validità CDN]** restituisce il seguente URL generato nell&#39;interfaccia di annullamento validità CDN:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   Nella casella di riepilogo URL, seleziona **[!UICONTROL Continua]** per cancellare la cache per quella specifica chiamata URL immagine. Puoi anche aggiungere URL digitandoli o incollandoli nella casella di riepilogo URL; non è necessario impostare il modello in anticipo.

   Dopo aver selezionato il modello di annullamento validità CDN e aver effettuato una richiesta di annullamento validità CDN, viene visualizzato un indicatore nell’interfaccia utente. Fornisce una stima di quanto tempo ci vuole per cancellare la cache.

   Analogamente, se all&#39;interno di Adobe Dynamic Media Classic sono selezionate più immagini quando si passa a **[!UICONTROL File]** > **[!UICONTROL Annulla validità CDN]**, nell&#39;URL del modello salvato viene fatto riferimento a ciascuna immagine. Di conseguenza, puoi definire un modello di annullamento validità CDN facendo riferimento a ciascun URL a cui si fa riferimento sul sito web (ad esempio dettagli del prodotto e risultati di ricerca). Quindi, quando selezioni una o più immagini della cache di cui annullare la validità, gli URL compilano automaticamente l’interfaccia.

   Consultate [Memorizzazione dei contenuti nella cache](dmc-platform-overview.md#content_caching).

   Consultate [Risorse ripubblicate e ritardi CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Sfoglia

* **[!UICONTROL Mostra progetti]** : determina se i progetti sono disponibili come mezzo per organizzare le risorse Adobe Dynamic Media Classic. Consultate Organizzazione del lavoro mediante i progetti.

* **[!UICONTROL Mostra contenuto eVideo campione]** : attiva o disattiva la visualizzazione del contenuto di esempio eVideo.

* **[!UICONTROL Mostra contenuto generato]** : nelle cartelle viene visualizzato il contenuto generato da una risorsa. Ad esempio, quando un file PDF viene rasterizzato durante il caricamento, in Adobe Dynamic Media Classic viene creata un’immagine per ogni pagina del PDF originale. Se l’opzione Mostra contenuto generato è selezionata, ogni immagine generata durante il caricamento del PDF originale viene visualizzata insieme al PDF nella cartella in cui questo è stato caricato.

* **[!UICONTROL Mostra video codificati]**  - Deselezionato (disattivato) per impostazione predefinita.

   Per cercare e sfogliare rapidamente i video in Adobe Dynamic Media Classic senza dover navigare in numerosi derivati codificati dello stesso video, lascia deselezionata questa opzione (impostazione predefinita). Vengono visualizzate solo la miniatura del video principale (il video sorgente caricato e utilizzato per creare i derivati) e la miniatura del set video adattivo &quot;principale&quot; (che contiene i derivati &quot;secondari&quot; del set video codificato).

   Tuttavia, potete comunque accedere ai singoli video codificati a partire dal video principale o dal set video adattivo. A questo scopo, fate doppio clic sulla miniatura del video per aprire la visualizzazione Dettagli. Quindi seleziona **[!UICONTROL Video codificati]** nel pannello di destra in modo da poter accedere a tutti i video &quot;secondari&quot;.

   Puoi anche andare su **[!UICONTROL File]** > **[!UICONTROL Rielabora]** per creare video &quot;secondari&quot; codificati più direttamente da un set video adattivo. Adobe Dynamic Media Classic trova automaticamente il video principale &quot;principale&quot; del set di video adattivi e lo utilizza come video sorgente per la transcodifica. Quando salvate i nuovi video codificati, tuttavia, questi non vengono visti nelle operazioni di ricerca o navigazione. Sono comunque accessibili dalla scheda Video codificati in visualizzazione Dettagli.

   Consulta [Caricare e transcodificare video](uploading-encoding-videos.md#uploading_and_encoding_videos).

   Per poter accedere a tutte le versioni derivate codificate durante la ricerca e la navigazione, selezionate **[!UICONTROL Mostra video codificati]**.

   Alcune azioni nel menu Genera funzionano solo o eventualmente con singoli video. Questa funzionalità rende necessaria la visualizzazione di tutte le versioni derivate di video codificati disponibili per la selezione, a prescindere dall’impostazione di **[!UICONTROL Mostra video codificati]**. Le azioni Build che ignorano l’impostazione **[!UICONTROL Mostra video codificati]** includono **[!UICONTROL Set di video adattivi]** e **[!UICONTROL eCatalogs]**.

   >[!NOTE]
   >
   >Se non hai utilizzato Adobe Dynamic Media Classic per caricare e codificare le risorse video, Adobe Dynamic Media Classic mostra tutti i singoli video codificati, anche se questa opzione è deselezionata.

* **[!UICONTROL Mostra pulsante Aggiorna sottocartelle]**  - Attiva o disattiva la visualizzazione del pulsante Aggiorna sottocartelle.

### Adobe Dynamic Media Classic FTP Account

* **[!UICONTROL Server]** : elenca il server dell&#39;account FTP.

* **[!UICONTROL Nome utente]** : elenca il nome utente dell&#39;account FTP.

### Carica nell’applicazione

* **[!UICONTROL Sovrascrivi immagini]** : ad Adobe Dynamic Media Classic non consente a due file di avere lo stesso nome. L&#39;ID Dynamic Media Classic Adobe di ogni elemento (il nome dell&#39;immagine meno l&#39;estensione del nome del file) deve essere univoco. In virtù di questa regola, nella finestra di dialogo Carica è disponibile l’opzione Sovrascrivi. Il risultato effettivo di questa opzione dipende dal valore impostato per l’opzione Sovrascrivi immagini. È possibile specificare come caricare le immagini sostitutive, ossia se devono sostituire le immagini originali o diventare duplicati di tali immagini. Le immagini duplicate vengono rinominate con il suffisso “-1” (ad esempio, il file sedia.tif viene rinominato sedia-1.tif). Queste opzioni interessano le immagini caricate in una cartella diversa da quella degli originali o le immagini con una diversa estensione file (ad esempio, JPG, TIF o PNG). Consultate Utilizzo dell’opzione Sovrascrivi immagini.

   * **[!UICONTROL Sovrascrivi nella cartella corrente, nome/estensione]**  immagine di base - Questa opzione è la regola più rigida per la sostituzione. Richiede che l’immagine sostitutiva sia caricata nella stessa cartella dell’immagine originale e che abbia la stessa estensione del nome file dell’originale. Se entrambi i requisiti non vengono soddisfatti, viene creata una copia dell’immagine.

   * **[!UICONTROL Sovrascrivi nella cartella corrente, lo stesso nome della risorsa di base indipendentemente dall&#39;estensione]**  - Richiede di caricare l&#39;immagine di sostituzione nella stessa cartella dell&#39;originale, tuttavia l&#39;estensione del nome file può essere diversa dall&#39;originale. Ad esempio, sedia.tif sostituisce sedia.jpg.

   * **[!UICONTROL Sovrascrivi in qualsiasi cartella, stesso nome/estensione della risorsa base]**  - Richiede che l&#39;immagine sostitutiva abbia la stessa estensione del nome file dell&#39;immagine originale (ad esempio, sedia.jpg deve sostituire sedia.jpg, non sedia.tif). Tuttavia, è possibile caricare l’immagine sostitutiva in una cartella diversa da quella dell’originale. L’immagine aggiornata sarà contenuta nella nuova cartella e il file verrà rimosso dal percorso originale.

   * **[!UICONTROL Sovrascrivi in qualsiasi cartella, lo stesso nome della risorsa di base indipendentemente dall&#39;estensione]**  - Questa opzione è la regola di sostituzione più inclusiva. L’immagine sostitutiva può essere caricata in una cartella diversa da quella dell’originale, con una diversa estensione file, e sostituire il file originale. Se il file originale si trova in un’altra cartella, l’immagine sostitutiva sarà contenuta nella nuova cartella nella quale è stata caricata.

* **[!UICONTROL Mantieni pubblicazione]** : specifica se un&#39;immagine sostitutiva caricata in Adobe Dynamic Media Classic mantiene l&#39;impostazione Pronto per la pubblicazione dell&#39;immagine che sta sostituendo, oppure se l&#39;impostazione è specificata al momento del caricamento.

* **[!UICONTROL Profili colore predefiniti]**  - Specifica i profili colore applicati come parte delle Opzioni profilo colore predefinito durante l&#39;aggiunta di immagini CMYK.

* **[!UICONTROL Opzioni di caricamento predefinite]** : apre la finestra di dialogo Opzioni processo di caricamento, in cui è possibile specificare le opzioni di caricamento predefinite. Per informazioni su queste opzioni, consultate Opzioni di caricamento.

### Editor mappa immagine, su applicazione

* **[!UICONTROL HREF]**  di mappatura immagine predefinito - Definisce l&#39;URL predefinito utilizzato per la colonna HREF nel mapping delle immagini. Questo è l’URL predefinito visualizzato quando create mappe immagine.

* **[!UICONTROL Modello di mappatura immagine predefinito]** : definisce il JavaScript predefinito per il modello HREF nel mapping delle immagini. Puoi impostare un codice personalizzato da eseguire qui ogni volta che selezioni una mappa immagine.

### Altre impostazioni, su applicazione

* **[!UICONTROL Il cestino può pulire gli avvisi]** : le risorse nel cestino vengono rimosse automaticamente entro sette giorni. Selezionate “Invia e-mail prima che gli elementi nel cestino siano eliminati automaticamente” se desiderate che vengano inviate notifiche agli amministratori dell’azienda quattro giorni prima che le risorse nel cestino vengano definitivamente eliminate. Consultate Gestione della cartella Cestino.

## Utilizzare l’opzione Sovrascrivi immagini {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic non consente a due file di avere lo stesso nome. L&#39;ID Dynamic Media Classic Adobe di ogni elemento (il nome dell&#39;immagine meno l&#39;estensione del nome del file) deve essere univoco. In virtù di questa regola, nella finestra di dialogo Carica è disponibile l’opzione Sovrascrivi immagini. L&#39;effetto esatto di questa opzione dipende da un&#39;impostazione per le impostazioni interne Dynamic Media Classic di Adobe di ciascuna azienda.

Se in precedenza hai caricato le immagini e poi le hai modificate (o sostituite), l’opzione Sovrascrivi selezionata specifica in che modo Adobe Dynamic Media Classic sostituisce le immagini. I dati relativi all’immagine non vengono modificati, ma la nuova immagine sostituisce la precedente. Se la cartella contiene anche immagini che non sono già presenti in Adobe Dynamic Media Classic, queste immagini vengono aggiunte.

Usate questa opzione se le immagini caricate sono state modificate (l’immagine è stata manipolata) ma il riferimento all’immagine è rimasto inalterato. L’opzione Sovrascrivi è utile anche quando si caricano e si estraggono dati da file Adobe® PDF. Per ottimizzare l&#39;Adobe di Dynamic Media Classic *rips* dell&#39;immagine, regola le opzioni del profilo colore ICC nella finestra di dialogo Carica e ricarica utilizzando la funzione Sovrascrivi.

Gli ID Adobe Dynamic Media Classic utilizzati per accedere alle immagini dai server di produzione sono derivati dai nomi dei file immagine. L’utilizzo di caratteri maiuscoli e minuscoli nel nome file è importante sia per la sostituzione dei file esistenti sia per gli ID Dynamic Media Classic di Adobe utilizzati per accedere all’immagine. Assicurati che l’uso di caratteri maiuscoli e minuscoli nei nomi dei file sia corretto prima di caricarli in Adobe Dynamic Media Classic per evitare ID di Dynamic Media Classic Adobi che differiscono solo nel caso della stessa immagine.

Se deselezionate questa opzione, tutte le immagini con lo stesso nome file delle immagini esistenti vengono considerate copie e non vengono aggiunte.

## Predefiniti immagine {#image-presets}

Nella schermata Predefiniti immagine è possibile creare e modificare i predefiniti per le immagini. I predefiniti per immagini consentono ad Adobe Dynamic Media Classic di distribuire dinamicamente immagini di dimensioni diverse dalla stessa immagine master. Ogni predefinito immagine rappresenta una raccolta predefinita di comandi di ridimensionamento e formattazione per la visualizzazione delle immagini. Quando crei un predefinito per immagini, selezioni una dimensione per la distribuzione delle immagini. È inoltre possibile selezionare i comandi di formattazione in modo che l&#39;aspetto dell&#39;immagine sia ottimizzato quando l&#39;immagine viene consegnata per la visualizzazione.

Gli amministratori possono creare predefiniti per l’esportazione delle risorse. Gli utenti possono scegliere un predefinito al momento dell’esportazione delle immagini, che riformatta anche le immagini in base alle specifiche specificate dall’amministratore.

Per aprire la schermata Preimpostazioni immagine, nella barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**.

Vedere [Smart imaging](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

### Creare e modificare i predefiniti immagine {#creating-and-editing-image-presets}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagini]**.
1. Crea un predefinito o inizia da uno esistente:

   * **Crea un predefinito**  per immagini - Seleziona  **[!UICONTROL Aggiungi]**.
   * **Crea un predefinito per immagini da un predefinito**  esistente: seleziona il predefinito per immagini più simile a quello che desideri creare, quindi seleziona  **[!UICONTROL Modifica]**.

1. Nella pagina Aggiungi (o Modifica) predefinito , immetti un nome per il predefinito.
1. Impostate le opzioni desiderate. 

   Consultate [Opzioni dei predefiniti immagine](application-setup.md#image_preset_options).

1. Seleziona **[!UICONTROL Salva]** oppure, se hai iniziato da un predefinito esistente, seleziona **[!UICONTROL Salva con nome]**.
1. Per visualizzare l&#39;anteprima del predefinito con la tua immagine, seleziona **[!UICONTROL Sfoglia]** e seleziona un&#39;immagine. Per visualizzare l&#39;anteprima con l&#39;immagine predefinita, selezionare **[!UICONTROL Ripristina]**.

Per modificare un predefinito per immagini, selezionane il nome nella schermata Predefiniti immagini e seleziona **[!UICONTROL Modifica]**. Per eliminare un predefinito per immagini, selezionalo e seleziona **[!UICONTROL Elimina]**.

### Opzioni dei predefiniti immagine {#image-preset-options}

Nelle schermate Aggiungi predefinito e Modifica predefinito sono disponibili le seguenti opzioni per creare e modificare i predefiniti immagine:

* **[!UICONTROL Nome predefinito]**  - Inserisci un nome descrittivo senza spazi vuoti. Per aiutare gli utenti a identificare questo predefinito per immagini, includi nel nome la specifica della dimensione dell’immagine.

* **[!UICONTROL Larghezza e altezza]** : immetti in pixel le dimensioni in cui l’immagine viene distribuita.

* **[!UICONTROL Formato]** : consente di selezionare un formato dal menu. Quando si sceglie il formato GIF, JPEG, PDF o TIFF vengono visualizzate più opzioni:

   * Opzioni Quantizzazione colore GIF

      * **[!UICONTROL Tipo]** : seleziona Adattivo (opzione predefinita), Web o Macintosh. Se si seleziona **[!UICONTROL GIF con Alpha]**, l&#39;opzione Macintosh non è disponibile.

      * **[!UICONTROL Dither]**  - Selezionare Diffusa o Disattivata.

      * **[!UICONTROL Numero di colori]**  - Trascinare il cursore per inserire 2-255.

      * **[!UICONTROL Elenco colori]**  - Inserisci un elenco separato da virgole. Ad esempio, per bianco, grigio e nero inserite `000000,888888,ffffff`.
   * Opzioni JPEG

      * **[!UICONTROL Qualità]**  - Controlla il livello di compressione JPEG. Questa impostazione interessa sia le dimensioni del file che la qualità dell’immagine. La scala di qualità JPEG è 1-100.

      * **[!UICONTROL Attiva il downsampling della crominanza JPG]** : poiché l&#39;occhio è meno sensibile alle informazioni sui colori ad alta frequenza rispetto alla luminanza ad alta frequenza, le immagini JPEG dividono le informazioni sulle immagini in componenti di luminanza e colore. Quando un’immagine JPEG viene compressa, il componente della luminanza viene lasciato alla massima risoluzione, mentre per i componenti colore viene eseguito il downsampling calcolando la media di gruppi di pixel. Il downsampling riduce di metà o un terzo il volume di dati, con impatto trascurabile sulla qualità percepita. Non è possibile eseguire il downsampling sulle immagini in scala di grigio. Questa tecnica riduce il fattore di compressione ed è utile per le immagini ad alto contrasto (ad esempio, immagini con testo sovrapposto).
   * Opzioni PDF e TIFF

      * **[!UICONTROL Compressione]**  - Seleziona un algoritmo di compressione.



* **[!UICONTROL Spazio colore]** : consente di selezionare uno spazio colore.

* **[!UICONTROL Nitidezza]** : seleziona l’opzione Abilita nitidezza semplice per applicare all’immagine un filtro di nitidezza di base dopo che è stata effettuata la modifica in scala. La nitidezza contribuisce a compensare la sfocatura che può prodursi quando si visualizza un’immagine in dimensioni diverse.

   Per ulteriori informazioni sulla nitidezza, le modalità di ricampionamento e la maschera di contrasto, consulta [Nitidezza di un&#39;immagine](sharpening-image.md#sharpening_an_image).

* **[!UICONTROL Modalità di campionamento]**  - Seleziona un&#39;opzione della modalità di ricampionamento. Queste opzioni aumentano la nitidezza quando si esegue il downsampling dell’immagine:

* **[!UICONTROL B-Lineare]** : metodo di ricampionamento più veloce; alcuni artefatti di aliasing sono evidenti.

* **[!UICONTROL Bi-Cubic]**  - Aumenta l&#39;utilizzo della CPU sul server di immagini, ma produce immagini più nitide con artefatti di aliasing meno evidenti.

* **[!UICONTROL Sharp2]**  - Può produrre risultati leggermente più nitidi rispetto all&#39;opzione Bi-Cubic, ma a costi di CPU ancora più elevati sul server di immagini.

* **[!UICONTROL Tri-Lineare]** : utilizza risoluzioni sia superiori che inferiori, se disponibili; consigliato solo quando l’aliasing è un problema. Questo metodo riduce le dimensioni JPEG grazie a una minore quantità di dati ad alta frequenza.

* **[!UICONTROL Maschera definizione dettagli]** : scegli le seguenti opzioni per regolare con precisione la nitidezza:

* **[!UICONTROL Importo]** : controlla la quantità di contrasto applicata ai pixel del bordo. Il valore predefinito è 1,0. Per le immagini ad alta risoluzione, è possibile aumentare questo valore fino a 5,0. Il fattore può essere interpretato come una misura dell’intensità del filtro.

* **[!UICONTROL Raggio]** : determina il numero di pixel intorno ai pixel del bordo che influiscono sulla nitidezza. Per immagini ad alta risoluzione, inserite un valore da 1 a 2. Con un valore basso si agisce solo sui pixel del bordo; con un valore più elevato si agisce su una fascia più ampia di pixel. Il valore più adatto dipende dalle dimensioni dell’immagine.

* **[!UICONTROL Soglia]** : determina l’intervallo di contrasto da ignorare quando viene applicato il filtro Maschera definizione dettagli. In altre parole, questa opzione specifica quale deve essere il grado di differenza dei pixel da rendere più nitidi rispetto all’area circostante, affinché vengano considerati pixel di un bordo e quindi resi più nitidi. Per evitare la comparsa di disturbi, provate con valori compresi tra 0,02 e 0,2. Con il valore predefinito 6 la nitidezza viene applicata a tutti i pixel nell’immagine.

* **[!UICONTROL Spazio colore]** : determina se l’immagine utilizza lo spazio in cui è stata creata, in genere RGB (Originale) o uno spazio di luminanza (Intensità).

* **** ColoreScegli le seguenti opzioni:

* **[!UICONTROL Profilo colore di output]** : seleziona  **[!UICONTROL Usa]** predefinito per uno dei profili colore ICC disponibili nell’Adobe Dynamic Media Classic.

   Consultate anche [Profili ICC](icc-profiles.md#icc_profiles).

* **[!UICONTROL Intento di rendering]** : seleziona un’opzione se desideri ignorare l’intento di rendering predefinito del profilo colore. Utilizza questa opzione quando uno dei profili ICC predefiniti è lo spazio colore di destinazione di una conversione di colore. Oppure, una periferica di output (stampante o monitor) è caratterizzata da questo profilo e l&#39;intento di rendering specificato è valido per questo profilo.

* **[!UICONTROL Incorpora profilo]** : seleziona questa opzione in modo che, se apri questa immagine in Adobe® Photoshop®, utilizzi questo profilo.

* **[!UICONTROL Risoluzione]**  di stampa: selezionare una risoluzione per la stampa dell&#39;immagine; Il valore predefinito è 72 pixel.

* **[!UICONTROL Modificatori URL]** : se preferisci specificare i modificatori URL che definiscono il predefinito immagine, anziché le impostazioni, immetti qui i modificatori .

* **[!UICONTROL URL immagine di esempio]** : elenca la stringa URL &quot;grezza&quot; utilizzata dal server immagini di Dynamic Media per fornire immagini con il predefinito immagine che si sta aggiungendo o modificando. Nella stringa URL vengono codificate tutte le impostazioni di formattazione selezionate nella schermata Aggiungi predefinito o Modifica predefinito.

### Modificare, rimuovere o disattivare un predefinito immagine {#editing-removing-or-deactivating-an-image-preset}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagini]**.
1. Nella schermata Predefiniti immagine, selezionate un predefinito nella tabella ed effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Modifica]** e specifica le nuove opzioni nella finestra di dialogo Modifica predefinito.
   * Seleziona **[!UICONTROL Elimina]** per rimuovere il predefinito dall&#39;elenco.
   * Deseleziona la casella di controllo **[!UICONTROL Attivo]** accanto al nome di un predefinito se desideri rimuoverlo dall&#39;intera interfaccia utente di Adobe Dynamic Media Classic per gli utenti di MediaPortal.

## Attivare o disattivare i predefiniti video adattivi {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic offre predefiniti di codifica per video adattivi. Si tratta di un elenco di predefiniti in cui sono raggruppati i predefiniti per video adattivi da 16:9 e da 4:3. Tali predefiniti riflettono le impostazioni di codifica più comuni e sono ottimizzati per la riproduzione su dispositivi mobili, tablet e computer desktop.

Solo i predefiniti di codifica video adattiva sono attivati (o “abilitati”) per impostazione predefinita. Se necessario, potete disattivarli. I predefiniti per video adattivi non attivati non vengono visualizzati come opzione selezionabile nella sezione eVideo della finestra di dialogo Opzioni processo di caricamento.

Consulta [Caricare e codificare i video](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Per attivare o disattivare i predefiniti video adattivi:**

1. Nell&#39;angolo in alto a destra di Adobe Dynamic Media Classic, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Predefiniti video]** > **[!UICONTROL Predefiniti video adattivi]**.
1. Nella pagina Predefiniti video adattati, deselezionate la casella di controllo accanto al nome di un predefinito per eliminarlo dall’elenco Opzioni eVideo nella finestra di dialogo Opzioni processo di caricamento.
1. Selezionare **[!UICONTROL Chiudi]**.

## Predefiniti video per la codifica di file video {#video-presets-for-encoding-video-files}

Per selezionare un predefinito di codifica, seleziona **[!UICONTROL Opzioni lavoro]** nell’angolo inferiore destro della pagina Carica. Nella finestra di dialogo Opzioni processo di caricamento , espandi Opzioni eVideo e seleziona i predefiniti di codifica video desiderati.

>[!NOTE]
>
>Ad eccezione di &quot;Adaptive Video&quot;, che è abilitato per impostazione predefinita, non è possibile visualizzare tutti gli altri predefiniti di codifica video adattivo o video singolo nella finestra di dialogo Opzioni processo di caricamento. Ad Adobe, gli amministratori di Dynamic Media Classic determinano quali predefiniti di codifica video sono visibili nella finestra di dialogo Opzioni processo di caricamento .

* Seleziona uno dei seguenti predefiniti di codifica video adattiva o di codifica singola:

   * **[!UICONTROL 16:9 Adaptive Video]**  - Crea video con rapporto di formato 16:9 per la distribuzione su desktop, dispositivi mobili (iPhone, iPad, Android™) e tablet (iPad, Android™), ottimizzati con la risoluzione e il bit rate che meglio corrispondono alla velocità di connessione del visualizzatore.

   * **[!UICONTROL Video adattivo 4:3]**  - Crea video con rapporto di formato 4:3 per la distribuzione su desktop, dispositivi mobili (iPhone, iPad, Android™) e tablet (iPad, Android™), ottimizzati con risoluzione e bit rate che corrispondano meglio alla velocità di connessione del visualizzatore.

   * **[!UICONTROL Video adattivo]** : un singolo predefinito di codifica che funziona con qualsiasi proporzione per creare video da distribuire a dispositivi mobili, tablet e desktop. I video sorgente caricati e codificati con questo predefinito sono impostati su un’altezza specifica. Tuttavia, il valore della larghezza viene ridimensionato automaticamente per mantenere le proporzioni del video.

      La flessibilità di questo ridimensionamento automatico è disponibile anche per impostazione predefinita quando create un predefinito di codifica video personalizzato.

      Consulta [Aggiungere o modificare un predefinito di codifica video](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL Codifica video adattiva (16:9 o 4:3)]**  - Crea video con rapporto di formato 16:9 e 4:3 per la distribuzione su desktop, dispositivi mobili (iPhone, iPad, Android™) e tablet (iPad, Android™). Tutto ottimizzato con la risoluzione e il bit rate che meglio corrispondono alla velocità di connessione del visualizzatore.

      Consultate [Predefiniti per codifica video adattiva (16:9 o 4:3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   * **[!UICONTROL Predefiniti codifica singola]**

      >[!NOTE]
      >
      >Per inviare un video agli iPad, puoi selezionare un predefinito di codifica Mobile o un predefinito di codifica Tablet . I predefiniti Tablet sono stati creati appositamente per gli iPad, generalmente con risoluzione e qualità più alta per usufruire delle dimensioni delle schermo e della connessione di banda più elevata. La visualizzazione di file video codificati con un predefinito Tablet richiede di includere un codice di rilevamento dispositivi al sito mobile o all’applicazione. questo codice è disponibile per i video visualizzati su iPhone o iPad, a seconda del dispositivo di riproduzione. Se si sceglie un predefinito Mobile per la consegna dei file video ad iPad, il flusso di lavoro risulta semplificato poiché potete scegliere lo stesso file video sia per iPhone che per iPad. Tuttavia, la qualità viene standardizzata all’esperienza iPhone con risoluzione ridotta.

      * Nel gruppo Predefiniti di codifica, nell’elenco a discesa Ordina predefiniti codifica, selezionate Nome o Dimensioni per ordinare i predefiniti per nome o per dimensione di risoluzione.
      * Seleziona un predefinito di codifica in base alle dimensioni della risoluzione e alla larghezza di banda con cui intendi riprodurre il video.
      * È possibile selezionare Codifica video adattiva e uno o più predefiniti di codifica per video. Ad esempio, potete codificare un file per desktop e dispositivo mobile in un unico processo di caricamento.

Dopo aver selezionato **[!UICONTROL Avvia il caricamento]**, il file video principale originale viene caricato e i file codificati vengono generati dal file principale.

### Le opzioni dei predefiniti di codifica {#about-encoding-preset-options}

I parametri delle opzioni dei predefiniti di codifica sono i seguenti:

* **[!UICONTROL Velocità di connessione di destinazione]** : la velocità di connessione Internet dell&#39;utente finale di destinazione.

* **[!UICONTROL Suffisso file codificato]** : il suffisso allegato al file video codificato a scopo di identificazione.

* **[!UICONTROL Bit rate video (velocità dati)]** : la quantità di dati codificati per creare un secondo di riproduzione video (in kilobit al secondo).

* **[!UICONTROL Larghezza/Altezza]**  pixel: dimensione della larghezza dell’immagine dello schermo, in pixel; la dimensione in altezza dell’immagine dello schermo (in pixel).

* **[!UICONTROL Frame al secondo (fps)]**  - Il numero di fotogrammi o immagini fisse per ogni secondo di video. Negli Stati Uniti e in Giappone, i video sono solitamente ripresi a 29,97 fps; in Europa e in Asia (escluso il Giappone), sono invece ripresi a 25 fps. I film sono ripresi a 24 fps.

* **[!UICONTROL Bit rate]**  audio: la quantità di dati codificati per creare un secondo di riproduzione audio, espressa in kilobit al secondo.

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

Di seguito sono elencati i predefiniti di codifica disponibili per video adattivi; combinano una serie di singoli predefiniti di codifica selezionati automaticamente in base alle proporzioni del video caricato. Ad esempio, se caricate un video da 4:3, questo viene codificato automaticamente utilizzando i cinque predefiniti da 4:3 inclusi nell’elenco dei predefiniti principali per l’opzione **Codifica video adattiva (16:9 o 4:3)**.

Per informazioni sui parametri delle opzioni di codifica, consultate [Le opzioni dei predefiniti di codifica](application-setup.md#about_encoding_preset_options).

**Predefiniti per codifica video adattiva (16:9 o 4:3)**

|  | Nome predefinito di codifica/Descrizione | Velocità di connessione di destinazione (Kbps) | Suffisso del file codificato | Velocità dati video (Kbps) | Larghezza/Altezza (Pixel) | Fps | Bitrate audio (Kbps) | Consigli |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384x288 | Come sorgente | 64 | Bassa risoluzione, 3G |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512x288 | Come sorgente | 64 | Risoluzione media, 3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_384x288_600 | 800 | 384 x 288 | Come sorgente | 64 | Risoluzione media, 3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640x360 | Come sorgente | 80 | Risoluzione media, WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x480_800K | 600 | 640x480 | Come sorgente | 80 | Risoluzione media, WiFi |
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
| 1 | 16:9, 800x450 (1200 Kbps) | 1,5 Mbps | _800x450_1200K | 1200 | 800x450 | Come sorgente | 96 | Risoluzione medio-alta |
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
| 1 | 16:9, 800x450 (1200 Kbps), OGG | 1,5 Mbps | _OGG_800x450_1200K | 1200 | 800 x 450 | Come sorgente | 96 | Risoluzione medio-alta |
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
| 1 | 16:9, 512x288, Mobile (800 Kbps) | 900 | _Mobile_512x288_800K | 800 | 512x288 | Come sorgente | 80 | Risoluzione media, Wi-Fi |
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
>**Avviso sulla fine del ciclo di vita dei visualizzatori di Flash** : a partire dal 31 gennaio 2017, Adobe Classic ha ufficialmente terminato il supporto per la piattaforma di visualizzatori di Flash.

Un *predefinito per visualizzatori* è un gruppo di impostazioni con cui viene definito in che modo le risorse multimediali verranno visualizzate sullo schermo del computer e sui dispositivi mobili dell’utente. In qualità di amministratore, potete creare dei predefiniti per visualizzatori. Sono disponibili impostazioni per un’ampia gamma di opzioni di configurazione dei visualizzatori. Ad esempio, è possibile modificare le dimensioni dello schermo del visualizzatore, il comportamento dello zoom, gli schemi di colori, i bordi e i font.

Come best practice, utilizza i visualizzatori video HTML5 di Adobe Classic. I predefiniti utilizzati nei visualizzatori Video HTML5 sono lettori video affidabili.

Combinando in un singolo player quanto segue:

* La possibilità di progettare i componenti di riproduzione utilizzando HTML5 e CSS.
* Riproduzione incorporata.
* Utilizza lo streaming adattivo e progressivo a seconda delle funzionalità del browser.

Estendi la portata dei contenuti rich media agli utenti desktop, tablet e dispositivi mobili e assicurati un’esperienza video semplificata.

Consulta [Informazioni sui visualizzatori HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) nella Guida di riferimento per i visualizzatori di Adobi.

Consulta [Adobe Matrice di compatibilità dei predefiniti per visualizzatori Dynamic Media Classic](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Consultate [Procedura ottimale: utilizzo del visualizzatore video HTML5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

In base al visualizzatore, potete aggiungere delle funzioni per community. e comprendono i pulsanti Incorpora, E-mail, Collega e Visita. Questi pulsanti consentono agli utenti che utilizzano i visualizzatori di condividere il visualizzatore con altri utenti o di aprire il sito Web Adobe Dynamic Media Classic.

Consulta anche [Esempi della libreria di riferimento visualizzatori di Adobi](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Supporto nei visualizzatori per pagine Web reattive {#viewer-support-for-responsive-designed-web-pages}

Diversi tipi di pagine Web hanno esigenze differenti. A volte si desidera una pagina web che fornisca un collegamento che apre il visualizzatore HTML5 in una finestra separata del browser. In altri casi, è necessario incorporare il visualizzatore HTML5 direttamente nella pagina di hosting. In quest&#39;ultimo caso, la pagina web ha probabilmente un layout statico. Oppure, è &quot;reattivo&quot; e viene visualizzato in modo diverso su diversi dispositivi o per diverse dimensioni della finestra del browser. Per soddisfare queste esigenze, i visualizzatori HTML5 forniti con Adobe Dynamic Media Classic supportano sia pagine web statiche che pagine web reattive.

Per ulteriori informazioni su come incorporare i visualizzatori reattivi nelle pagine web, consulta [Informazioni sulla libreria di immagini reattive](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api), [Utilizzare la libreria di immagini reattive](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api) e [Riferimento ai comandi - Attributi dei comandi](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library).

### Tipi di predefiniti per visualizzatori {#viewer-preset-types}

Gli amministratori possono creare e personalizzare i seguenti tipi di predefiniti per visualizzatori.

* **[!UICONTROL Visualizzatore eCatalog]**  - Simula l’esperienza di lettura di un catalogo stampato. È possibile spostarsi da una pagina all’altra, ingrandire e ridurre gli elementi di una pagina, utilizzare mappe immagine per visualizzare ulteriori informazioni sugli elementi della pagina o cercare nel catalogo. Potete inoltre includere un pannello Info con le informazioni dettagliate su un articolo collegato a una mappa, se all’area della mappa è assegnato un attributo rollover_key valido. Per includere un pannello Info, specificate l’URL di un server informazioni nel riquadro Impostazioni pannello Info, nella finestra Predefinito visualizzatore eCatalog.

* **[!UICONTROL Visualizzatore set di campioni]**  - Visualizza un&#39;immagine in un colore, materiale, texture, finitura o tessuto diverso. Per visualizzare le varianti dell’immagine, gli utenti selezionano una miniatura.

* **[!UICONTROL Visualizzatore set di file multimediali diversi]** : consente di visualizzare diversi tipi di file multimediali in un unico visualizzatore. Potete includere set di campioni, set 360 gradi, immagini e video. Potete configurare schede per diversi tipi di contenuto, ad esempio una scheda per i set di immagini e una scheda per i video. Per la riproduzione dei video da un set di file multimediali diversi viene usato un visualizzatore standard con un indicatore temporale e controlli per interrompere, mettere in pausa, riavvolgere e riprodurre il video. Quando configurate il predefinito per visualizzatori di un set di file multimediali diversi, specificate i visualizzatori da usare per i diversi tipi di risorse del set. Per visualizzare un set di file multimediali diversi potete anche usare il visualizzatore Griglia o Carosello.

* **[!UICONTROL Visualizzatore set 360 gradi]** : fornisce più visualizzazioni di un’immagine che consentono agli utenti di ruotare l’oggetto per esaminare i diversi lati e angoli.

* **Visualizzatore video** : consente di visualizzare i video utilizzando le dimensioni di risoluzione del file sorgente o una dimensione personalizzata. Ad Adobe, Dynamic Media Classic viene fornito con molti predefiniti visualizzatore per la riproduzione di video e, se siete amministratori, potete creare predefiniti visualizzatore video personalizzati. Sono disponibili oltre dodici diverse impostazioni per la configurazione del visualizzatore video. Potete configurare la relativa dimensione, il colore di primo piano e di sfondo, i controlli audio e video, la barra di avanzamento, l’interfaccia utente, le funzioni per social networking e l’Aiuto.

* **[!UICONTROL Visualizzatori zoom]**  - Offre tre tipi di visualizzatori zoom disponibili:

* **[!UICONTROL Zoom Viewer]** : consente agli utenti di ingrandire l’area selezionandola. È possibile selezionare i controlli per ingrandire, ridurre e ripristinare le dimensioni predefinite dell&#39;immagine.

* **[!UICONTROL Visualizzatore zoom: Uscita rapida]** : visualizza una seconda immagine dell’area ingrandita accanto all’immagine originale. Non vi sono controlli; gli utenti devono semplicemente spostare la selezione sull’area da visualizzare.

Quando calcolate l’utilizzo di larghezza di banda totale per questo visualizzatore, tenete presente che nel visualizzatore vengono caricate sia l’immagine principale che l’immagine a comparsa. Le dimensioni dell’immagine principale (Larghezza e Altezza area visualizzazione) e il fattore di zoom determinano le dimensioni dell’immagine a comparsa. Per impedire che le dimensioni del file dell’immagine a comparsa diventino eccessive, bilanciate questi due valori: se le dimensioni dell’immagine principale sono grandi, riducete il fattore di zoom. I valori Larghezza a comparsa e Altezza comparsa determinano le dimensioni della finestra a comparsa ma non dell’immagine a comparsa caricata nel visualizzatore.

Ad esempio, se le dimensioni dell’immagine principale sono 350 x 350 pixel, con un fattore di zoom pari a 3 l’immagine a comparsa risultante sarà di 1050 x 1050 pixel. Se le dimensioni dell’immagine principale sono 300 x 300 pixel, con un fattore di zoom pari a 4 l’immagine a comparsa risultante sarà di 1200 x 1200 pixel. In base alla qualità JPEG impostata (impostazioni consigliate: 80-90), potete ridurre sensibilmente le dimensioni del file. I fattori di zoom consigliati sono i valori compresi tra 2,5 e 4, a seconda delle dimensioni dell’immagine principale.

### Adobe Matrice di compatibilità dei predefiniti per visualizzatori Dynamic Media Classic {#scene-viewer-preset-compatibility-matrix}

**Avviso** sulla fine del ciclo di vita dei visualizzatori di Flash: A partire dal 31 gennaio 2017, Adobe Dynamic Media Classic ha ufficialmente terminato il supporto per la piattaforma di visualizzatori di Flash.

Nella tabella seguente sono elencati i predefiniti per visualizzatori Adobe Classic attualmente disponibili. Viene inoltre specificata la compatibilità con dispositivi desktop e mobili nonché la tecnologia utilizzata per ciascun visualizzatore.

Consulta anche [Esempi della libreria di riferimento visualizzatori di Adobi](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Per informazioni sui browser Web e sulle versioni del sistema operativo supportati per i visualizzatori, consultate le relative Note sulla versione.

Consulta [Note sulla versione di riferimento per visualizzatori di Adobi](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

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
| Universal_HTML5_eCatalog_Adv(Include il supporto per i social media e la ricerca nel catalogo.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Include il supporto per i social media e la ricerca nel catalogo). | HTML5 | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori per set 360 gradi |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**Visualizzatori per eVideo**

Adobe Dynamic Media Classic supporta la riproduzione video mobile per video MP4 H.264.

* I dispositivi BlackBerry® che supportano questo formato video sono disponibili nel seguente sito: [Formati video supportati su BlackBerry®](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* È inoltre possibile trovare i dispositivi Windows® che supportano questo formato video nel seguente percorso: [Formati video supportati su Windows® Phone](https://docs.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ | Smartphone BlackBerry® | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Include il supporto per sottotitoli codificati). Consultate [Procedura consigliata: utilizzo del visualizzatore universale per video HTML5.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social (include il supporto per sottotitoli codificati e social media) | HTML5 | X | X | X | X | X | X | X |

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Set di file multimediali diversi |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Matrice dei gesti supportati dai visualizzatori per dispositivi mobili {#supported-mobile-viewers-gestures-matrix}

La tabella seguente identifica i gesti del visualizzatore mobile supportati sui dispositivi iOS, Android™ 2.x e Android™ 3.x.

|  | Tecnologia del visualizzatore | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizzatori per set di immagini |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Informazioni sulla schermata Preimpostazioni visualizzatore {#about-the-viewer-preset-screen}

Potete creare e gestire i predefiniti per visualizzatori nella schermata Predefiniti per visualizzatore. Per aprire questa schermata, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.

La schermata Predefiniti visualizzatore offre strumenti che consentono di eseguire le seguenti attività:

* **Aggiungi un predefinito** : seleziona  **** Aggiungi e fai clic su nella finestra di dialogo Aggiungi predefinito visualizzatore .

       Consulta [Aggiungere e modificare i predefiniti visualizzatore](application-setup.md#adding_and_editing_viewer_presets).
   
* **Modifica un predefinito** : seleziona un predefinito, quindi seleziona  **[!UICONTROL Modifica]**.

       Consulta [Aggiungere e modificare i predefiniti visualizzatore](application-setup.md#adding_and_editing_viewer_presets).
   
* **Elimina un predefinito** : seleziona un predefinito, quindi seleziona  **[!UICONTROL Elimina]**.

* **Esporta un predefinito** : seleziona un predefinito visualizzatore HTML5, quindi seleziona  **** Esporta per scaricare lo skin del visualizzatore in modo da poterlo utilizzare come base per creare e aggiungere un altro predefinito visualizzatore.

       Consulta [Esportare un predefinito visualizzatore HTML5](application-setup.md#export_an_html5_viewer_preset).
   
* **Filtra l’elenco**  Predefiniti visualizzatore : utilizza questi strumenti per filtrare l’elenco:

       * Apri l’elenco a discesa **Attivo/Inattivo** e seleziona un’opzione per mostrare i predefiniti attivi, inattivi o tutti i predefiniti.
       * Apri l’elenco a discesa **Visualizzatore** e seleziona un’opzione per visualizzare solo i visualizzatori di un determinato tipo. Seleziona **[!UICONTROL Tutti i visualizzatori]** per visualizzare tutti i visualizzatori.
   
* **Ordina predefiniti** : seleziona un’intestazione di colonna (**[!UICONTROL Attivo]**,  **[!UICONTROL Tipo]**,  **[!UICONTROL Predefinito]** o  **[!UICONTROL Piattaforma]**) per ordinare l’elenco in base a una colonna. Seleziona un’intestazione di colonna una seconda volta per ordinare l’elenco in ordine decrescente (o crescente).

* **Attiva e disattiva i predefiniti** : seleziona un predefinito, quindi seleziona la relativa opzione Attivo per attivarlo o disattivarlo.

       Consultate [Attivare o disattivare i predefiniti visualizzatore](application-setup.md#activating_or_deactivating_viewer_presets).
   
>[!NOTE]
>
>Seleziona **[!UICONTROL Anteprima]** sul lato destro della pagina Predefiniti visualizzatore per verificare l’aspetto di una risorsa nel predefinito visualizzatore selezionato. Per visualizzare una risorsa diversa, seleziona **[!UICONTROL Sfoglia]** nella pagina Predefiniti visualizzatore e seleziona una risorsa diversa nella finestra di dialogo Seleziona anteprima risorsa .

### Aggiungere e modificare i predefiniti visualizzatore {#adding-and-editing-viewer-presets}

Oltre ad aggiungere i predefiniti visualizzatore utilizzando **[!UICONTROL Aggiungi]** nell’interfaccia utente, puoi anche utilizzare **[!UICONTROL Esporta]** per aggiungere un predefinito visualizzatore. È sufficiente esportare un predefinito visualizzatore HTML5 esistente e utilizzarlo come base per il nuovo predefinito.

Consulta [Esportare un predefinito visualizzatore HTML5](application-setup.md#exporting_an_html5_viewer_preset).

**Per aggiungere o modificare dei predefiniti per visualizzatori:**

1. Nell’angolo in alto a destra di Adobe Dynamic Media Classic, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.

   Potete filtrare l’elenco dei predefiniti. Ad esempio, per visualizzare soltanto i predefiniti per i visualizzatori video, selezionate Visualizzatore video dall’elenco a discesa Visualizzatori nella barra degli strumenti che si trova appena sopra la tabella.

1. Nella pagina Predefiniti visualizzatore , aggiungi o modifica il predefinito visualizzatore nella schermata Predefiniti visualizzatore .

   * **Aggiungi** : nella barra degli strumenti, seleziona  **[!UICONTROL Aggiungi]**. Nella finestra di dialogo Aggiungi predefinito visualizzatore , seleziona una piattaforma e un tipo di risorsa rich media.

          Al termine della creazione del predefinito visualizzatore, seleziona **[!UICONTROL Salva con nome]**.
      
   * **Aggiungi iniziando da un predefinito visualizzatore esistente** . Nella tabella, seleziona un predefinito visualizzatore video e seleziona  **** Modifica nella barra degli strumenti.

          Dopo aver riconfigurato il Visualizzatore video, seleziona **[!UICONTROL Salva con nome]** per salvare il predefinito utilizzando un nome diverso nel campo di testo Nome predefinito.
      
   * **Modifica** : seleziona un predefinito per visualizzatori esistente, quindi seleziona  **[!UICONTROL Modifica]**.

1. Nella schermata Configura visualizzatore, immetti o modifica il nome del predefinito nel campo Nome predefinito .
1. Impostate le opzioni rimanenti in base alle vostre esigenze.

   >[!NOTE]
   >
   >Seleziona **[!UICONTROL Come sorgente]** per ridimensionare automaticamente il visualizzatore video in base alle dimensioni di risoluzione del video codificato stesso. Se si seleziona questa opzione, non è possibile immettere la larghezza e l&#39;altezza dello stage. e tali valori verranno invece determinati dal video stesso. Se si seleziona **[!UICONTROL Come origine]**, impostare l&#39;opzione Dimensione margine in modo che rifletta le dimensioni dell&#39;interfaccia all&#39;esterno dell&#39;area di riproduzione video. Le dimensioni del margine corrispondono all’altezza e alla larghezza in pixel dei controlli video. L’immagine seguente consente di determinare le dimensioni del margine da utilizzare.*

   ![Configurazione del margine del visualizzatore video](assets/vs_video_viewer_configure_margin.png)

1. Effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Salva con nome]** se hai aggiunto un predefinito visualizzatore a partire da un predefinito esistente.
   * Seleziona **[!UICONTROL Salva]** se hai aggiunto o modificato un predefinito visualizzatore.

### Esportare un predefinito per visualizzatori HTML5 {#exporting-an-html-viewer-preset}

È possibile esportare un predefinito per visualizzatori HTML5 esistente da usare come base per la creazione di un predefinito per visualizzatori HTML5. In questo modo si evita di dover creare un visualizzatore da zero. Se esportate un predefinito con aspetto e comportamento simili a quelli desiderati, potrete usarlo come base di partenza per apportare le regolazioni necessarie.

Tutti i file CSS predefiniti del visualizzatore in Adobe Dynamic Media Classic utilizzano percorsi di trasmissione delle immagini relativi che puntano alle risorse su `Scene7SharedAssets`. Ad esempio, il seguente è un percorso relativo a una risorsa immagine in un file CSS predefinito per visualizzatori su

`Scene7SharedAsset`:  `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

Tuttavia, se si ospitano file CSS del visualizzatore sul proprio sito, è necessario risolvere questi percorsi immagine relativi utilizzando un percorso esplicito del server immagini nel proprio ambiente. Ad esempio, se devi aggiornare il percorso relativo sopra a un percorso esplicito, potrebbe essere simile al seguente, dove `https://s7d1.scene7.com` è il percorso diretto al server di immagini: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Per esportare un predefinito visualizzatore HTML5:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Nella barra degli strumenti Predefiniti visualizzatore, seleziona **[!UICONTROL HTML5]** dal secondo elenco a discesa a sinistra.
1. Selezionate **[!UICONTROL Tutti i visualizzatori]** nel terzo elenco a discesa da sinistra.
1. Seleziona il predefinito per visualizzatori da usare come base per un nuovo predefinito per visualizzatori HTML5.
1. Nella barra degli strumenti, seleziona **[!UICONTROL Esporta]**.
1. Nella finestra di dialogo Esporta risorse selezionate, seleziona **[!UICONTROL Invia esportazione]**.

   Dopo l’esportazione, ottieni un file CSS. Scaricate e decomprimete il file.

1. Aprite il file CSS in un Editor CSS, apportate le modifiche e salvate il file.
1. Carica il file CSS in Adobe Dynamic Media Classic.

   Consultate [Caricamento dei file](uploading-files.md#uploading_files).

1. Pubblica il file CSS sul server di immagini Dynamic Media.

   Consultate [Pubblicazione dei file](publishing-files.md#publishing_files).

1. Aggiungete il nuovo predefinito per visualizzatori seguendo la procedura standard. Seleziona il file CSS del visualizzatore caricato.

   Consultate [Aggiunta e modifica dei predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets).

### Attivare o disattivare i predefiniti visualizzatore {#activating-or-deactivating-viewer-presets}

Per creare un URL per la visualizzazione delle risorse, gli utenti aprono l’elenco a discesa Predefiniti nella finestra di dialogo Anteprima, selezionano un predefinito visualizzatore, quindi selezionano **[!UICONTROL Copia URL]** (consulta [Copia l’URL di un predefinito visualizzatore](application-setup.md#copying_the_url_of_a_viewer_preset)). Questo elenco di predefiniti offre i predefiniti per visualizzatori aggiunti e gestiti dagli amministratori nella schermata Predefiniti per visualizzatore. Ad esempio, tutti i predefiniti per visualizzatori eCatalog attivi vengono visualizzati nell’elenco a discesa Predefiniti nella finestra di dialogo Anteprima quando un utente esegue l’anteprima di un eCatalog.

Se i predefiniti per visualizzatori non vengono disattivati nella schermata Predefiniti per visualizzatore, nell’elenco a discesa Predefiniti nella finestra di dialogo Anteprima potrebbero accumularsi troppi predefiniti. 

**Per attivare o disattivare i predefiniti per visualizzatori:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Nella pagina Predefiniti visualizzatore , seleziona o deseleziona le opzioni **[!UICONTROL Attivo]** per attivare o disattivare i predefiniti visualizzatore.

### Copiare l’URL di un predefinito per visualizzatori {#copying-the-url-of-a-viewer-preset}

Una volta pubblicata una risorsa, potete copiare un URL per visualizzare la risorsa con le impostazioni di un predefinito per visualizzatore.

L’URL viene copiato negli Appunti. Potete utilizzarlo come desiderate nel codice HTML di una pagina Web, in un dispositivo mobile o in un’applicazione.

**Per copiare l’URL di un predefinito per visualizzatori:**

1. Selezionate la risorsa nel pannello Sfoglia.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Vista griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato.
   * Selezionare **[!UICONTROL Vista griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi, sotto l’immagine miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Copia URL]**.

   * Selezionare **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi, a destra della miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Copia URL]**.

   * Selezionare **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]** o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Copia URL]**.

### Copiare il codice di incorporamento di un predefinito per visualizzatori {#copying-the-embed-code-of-a-viewer-preset}

La funzione Incorpora codice permette di analizzare il codice visualizzatore del predefinito per visualizzatori selezionato. Potete anche copiare il codice negli Appunti per poi incollarlo nelle pagine Web su cui verrà distribuito il visualizzatore. 

La modifica del codice non è consentita nella finestra di dialogo Incorpora codice.

**Per copiare il codice da incorporare di un predefinito per visualizzatori:**

1. Selezionate la risorsa nel pannello delle risorse.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Vista griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL a destra, seleziona **[!UICONTROL Codice di incorporamento]**.
   * Selezionare **[!UICONTROL Vista griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi, sotto l’immagine miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi, a destra della miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]** o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.
   Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

1. Nella finestra di dialogo Incorpora codice selezionare **[!UICONTROL Copia negli Appunti]**.
1. Selezionare **[!UICONTROL Chiudi]**.

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

1. Nell&#39;elenco a discesa Configurazione, selezionare **[!UICONTROL Impostazione applicazione]**.
1. Nella finestra Configurazione, nel riquadro a sinistra, vai a **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Visualizzatori]**
1. Seleziona **[!UICONTROL Visualizzatori predefiniti]**.
1. Nella finestra Visualizzatori predefiniti, nell’elenco a discesa per ogni tipo di risorsa, selezionate il visualizzatore da associare all’anteprima della risorsa.
1. Nell&#39;angolo in basso a destra della finestra Visualizzatori predefiniti, seleziona **[!UICONTROL Salva impostazioni]**.
1. Nell&#39;angolo in basso a destra della finestra Configurazione, selezionare **[!UICONTROL Chiudi]** per tornare alla finestra Risorsa.

## Visualizzazione metadati {#metadata-views}

I *metadati* sono informazioni standardizzate su una risorsa. Potete utilizzare i metadati per semplificare il flusso di lavoro, organizzare le risorse e migliorare le ricerche. Adobe Dynamic Media Classic supporta lo standard IPTC (International Press Telecommunications Council) e lo standard XMP (Extensible Metadata Platform). Prima che gli utenti visualizzino o immettano i metadati di una risorsa in Vista dettagli, possono aprire il menu Visualizzazioni metadati . Da qui, possono selezionare il set di campi di metadati che desiderano visualizzare o utilizzare per descrivere la risorsa.

Adobe Dynamic Media Classic viene fornito con Visualizzazioni metadati predefinite e gli amministratori possono creare le proprie Visualizzazioni metadati per consentire agli utenti di scegliere quando inserire i metadati.

### Creazione di una visualizzazione metadati {#creating-a-metadata-view}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Visualizzazioni metadati]**.
1. Selezionare **[!UICONTROL Aggiungi]**.
1. Nel campo di testo Nome predefinito , immetti un nome per la visualizzazione.
1. (Facoltativo) Selezionare **[!UICONTROL Imposta come predefinito]** per fare in modo che questa visualizzazione sia quella visibile agli utenti quando aprono il pannello Metadati in Vista dettagli.
1. (Facoltativo) Selezionare **[!UICONTROL Includi UDF]** per includere nella visualizzazione i campi definiti dall&#39;utente. Questi vengono presentati nella parte superiore del pannello Metadati in visualizzazione Dettagli.
1. Selezionare i campi desiderati per la visualizzazione (selezionare **[!UICONTROL Seleziona tutto]** per selezionare tutti i campi).
1. Selezionare **[!UICONTROL Salva]**.

   Le categorie e i campi selezionati per la visualizzazione vengono visualizzati nel pannello Anteprima.

### Gestione delle visualizzazioni metadati {#managing-metadata-views}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Visualizzazioni metadati]**.
1. Effettuate una delle seguenti operazioni:

   * Per visualizzare un’anteprima di una visualizzazione, selezionatela. I campi della visualizzazione vengono visualizzati nel pannello Anteprima.
   * Per modificare una visualizzazione, selezionala e seleziona **[!UICONTROL Modifica]**. Selezionare o deselezionare i nomi dei campi nel pannello Anteprima e selezionare o deselezionare l&#39;opzione **[!UICONTROL Includi UDF]**.
   * Per eliminare una visualizzazione, selezionarla e selezionare **[!UICONTROL Elimina]**.
   * Per rendere una visualizzazione predefinita, selezionala, quindi seleziona **[!UICONTROL Imposta come predefinita]**. La visualizzazione predefinita è quella che gli utenti visualizzano quando aprono una risorsa in Vista dettagli e accedono al pannello Metadati.

## Predefiniti per metadati {#metadata-presets}

I predefiniti per metadati consentono agli amministratori di controllare e modificare i metadati assegnati alle risorse. Nella Vista dettagli, un utente può immettere i metadati di una risorsa nei campi forniti a tal fine. Ad esempio, un utente può inserire un nome proprietario, una descrizione del copyright e un indirizzo. Per fare in modo che gli utenti inseriscano queste informazioni in modo accurato e completo, puoi creare i predefiniti per metadati. Quando si sceglie un predefinito per metadati nella visualizzazione dettagli, i campi di metadati vengono compilati con valori predefiniti. Ad esempio, il nome proprietario, la descrizione del copyright e l’indirizzo vengono inseriti automaticamente.

Crea un predefinito per metadati per ogni set di valori di metadati che desideri che gli utenti siano in grado di immettere automaticamente in Vista dettagli per descrivere una risorsa.

### Creazione o modifica di un predefinito per metadati {#creating-or-editing-a-metadata-preset}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Predefiniti metadati]**.
1. Nella schermata Predefiniti metadati, effettuate una delle seguenti operazioni:

   * Per creare un predefinito, seleziona **[!UICONTROL Aggiungi]**. Nel campo di testo Nome modello metadati , digita un nome per il predefinito. Seleziona **[!UICONTROL Visualizzazioni metadati]**, quindi seleziona una visualizzazione dall’elenco a discesa (consulta [Visualizzazioni metadati](application-setup.md#metadata_views)).
   * Per modificare un predefinito esistente, selezionalo dall’elenco Predefiniti metadati , quindi seleziona **[!UICONTROL Modifica]**.

1. Espandete i titoli che desiderate includere nel predefinito e inserite i valori nei diversi campi da includere nel predefinito.
1. Selezionare **[!UICONTROL Salva]**.

   Le categorie e i campi selezionati per il predefinito vengono visualizzati nel pannello dell’anteprima.

### Gestione dei predefiniti per metadati {#managing-metadata-presets}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Predefiniti metadati]**.
1. Effettuate una delle seguenti operazioni:

   * Per visualizzare l’anteprima di un predefinito, selezionate il predefinito. Le informazioni sul predefinito (categorie e campi) vengono visualizzate nella schermata Anteprima.
   * Per eliminare un predefinito, selezionalo e seleziona **[!UICONTROL Elimina]**.

## Campi definiti dall’utente {#user-defined-fields}

I campi metadati definiti dall’utente possono essere creati solo da un amministratore di Media Portal o un amministratore società. I campi personalizzati possono essere utili per organizzare le risorse in Adobe Dynamic Media Classic. Se necessario, è possibile contrassegnare i campi come Attivo. Quando sono attivati, i nomi di questi campi di metadati personalizzati vengono visualizzati nel pannello Metadati in Vista dettagli. Nei campi di metadati definiti dall’utente gli utenti possono immettere informazioni per descrivere le risorse. Gli utenti possono inoltre utilizzare tali campi di metadati come criteri di ricerca.

I campi metadati definiti dall’utente sono utili ad esempio per ritardare il momento di attivazione di una risorsa per un lancio o una promozione. Puoi definire un campo &quot;attivazione&quot; in base al tipo *Data*. Quindi, utilizzando il pannello **[!UICONTROL Metadati]** in Vista dettagli o **[!UICONTROL File]** > **[!UICONTROL Modifica informazioni]**, puoi specificare quando la risorsa viene attivata. Adobe Dynamic Media Classic controlla lo stato di pubblicazione di una risorsa e la cronologia di pubblicazione. Se non rientra nel tempo di attivazione, lo stato di pubblicazione è indicato come &quot;Non pubblicato&quot;.

>[!NOTE]
>
>Per visualizzare i campi definiti dall’utente nel pannello Metadati in Vista dettagli, includi i campi definiti dall’utente in Visualizzazioni metadati. Nella schermata Visualizzazioni metadati, selezionate l’opzione Includi UDF (User-Defined Fields, campi definiti dall’utente). Per ulteriori informazioni, consultate [Visualizzazione metadati](application-setup.md#metadata_views).

>[!NOTE]
>
>Per cercare le risorse utilizzando campi personalizzati definiti dall’utente, passa a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**, quindi seleziona **[!UICONTROL Includi UDF nella ricerca]**. Consultate [Configurazione personale](personal-setup.md#personal_setup).

### Creare un campo di metadati definito dall’utente {#creating-a-user-defined-metadata-field}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Campi definiti dall&#39;utente]**.
1. Seleziona **[!UICONTROL Aggiungi]**
1. Nella finestra di dialogo Campo personalizzato, impostate le opzioni desiderate.

   * **[!UICONTROL Nome]** : immetti un nome per il campo metadati.

   * **[!UICONTROL Tipo]** : seleziona un’opzione che definisce il tipo di informazioni che gli utenti possono immettere nel campo metadati:

   * **[!UICONTROL Stringa]**  - Una stringa di testo.

   * **[!UICONTROL Int]**  - Un numero intero.

   * **[!UICONTROL Mobile]**  - Un numero a virgola mobile.

   * **[!UICONTROL Sì/No]**  - Un valore booleano sì/no.

   * **[!UICONTROL Data]** : una data. Il formato consentito è GG/MM/AAAA.

   * **[!UICONTROL Nome file]**  - Il nome di un file.

   * **[!UICONTROL Colore]**  - Il nome di un colore.

   * **[!UICONTROL Dimension]** : larghezza e altezza della risorsa.

   * **[!UICONTROL Senza tipo]**  - Per compatibilità con le versioni precedenti. Non selezionate questa opzione.

   * **[!UICONTROL Valore predefinito]** : facoltativamente, immetti il valore che gli utenti avranno più probabilità di immettere nel campo. Il valore immesso diventa il valore predefinito per il nuovo campo creato.

   * **[!UICONTROL Si applica a]** : se lo desideri, seleziona un tipo di risorsa se desideri che il campo metadati sia applicabile solo a un tipo specifico di risorsa.

      >[!NOTE]
      >
      >Selezionare con attenzione l&#39;opzione **[!UICONTROL Si applica a]** perché non è possibile modificare l&#39;opzione **[!UICONTROL Si applica a]** dopo aver creato un campo definito dall&#39;utente. Adobe Dynamic Media Classic consente di modificare il nome, il tipo e il valore predefinito di un campo definito dall&#39;utente, ma non l&#39;impostazione **[!UICONTROL Si applica a]**. *

1. Al termine della creazione del campo metadati, seleziona **[!UICONTROL Salva]** .

### Gestire i campi definiti dall’utente {#manage-user-defined-fields}

Nella schermata Campi definiti dall’utente sono disponibili i comandi necessari per gestire i campi di metadati personalizzati, definiti dall’utente. 

I campi definiti dall’utente possono essere gestiti solo da un amministratore di Media Portal o un amministratore società.

Per aprire questa schermata, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Campi definiti dall&#39;utente]**.

* **Modifica un campo** : seleziona il campo, quindi seleziona  **[!UICONTROL Modifica]**.

* **Elimina un campo** : seleziona il campo, quindi seleziona  **[!UICONTROL Elimina]**.

* **Attiva campo** : seleziona o deseleziona l’opzione  **** Attiva accanto al nome di un campo. Se hai un ruolo di amministrazione aziendale, questa opzione non viene visualizzata. Poiché questa opzione è correlata a MediaPortal, è necessario selezionare (attivare) Mostra funzionalità MediaPortal in Configurazione personale per visualizzare i campi di attivazione.

## Ottimizzare i file {#optimize-files}

Quando carichi i file nell’Adobe Dynamic Media Classic, il sistema li ottimizza per l’archiviazione e la pubblicazione. Tuttavia, se il processo di caricamento viene interrotto, alcune immagini potrebbero non essere ottimizzate. In questo caso viene visualizzato il messaggio “Immagine non ancora ottimizzata”. Tali file possono comunque essere ottimizzati dagli utenti con ruolo di amministratore.

Adobe Dynamic Media Classic esegue ricerche nei file e ottimizza solo le immagini che non erano completamente ottimizzate in precedenza.

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]**, quindi seleziona **[!UICONTROL Ottimizza file]**.
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

   È possibile selezionare la casella di controllo **[!UICONTROL Visualizza codice]** per visualizzare il valore dell&#39;espressione regolare creato accanto alle selezioni del modulo. Qualora la visualizzazione modulo presenti delle limitazioni, potete inserire o modificare tali valori per definire meglio gli elementi di denominazione. Se i valori non possono essere analizzati nella visualizzazione modulo, i campi modulo diventano inattivi.

   >[!NOTE]
   >
   >i campi del modulo disattivati non indicano che l’espressione regolare non è valida. Non è disponibile una funzione di convalida delle espressioni regolari generate. I risultati dell’espressione regolare generata verranno visualizzati per ogni elemento dopo la riga Risultato. L’espressione regolare completa è riportata nella parte inferiore della pagina.

1. Espandete ciascun elemento come opportuno e inserite le convenzioni di denominazione da usare.
1. Se necessario, seleziona **[!UICONTROL Aggiungi]** per aggiungere un’altra convenzione di denominazione per un elemento. Oppure, seleziona **[!UICONTROL Rimuovi]** per eliminare una convenzione di denominazione per un elemento.
1. Seleziona **[!UICONTROL Salva con nome]** e digita un nome per il predefinito. Oppure, seleziona **[!UICONTROL Salva]** se stai modificando un predefinito esistente.

In alternativa, potete usare l’opzione Visualizza codice, senza campi del modulo. In questa visualizzazione puoi creare le definizioni delle convenzioni di denominazione utilizzando esclusivamente espressioni regolari.

Per la definizione sono disponibili due elementi, Corrispondenza e Nome base. Questi campi consentono di definire tutti gli elementi di una convenzione di denominazione e identificare la porzione della convenzione usata per denominare il set in cui sono contenuti. Una convenzione di denominazione individuale di un’azienda può utilizzare una o più righe di definizione per ciascuno di questi elementi. Potete usare tutte le righe necessarie a creare una definizione univoca e raggrupparle in elementi distinti, ad esempio per l’immagine principale, l’elemento colore, l’elemento visualizzazione alternativa e l’elemento campione.

### Creare un predefinito per set di batch {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic utilizza i predefiniti per set di batch per organizzare le risorse che condividono alcune informazioni o contenuti in set di immagini da visualizzare nei visualizzatori. Le ricette predefinite per set di batch vengono eseguite automaticamente insieme ai processi di importazione delle risorse programmati in Adobe Dynamic Media Classic.

Usate la schermata Predefinito set di batch per creare, modificare e gestire i predefiniti per set di batch. Puoi creare tutti i predefiniti necessari per coprire tutti i processi di inserimento delle risorse necessari. Esistono due forme di definizioni di predefiniti per set di batch: uno per una convenzione di denominazione predefinita configurata e uno per convenzioni di denominazione personalizzate create al volo.

È possibile utilizzare il metodo campo modulo per definire un predefinito per set di batch o il metodo del codice, che consente di utilizzare espressioni regolari. Come in **[!UICONTROL Denominazione predefinita]**, è possibile selezionare **[!UICONTROL Vista codice]** contemporaneamente alla definizione nella visualizzazione modulo e all&#39;utilizzo di espressioni regolari per creare le definizioni. In alternativa, potete deselezionare una delle due visualizzazioni e usare solo l’altra.

Vedere anche [Creare un set di batch predefinito per la generazione automatica di un set 360 gradi 2D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**Per creare un predefinito per set di batch:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti set di batch]** > **[!UICONTROL Predefinito set di batch]**. La vista predefinita e **[!UICONTROL Visualizza modulo]**, come impostato nell’angolo in alto a destra della pagina Dettagli.
1. Nel pannello Elenco predefiniti, seleziona **[!UICONTROL Aggiungi]** per attivare i campi di definizione nel pannello Dettagli sul lato destro della pagina.
1. Nel pannello Dettagli, digitate nel campo Nome predefinito il nome da assegnare al predefinito.
1. Selezionate il tipo di predefinito dal menu Tipo set di batch.

   Per generare automaticamente un set 360 gradi, selezionate **[!UICONTROL Set 360 gradi con asse multiplo]** dall’elenco a discesa Tipo set di batch.

1. Effettuate una delle seguenti operazioni:

   * Se utilizzi una convenzione di denominazione predefinita impostata in precedenza in **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti set di batch]** > **[!UICONTROL Denominazione predefinita]**, espandi **[!UICONTROL Convenzioni di denominazione delle risorse]**, quindi seleziona **[!UICONTROL Predefinito]** dall’elenco a discesa Denominazione file.
   * Per definire una convenzione di denominazione durante la configurazione del predefinito, espandi **[!UICONTROL Convenzioni di denominazione delle risorse]**, quindi seleziona **[!UICONTROL Personalizzato]** nell’elenco a discesa Denominazione file .

1. Per Ordine di sequenza, definisci l’ordine delle immagini dopo il raggruppamento del set in Adobe Dynamic Media Classic. Per impostazione predefinita le risorse sono elencate in ordine alfabetico. Tuttavia, potete definirne l’ordine utilizzando un elenco separato da virgole delle espressioni regolari.
1. Per Imposta convenzione di denominazione e creazione, specificate il suffisso o il prefisso da aggiungere al nome di base definito nella convenzione di denominazione della risorsa. Definisci anche dove viene creato il set di immagini nella struttura di cartelle Adobe Dynamic Media Classic.

   Se definisci un numero elevato di set di immagini, mantieni questi set separati dalle cartelle contenenti le risorse stesse. Molti clienti creano una cartella con i set di immagini e reindirizzano l’applicazione in modo che memorizzi in tale cartella i set di batch generati.

1. Selezionare **[!UICONTROL Salva]** nel pannello Dettagli.

### Crea un set di batch predefinito per la generazione automatica di un set 360 gradi 2D {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Potete usare il tipo di set di batch **Set 360 gradi con asse multiplo** per creare una definizione che automatizza la generazione di set 360 gradi 2D. Il raggruppamento delle immagini utilizza espressioni regolari per riga e colonna per il corretto allineamento delle risorse di immagini nella posizione corrispondente nell’array multidimensionale.

Vedere anche [Creare un Batch Set Preset](application-setup.md#creating_a_batch_set_preset).

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

Con queste informazioni, la ricetta Tipo set di batch può essere creata come segue:

![Immagine ricetta set di batch](assets/se_batch_set_recipe.png)

Il raggruppamento per la parte del nome della risorsa condivisa del set 360 gradi viene aggiunto al campo Match (Corrispondenza) (come evidenziato). La parte variabile del nome della risorsa, contenente la riga e la colonna, viene aggiunta rispettivamente ai campi Riga e Colonna.

Quando il set 360 gradi viene caricato e pubblicato, puoi attivare il nome della definizione del set 360 gradi 2D che è riportato in **[!UICONTROL Predefiniti set di batch]**, nella finestra di dialogo Opzioni processo di caricamento.

**Per creare un predefinito per set di batch per la generazione automatica di un set 360 gradi 2D:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti set di batch]** > **[!UICONTROL Predefinito set di batch]**. La vista predefinita e **[!UICONTROL Visualizza modulo]**, come impostato nell’angolo in alto a destra della pagina Dettagli.
1. Nel pannello Elenco predefiniti, seleziona **[!UICONTROL Aggiungi]** per attivare i campi di definizione nel pannello Dettagli sul lato destro della pagina.
1. Nel pannello Dettagli, digitate nel campo Nome predefinito il nome da assegnare al predefinito.
1. Nel menu a discesa Tipo set di batch, seleziona **[!UICONTROL Set risorse]**.
1. Nell’elenco a discesa Sottotipo, selezionate **[!UICONTROL Set 360 gradi con asse multiplo]**.
1. Espandi **[!UICONTROL Convenzioni di denominazione delle risorse]**, quindi seleziona **[!UICONTROL Personalizzato]** nell’elenco a discesa Denominazione file .
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
   >Se la combinazione di espressioni regolari per riga e colonna non è in grado di determinare la posizione della risorsa all’interno della matrice del set 360 gradi multidimensionale, tale risorsa non viene aggiunta al set e viene registrato un errore.

1. Per Imposta convenzione di denominazione e creazione, specificate il suffisso o il prefisso da aggiungere al nome di base definito nella convenzione di denominazione della risorsa. Definisci anche dove viene creato il set di immagini nella struttura di cartelle Adobe Dynamic Media Classic.

   Se definisci un numero elevato di set di immagini, mantieni questi set separati dalle cartelle contenenti le risorse stesse. Molti clienti creano una cartella con i set di immagini e reindirizzano l’applicazione in modo che memorizzi in tale cartella i set di batch generati.

1. Selezionare **[!UICONTROL Salva]** nel pannello Dettagli.
1. Caricate e pubblicate normalmente il set 360 gradi, assicurandovi di attivare il nome del set 360 gradi 2D nella finestra di dialogo Opzioni processo di caricamento, nella sezione Predefiniti per set di batch.

>[!MORELIKETHIS]
>
>* [Visualizzare un&#39;anteprima di una risorsa](previewing-asset.md#previewing_an_asset)
>* [Impostazione dei predefiniti per immagini](setting-image-presets.md#setting_up_image_presets)
>* [Visualizzare, aggiungere ed esportare metadati](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Controllare i file di processo](checking-job-files.md#checking_job_files)

