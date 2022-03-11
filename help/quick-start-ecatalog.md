---
title: '"Avvio rapido: eCatalogs"'
description: Introduzione e avvio rapido agli eCatalog per aiutarti a iniziare rapidamente a usare le tecniche di eCatalog in Adobe Dynamic Media Classic.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: ec1a981dd5cfa92ce4ae8e2676dd131d1509216f
workflow-type: tm+mt
source-wordcount: '1558'
ht-degree: 37%

---

# Avvio rapido: eCatalogs{#quick-start-ecatalogs}

Un eCatalog è la versione digitale per il Web di un materiale originariamente destinato alla stampa, come ad esempio un catalogo, una brochure, un volantino, un manuale di un prodotto o un annuncio pubblicitario. Un eCatalog può essere visualizzato in un sito Web mediante un visualizzatore per eCatalog. Tale visualizzatore simula l’esperienza della lettura di una copia stampata.

Vedi anche i seguenti video di formazione:

* [Avvio rapido 1: eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Avvio rapido 2: eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

A seconda delle impostazioni selezionate per l’eCatalog, il visualizzatore può effettuare le seguenti operazioni:

* Cerca una parola chiave o parole chiave nel catalogo. I risultati della ricerca vengono visualizzati come un elenco di miniature in un pannello di ricerca sul lato sinistro del catalogo. Ogni miniatura cliccabile rappresenta un catalogo diffuso in cui è stato trovato il termine di ricerca evidenziato.

* condividere il catalogo tramite i social media; scaricare il catalogo per visualizzare offline; abilitare Preferiti per contrassegnare rapidamente gli elementi che si desidera restituire o stampare il catalogo.
* Spostarsi nel catalogo utilizzando il sommario o la vista griglia della pagina; in avanti o indietro facendo clic sul bordo centrale di una pagina.
* Ingrandire, ridurre e scorrere per esaminare i vari elementi presenti in una pagina
* Spostare il puntatore su un&#39;area della pagina (o mappa immagine) in modo da visualizzare una finestra a comparsa con informazioni su un elemento.
* Seleziona un’area della pagina in modo da aprire una nuova pagina web con ulteriori informazioni su un elemento.
* Scrivere una nota e allegarla a una pagina eCatalog
* Tocca le icone della mappa immagine se desideri avviare pagine web correlate o pannelli di informazioni contestuali.
* Usare gesti quali avvicinare le dita per ingrandire o passare il dito per voltare pagina
* Effettuare ricerche di elementi mediante parole chiave

![L’eCatalog come viene visualizzato agli utenti. A) Pagina di apertura eCatalog. B)eCatalog girato a pagina 2.](/help/assets/ec_cat_viewer_popup.png)

Per creare un eCatalog, in genere si utilizzano file PDF ad alta risoluzione creati in Adobe Acrobat o in un altro programma di stampa, ma è anche possibile creare un eCatalog da file di immagine.

Durante la creazione di un eCatalog, potete ordinare le pagine o affiancarle come desiderate. Potete anche scegliere se visualizzare pagine singole o affiancare due o più pagine. È possibile creare mappe immagine per le aree della pagina in modo che gli utenti possano, ad esempio, selezionare un’area nella pagina e aprire una nuova pagina sul sito web. Potete gestire il testo di rollover visualizzato utilizzando le impostazioni del pannello Info nella schermata eCatalog. Potete inoltre configurare il visualizzatore per eCatalog scegliendo tra 100 diverse opzioni di configurazione. Potete adattare le funzioni e l’aspetto del visualizzatore in base alle esigenze di utenti specifici.

