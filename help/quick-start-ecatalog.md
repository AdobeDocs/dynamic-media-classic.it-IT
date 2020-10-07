---
title: '"Avvio rapido: eCatalog"'
seo-title: '"Avvio rapido: eCatalog"'
description: 'null'
seo-description: Introduzione e avvio rapido agli eCatalog per consentirvi di imparare a usare le tecniche eCatalog in modo rapido.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
translation-type: tm+mt
source-git-commit: 83b88623b898fdadd1b334b1c12901830c831c5c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Avvio rapido: eCatalog{#quick-start-ecatalogs}

Un eCatalog è la versione digitale per il Web di un materiale originariamente destinato alla stampa, come ad esempio un catalogo, una brochure, un volantino, un manuale di un prodotto o un annuncio pubblicitario. Un eCatalog può essere visualizzato in un sito Web mediante un visualizzatore per eCatalog. Tale visualizzatore simula l’esperienza della lettura di una copia stampata. A seconda delle impostazioni selezionate per l’eCatalog, il visualizzatore può effettuare le seguenti operazioni:

* Cercate una parola chiave o parole chiave nel catalogo. I risultati della ricerca vengono visualizzati come elenco di miniature in un pannello di ricerca sul lato sinistro del catalogo. Ogni miniatura selezionabile rappresenta un set di pagine affiancate di catalogo in cui è stato trovato il termine di ricerca evidenziato.

* condividere il catalogo tramite social media; scaricare il catalogo per visualizzare offline; abilitare i preferiti per contrassegnare rapidamente gli elementi a cui si desidera tornare oppure per stampare il catalogo.
* Spostarsi nel catalogo utilizzando il sommario o la visualizzazione griglia delle pagine; in avanti o indietro facendo clic sul bordo centrale di una pagina.
* Ingrandire, ridurre e scorrere per esaminare i vari elementi presenti in una pagina
* Passare il puntatore su un’area della pagina (chiamata Mappa immagine) per ottenere una finestra a comparsa con informazioni su un particolare elemento
* Fare clic su un’area della pagina per aprire una nuova pagina Web con altre informazioni su un particolare elemento
* Scrivere una nota e allegarla a una pagina eCatalog
* Toccare le icone mappa immagine per avviare le relative pagine Web o i pannelli di informazioni contestuali
* Usare gesti quali avvicinare le dita per ingrandire o passare il dito per voltare pagina
* Effettuare ricerche di elementi mediante parole chiave

![eCatalog visualizzato dagli utenti finali. A) Pagina di apertura dell’eCatalog. B)eCatalog turned to page 2.](/help/assets/ec_cat_viewer_popup.png)

Per creare un eCatalog, di solito vengono utilizzati file PDF ad alta risoluzione creati con Adobe® Acrobat® o con un altro programma per la stampa. Tuttavia potete anche creare un eCatalog da file di immagini.

Durante la creazione di un eCatalog, potete ordinare le pagine o affiancarle come desiderate. Potete anche scegliere se visualizzare pagine singole o affiancare due o più pagine. Potete creare delle mappe immagine per specifiche aree di una pagina in modo che gli utenti possano, ad esempio, fare clic su un’area della pagina per aprire una nuova pagina nel sito Web. Potete gestire il testo di rollover visualizzato utilizzando le impostazioni del pannello Info nella schermata eCatalog. Potete inoltre configurare il visualizzatore per eCatalog scegliendo tra 100 diverse opzioni di configurazione. Potete adattare le funzioni e l’aspetto del visualizzatore in base alle esigenze di utenti specifici.

