---
title: Creazione di mappe immagine per un eCatalog
description: Scopri come creare mappe immagine di eCatalog.
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Visualizzatori,eCatalog
role: Business Practitioner
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
source-git-commit: bd0659c015f259e25d6d07b620f5b1e948cabcbf
workflow-type: tm+mt
source-wordcount: '1484'
ht-degree: 55%

---

# Creazione di mappe immagine per un eCatalog{#creating-ecatalog-image-maps}

Una mappa immagine è un’area in una pagina eCatalog su cui l’utente può passare il mouse o fare clic per effettuare operazioni di vario tipo. Quando si sposta il puntatore su una mappa immagine, ad esempio, viene visualizzata una descrizione testuale di rollover di un elemento. Quando fate clic su una Mappa immagine, viene avviata un’altra azione. Ad esempio, potete aprire una pagina Web per consentire agli utenti di visualizzare ulteriori informazioni su un elemento o per acquistarlo, oppure per avviare un video che ne illustra l’uso.

## Disegnare mappe immagine per eCatalog {#drawing-ecatalog-image-maps}

Per gli eCatalog, potete disegnare le mappe immagine nella scheda Mappe pagine della schermata eCatalog. Questa schermata include l’area Mappa immagine in cui vengono visualizzate le pagine eCatalog e, a destra, l’elenco delle mappe immagine. Quando create delle mappe immagine, i relativi nomi vengono inseriti nell’elenco delle mappe immagine.

1. Fate clic sul pulsante rollover **[!UICONTROL Modifica]** dell’eCatalog.
1. Fai clic su **[!UICONTROL Mappa pagine]**.
1. A sinistra della schermata Mappe pagine, selezionate la pagina che ci interessa.
1. Nell’area Mappa immagine, disegnate una mappa immagine rettangolare o poligonale:

   * **Mappa rettangolare** : seleziona lo strumento Mappa immagine rettangolare e trascina sulla pagina per creare il rettangolo.

   * **Mappa poligonale** : selezionate lo strumento Mappa immagine poligonale e fate clic il numero di volte necessario intorno al perimetro dell&#39;immagine. Facendo clic su, Dynamic Media Classic disegna i bordi della mappa immagine.

      Dopo aver disegnato una mappa immagine, Dynamic Media Classic le assegna un nome nell’elenco Mappa immagine. Per creare il nome, Dynamic Media Classic aggiunge un numero sequenziale al nome della pagina eCatalog in cui si sta lavorando.

1. (Facoltativo) Nell’elenco delle mappe immagini, nella colonna Nome, immettete un nuovo nome per la mappa immagine. Non includete spazi nel nome inserito.
1. Una mappa immagine può essere usata per consentire agli utenti di aprire una nuova pagina Web quando fanno clic sulla mappa immagine. Nell’elenco delle mappe immagini, inserite l’URL della pagina Web nella colonna URL.

   Per semplificare l’immissione degli URL (modelli Href), fai clic su **[!UICONTROL Modifica]** e immetti un modello.

