---
title: "Quick Inizia: eCatalog"
description: Un'introduzione e una rapida Inizia per gli eCatalog per aiutarti a velocizzare e correre rapidamente con le tecniche del Adobe Systems Dynamic Media.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 36%

---

# Inizia rapida: eCatalog{#quick-start-ecatalogs}

Un eCatalog è la versione digitale per il Web di un materiale originariamente destinato alla stampa, come ad esempio un catalogo, una brochure, un volantino, un manuale di un prodotto o un annuncio pubblicitario. Un eCatalog può essere visualizzato in un sito Web mediante un visualizzatore per eCatalog. Tale visualizzatore simula l’esperienza della lettura di una copia stampata.

Vedi anche i seguenti video training:

* [Avvio rapido 1: eCatalog](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Avvio rapido 2: eCatalog](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

A seconda delle impostazioni selezionate per l&#39;eCatalog, il visualizzatore può consentire di effettuare le seguenti operazioni:

* Search il catalogo per una parola chiave o parole chiave. I risultati ricerca vengono visualizzati come un elenco di miniature in un pannello ricerca sul lato sinistro del catalogo. Ogni cliccabile miniatura rappresenta uno spread del catalogo in cui è stato trovato il ricerca termine evidenziato.

* Condividere il catalogo tramite social media; scaricare il catalogo per la visualizzazione offline; Abilita i preferiti per contrassegnare rapidamente gli elementi a cui desideri tornare o stamparlo.
* Individuate il catalogo utilizzando il sommario o la visualizzazione griglia della pagina; avanti o indietro la pagina facendo clic sul bordo centrale di una pagina.
* Ingrandire, ridurre e scorrere per esaminare i vari elementi presenti in una pagina
* Sposta il puntatore su una pagina area geografica (denominata Immagine mappa) in modo da visualizzare una finestra di finestra a comparsa con informazioni su un elemento.
* Seleziona una pagina area geografica quindi apre una nuova pagina Web con ulteriori informazioni su un elemento.
* Scrivere una nota e allegarla a una pagina eCatalog
* Toccate le icone delle mappe immagine per lanciare pagine Web correlate o pannelli di informazioni contestuali.
* Usare gesti quali avvicinare le dita per ingrandire o passare il dito per voltare pagina
* Effettuare ricerche di elementi mediante parole chiave

![L&#39;eCatalog come appare agli utenti. A) pagina di apertura di eCatalog. B) eCatalog si è rivolto a pagina 2.](/help/assets/ec_cat_viewer_popup.png)

Per creare un eCatalog, in genere si utilizzano file PDF ad alta risoluzione creati in Adobe Systems Acrobat o in un altro programma di stampa, ma è anche possibile creare un eCatalog da file di immagine.

Durante la creazione di un eCatalog, potete ordinare le pagine o affiancarle come desiderate. Potete anche scegliere se visualizzare pagine singole o affiancare due o più pagine. Potete creare Immagine mappe per le aree della pagina in modo che i visualizzatori possano, ad esempio, selezionare un&#39;area della pagina e aprire una nuova pagina sul sito Web. Potete gestire il testo di rollover visualizzato utilizzando le impostazioni del pannello Info nella schermata eCatalog. Potete inoltre configurare il visualizzatore per eCatalog scegliendo tra 100 diverse opzioni di configurazione. Potete adattare le funzioni e l’aspetto del visualizzatore in base alle esigenze di utenti specifici.

>[!NOTE]
>
>Se sei una modalità Dynamic Media Scene7 utente e desideri utilizzare gli eCatalog, modifica il `pdfbrochure` valore in CRXDE Lite. Per farlo, in Adobe Experience Manager, vai a **[!UICONTROL strumenti]** > **[!UICONTROL Generale]** > **[!UICONTROL CRXDE Lite]** . Nel pannello a sinistra navigazione albero, passate a `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf` .
>
>Nel riquadro in basso a destra, nella **[!UICONTROL Proprietà]** scheda, selezionare la `jobParam` riga. Impostate il valore `pdfbrochure` da `false` a a `true` . Come in `pdfbrochure=true`
>
>Nell&#39;angolo in alto a sinistra della pagina CRXDE Lite, seleziona **[!UICONTROL Salva tutto]** .
>
>Ora puoi creare eCatalog in Adobe Systems Dynamic Media Classic.

Questa sezione è stata progettata per aiutarvi a imparare a usare rapidamente gli eCatalog. Seguite i passaggi da 1 a 7. Dopo ogni passaggio, esiste un riferimento incrociato all&#39;intestazione di un argomento in cui è possibile trovare ulteriori informazioni.

## 1. carica i file PDF

I file Adobe PDF sono di solito usati come file sorgente per un eCatalog. Poiché sono destinati alla stampa, i file PDF contengono generalmente immagini CMYK. Adobe Systems Dynamic Media Classic rileva queste immagini e le converte utilizzando un profilo colore standard CMYK. Tuttavia, è necessario caricare e utilizzare un profilo colore personalizzato.

Nella barra di navigazione globale, selezionate **[!UICONTROL carica]** per avviare il caricamento di file PDF o immagini per il vostro eCatalog. Potete caricare i file dal desktop o via FTP; l’FTP è il metodo consigliato nel caso di molti file o file più grandi di 100 MB.

Le Opzioni PDF nella schermata Carica riguardano il caricamento dei file PDF nella risoluzione e nello spazio colore corretti. Si consiglia di usare una risoluzione di 150 pixel per pollice. Con l’opzione Genera automaticamente eCatalog potete creare un eCatalog durante il caricamento di un file PDF. 

Consultate [ caricare i file ](uploading-pdf-files.md#uploading_the_pdf_files) PDF.

## 2. Crea un eCatalog

Crea il tuo eCatalog selezionando file PDF o immagine nel pannello Sfoglia. Seleziona **[!UICONTROL genera]** , quindi scegli **[!UICONTROL eCatalog]** .

Nella pagina eCatalog, **[!UICONTROL nelle pagine]** ordine scheda, selezionare un&#39;opzione layout: **[!UICONTROL 1]** su, **[!UICONTROL 2]** in su o **[!UICONTROL personalizzato]** . Potete riordinare le pagine o pagine affiancate trascinandole oppure, negli eCatalog di grandi dimensioni, scegliendo un nome di pagina nel menu Sposta a.

Per aggiungere delle pagine, selezionate una cartella nella Libreria risorse, quindi trascinate i file PDF o i file di immagini nella schermata Ordina pagine. Invece dei numeri di pagina predefiniti, potete fornire nomi di pagina personalizzati o importare molti nomi di pagina.

Selezionate **[!UICONTROL Salva]** , immettete un nome per l&#39;eCatalog, scegliete un Adobe Systems Dynamic Media cartella classica da archiviare e selezionate **[!UICONTROL Salva]** . Ogni volta che modifichi l&#39;ordine di pagina o modifichi l&#39;eCatalog, Salva le modifiche facendo clic su **[!UICONTROL Salva]** .

Consultate [ Crea un eCatalog ](creating-ecatalog.md) .

## 3. Crea Immagine mappe

Immagine mappe aggiungono un altro aspetto alle pagine di eCatalog. Una mappa immagine è l’area di una pagina che fornisce ulteriori informazioni su un elemento. Quando un utenti passa il puntatore su una mappa immagine, viene visualizzata una descrizione dell’elemento. Facendo clic su una mappa immagine si attiva un riferimento esterno per l’apertura di una nuova pagina Web con ulteriori informazioni sull’elemento corrispondente.

Per creare una mappa immagine, aprite la schermata eCatalog. Quindi passa alle pagine ]**della mappa scheda della schermata eCatalog e inquadrare**[!UICONTROL  la mappa con il rettangolo Immagine mappa strumento o poligono Immagine mappa strumento. Potete regolare la posizione e la dimensione delle mappe immagine trascinando i bordi delle mappe con lo strumento scorrimento .

Dopo aver incorniciato la mappa Immagine, immettete l&#39;indirizzo URL a cui desiderate passare quando selezionate la mappa Immagine. Potete anche inserire il testo di rollover visualizzato quando si passa il puntatore sulla mappa immagine. 

Consulta [ Crea immagine mappe ](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps) di eCatalog.

Consultate [ utilizzare immagine mappe per incorporare Rich Media in un eCatalog ](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog) .

Potete impostare e gestire il testo della mappa immagine mediante le impostazioni del pannello Informazioni nella schermata eCatalog. 

Consultate [ gestione contenuto pannello informazioni in eCatalog ](/help/info-panel-content-ecatalog.md) .

## 4. Configura il Visualizzatore di eCatalog Predefiniti

Gli utenti finali possono vedere l’eCatalog nel visualizzatore per eCatalog. Se siete un amministratore, potete configurare il visualizzatore per eCatalog e personalizzarlo modificandone il colore di contorno e selezionando una nuova interfaccia. Adobe Systems Dynamic Media Classic include diversi Predefiniti visualizzatore eCatalog &quot;Best Practice&quot;. Potete scegliere uno di questi predefiniti per la visualizzazione dell’eCatalog. Se siete un amministratore, potete inoltre creare un predefinito personalizzato per visualizzatori di eCatalog.

Per creare un predefinito per visualizzatori di eCatalog, nella barra di navigazione globale, selezionate **[!UICONTROL configurazione]** , quindi scegliete **[!UICONTROL Visualizzatore predefiniti]** . Seleziona **[!UICONTROL Aggiungi]** , scegli una piattaforma, quindi seleziona **[!UICONTROL eCatalog]** > **[!UICONTROL Visualizzatore]** .

Consultate [ configurare predefiniti ](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets) Visualizzatore eCatalog.

## 5. Anteprima eCatalogs nel Visualizzatore eCatalog

I predefiniti per visualizzatori di eCatalog determinano lo stile e il comportamento di tali visualizzatori.

Per scoprire come Predefiniti Visualizza il tuo eCatalog per visualizzatori eCatalog, seleziona il tuo eCatalog nel pannello Sfoglia, quindi seleziona **[!UICONTROL Anteprima]** . La schermata Anteprima si apre nel visualizzatore predefinito.

Notate l’orientamento, lo schema colori, l’aspetto dei controlli per passare alle diverse pagine e come si presentano le pagine voltate. 

Consultate [ Anteprima eCatalog nel visualizzatore ](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer) di Ecatalogo.

## 6. Publish eCatalog e PDF associati

Pubblicazione il tuo eCatalog e il PDF associato lo posiziona sui Dynamic Media Immagine server in modo che possa essere consegnato al tuo sito Web e applicazione. Come parte del processo di pubblicazione, Adobe Systems Dynamic Media Classic attiva la stringa di URL per il tuo eCatalog. Utilizza questo URL per richiamare l&#39;eCatalog da Dynamic Media Immagine server al sito Web o applicazione.

Dopo aver selezionato l&#39;eCatalog e il PDF per pubblicare nel pannello Sfoglia, selezionate il pulsante Publish nella barra di navigazione globale per avviare un pubblicare. Nella schermata Publish, seleziona **[!UICONTROL invia Publish]** .

Consultate [ Publish eCatalog e PDF ](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs) associati.

## 7. collega un eCatalog a una pagina Web

Adobe Systems Dynamic Media Classic attiva la stringa di callout URL necessaria per visualizzare l&#39;eCatalog quando viene pubblicare per Dynamic Media immagine server. Potete copiare questa URL stringa dalla schermata Anteprima e dal pannello Sfoglia (in dettaglio Visualizza) selezionando gli URL nel pannello. Dopo aver copiato la stringa URL, la potete inserire nei vostri siti Web e nelle vostre applicazioni.

Consultate il personale IT per inserire il collegamento all’eCatalog nella posizione appropriata sulla pagina Web. Quando gli utenti selezionano il collegare, viene visualizzato il Visualizzatore eCatalog e gli utenti possono sfogliare il tuo eCatalog.

Consultate [ collegare un eCatalog a una pagina ](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page) Web.
