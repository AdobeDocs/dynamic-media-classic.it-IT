---
title: '"Avvio rapido: eCatalogs"'
description: Introduzione e avvio rapido agli eCatalog per aiutarti a iniziare rapidamente a usare le tecniche di eCatalog.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Visualizzatori,eCatalog
role: Business Practitioner
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 51%

---

# Avvio rapido: eCatalogs{#quick-start-ecatalogs}

Un eCatalog è la versione digitale per il Web di un materiale originariamente destinato alla stampa, come ad esempio un catalogo, una brochure, un volantino, un manuale di un prodotto o un annuncio pubblicitario. Un eCatalog può essere visualizzato in un sito Web mediante un visualizzatore per eCatalog. Tale visualizzatore simula l’esperienza della lettura di una copia stampata. A seconda delle impostazioni selezionate per l’eCatalog, il visualizzatore può effettuare le seguenti operazioni:

* Cerca una parola chiave o parole chiave nel catalogo. I risultati della ricerca vengono visualizzati come un elenco di miniature in un pannello di ricerca sul lato sinistro del catalogo. Ogni miniatura cliccabile rappresenta un catalogo diffuso in cui è stato trovato il termine di ricerca evidenziato.

* condividere il catalogo tramite i social media; scaricare il catalogo per visualizzare offline; abilitare Preferiti per contrassegnare rapidamente gli elementi che si desidera restituire o stampare il catalogo.
* Spostarsi nel catalogo utilizzando il sommario o la vista griglia della pagina; in avanti o indietro facendo clic sul bordo centrale di una pagina.
* Ingrandire, ridurre e scorrere per esaminare i vari elementi presenti in una pagina
* Spostare il puntatore su un&#39;area della pagina (o mappa immagine) in modo da visualizzare una finestra a comparsa con informazioni su un elemento.
* Fare clic su un&#39;area della pagina per aprire una nuova pagina Web con ulteriori informazioni su un elemento.
* Scrivere una nota e allegarla a una pagina eCatalog
* Tocca le icone della mappa immagine se desideri avviare pagine web correlate o pannelli di informazioni contestuali.
* Usare gesti quali avvicinare le dita per ingrandire o passare il dito per voltare pagina
* Effettuare ricerche di elementi mediante parole chiave

![L’eCatalog come viene visualizzato agli utenti. A) Pagina di apertura eCatalog. B)eCatalog girato a pagina 2.](/help/assets/ec_cat_viewer_popup.png)

Per creare un eCatalog, di solito vengono utilizzati file PDF ad alta risoluzione creati con Adobe® Acrobat® o con un altro programma per la stampa. Tuttavia potete anche creare un eCatalog da file di immagini.

Durante la creazione di un eCatalog, potete ordinare le pagine o affiancarle come desiderate. Potete anche scegliere se visualizzare pagine singole o affiancare due o più pagine. Potete creare delle mappe immagine per specifiche aree di una pagina in modo che gli utenti possano, ad esempio, fare clic su un’area della pagina per aprire una nuova pagina nel sito Web. Potete gestire il testo di rollover visualizzato utilizzando le impostazioni del pannello Info nella schermata eCatalog. Potete inoltre configurare il visualizzatore per eCatalog scegliendo tra 100 diverse opzioni di configurazione. Potete adattare le funzioni e l’aspetto del visualizzatore in base alle esigenze di utenti specifici.

