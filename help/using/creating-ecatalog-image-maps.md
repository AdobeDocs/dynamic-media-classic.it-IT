---
title: Crea mappe immagine eCatalog
description: Scopri come creare mappe immagine eCatalog in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 26%

---

# Crea mappe immagine eCatalog{#creating-ecatalog-image-maps}

Una mappa immagine è un&#39;area di una pagina eCatalog che è possibile spostare con il mouse o selezionare per attivare azioni di vario tipo. Quando si sposta il puntatore su una mappa immagine, ad esempio, viene visualizzata una descrizione di testo di rollover di un elemento. Quando selezioni una mappa immagine, viene avviata un’altra azione. Ad esempio, è possibile aprire una pagina Web in modo che gli utenti possano saperne di più su un elemento o acquistarlo oppure è possibile avviare un video per visualizzare un elemento in uso.

## Disegna mappe immagine eCatalog {#drawing-ecatalog-image-maps}

Per gli eCatalog, potete disegnare le mappe immagine nella scheda Mappe pagine della schermata eCatalog. Questa schermata include l’area Mappa immagine in cui vengono visualizzate le pagine eCatalog e, a destra, l’elenco delle mappe immagine. Quando si creano le mappe immagine, i relativi nomi vengono immessi nell&#39;elenco Mappa immagine.

1. Seleziona il pulsante di rollover **[!UICONTROL Modifica]** dell&#39;eCatalog.
1. Seleziona **[!UICONTROL Mappa pagine]**.
1. A sinistra della schermata Mappe pagine, selezionate la pagina che ci interessa.
1. Nell’area Mappa immagine, disegnate una mappa immagine rettangolare o poligonale:

   * **Mappa rettangolare**: selezionare lo strumento Mappa immagine rettangolare e trascinare nella pagina per creare il rettangolo.

   * **Mappa poligonale**: selezionare lo strumento Mappa immagine poligonale, quindi selezionare il numero di volte necessario intorno al perimetro dell&#39;immagine. Quando si seleziona, Adobe Dynamic Media Classic disegna i bordi della mappa immagine.

     Dopo aver disegnato una mappa immagine, Adobe Dynamic Media Classic le assegna un nome nell&#39;elenco Mappa immagine. Per formare il nome, Adobe Dynamic Media Classic aggiunge un numero sequenziale al nome della pagina eCatalog in cui si sta lavorando.

1. (Facoltativo) Nell&#39;elenco Mappa immagine, nella colonna [!UICONTROL Nome], è possibile immettere un nuovo nome per la mappa immagine. Non includete spazi nel nome inserito.
1. Quando si seleziona Mappa immagine, è possibile che i visualizzatori aprano una nuova pagina Web. Nel pannello elenco Mappa immagine, immettete l&#39;URL della pagina Web nella colonna URL.

   Per semplificare l&#39;immissione degli URL (modelli Href), selezionare **[!UICONTROL Modifica]** e immettere un modello.