>[!NOTE]
>
>Se siete utenti in modalità AEM contenuti multimediali dinamici - Scene7 e desiderate usare gli eCatalog, dovrete modificare il `pdfbrochure` valore in CRXDE Lite. A tale scopo, in AEM fare clic su **[!UICONTROL Strumenti > Generale > CRXDE Lite]**. Nella struttura di navigazione del pannello a sinistra, andate a `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Nel riquadro in basso a destra, nella scheda **[!UICONTROL Proprietà]** , selezionare la `jobParam` riga. Impostate il valore per `pdfbrochure` da `false` a `true`. Come `pdfbrochure=true`
>
>Nell’angolo in alto a sinistra della pagina dei CRXDE Lite, fate clic su **[!UICONTROL Salva tutto]**.
>
>Ora potete creare eCatalog in Dynamic Media Classic.

**Avvio rapido**

Questa sezione è stata progettata per aiutarvi a imparare a usare rapidamente gli eCatalog. Seguite i passaggi da 1 a 7. Alla fine di ciascun passaggio è riportato un riferimento a un argomento correlato con ulteriori informazioni.

**1. Caricamento di file PDF**

I file Adobe PDF sono di solito usati come file sorgente per un eCatalog. Poiché sono destinati alla stampa, i file PDF contengono generalmente immagini CMYK. Dynamic Media Classic rileva queste immagini e le converte utilizzando un profilo colore CMYK standard. Se necessario, potete caricare e usare un profilo colore personalizzato.

Fate clic su Carica nella barra di navigazione globale per avviare il caricamento di file PDF o immagini per l’eCatalog. Potete caricare i file dal desktop o via FTP; l’FTP è il metodo consigliato nel caso di molti file o file più grandi di 100 MB.

Le Opzioni PDF nella schermata Carica riguardano il caricamento dei file PDF nella risoluzione e nello spazio colore corretti. Si consiglia di usare una risoluzione di 150 pixel per pollice. Con l’opzione Genera automaticamente eCatalog potete creare un eCatalog durante il caricamento di un file PDF. 

Consultate [Caricamento di file PDF](uploading-pdf-files.md#uploading_the_pdf_files).

**2. Creazione di un eCatalog**

Per creare un eCatalog, selezionate dei file PDF o di immagini nel pannello Sfoglia, fate clic sul pulsante Genera e scegliete eCatalog. Viene visualizzata la schermata eCatalog.

Nella scheda Ordina pagine, selezionate uno dei pulsante Layout (1 immagine, 2 immagini o Personalizzato) per scegliere se presentare le pagine come pagine singole, pagine doppie o più pagine affiancate). Potete riordinare le pagine o pagine affiancate trascinandole oppure, negli eCatalog di grandi dimensioni, scegliendo un nome di pagina nel menu Sposta a.

Per aggiungere delle pagine, selezionate una cartella nella Libreria risorse, quindi trascinate i file PDF o i file di immagini nella schermata Ordina pagine. Invece di numeri di pagina predefiniti, potete fornire nomi di pagina personalizzati o importare una grande quantità di nomi di pagina.

Fate clic su **[!UICONTROL Salva]**, inserite un nome per l’eCatalog, scegliete una cartella Dynamic Media Classic in cui memorizzarlo e fate clic su **[!UICONTROL Salva]**. Each time you change the page order or edit your eCatalog, save your changes by clicking **[!UICONTROL Save]**.

Consultate [Creazione di un eCatalog](creating-ecatalog.md).

**3. Creazione di mappe immagine**

Le mappe immagine aggiungono un’altra dimensione alle pagine eCatalog. Una mappa immagine è l’area di una pagina che fornisce ulteriori informazioni su un elemento. Quando un utenti passa il puntatore su una mappa immagine, viene visualizzata una descrizione dell’elemento. Facendo clic su una mappa immagine si attiva un riferimento esterno per l’apertura di una nuova pagina Web con ulteriori informazioni sull’elemento corrispondente.

Per creare una mappa immagine, aprite la schermata eCatalog. Then go to the **[!UICONTROL Map Pages]** tab of the eCatalog screen, and draw the map with the Rectangle Image Map tool or Polygon Image Map tool. Potete regolare la posizione e la dimensione delle mappe immagine trascinando i bordi delle mappe con lo strumento scorrimento .

Dopo aver disegnato la mappa immagine, inserite l’indirizzo URL a cui accedere quando si fa clic su di essa. Potete anche inserire il testo di rollover visualizzato quando si passa il puntatore sulla mappa immagine. 

Consultate [Creazione di mappe immagine per un eCatalog](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Consultate [Incorporamento di contenuti multimediali in un eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Potete impostare e gestire il testo della mappa immagine mediante le impostazioni del pannello Informazioni nella schermata eCatalog. 

Consultate [Gestione del contenuto del pannello Informazioni](info-panel-content.md#managing-info-panel-content).

**4. Impostazione dei predefiniti per il visualizzatore di eCatalog**

Gli utenti finali possono vedere l’eCatalog nel visualizzatore per eCatalog. Se siete un amministratore, potete configurare il visualizzatore per eCatalog e personalizzarlo modificandone il colore di contorno e selezionando una nuova interfaccia. Dynamic Media Classic viene fornito con diversi predefiniti per visualizzatori di eCatalog &quot;best practice&quot;. Potete scegliere uno di questi predefiniti per la visualizzazione dell’eCatalog. Se siete un amministratore, potete inoltre creare un predefinito personalizzato per visualizzatori di eCatalog.

Per creare un predefinito per visualizzatori di eCatalog, nella barra di navigazione globale fate clic su **[!UICONTROL Configurazione]** e scegliete Predefiniti per **[!UICONTROL visualizzatori]**. Then click **[!UICONTROL Add]**, choose a platform, then click **[!UICONTROL eCatalog > Viewer]**.

Consultate [Impostazione dei predefiniti per il visualizzatore di eCatalog](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

**5. Anteprima dell’eCatalog nel visualizzatore di eCatalog**

I predefiniti per visualizzatori di eCatalog determinano lo stile e il comportamento di tali visualizzatori.

To find out how eCatalog Viewer Presets display your eCatalog, select your eCatalog in the Browse Panel and click **[!UICONTROL Preview]**. La schermata Anteprima si apre nel visualizzatore predefinito.

Notate l’orientamento, lo schema colori, l’aspetto dei controlli per passare alle diverse pagine e come si presentano le pagine voltate. 

Consultate [Anteprima di eCatalog nel visualizzatore di eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

**6. Pubblicazione di eCatalog e PDF associati**

Quando un eCatalog viene pubblicato e i PDF associati, viene inserito sui server immagini per file multimediali dinamici in modo che possa essere trasmesso al sito Web o all’applicazione in cui deve essere visualizzato. Come parte del processo di pubblicazione, Dynamic Media Classic attiva la stringa URL per l’eCatalog. Utilizzate questo URL per richiamare l’eCatalog dai server immagini per file multimediali dinamici al sito Web o all’applicazione.

Per avviare la pubblicazione, contrassegnate l’eCatalog e il PDF per la pubblicazione nel pannello Sfoglia, quindi fate clic sul pulsante Pubblica nella barra di navigazione globale. On the Publish screen, click **[!UICONTROL Start Publish]**.

Consultate [Pubblicazione di eCatalog e PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)associati.

**7. Collegamento di un eCatalog a una pagina Web**

Dynamic Media Classic attiva la stringa di richiesta dell’URL necessaria per visualizzare l’eCatalog quando questo viene pubblicato sui server immagini per elementi multimediali dinamici. Potete copiare questa stringa URL dalla schermata Anteprima e dal pannello Sfoglia (in visualizzazione Dettagli) selezionando l’opzione URL nel pannello. Dopo aver copiato la stringa URL, la potete inserire nei vostri siti Web e nelle vostre applicazioni.

Consultate il personale IT per inserire il collegamento all’eCatalog nella posizione appropriata sulla pagina Web. Quando un utente farà clic sul collegamento, verrà aperto il visualizzatore di eCatalog che consente all’utente di sfogliare l’eCatalog. 

Consultate [Collegamento di un eCatalog a una pagina Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