Consulta [Utilizzo di un modello per immettere JavaScript™ e URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Facoltativo) Nell&#39;elenco a discesa Mostra, fare clic su **[!UICONTROL Testo di rollover]**, quindi immettere il testo che gli utenti dovranno visualizzare sullo schermo quando passano il puntatore sulla mappa immagine.
1. (Facoltativo) Nell&#39;elenco a discesa Mostra , fai clic su **[!UICONTROL Altre azioni]** e immetti un attributo per attivare un&#39;azione di sfocatura o messa a fuoco quando gli utenti spostano i loro puntatori su una mappa immagine.

   Consultate [Definizione di altre azioni per le mappe immagine](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Fate clic su **[!UICONTROL Salva]**.
1. (Facoltativo) Fai clic su **[!UICONTROL Anteprima]** per visualizzare l&#39;eCatalog con il visualizzatore di eCatalog predefinito.

Per eliminare una mappa immagine, selezionane il nome nell’elenco Mappa immagine e fai clic su **[!UICONTROL Elimina]**. Per disattivare temporaneamente una mappa immagine in una pagina senza eliminarla completamente, deselezionate l’opzione Attivato corrispondente nel pannello di elencazione delle mappe immagine.

## Incorporamento di contenuti multimediali in un eCatalog {#embedding-rich-media-in-an-ecatalog}

È possibile utilizzare l’opzione Contenuti multimediali avanzati dell’eCatalog per includere video in formato MP4 o set 360 gradi nelle mappe immagine aggiunte a un eCatalog. Quando un utente fa clic sull’area della mappa immagine nell’eCatalog, viene visualizzato il video o set 360 gradi associato. Questa funzione è particolarmente utile quando si desidera illustrare ai clienti l’utilizzo di un oggetto oppure per mostrare l’oggetto da angolazioni e prospettive diverse.

Facoltativamente, puoi anche visualizzare il testo della descrizione comando quando i clienti spostano i loro puntatori sulla mappa immagine in modo che sappiano cosa stanno facendo.

**Per incorporare contenuti multimediali in un eCatalog:**

1. Disegnate una mappa immagine nell’eCatalog.

   Consultate [Disegnare mappe immagine per eCatalog](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Nell’elenco a discesa Mostra , seleziona **[!UICONTROL Contenuti multimediali avanzati]**.
1. Nel pannello Aggiungi risorse sulla sinistra, individuate la cartella che contiene il set 360 gradi o il video (formato MP4) da incorporare.
1. Trascinate la risorsa sulla mappa immagine.
1. (Facoltativo) Nel pannello elenco Mappa immagine, sotto l&#39;intestazione di colonna **[!UICONTROL Descrizione comandi]** , immetti il testo che gli utenti dovranno visualizzare sullo schermo quando posizionano il puntatore del mouse sulla mappa immagine.
1. Fate clic su **[!UICONTROL Salva]**.

## Modifica di mappe immagine per eCatalog {#editing-ecatalog-image-maps}

Nella scheda Mappe pagine della schermata eCatalog, utilizzate le tecniche seguenti per modificare le mappe immagine per l’eCatalog:

* **Regolazione della posizione** : seleziona lo strumento Panning e sposta il puntatore vicino ma non oltre il bordo della mappa. Quando il puntatore diventa una freccia a quattro punte, trascinate l’intera mappa immagine in una nuova posizione.

   Consultate [Regolazione della posizione, forma e dimensione delle mappe immagine](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Modifica della forma e delle dimensioni** : per ridimensionare una mappa immagine rettangolare, selezionate lo strumento Panning. Portate il puntatore su un lato o un angolo e quando compare l’icona della freccia a due punte, trascinate. Per ridimensionare una mappa immagine poligonale, trascinate una maniglia di selezione quadrata. Per creare una maniglia di selezione, fate clic sul bordo della mappa immagine e trascinate.

   Consultate [Regolazione della posizione, forma e dimensione delle mappe immagine](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Eliminazione delle mappe immagine** : selezionate lo strumento Panning, fate clic sulla mappa immagine per selezionarla, quindi fate clic su  **[!UICONTROL Elimina]**.

   Per rimuovere tutte le mappe immagine da un eCatalog, fai clic sulla scheda **[!UICONTROL Ordina pagine]** , quindi fai clic su **[!UICONTROL Cancella mappe]**.

* **Gestione delle mappe immagine sovrapposte**  - Trascinate per modificare l’ordine delle mappe immagine nell’elenco Mappa immagine.

   Consultate [Gestione delle mappe immagine sovrapposte](creating-image-maps.md#handling_overlapping_image_maps).

* **Copiare le mappe immagine in altre pagine**  - Fate clic su  **[!UICONTROL Copia mappe in]**  (accertatevi di essere nella scheda Mappe pagine). Nella schermata Seleziona immagini , seleziona la pagina o le pagine in cui desideri copiare le mappe immagine e fai clic su **[!UICONTROL Seleziona]**.

   Consultate [Copia delle mappe immagine in altre immagini](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Oltre a copiare le mappe immagine in pagine diverse di un eCatalog, puoi copiare tutte le mappe immagine di un eCatalog in un altro eCatalog. Consultate [Copia di mappe immagine tra diversi eCatalog](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs)

## Revisione e importazione dei dati delle mappe immagine {#reviewing-and-importing-image-map-data}

La schermata Riepilogo mappe fornisce i metadati relativi all’eCatalog. Potete anche importare in batch i dati delle mappe immagine per l’eCatalog partendo dalla schermata Riepilogo mappe. L’importazione dei dati delle mappe immagine in questo modo consente di inserire in modo semplice gli URL delle mappe immagine e il testo di rollover.

Per visualizzare la schermata Riepilogo mappe, nella scheda Mappe pagine della schermata eCatalog fate clic su Riepilogo.

### Rivedere il riepilogo dei dati delle mappe immagine {#review-image-map-data-summary}

1. Nella schermata Mappa pagine, fai clic su **[!UICONTROL Riepilogo]**.

   Nella schermata Riepilogo mappe viene visualizzato il numero di mappe immagine, di URL, di descrizioni di testi di rollover e di altre azioni presenti nell’eCatalog.

1. In caso di errori con la chiave di rollover, fai clic sull’errore nella colonna **[!UICONTROL Errore rollover_Key]** per vedere cosa deve cambiare nel foglio di calcolo per correggere l’errore. Potete selezionare e copiare il testo di questo messaggio e incollarlo nel foglio dati.
1. Fai clic su **[!UICONTROL Anteprima]** per esaminare una pagina nel visualizzatore di eCatalog, fai clic sulla X per chiudere la schermata Riepilogo e tornare alla schermata Mappa pagine oppure fai clic su **[!UICONTROL Chiudi]** per tornare a Sfoglia.

### Importare i dati per le mappe immagine {#import-image-map-data}

Invece di inserire i dati relativi alle mappe immagine in ciascuna pagina, potete importare i dati per l’intero eCatalog nella schermata Riepilogo mappe. Potete importare i dati delle mappe immagine come un file delimitato da tabulazioni o un file XML DTD. I campi presenti nel file devono essere nell’ordine visualizzato nella schermata Riepilogo mappe: Nome, Etichette di sommario, Mappe, URL, Testo di rollover, Altre azioni e Stringhe di ricerca. Importando i dati delle mappe immagine si evita di dover inserire i dati nell’elenco delle mappe immagine durante la creazione di ciascuna mappa immagine.

>[!NOTE]
>
>prima di importare i dati delle mappe immagine, dovete già aver creato le mappe immagine.

Nella schermata Riepilogo mappe, seguite queste istruzioni per importare i dati della mappa immagine per le mappe immagine create:

1. Fai clic su **[!UICONTROL Importa dati mappa]**.
1. Nella finestra di dialogo Importa metadati fare clic su **[!UICONTROL Sfoglia]**, quindi selezionare il file DTD XML o delimitato da tabulazioni.
1. Nel campo Nome processo, digitate un nome per il file (fate attenzione a mantenere l’estensione).
1. Fate clic su **[!UICONTROL Carica]**.

## Copia di mappe immagine tra diversi eCatalog {#copying-image-maps-between-ecatalogs}

Potete copiare tutte le mappe immagine di un eCatalog in un diverso eCatalog. Questo è utile ad esempio per copiare le mappe immagine tra versioni in lingue diverse di uno stesso eCatalog. Affinché la copia abbia successo, Dynamic Media Classic consiglia di copiare tra eCatalogs con lo stesso numero di pagine e le stesse immagini.

>[!NOTE]
>
>se l’eCatalog in cui copiate le mappe immagine ne contiene già altre, queste ultime verranno sostituite a seguito della copia.

Per copiare tutte le mappe immagine di un eCatalog in un altro eCatalog, procedi come segue:

1. Seleziona l’eCatalog con le mappe immagine da copiare e fai clic sul pulsante rollover dell’eCatalog **[!UICONTROL Modifica]** .
1. Nella scheda Pagine ordine fare clic su **[!UICONTROL Copia mappe]**.
1. Nella finestra di dialogo Seleziona risorsa , seleziona l’eCatalog in cui desideri copiare le mappe immagine, quindi fai clic su **[!UICONTROL Seleziona]**.

Dynamic Media Classic visualizza un messaggio di avviso se l’eCatalog di destinazione (l’eCatalog in cui copiate le mappe immagine) ha un numero diverso di pagine o immagini di dimensioni diverse. Fai clic su **[!UICONTROL Continua]** per copiare le mappe immagine nonostante l&#39;avviso.
