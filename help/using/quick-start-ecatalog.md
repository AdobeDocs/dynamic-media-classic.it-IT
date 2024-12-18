---
title: 'Guida introduttiva: eCatalog'
description: Introduzione e Guida rapida agli eCatalog per aiutarti a iniziare rapidamente a utilizzare le tecniche di eCatalog in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 25%

---

# Guida introduttiva: eCatalog{#quick-start-ecatalogs}

Un eCatalog è una versione Web digitale del materiale stampato, ad esempio un catalogo, una brochure, un volantino, un manuale del prodotto o una circolare pubblicitaria. Un eCatalog viene visualizzato in un visualizzatore eCatalog in un sito Web. Questo visualizzatore simula l&#39;esperienza di lettura del materiale stampato.

Consulta anche i seguenti video di formazione:

* [Guida rapida 1: eCatalog](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Guida introduttiva 2: eCatalog](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

A seconda delle impostazioni selezionate per l&#39;eCatalog, il visualizzatore consente di effettuare le seguenti operazioni:

* Cercare nel catalogo una o più parole chiave. I risultati della ricerca vengono visualizzati sotto forma di elenco di miniature in un pannello di ricerca sul lato sinistro del catalogo. Ogni miniatura cliccabile rappresenta una pagina del catalogo in cui è stato trovato il termine di ricerca evidenziato.

* Condividi il catalogo tramite social media; scarica il catalogo per visualizzarlo offline; abilita Preferiti per contrassegnare gli elementi a cui desideri tornare rapidamente o stampare il catalogo.
* Spostarsi nel catalogo utilizzando il sommario o la visualizzazione griglia della pagina; spostarsi avanti o indietro selezionando il bordo centrale di una pagina.
* Ingrandire, ridurre e scorrere per esaminare i vari elementi presenti in una pagina
* Spostare il puntatore su un&#39;area della pagina, denominata Mappa immagine, in modo da visualizzare una finestra popup con informazioni su un elemento.
* Selezionare un&#39;area di pagina per aprire una nuova pagina Web contenente ulteriori informazioni su un elemento.
* Scrivere una nota e allegarla a una pagina eCatalog
* Tocca le icone Mappa immagine se desideri avviare le pagine web o i pannelli di informazioni contestuali correlati.
* Usare gesti quali avvicinare le dita per ingrandire o passare il dito per voltare pagina
* Effettuare ricerche di elementi mediante parole chiave

![L&#39;eCatalog visualizzato agli utenti. A) Pagina di apertura eCatalog. B)eCatalog è passato alla pagina 2.](/help/using/assets/ec_cat_viewer_popup.png)

Per creare un eCatalog, in genere si utilizzano file PDF ad alta risoluzione creati in Adobe Acrobat o in un altro programma di stampa, ma è anche possibile creare un eCatalog da file di immagine.

Durante la creazione di un eCatalog, potete ordinare le pagine o affiancarle come desiderate. Potete anche scegliere se visualizzare pagine singole o affiancare due o più pagine. È possibile creare mappe immagine per le aree della pagina in modo che i visualizzatori possano, ad esempio, selezionare un&#39;area della pagina e aprire una nuova pagina nel sito Web. Potete gestire il testo di rollover visualizzato utilizzando le impostazioni del pannello Info nella schermata eCatalog. Potete inoltre configurare il visualizzatore per eCatalog scegliendo tra 100 diverse opzioni di configurazione. Potete adattare le funzioni e l’aspetto del visualizzatore in base alle esigenze di utenti specifici.

>[!NOTE]
>
>Se sei un utente in modalità Dynamic Media: Scene7 e desideri utilizzare gli eCatalog, modifica il valore `pdfbrochure` in CRXDE Lite. Per farlo, in Adobe Experience Manager, vai a **[!UICONTROL Strumenti]** > **[!UICONTROL Generale]** > **[!UICONTROL CRXDE Lite]**. Nella struttura di navigazione del pannello sinistro, passa a `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Nel riquadro in basso a destra, nella scheda **[!UICONTROL Proprietà]**, selezionare la riga `jobParam`. Impostare il valore per `pdfbrochure` da `false` a `true`. Come in `pdfbrochure=true`
>
>Nell&#39;angolo superiore sinistro della pagina CRXDE Lite, selezionare **[!UICONTROL Salva tutto]**.
>
>Ora puoi creare eCatalog in Adobe Dynamic Media Classic.

Questa sezione è stata progettata per aiutarvi a imparare a usare rapidamente gli eCatalog. Seguite i passaggi da 1 a 7. Dopo ogni passaggio, viene inserito un riferimento incrociato a un titolo di argomento in cui è possibile trovare ulteriori informazioni.

## 1. Caricare i file PDF

I file Adobe PDF sono di solito usati come file sorgente per un eCatalog. Poiché sono destinati alla stampa, i file PDF contengono generalmente immagini CMYK. Adobe Dynamic Media Classic rileva queste immagini e le converte utilizzando un profilo colore CMYK standard. Tuttavia, devi caricare e utilizzare un profilo colore personalizzato.

Sulla barra di navigazione globale, seleziona **[!UICONTROL Carica]** per iniziare a caricare file o immagini PDF per l&#39;eCatalog. Puoi caricare i file dal desktop o tramite FTP; l’FTP è consigliato se carichi molti file o file di dimensioni superiori a 100 MB.

Le Opzioni PDF nella schermata Carica riguardano il caricamento dei file PDF nella risoluzione e nello spazio colore corretti. Si consiglia di usare una risoluzione di 150 pixel per pollice. È possibile selezionare l&#39;opzione **[!UICONTROL Generazione automatica eCatalog]** per creare un eCatalog quando si carica un file PDF.

Consulta [Caricare i file PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Creare un eCatalog

Crea l’eCatalog selezionando i file di PDF o immagine nel pannello Sfoglia. Seleziona **[!UICONTROL Build]**, quindi scegli **[!UICONTROL eCatalog]**.

Nella scheda **[!UICONTROL Ordina pagine]** della pagina eCatalog selezionare un&#39;opzione Layout: **[!UICONTROL 1 Su]**, **[!UICONTROL 2 Su]** o **[!UICONTROL Personalizzato]**. Potete riordinare le pagine o pagine affiancate trascinandole oppure, negli eCatalog di grandi dimensioni, scegliendo un nome di pagina nel menu Sposta a.

Per aggiungere delle pagine, selezionate una cartella nella Libreria risorse, quindi trascinate i file PDF o i file di immagini nella schermata Ordina pagine. Invece dei numeri di pagina predefiniti, puoi fornire nomi di pagina personalizzati o importare più nomi di pagina.

Seleziona **[!UICONTROL Salva]**, immetti un nome per l&#39;eCatalog, scegli una cartella Adobe Dynamic Media Classic per memorizzarlo e seleziona **[!UICONTROL Salva]**. Ogni volta che modifichi l&#39;ordine delle pagine o l&#39;eCatalog, salva le modifiche selezionando **[!UICONTROL Salva]**.

Vedere [Creare un eCatalog](creating-ecatalog.md).

## 3. Creare mappe immagine

Le mappe immagine aggiungono un altro aspetto alle pagine eCatalog. Una mappa immagine è l’area di una pagina che fornisce ulteriori informazioni su un elemento. Quando un utenti passa il puntatore su una mappa immagine, viene visualizzata una descrizione dell’elemento. Facendo clic su una mappa immagine viene attivato un riferimento esterno che apre una nuova pagina Web in cui è possibile ottenere ulteriori informazioni su un elemento.

Per creare una mappa immagine, aprite la schermata eCatalog. Quindi vai alla scheda **[!UICONTROL Pagine mappa]** della schermata eCatalog e inquadra la mappa con lo strumento mappa immagine rettangolare o mappa immagine poligonale. È possibile regolare la posizione e le dimensioni delle mappe immagine trascinando i bordi delle mappe con lo strumento Panning.

Dopo aver inquadrato la mappa immagine, immettere l&#39;indirizzo URL a cui si desidera passare quando si seleziona la mappa immagine. Potete anche inserire il testo di rollover visualizzato quando si passa il puntatore sulla mappa immagine. 

Consulta [Creare mappe immagine eCatalog](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Vedi [Utilizzare mappe immagine per incorporare rich media in un eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Potete impostare e gestire il testo della mappa immagine utilizzando le impostazioni del pannello Info nella schermata eCatalog.

Consulta [Gestire il contenuto del pannello informazioni negli eCatalog](/help/using/info-panel-content-ecatalog.md).

## 4. Configurare i predefiniti per il visualizzatore eCatalog

Gli utenti finali possono vedere l’eCatalog nel visualizzatore per eCatalog. Se siete un amministratore, potete configurare il visualizzatore per eCatalog Puoi modificarne il colore di struttura e selezionare una nuova &quot;interfaccia&quot; per applicare il marchio al tuo eCatalog. Adobe Dynamic Media Classic viene fornito con diversi predefiniti visualizzatore eCatalog basati sulle best practice. Potete scegliere uno di questi predefiniti per la visualizzazione dell’eCatalog. Se siete un amministratore, potete inoltre creare un predefinito personalizzato per visualizzatori di eCatalog.

Per creare un predefinito visualizzatore eCatalog, sulla barra di spostamento globale selezionare **[!UICONTROL Configurazione]**, quindi scegliere **[!UICONTROL Predefiniti visualizzatore]**. Selezionare **[!UICONTROL Aggiungi]**, scegliere una piattaforma, quindi selezionare **[!UICONTROL eCatalog]** > **[!UICONTROL Visualizzatore]**.

Vedere [Configurare i predefiniti visualizzatore eCatalog](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. Anteprima degli eCatalog nel visualizzatore eCatalog

I predefiniti per visualizzatori di eCatalog determinano lo stile e il comportamento di tali visualizzatori.

Per informazioni sulla visualizzazione dell&#39;eCatalog tramite i predefiniti visualizzatore eCatalog, selezionare l&#39;eCatalog nel pannello Sfoglia, quindi selezionare **[!UICONTROL Anteprima]**. La schermata Anteprima si apre nel visualizzatore predefinito.

Notate l’orientamento, lo schema colori, l’aspetto dei controlli per passare alle diverse pagine e come si presentano le pagine voltate. 

Vedi [Anteprima eCatalog nel visualizzatore eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Publish eCatalog e PDF associati

La pubblicazione dell&#39;eCatalog e dei PDF associati lo colloca nei server immagini Dynamic Media in modo che possa essere consegnato al sito Web e all&#39;applicazione. Come parte del processo di pubblicazione, Adobe Dynamic Media Classic attiva la stringa URL per l’eCatalog. Utilizzare questo URL per chiamare l&#39;eCatalog dai server immagini Dynamic Media al sito Web o all&#39;applicazione.

Dopo aver contrassegnato l’eCatalog e il PDF per la pubblicazione nel pannello Sfoglia, seleziona il pulsante Publish nella barra di navigazione globale per avviare una pubblicazione. Nella pagina Pubblicazione, seleziona **[!UICONTROL Invia Publish]**.

Vedi [eCatalog Publish e PDF associati](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Collegare un eCatalog a una pagina Web

Adobe Dynamic Media Classic attiva la stringa di callout URL necessaria per visualizzare l&#39;eCatalog quando viene pubblicato su Dynamic Media Image Server. Puoi copiare questa stringa di URL dalla schermata Anteprima e dal pannello Sfoglia (in Vista dettagli) selezionando URL nel pannello. Dopo aver copiato la stringa URL, questa sarà disponibile per i siti Web e le applicazioni.

Collabora con il tuo team IT per inserire il collegamento all’eCatalog nella posizione appropriata all’interno della pagina Web. Quando gli utenti selezionano il collegamento, viene visualizzato il visualizzatore eCatalog e gli utenti possono sfogliare l&#39;eCatalog.

Vedi [Collegare un eCatalog a una pagina Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