>[!NOTE]
>
>Se sei un utente in modalità Dynamic Media - Scene7 e desideri utilizzare gli eCatalogs, devi modificare il valore `pdfbrochure` in CRXDE Lite. Per farlo, in Adobe Experience Manager fai clic su **[!UICONTROL Strumenti]** > **[!UICONTROL Generale]** > **[!UICONTROL CRXDE Lite]**. Nella struttura di navigazione del pannello a sinistra, passa a `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Nel riquadro in basso a destra, nella scheda **[!UICONTROL Proprietà]** selezionare la riga `jobParam`. Imposta il valore per `pdfbrochure` da `false` a `true`. Come in `pdfbrochure=true`
>
>Nell&#39;angolo in alto a sinistra della pagina CRXDE Lite, fai clic su **[!UICONTROL Salva tutto]**.
>
>Ora puoi creare eCatalogs in Dynamic Media Classic.

Questa sezione è stata progettata per aiutarvi a imparare a usare rapidamente gli eCatalog. Seguite i passaggi da 1 a 7. Alla fine di ciascun passaggio è riportato un riferimento a un argomento correlato con ulteriori informazioni.

## 1. Caricamento dei file PDF

I file Adobe PDF sono di solito usati come file sorgente per un eCatalog. Poiché sono destinati alla stampa, i file PDF contengono generalmente immagini CMYK. Dynamic Media Classic rileva queste immagini e le converte utilizzando un profilo colore CMYK standard. Tuttavia, devi caricare e utilizzare un profilo colore personalizzato.

Nella barra di navigazione globale, fai clic su **[!UICONTROL Carica]** per iniziare a caricare file PDF o immagini per il tuo eCatalog. Potete caricare i file dal desktop o via FTP; l’FTP è il metodo consigliato nel caso di molti file o file più grandi di 100 MB.

Le Opzioni PDF nella schermata Carica riguardano il caricamento dei file PDF nella risoluzione e nello spazio colore corretti. Si consiglia di usare una risoluzione di 150 pixel per pollice. Con l’opzione Genera automaticamente eCatalog potete creare un eCatalog durante il caricamento di un file PDF. 

Consultate [Caricamento di file PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Creazione di un eCatalog

Crea l’eCatalog selezionando i file PDF o di immagine nel pannello Sfoglia. Fai clic su **[!UICONTROL Build]**, quindi scegli **[!UICONTROL eCatalogs]**.

Nella pagina eCatalog, nella scheda **[!UICONTROL Ordina pagine]** , seleziona un’opzione Layout: **[!UICONTROL 1 Su]**, **[!UICONTROL 2 Su]** o **[!UICONTROL Personalizzato]**. Potete riordinare le pagine o pagine affiancate trascinandole oppure, negli eCatalog di grandi dimensioni, scegliendo un nome di pagina nel menu Sposta a.

Per aggiungere delle pagine, selezionate una cartella nella Libreria risorse, quindi trascinate i file PDF o i file di immagini nella schermata Ordina pagine. Invece dei numeri di pagina predefiniti, è possibile fornire nomi di pagina personalizzati o importare molti nomi di pagina.

Fai clic su **[!UICONTROL Salva]**, immetti un nome per il tuo eCatalog, scegli una cartella Dynamic Media Classic per memorizzarlo e fai clic su **[!UICONTROL Salva]**. Ogni volta che modifichi l’ordine delle pagine o modifichi l’eCatalog, salva le modifiche facendo clic su **[!UICONTROL Salva]**.

Consultate [Creazione di un eCatalog](creating-ecatalog.md).

## 3. Creazione di mappe immagine

Le mappe immagine aggiungono un altro aspetto alle pagine di eCatalog. Una mappa immagine è l’area di una pagina che fornisce ulteriori informazioni su un elemento. Quando un utenti passa il puntatore su una mappa immagine, viene visualizzata una descrizione dell’elemento. Facendo clic su una mappa immagine si attiva un riferimento esterno per l’apertura di una nuova pagina Web con ulteriori informazioni sull’elemento corrispondente.

Per creare una mappa immagine, aprite la schermata eCatalog. Quindi vai alla scheda **[!UICONTROL Mappa pagine]** della schermata eCatalog e incorniciala con lo strumento Mappa immagine rettangolo o Mappa immagine poligonale. Potete regolare la posizione e la dimensione delle mappe immagine trascinando i bordi delle mappe con lo strumento scorrimento .

Dopo aver incorniciato la mappa immagine, immetti l’indirizzo URL a cui desideri indirizzarti quando fai clic sulla mappa immagine. Potete anche inserire il testo di rollover visualizzato quando si passa il puntatore sulla mappa immagine. 

Consultate [Creazione di mappe immagine per un eCatalog](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Consultate [Incorporamento di contenuti multimediali in un eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Potete impostare e gestire il testo della mappa immagine mediante le impostazioni del pannello Informazioni nella schermata eCatalog. 

Consultate [Gestione del contenuto del pannello Informazioni](info-panel-content.md#managing-info-panel-content).

## 4. Configurazione dei predefiniti per visualizzatori di eCatalog

Gli utenti finali possono vedere l’eCatalog nel visualizzatore per eCatalog. Se siete un amministratore, potete configurare il visualizzatore per eCatalog e personalizzarlo modificandone il colore di contorno e selezionando una nuova interfaccia. Dynamic Media Classic include diversi predefiniti per visualizzatori di eCatalog &quot;best practice&quot;. Potete scegliere uno di questi predefiniti per la visualizzazione dell’eCatalog. Se siete un amministratore, potete inoltre creare un predefinito personalizzato per visualizzatori di eCatalog.

Per creare un predefinito per visualizzatori di eCatalog, nella barra di navigazione globale fate clic su **[!UICONTROL Configurazione]** e scegliete **[!UICONTROL Predefiniti visualizzatore]**. Quindi fai clic su **[!UICONTROL Aggiungi]**, scegli una piattaforma, quindi fai clic su **[!UICONTROL eCatalog > Visualizzatore]**.

Consultate [Impostazione dei predefiniti per il visualizzatore di eCatalog](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. Anteprima degli eCatalog nel visualizzatore di eCatalog

I predefiniti per visualizzatori di eCatalog determinano lo stile e il comportamento di tali visualizzatori.

Per scoprire come i predefiniti per visualizzatori di eCatalog visualizzano l’eCatalog, seleziona l’eCatalog nel pannello di navigazione e fai clic su **[!UICONTROL Anteprima]**. La schermata Anteprima si apre nel visualizzatore predefinito.

Notate l’orientamento, lo schema colori, l’aspetto dei controlli per passare alle diverse pagine e come si presentano le pagine voltate. 

Consultate [Anteprima di eCatalog nel visualizzatore di eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Pubblicazione di eCatalog e PDF associati

Quando si pubblica l’eCatalog e il PDF associato, questo viene inserito sui server di immagini Dynamic Media in modo che possa essere distribuito al sito Web e all’applicazione. Come parte del processo di pubblicazione, Dynamic Media Classic attiva la stringa URL per l’eCatalog. Utilizza questo URL per chiamare l&#39;eCatalog dai server di immagini Dynamic Media al tuo sito web o applicazione.

Dopo aver contrassegnato l’eCatalog e il PDF per la pubblicazione nel pannello Sfoglia, selezionate il pulsante Pubblica nella barra di navigazione globale per avviare una pubblicazione. Nella schermata Pubblica , fai clic su **[!UICONTROL Invia pubblicazione]**.

Consulta [Pubblicazione di eCatalog e PDF associati](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Collegamento di un eCatalog a una pagina web

Dynamic Media Classic attiva la stringa di callout degli URL necessaria per visualizzare l’eCatalog quando lo si pubblica in Dynamic Media Image Server. Potete copiare questa stringa URL dalla schermata Anteprima e dal pannello Sfoglia (in visualizzazione Dettagli) selezionando l’opzione URL nel pannello. Dopo aver copiato la stringa URL, la potete inserire nei vostri siti Web e nelle vostre applicazioni.

Consultate il personale IT per inserire il collegamento all’eCatalog nella posizione appropriata sulla pagina Web. Quando un utente farà clic sul collegamento, verrà aperto il visualizzatore di eCatalog che consente all’utente di sfogliare l’eCatalog. 

Consultate [Collegamento di un eCatalog a una pagina Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