>[!NOTE]
>
>Se sei un utente in modalità Dynamic Media - Scene7 e desideri utilizzare gli eCatalogs, modifica la `pdfbrochure` in CRXDE Lite. Per farlo, in Adobe Experience Manager, vai a **[!UICONTROL Strumenti]** > **[!UICONTROL Generale]** > **[!UICONTROL CRXDE Lite]**. Nella struttura di navigazione del pannello a sinistra, seleziona `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Nel riquadro in basso a destra, nella **[!UICONTROL Proprietà]** seleziona la scheda `jobParam` fila. Imposta il valore per `pdfbrochure` da `false` a `true`. Come in `pdfbrochure=true`
>
>Nell’angolo in alto a sinistra della pagina CRXDE Lite, seleziona **[!UICONTROL Salva tutto]**.
>
>Ora puoi creare eCatalogs in Adobe Dynamic Media Classic.

Questa sezione è stata progettata per aiutarvi a imparare a usare rapidamente gli eCatalog. Seguite i passaggi da 1 a 7. Alla fine di ciascun passaggio è riportato un riferimento a un argomento correlato con ulteriori informazioni.

## 1. Carica i file PDF

I file Adobe PDF sono di solito usati come file sorgente per un eCatalog. Poiché sono destinati alla stampa, i file PDF contengono generalmente immagini CMYK. Adobe Dynamic Media Classic rileva queste immagini e le converte utilizzando un profilo colore CMYK standard. Tuttavia, devi caricare e utilizzare un profilo colore personalizzato.

Nella barra di navigazione globale, seleziona **[!UICONTROL Carica]** per iniziare a caricare file o immagini di PDF per il tuo eCatalog. Potete caricare i file dal desktop o via FTP; l’FTP è il metodo consigliato nel caso di molti file o file più grandi di 100 MB.

Le Opzioni PDF nella schermata Carica riguardano il caricamento dei file PDF nella risoluzione e nello spazio colore corretti. Si consiglia di usare una risoluzione di 150 pixel per pollice. Con l’opzione Genera automaticamente eCatalog potete creare un eCatalog durante il caricamento di un file PDF. 

Vedi [Caricare i file PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Creare un eCatalog

Crea l’eCatalog selezionando i file di PDF o immagini nel pannello Sfoglia. Seleziona **[!UICONTROL Crea]**, quindi scegli **[!UICONTROL eCatalogs]**.

Nella pagina eCatalog, nella pagina **[!UICONTROL Pagine ordine]** seleziona un’opzione Layout : **[!UICONTROL 1]**, **[!UICONTROL 2]** oppure **[!UICONTROL Personalizzato]**. Potete riordinare le pagine o pagine affiancate trascinandole oppure, negli eCatalog di grandi dimensioni, scegliendo un nome di pagina nel menu Sposta a.

Per aggiungere delle pagine, selezionate una cartella nella Libreria risorse, quindi trascinate i file PDF o i file di immagini nella schermata Ordina pagine. Invece dei numeri di pagina predefiniti, è possibile fornire nomi di pagina personalizzati o importare molti nomi di pagina.

Seleziona **[!UICONTROL Salva]**, immetti un nome per il tuo eCatalog, scegli una cartella Adobe Dynamic Media Classic per memorizzarlo e seleziona **[!UICONTROL Salva]**. Ogni volta che modifichi l’ordine delle pagine o modifichi l’eCatalog, salva le modifiche facendo clic su **[!UICONTROL Salva]**.

Vedi [Creare un eCatalog](creating-ecatalog.md).

## 3. Creare mappe immagine

Le mappe immagine aggiungono un altro aspetto alle pagine di eCatalog. Una mappa immagine è l’area di una pagina che fornisce ulteriori informazioni su un elemento. Quando un utenti passa il puntatore su una mappa immagine, viene visualizzata una descrizione dell’elemento. Facendo clic su una mappa immagine si attiva un riferimento esterno per l’apertura di una nuova pagina Web con ulteriori informazioni sull’elemento corrispondente.

Per creare una mappa immagine, aprite la schermata eCatalog. Quindi vai al **[!UICONTROL Mappa pagine]** scheda della schermata eCatalog e cornice la mappa con lo strumento Mappa immagine rettangolo o Mappa immagine poligonale. Potete regolare la posizione e la dimensione delle mappe immagine trascinando i bordi delle mappe con lo strumento scorrimento .

Dopo aver incorniciato la mappa immagine, immetti l’indirizzo URL a cui desideri indirizzarti quando selezioni la mappa immagine. Potete anche inserire il testo di rollover visualizzato quando si passa il puntatore sulla mappa immagine. 

Vedi [Creare mappe immagine di eCatalog](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Vedi [Utilizzare le mappe immagine per incorporare contenuti multimediali complessi in un eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Potete impostare e gestire il testo della mappa immagine mediante le impostazioni del pannello Informazioni nella schermata eCatalog. 

Vedi [Gestire il contenuto del pannello informazioni negli eCatalog](/help/info-panel-content-ecatalog.md).

## 4. Configurazione dei predefiniti per visualizzatori di eCatalog

Gli utenti finali possono vedere l’eCatalog nel visualizzatore per eCatalog. Se siete un amministratore, potete configurare il visualizzatore per eCatalog e personalizzarlo modificandone il colore di contorno e selezionando una nuova interfaccia. Adobe Dynamic Media Classic viene fornito con diversi predefiniti per visualizzatori di eCatalog &quot;best practice&quot;. Potete scegliere uno di questi predefiniti per la visualizzazione dell’eCatalog. Se siete un amministratore, potete inoltre creare un predefinito personalizzato per visualizzatori di eCatalog.

Per creare un predefinito per visualizzatori di eCatalog, nella barra di navigazione globale, seleziona **[!UICONTROL Configurazione]**, quindi scegli **[!UICONTROL Predefiniti visualizzatore]**. Seleziona **[!UICONTROL Aggiungi]**, scegli una piattaforma e seleziona **[!UICONTROL eCatalog]** > **[!UICONTROL Visualizzatore]**.

Vedi [Configurare i predefiniti per visualizzatori di eCatalog](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. Anteprima di eCatalog nel visualizzatore di eCatalog

I predefiniti per visualizzatori di eCatalog determinano lo stile e il comportamento di tali visualizzatori.

Per scoprire come i predefiniti per visualizzatori di eCatalog visualizzano l’eCatalog, selezionate l’eCatalog nel pannello Sfoglia, quindi selezionate **[!UICONTROL Anteprima]**. La schermata Anteprima si apre nel visualizzatore predefinito.

Notate l’orientamento, lo schema colori, l’aspetto dei controlli per passare alle diverse pagine e come si presentano le pagine voltate. 

Vedi [Anteprima di eCatalog nel visualizzatore di eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Pubblicare eCatalog e PDF associati

Quando si pubblica l’eCatalog e i relativi PDF, questo viene inserito sui server di immagini Dynamic Media in modo che possa essere distribuito al sito Web e all’applicazione. Come parte del processo di pubblicazione, Adobe Dynamic Media Classic attiva la stringa URL per l’eCatalog. Utilizza questo URL per chiamare l&#39;eCatalog dai server di immagini Dynamic Media al tuo sito web o applicazione.

Dopo aver contrassegnato l’eCatalog e PDF per la pubblicazione nel pannello Sfoglia, seleziona il pulsante Pubblica nella barra di navigazione globale per avviare una pubblicazione. Nella schermata Pubblica , seleziona **[!UICONTROL Invia pubblicazione]**.

Vedi [Pubblicare eCatalog e PDF associati](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Collegare un eCatalog a una pagina web

Adobe Dynamic Media Classic attiva la stringa di callout degli URL necessaria per visualizzare l’eCatalog quando lo si pubblica sui server di immagini Dynamic Media. Puoi copiare questa stringa URL dalla schermata Anteprima e dal pannello Sfoglia (in Vista dettaglio) selezionando URL nel pannello. Dopo aver copiato la stringa URL, la potete inserire nei vostri siti Web e nelle vostre applicazioni.

Consultate il personale IT per inserire il collegamento all’eCatalog nella posizione appropriata sulla pagina Web. Quando gli utenti selezionano il collegamento, viene visualizzato il visualizzatore di eCatalog e gli utenti possono navigare nell’eCatalog.

Vedi [Collegamento di un eCatalog a una pagina web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
