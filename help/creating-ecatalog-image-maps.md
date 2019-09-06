---
title: Creazione di mappe immagine per un eCatalog
seo-title: Creazione di mappe immagine per un eCatalog
description: 'null'
seo-description: Scoprite come creare mappe immagine ecatalog.
uuid: 943 ad 3 f 7-a 885-4 bc 2-88 cb -77083384 bdf 8
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/ecatalogs
discoiquuid: 4 cf 63359-63 b 5-4 da 7-9498-335 d 91 b 4776 c
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Creazione di mappe immagine per un eCatalog{#creating-ecatalog-image-maps}

Una mappa immagine è un’area in una pagina eCatalog su cui l’utente può passare il mouse o fare clic per effettuare operazioni di vario tipo. Quando si passa il puntatore su una mappa immagine, si può ad esempio visualizzare la descrizione a comparsa di un elemento. Quando fate clic su una Mappa immagine, viene avviata un’altra azione. Ad esempio, potete aprire una pagina Web per consentire agli utenti di visualizzare ulteriori informazioni su un elemento o per acquistarlo, oppure per avviare un video che ne illustra l’uso.

## Disegnare mappe immagine per eCatalog {#drawing-ecatalog-image-maps}

Per gli eCatalog, potete disegnare le mappe immagine nella scheda Mappe pagine della schermata eCatalog. Questa schermata include l’area Mappa immagine in cui vengono visualizzate le pagine eCatalog e, a destra, l’elenco delle mappe immagine. Quando create delle mappe immagine, i relativi nomi vengono inseriti nell’elenco delle mappe immagine.

1. Fate clic sul pulsante rollover Modifica dell’eCatalog.
1. Click **Map Pages**.
1. A sinistra della schermata Mappe pagine, selezionate la pagina che ci interessa.
1. Nell’area Mappa immagine, disegnate una mappa immagine rettangolare o poligonale:

   **Mappa rettangolare** Selezionate lo strumento rettangolo e trascinate sulla pagina per creare il rettangolo.

   **Mappa poligonale** Selezionate lo strumento poligono e fate clic il numero di volte necessario intorno al perimetro dell'immagine. Quando fate clic su, Dynamic Media Classic disegna i bordi della mappa immagine.

   Dopo aver disegnato una mappa immagine, Dynamic Media Classic le assegna un nome nell'elenco Mappa immagine. Per formare il nome, Dynamic Media Classic aggiunge un numero sequenziale al nome della pagina ecatalog in cui state lavorando.

1. (Facoltativo) Nell’elenco delle mappe immagini, nella colonna Nome, immettete un nuovo nome per la mappa immagine. Non includete spazi nel nome inserito.
1. Una mappa immagine può essere usata per consentire agli utenti di aprire una nuova pagina Web quando fanno clic sulla mappa immagine. Nell’elenco delle mappe immagini, inserite l’URL della pagina Web nella colonna URL.

   Fate clic su Modifica e inserite un modello per facilitare l’inserimento degli URL (modelli Href).

   Consultate [Utilizzo di un modello per inserire JavaScript e URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Optional) In the Show drop-down list, click **Rollover Text**, and then enter the text that you want users to see onscreen when they move their pointers over the Image Map.
1. (Optional) In the Show drop-down list, click **Other Actions**, and enter an attribute to trigger a blur or focus action when users move their pointers over an Image Map.

   Consultate [Definizione di altre azioni per le mappe immagine](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Fate clic su **Salva**.
1. (Optional) Click **Preview** to view the eCatalog with the default eCatalog Viewer preset.

Per eliminare una mappa immagine, selezionatene il nome nell’elenco Mappa immagine e fate clic su Elimina. Per disattivare temporaneamente una mappa immagine in una pagina senza eliminarla completamente, deselezionate l’opzione Attivato corrispondente nel pannello di elencazione delle mappe immagine.

## Incorporamento di contenuti multimediali in un eCatalog {#embedding-rich-media-in-an-ecatalog}

È possibile utilizzare l’opzione Contenuti multimediali avanzati dell’eCatalog per includere video in formato MP4 o set 360 gradi nelle mappe immagine aggiunte a un eCatalog. Quando un utente fa clic sull’area della mappa immagine nell’eCatalog, viene visualizzato il video o set 360 gradi associato. Questa funzione è particolarmente utile quando si desidera illustrare ai clienti l’utilizzo di un oggetto oppure per mostrare l’oggetto da angolazioni e prospettive diverse.

Potete anche visualizzare un testo descrittivo a comparsa quando i clienti passano il mouse sulla mappa immagine, per informarli del contenuto che stanno selezionando.

**Per incorporare contenuti multimediali in un eCatalog**

1. Disegnate una mappa immagine nell’eCatalog.

   Consultate [Disegnare mappe immagine per eCatalog](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Nell’elenco a discesa Mostra, selezionate Contenuti multimediali avanzati.
1. Nel pannello Aggiungi risorse sulla sinistra, individuate la cartella che contiene il set 360 gradi o il video (formato MP4) da incorporare.
1. Trascinate la risorsa sulla mappa immagine.
1. (Facoltativo) Nel pannello Mappa immagine, nella colonna Descrizione, inserite il testo che gli utenti devono vedere quando passano il mouse sulla mappa immagine.
1. Fate clic su Salva.

## Modifica di mappe immagine per eCatalog {#editing-ecatalog-image-maps}

Nella scheda Mappe pagine della schermata eCatalog, utilizzate le tecniche seguenti per modificare le mappe immagine per l’eCatalog:

**Regolazione della posizione** Selezionate lo strumento scorrimento e portate il puntatore vicino ma non sopra il bordo della mappa. Quando il puntatore diventa una freccia a quattro punte, trascinate l’intera mappa immagine in una nuova posizione.

Consultate [Regolazione della posizione, forma e dimensione delle mappe immagine](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

**Modifica della forma e della dimensione** Per ridimensionare una mappa immagine rettangolare, selezionate lo strumento scorrimento. Portate il puntatore su un lato o un angolo e quando compare l’icona della freccia a due punte, trascinate. Per ridimensionare una mappa immagine poligonale, trascinate una maniglia di selezione quadrata. Per creare una maniglia di selezione, fate clic sul bordo della mappa immagine e trascinate.

Consultate [Regolazione della posizione, forma e dimensione delle mappe immagine](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

**Eliminazione delle mappe immagine** Selezionate lo strumento scorrimento, fate clic sulla mappa immagine per selezionarla, quindi fate clic su Elimina.

Per rimuovere tutte le mappe immagine di un eCatalog, passate alla scheda Ordina pagine e fate clic su Cancella mappe.

**Gestione delle mappe immagine sovrapposte** Trascinate per modificare l'ordine delle mappe immagine nell'elenco delle mappe immagine.

Consultate [Gestione delle mappe immagine sovrapposte](creating-image-maps.md#handling_overlapping_image_maps).

**Copia delle mappe immagine in altre pagine** Fate clic sul pulsante Copia mappe in (verificate di trovarvi nella scheda Mappe pagine). Nella schermata Seleziona immagini, selezionate la pagina o le pagine in cui desiderate copiare le mappe immagine e fate clic sul pulsante Seleziona. 

Consultate [Copia delle mappe immagine in altre immagini](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>oltre a copiare le mappe immagine in altre pagine di uno stesso eCatalog, potete copiare in un altro eCatalog tutte le mappe immagine di un eCatalog. Consultate [Copia di mappe immagine tra diversi eCatalog](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs)

## Revisione e importazione dei dati delle mappe immagine {#reviewing-and-importing-image-map-data}

La schermata Riepilogo mappe fornisce i metadati relativi all’eCatalog. Potete anche importare in batch i dati delle mappe immagine per l’eCatalog partendo dalla schermata Riepilogo mappe. L’importazione dei dati delle mappe immagine in questo modo consente di inserire in modo semplice gli URL delle mappe immagine e il testo di rollover.

Per visualizzare la schermata Riepilogo mappe, nella scheda Mappe pagine della schermata eCatalog fate clic su Riepilogo.

### Rivedere il riepilogo dei dati delle mappe immagine {#review-image-map-data-summary}

1. Nella schermata Mappe pagine, fate clic su Riepilogo.

   Nella schermata Riepilogo mappe viene visualizzato il numero di mappe immagine, di URL, di descrizioni di testi di rollover e di altre azioni presenti nell’eCatalog.

1. Se si verificano errori relativi al testo chiave di rollover, fate clic sull’errore nella colonna Errore Rollover_Key per visualizzare le modifiche da apportare nel foglio dati per correggere l’errore. Potete selezionare e copiare il testo di questo messaggio e incollarlo nel foglio dati.
1. Fate clic su Anteprima per esaminare una pagina nel visualizzatore di eCatalog, fate clic sulla X per chiudere la schermata Riepilogo e tornare alla schermata Mappe pagine oppure fate clic su Chiudi per tornare a Sfoglia.

### Importare i dati per le mappe immagine {#import-image-map-data}

Invece di inserire i dati relativi alle mappe immagine in ciascuna pagina, potete importare i dati per l’intero eCatalog nella schermata Riepilogo mappe. Potete importare i dati delle mappe immagine come un file delimitato da tabulazioni o un file XML DTD. I campi presenti nel file devono essere nell’ordine visualizzato nella schermata Riepilogo mappe: Nome, Etichette di sommario, Mappe, URL, Testo di rollover, Altre azioni e Stringhe di ricerca. Importando i dati delle mappe immagine si evita di dover inserire i dati nell’elenco delle mappe immagine durante la creazione di ciascuna mappa immagine.

>[!NOTE]
>
>prima di importare i dati delle mappe immagine, dovete già aver creato le mappe immagine.

Nella schermata Riepilogo mappe, seguite queste istruzioni per importare i dati della mappa immagine per le mappe immagine create:

1. Fate clic su Importa dati mappa.
1. Nella finestra di dialogo Importa metadati, fate clic su Sfoglia e selezionate il file DTD XML o delimitato da tabulazioni.
1. Nel campo Nome processo, digitate un nome per il file (fate attenzione a mantenere l’estensione).
1. Fate clic su Carica.

## Copia di mappe immagine tra diversi eCatalog {#copying-image-maps-between-ecatalogs}

Potete copiare tutte le mappe immagine di un eCatalog in un diverso eCatalog. Questo è utile ad esempio per copiare le mappe immagine tra versioni in lingue diverse di uno stesso eCatalog. Affinché la copia abbia esito positivo, Dynamic Media Classic consiglia di copiare tra ecatalog con lo stesso numero di pagine e le stesse immagini.

>[!NOTE]
>
>se l’eCatalog in cui copiate le mappe immagine ne contiene già altre, queste ultime verranno sostituite a seguito della copia.

Per copiare tutte le mappe immagine di un eCatalog in un altro eCatalog, effettuate le seguenti operazioni:

1. Selezionate l’eCatalog contenente le mappe immagine che desiderate copiare, quindi fate clic sul pulsante rollover Modifica dell’eCatalog.
1. Nella scheda Ordina pagine, fate clic su Copia mappe.
1. Nella finestra di dialogo Seleziona risorsa, selezionate l’eCatalog in cui desiderate copiare le mappe immagine, quindi fate clic su Seleziona.

Dynamic Media Classic visualizza un messaggio di avviso se l'ecatalog di destinazione (l'ecatalog in cui copiate le mappe immagine) ha un numero diverso di pagine o immagini di dimensioni diverse. Potete fate clic su Continua per copiare comunque le mappe immagine.