---
title: "Guida introduttiva: eCatalog"
description: Introduzione e Guida rapida agli eCatalog per aiutarti a iniziare rapidamente a utilizzare le tecniche di eCatalog in Adobe Dynamic Media Classic.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 36%

---

# Guida introduttiva: eCatalog{#quick-start-ecatalogs}

Un eCatalog è la versione digitale per il Web di un materiale originariamente destinato alla stampa, come ad esempio un catalogo, una brochure, un volantino, un manuale di un prodotto o un annuncio pubblicitario. Un eCatalog può essere visualizzato in un sito Web mediante un visualizzatore per eCatalog. Tale visualizzatore simula l’esperienza della lettura di una copia stampata.

Consulta anche i seguenti video di formazione:

* [Guida introduttiva 1: eCatalog](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Guida introduttiva 2: eCatalog](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

A seconda delle impostazioni selezionate per l&#39;eCatalog, il visualizzatore consente di effettuare le seguenti operazioni:

* Cercare nel catalogo una o più parole chiave. I risultati della ricerca vengono visualizzati sotto forma di elenco di miniature in un pannello di ricerca sul lato sinistro del catalogo. Ogni miniatura cliccabile rappresenta una pagina del catalogo in cui è stato trovato il termine di ricerca evidenziato.

* Condividi il catalogo tramite social media; scarica il catalogo per visualizzarlo offline; abilita Preferiti per contrassegnare gli elementi a cui desideri tornare rapidamente o stampare il catalogo.
* Spostarsi nel catalogo utilizzando il sommario o la visualizzazione griglia della pagina; spostarsi avanti o indietro facendo clic sul bordo centrale di una pagina.
* Ingrandire, ridurre e scorrere per esaminare i vari elementi presenti in una pagina
* Spostare il puntatore su un&#39;area della pagina, denominata Mappa immagine, in modo da visualizzare una finestra popup con informazioni su un elemento.
* Selezionare un&#39;area di pagina per aprire una nuova pagina Web con ulteriori informazioni su un elemento.
* Scrivere una nota e allegarla a una pagina eCatalog
* Tocca le icone della mappa immagine per avviare le pagine web correlate o i pannelli informazioni contestuali.
* Usare gesti quali avvicinare le dita per ingrandire o passare il dito per voltare pagina
* Effettuare ricerche di elementi mediante parole chiave

![L&#39;eCatalog visualizzato agli utenti. A) Pagina di apertura eCatalog. B)eCatalog è passato alla pagina 2.](/help/using/assets/ec_cat_viewer_popup.png)

Per creare un eCatalog, in genere si utilizzano file PDF ad alta risoluzione creati in Adobe Acrobat o in un altro programma di stampa, ma è anche possibile creare un eCatalog da file di immagine.

Durante la creazione di un eCatalog, potete ordinare le pagine o affiancarle come desiderate. Potete anche scegliere se visualizzare pagine singole o affiancare due o più pagine. È possibile creare mappe immagine per le aree della pagina in modo che i visualizzatori possano, ad esempio, selezionare un&#39;area della pagina e aprire una nuova pagina nel sito Web. Potete gestire il testo di rollover visualizzato utilizzando le impostazioni del pannello Info nella schermata eCatalog. Potete inoltre configurare il visualizzatore per eCatalog scegliendo tra 100 diverse opzioni di configurazione. Potete adattare le funzioni e l’aspetto del visualizzatore in base alle esigenze di utenti specifici.

>[!NOTE]
>
>Se sei un utente in modalità Dynamic Media - Scene7 e desideri utilizzare gli eCatalog, modifica il `pdfbrochure` valore in CRXDE Lite. Per farlo, in Adobe Experience Manager, vai a **[!UICONTROL Strumenti]** > **[!UICONTROL Generale]** > **[!UICONTROL CRXDE Lite]**. Nella struttura di navigazione del pannello sinistro, passa a `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Nel riquadro in basso a destra, nella **[!UICONTROL Proprietà]** , seleziona la scheda `jobParam` riga. Imposta il valore per `pdfbrochure` da `false` a `true`. Come in `pdfbrochure=true`
>
>Nell’angolo superiore sinistro della pagina CRXDE Lite, seleziona **[!UICONTROL Salva tutto]**.
>
>Ora puoi creare eCatalog in Adobe Dynamic Media Classic.

Questa sezione è stata progettata per aiutarvi a imparare a usare rapidamente gli eCatalog. Seguite i passaggi da 1 a 7. Dopo ogni passaggio, viene inserito un riferimento incrociato a un titolo di argomento in cui è possibile trovare ulteriori informazioni.

## 1. Caricare i file PDF

I file Adobe PDF sono di solito usati come file sorgente per un eCatalog. Poiché sono destinati alla stampa, i file PDF contengono generalmente immagini CMYK. Adobe Dynamic Media Classic rileva queste immagini e le converte utilizzando un profilo colore CMYK standard. Tuttavia, devi caricare e utilizzare un profilo colore personalizzato.

Sulla barra di navigazione globale, seleziona **[!UICONTROL Carica]** per iniziare a caricare file o immagini PDF per l&#39;eCatalog. Potete caricare i file dal desktop o via FTP; l’FTP è il metodo consigliato nel caso di molti file o file più grandi di 100 MB.

Le Opzioni PDF nella schermata Carica riguardano il caricamento dei file PDF nella risoluzione e nello spazio colore corretti. Si consiglia di usare una risoluzione di 150 pixel per pollice. Con l’opzione Genera automaticamente eCatalog potete creare un eCatalog durante il caricamento di un file PDF. 

Consulta [Carica i file PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Creare un eCatalog

Per creare l&#39;eCatalog, selezionare PDF o file immagine nel pannello Sfoglia. Seleziona **[!UICONTROL Genera]**, quindi scegli **[!UICONTROL eCatalog]**.

Nella pagina eCatalog, nella **[!UICONTROL Ordina pagine]** , selezionare un&#39;opzione Layout: **[!UICONTROL 1 immagine]**, **[!UICONTROL 2 Su]**, o **[!UICONTROL Personalizzato]**. Potete riordinare le pagine o pagine affiancate trascinandole oppure, negli eCatalog di grandi dimensioni, scegliendo un nome di pagina nel menu Sposta a.

Per aggiungere delle pagine, selezionate una cartella nella Libreria risorse, quindi trascinate i file PDF o i file di immagini nella schermata Ordina pagine. Invece dei numeri di pagina predefiniti, puoi fornire nomi di pagina personalizzati o importare più nomi di pagina.

Seleziona **[!UICONTROL Salva]**, immetti un nome per l&#39;eCatalog, scegli una cartella Adobe Dynamic Media Classic per la memorizzazione e seleziona **[!UICONTROL Salva]**. Ogni volta che modifichi l’ordine delle pagine o l’eCatalog, salva le modifiche facendo clic su **[!UICONTROL Salva]**.

Consulta [Creare un eCatalog](creating-ecatalog.md).

## 3. Creare mappe immagine

Le mappe immagine aggiungono un altro aspetto alle pagine eCatalog. Una mappa immagine è l’area di una pagina che fornisce ulteriori informazioni su un elemento. Quando un utenti passa il puntatore su una mappa immagine, viene visualizzata una descrizione dell’elemento. Facendo clic su una mappa immagine si attiva un riferimento esterno per l’apertura di una nuova pagina Web con ulteriori informazioni sull’elemento corrispondente.

Per creare una mappa immagine, aprite la schermata eCatalog. Quindi vai al **[!UICONTROL Mappa pagine]** della schermata eCatalog e inquadrare la mappa con lo strumento Mappa rettangolare immagine o Mappa immagine poligonale. Potete regolare la posizione e la dimensione delle mappe immagine trascinando i bordi delle mappe con lo strumento scorrimento .

Dopo aver inquadrato la mappa immagine, immettere l&#39;indirizzo URL a cui si desidera passare quando si seleziona la mappa immagine. Potete anche inserire il testo di rollover visualizzato quando si passa il puntatore sulla mappa immagine. 

Consulta [Crea mappe immagine eCatalog](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Consulta [Utilizzare le mappe immagine per incorporare rich media in un eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Potete impostare e gestire il testo della mappa immagine mediante le impostazioni del pannello Informazioni nella schermata eCatalog. 

Consulta [Gestire il contenuto del pannello informazioni nei cataloghi elettronici](/help/using/info-panel-content-ecatalog.md).

## 4. Configurare i predefiniti per il visualizzatore eCatalog

Gli utenti finali possono vedere l’eCatalog nel visualizzatore per eCatalog. Se siete un amministratore, potete configurare il visualizzatore per eCatalog e personalizzarlo modificandone il colore di contorno e selezionando una nuova interfaccia. Adobe Dynamic Media Classic viene fornito con diversi predefiniti visualizzatore eCatalog basati sulle best practice. Potete scegliere uno di questi predefiniti per la visualizzazione dell’eCatalog. Se siete un amministratore, potete inoltre creare un predefinito personalizzato per visualizzatori di eCatalog.

Per creare un predefinito visualizzatore eCatalog, nella barra di navigazione globale, seleziona **[!UICONTROL Configurazione]** e quindi scegliere **[!UICONTROL Predefiniti visualizzatore]**. Seleziona **[!UICONTROL Aggiungi]**, scegli una piattaforma, quindi seleziona **[!UICONTROL eCatalog]** > **[!UICONTROL Visualizzatore]**.

Consulta [Impostazione dei predefiniti per il visualizzatore eCatalog](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. Anteprima degli eCatalog nel visualizzatore eCatalog

I predefiniti per visualizzatori di eCatalog determinano lo stile e il comportamento di tali visualizzatori.

Per informazioni sulla modalità di visualizzazione dell&#39;eCatalog tramite i predefiniti visualizzatore eCatalog, selezionare l&#39;eCatalog nel pannello Sfoglia, quindi selezionare **[!UICONTROL Anteprima]**. La schermata Anteprima si apre nel visualizzatore predefinito.

Notate l’orientamento, lo schema colori, l’aspetto dei controlli per passare alle diverse pagine e come si presentano le pagine voltate. 

Consulta [Anteprima dei cataloghi elettronici nel visualizzatore eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Pubblicare eCatalog e PDF associati

La pubblicazione dell’eCatalog e dei PDF associati lo inserisce nei server immagini Dynamic Media in modo che possa essere consegnato al sito web e all’applicazione. Come parte del processo di pubblicazione, Adobe Dynamic Media Classic attiva la stringa URL per l’eCatalog. Utilizzare questo URL per chiamare l&#39;eCatalog dai server immagini Dynamic Media al sito Web o all&#39;applicazione.

Dopo aver contrassegnato l’eCatalog e il PDF per la pubblicazione nel pannello Sfoglia, seleziona il pulsante Pubblica sulla barra di navigazione globale per avviare una pubblicazione. Nella schermata Pubblica, seleziona **[!UICONTROL Invia pubblicazione]**.

Consulta [Pubblicare eCatalog e PDF associati](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Collegare un eCatalog a una pagina web

Adobe Dynamic Media Classic attiva la stringa di callout URL necessaria per visualizzare l&#39;eCatalog quando viene pubblicato su Dynamic Media Image Server. Puoi copiare questa stringa URL dalla schermata Anteprima e dal pannello Sfoglia (in Visualizzazione dettagli) selezionando URL nel pannello. Dopo aver copiato la stringa URL, la potete inserire nei vostri siti Web e nelle vostre applicazioni.

Consultate il personale IT per inserire il collegamento all’eCatalog nella posizione appropriata sulla pagina Web. Quando gli utenti selezionano il collegamento, viene visualizzato il visualizzatore eCatalog e gli utenti possono sfogliare l&#39;eCatalog.

Consulta [Collegare un eCatalog a una pagina Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