Vedi [Utilizzare un modello per immettere JavaScript e URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Facoltativo) Nell&#39;elenco a discesa Mostra, selezionare **[!UICONTROL Testo di rollover]**, quindi immettere il testo che si desidera visualizzare sullo schermo quando si spostano i puntatori sulla mappa immagine.
1. (Facoltativo) Nell&#39;elenco a discesa Mostra, selezionare **[!UICONTROL Altre azioni]** e immettere un attributo per attivare un&#39;azione di sfocatura o attivazione quando gli utenti spostano i puntatori su una mappa immagine.

   Vedi [Definire altre azioni per le mappe immagine](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Seleziona **[!UICONTROL Salva]**.
1. (Facoltativo) Seleziona **[!UICONTROL Anteprima]** per visualizzare l&#39;eCatalog con il predefinito visualizzatore eCatalog predefinito.

Per eliminare una mappa immagine, selezionarne il nome nell&#39;elenco Mappa immagine e selezionare **[!UICONTROL Elimina]**. È possibile disattivare temporaneamente una mappa immagine in una pagina senza eliminarla. Selezionare l&#39;opzione Mappa immagine attivata nel pannello elenco Mappa immagine.

## Incorporare rich media in un eCatalog {#embedding-rich-media-in-an-ecatalog}

Puoi utilizzare l’opzione Rich Media dell’eCatalog per aggiungere video in formato MP4 o set 360 gradi alle mappe immagine aggiunte a un eCatalog. Quando un utente seleziona l’area Mappa immagine nell’eCatalog, viene visualizzato il set 360 gradi o il video associato. Questa funzione è particolarmente utile quando si desidera illustrare ai clienti l’utilizzo di un oggetto oppure per mostrare l’oggetto da angolazioni e prospettive diverse.

Facoltativamente, puoi anche visualizzare il testo della descrizione quando i clienti spostano i puntatori sulla mappa immagine in modo che sappiano cosa stanno selezionando.

**Per incorporare rich media in un eCatalog:**

1. Disegnate una mappa immagine nell’eCatalog.

   Consulta [Disegnare mappe immagine eCatalog](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Nell&#39;elenco a discesa Mostra selezionare **[!UICONTROL Rich Media]**.
1. Nel pannello Aggiungi Assets a sinistra, passa a una cartella contenente la risorsa set 360 gradi o video (formato MP4) che desideri incorporare.
1. Trascinate la risorsa sulla mappa immagine.
1. (Facoltativo) Nel pannello dell&#39;elenco Mappa immagine, sotto l&#39;intestazione della colonna **[!UICONTROL Descrizione]**, immettere il testo che si desidera visualizzare sullo schermo quando si sposta il puntatore sulla mappa immagine.
1. Seleziona **[!UICONTROL Salva]**.

## Modifica di mappe immagine per eCatalog {#editing-ecatalog-image-maps}

Nella scheda Mappe pagine della schermata eCatalog, utilizzate le tecniche seguenti per modificare le mappe immagine per l’eCatalog:

* **Regolare la posizione**: selezionare lo strumento Panning e spostare il puntatore vicino ma non oltre il bordo della mappa. Quando il puntatore mostra una freccia a quattro punte, trascinare l&#39;intera mappa immagine in una nuova posizione.

  Consulta [Regolare la posizione, la forma e le dimensioni delle mappe immagine](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Modificare la forma e le dimensioni**: per ridimensionare una mappa immagine rettangolare, selezionare lo strumento Panning. Portate il puntatore su un lato o un angolo e quando compare l’icona della freccia a due punte, trascinate. Per ridimensionare una mappa immagine poligonale, trascinate una maniglia di selezione quadrata. Per creare un punto di manipolazione di selezione, seleziona il bordo della mappa immagine e trascina.

  Consulta [Regolare la posizione, la forma e le dimensioni delle mappe immagine](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Eliminazione mappe immagine**: selezionare lo strumento Panoramica, selezionare la mappa immagine per selezionarla, quindi selezionare **[!UICONTROL Elimina]**.

  Per rimuovere tutte le mappe immagine da un eCatalog, selezionare la scheda **[!UICONTROL Ordina pagine]**, quindi selezionare **[!UICONTROL Cancella mappe]**.

* **Gestione delle mappe immagine sovrapposte**: trascinate per modificare l&#39;ordine delle mappe immagine nell&#39;elenco Mappa immagine.

  Consulta [Gestire le mappe immagine sovrapposte](creating-image-maps.md#handling_overlapping_image_maps).

* **Copia mappe immagine in altre pagine**: Seleziona **[!UICONTROL Copia mappe in]** (assicurati di essere nella scheda Mappa pagine). Nella schermata Seleziona immagini, seleziona le pagine in cui desideri copiare le mappe immagine e seleziona **[!UICONTROL Seleziona]**.

  Vedi [Copia mappe immagine in altre immagini](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Quando si copiano mappe immagine in pagine diverse di un eCatalog, è possibile copiare tutte le mappe immagine di un eCatalog in un eCatalog diverso. Vedi [Copia mappe immagine tra gli altri eCatalog](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Rivedere e importare i dati di Image Map {#reviewing-and-importing-image-map-data}

La schermata Riepilogo mappe fornisce i metadati relativi all’eCatalog. Potete anche importare in batch i dati delle mappe immagine per l’eCatalog partendo dalla schermata Riepilogo mappe. L’importazione dei dati delle mappe immagine in questo modo consente di inserire in modo semplice gli URL delle mappe immagine e il testo di rollover.

Per visualizzare la schermata Riepilogo mappa, nella scheda Pagine mappa della schermata eCatalog, selezionare **[!UICONTROL Riepilogo]**.

### Rivedere il riepilogo dei dati delle mappe immagine {#review-image-map-data-summary}

1. Nella schermata Mappa pagine selezionare **[!UICONTROL Riepilogo]**.

   Nella schermata Riepilogo mappe viene visualizzato il numero di mappe immagine, URL, descrizioni di testo di rollover e altre azioni presenti nell’eCatalog.

1. Se sono presenti errori di chiave di rollover, seleziona l&#39;errore nella colonna **[!UICONTROL Errore di chiave di rollover]** per visualizzare le modifiche da apportare al foglio di calcolo per correggere l&#39;errore. Potete selezionare e copiare il testo di questo messaggio e incollarlo nel foglio dati.
1. Selezionare **[!UICONTROL Anteprima]** per esaminare una pagina nel visualizzatore eCatalog. Seleziona la X per chiudere la schermata Riepilogo e tornare alla schermata Mappa pagine, oppure seleziona **[!UICONTROL Chiudi]** per tornare a Sfoglia.

### Importare i dati per le mappe immagine {#import-image-map-data}

Invece di inserire i dati relativi alle mappe immagine in ciascuna pagina, potete importare i dati per l’intero eCatalog nella schermata Riepilogo mappe. Potete importare i dati delle mappe immagine come un file delimitato da tabulazioni o un file XML DTD. I campi presenti nel file devono essere nell’ordine visualizzato nella schermata Riepilogo mappe: Nome, Etichette di sommario, Mappe, URL, Testo di rollover, Altre azioni e Stringhe di ricerca. L&#39;importazione dei dati di Mappa immagine consente di evitare i problemi di immissione dei dati nell&#39;elenco Mappa immagine durante la creazione di ogni Mappa immagine.

>[!NOTE]
>
>prima di importare i dati delle mappe immagine, dovete già aver creato le mappe immagine.

Nella schermata Riepilogo mappe, seguite queste istruzioni per importare i dati della mappa immagine per le mappe immagine create:

1. Selezionare **[!UICONTROL Importa dati mappa]**.
1. Nella finestra di dialogo Importa metadati selezionare **[!UICONTROL Sfoglia]**, quindi selezionare il file DTD XML o delimitato da tabulazioni.
1. Nel campo Nome processo, digitate un nome per il file (fate attenzione a mantenere l’estensione).
1. Seleziona **[!UICONTROL Carica]**.

## Copiare mappe immagine tra gli altri eCatalog {#copying-image-maps-between-ecatalogs}

Potete copiare tutte le mappe immagine di un eCatalog in un diverso eCatalog. Questo è utile ad esempio per copiare le mappe immagine tra versioni in lingue diverse di uno stesso eCatalog. Affinché la copia abbia esito positivo, Adobe Dynamic Media Classic consiglia di copiare tra eCatalog con lo stesso numero di pagine e le stesse immagini.

>[!NOTE]
>
>se l’eCatalog in cui copiate le mappe immagine ne contiene già altre, queste ultime verranno sostituite a seguito della copia.

Per copiare tutte le mappe immagine in un eCatalog in un altro, effettuare le seguenti operazioni:

1. Seleziona l&#39;eCatalog con le mappe immagine da copiare, quindi fai clic sul pulsante di rollover **[!UICONTROL Modifica]** dell&#39;eCatalog.
1. Nella scheda Ordina pagine selezionare **[!UICONTROL Copia mappe]**.
1. Nella finestra di dialogo Seleziona risorsa, seleziona l&#39;eCatalog in cui desideri copiare le mappe immagine, quindi seleziona **[!UICONTROL Seleziona]**.

Adobe Dynamic Media Classic visualizza un messaggio di avviso se l’eCatalog di destinazione da cui si copiano le mappe immagine presenta un numero diverso di pagine o immagini di dimensioni diverse. Seleziona **[!UICONTROL Continua]** per copiare le mappe immagine nonostante l&#39;avviso.
