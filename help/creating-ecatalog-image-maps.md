---
title: Creare mappe immagine di eCatalog
description: Scopri come creare mappe immagine di eCatalog in Adobe Dynamic Media Classic.
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1493'
ht-degree: 40%

---

# Creare mappe immagine di eCatalog{#creating-ecatalog-image-maps}

Una mappa immagine è un’area su una pagina eCatalog su cui puoi passare il cursore con il mouse o selezionare per attivare azioni di vario tipo. Quando si sposta il puntatore su una mappa immagine, ad esempio, viene visualizzata una descrizione testuale di rollover di un elemento. Quando selezioni una mappa immagine, viene avviata un’altra azione. Ad esempio, potete aprire una pagina Web per consentire agli utenti di visualizzare ulteriori informazioni su un elemento o per acquistarlo, oppure per avviare un video che ne illustra l’uso.

## Disegnare mappe immagine di eCatalog {#drawing-ecatalog-image-maps}

Per gli eCatalog, potete disegnare le mappe immagine nella scheda Mappe pagine della schermata eCatalog. Questa schermata include l’area Mappa immagine in cui vengono visualizzate le pagine eCatalog e, a destra, l’elenco delle mappe immagine. Quando create delle mappe immagine, i relativi nomi vengono inseriti nell’elenco delle mappe immagine.

1. Seleziona il pulsante rollover dell’eCatalog **[!UICONTROL Modifica]** .
1. Seleziona **[!UICONTROL Mappa pagine]**.
1. A sinistra della schermata Mappe pagine, selezionate la pagina che ci interessa.
1. Nell’area Mappa immagine, disegnate una mappa immagine rettangolare o poligonale:

   * **Mappa rettangolare** : seleziona lo strumento Mappa immagine rettangolare e trascina sulla pagina per creare il rettangolo.

   * **Mappa poligonale** : selezionate lo strumento Mappa immagine poligonale, quindi selezionate il numero di volte necessario intorno al perimetro dell&#39;immagine. Come selezionato, Adobe Dynamic Media Classic disegna i bordi della mappa immagine.

      Dopo aver disegnato una mappa immagine, Adobe Dynamic Media Classic le assegna un nome nell’elenco Mappa immagine. Per creare il nome, in Adobe Dynamic Media Classic viene aggiunto un numero sequenziale al nome della pagina eCatalog in cui si sta lavorando.

1. (Facoltativo) Dall’elenco Mappa immagine, nella colonna [!UICONTROL Nome] puoi immettere un nuovo nome per la Mappa immagine. Non includete spazi nel nome inserito.
1. È possibile fare in modo che i visualizzatori aprano una nuova pagina web quando selezionano la mappa immagine. Nell’elenco delle mappe immagini, inserite l’URL della pagina Web nella colonna URL.

   Per semplificare l’immissione degli URL (modelli Href), seleziona **[!UICONTROL Modifica]** e inserisci un modello.

Consulta [Utilizzare un modello per immettere JavaScript e URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Facoltativo) Nell&#39;elenco a discesa Mostra, selezionare **[!UICONTROL Testo di rollover]**, quindi immettere il testo che gli utenti dovranno visualizzare sullo schermo quando passano il puntatore sulla mappa immagine.
1. (Facoltativo) Nell&#39;elenco a discesa Mostra , seleziona **[!UICONTROL Altre azioni]** e immetti un attributo per attivare un&#39;azione di sfocatura o messa a fuoco quando gli utenti spostano i loro puntatori su una mappa immagine.

   Consulta [Definire altre azioni per le mappe immagine](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Selezionare **[!UICONTROL Salva]**.
1. (Facoltativo) Seleziona **[!UICONTROL Anteprima]** per visualizzare l&#39;eCatalog con il visualizzatore di eCatalog predefinito.

Per eliminare una mappa immagine, selezionane il nome nell’elenco Mappa immagine e seleziona **[!UICONTROL Elimina]**. Per disattivare temporaneamente una mappa immagine in una pagina senza eliminarla completamente, deselezionate l’opzione Attivato corrispondente nel pannello di elencazione delle mappe immagine.

## Incorporare contenuti multimediali complessi in un eCatalog {#embedding-rich-media-in-an-ecatalog}

È possibile utilizzare l’opzione Contenuti multimediali avanzati dell’eCatalog per includere video in formato MP4 o set 360 gradi nelle mappe immagine aggiunte a un eCatalog. Quando un utente seleziona l’area Mappa immagine nell’eCatalog, viene visualizzato il set 360 gradi o il video associato. Questa funzione è particolarmente utile quando si desidera illustrare ai clienti l’utilizzo di un oggetto oppure per mostrare l’oggetto da angolazioni e prospettive diverse.

Facoltativamente, puoi anche visualizzare il testo della descrizione comando quando i clienti spostano i loro puntatori sulla mappa immagine in modo che sappiano cosa stanno selezionando.

**Per incorporare contenuti multimediali in un eCatalog:**

1. Disegnate una mappa immagine nell’eCatalog.

   Consulta [Disegnare mappe immagine di eCatalog](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Nell’elenco a discesa Mostra , seleziona **[!UICONTROL Contenuti multimediali avanzati]**.
1. Nel pannello Aggiungi risorse sulla sinistra, individuate la cartella che contiene il set 360 gradi o il video (formato MP4) da incorporare.
1. Trascinate la risorsa sulla mappa immagine.
1. (Facoltativo) Nel pannello elenco Mappa immagine, sotto l&#39;intestazione di colonna **[!UICONTROL Descrizione comandi]** , immetti il testo che gli utenti dovranno visualizzare sullo schermo quando posizionano il puntatore del mouse sulla mappa immagine.
1. Selezionare **[!UICONTROL Salva]**.

## Modifica di mappe immagine per eCatalog {#editing-ecatalog-image-maps}

Nella scheda Mappe pagine della schermata eCatalog, utilizzate le tecniche seguenti per modificare le mappe immagine per l’eCatalog:

* **Regolare la posizione** : selezionate lo strumento Panning e spostate il puntatore vicino ma non oltre il bordo della mappa. Quando il puntatore diventa una freccia a quattro punte, trascinate l’intera mappa immagine in una nuova posizione.

   Consultare [Regolare la posizione, la forma e le dimensioni delle mappe immagine](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Modifica forma e dimensione** : per ridimensionare una mappa immagine rettangolare, selezionate lo strumento Panning. Portate il puntatore su un lato o un angolo e quando compare l’icona della freccia a due punte, trascinate. Per ridimensionare una mappa immagine poligonale, trascinate una maniglia di selezione quadrata. Per creare una maniglia di selezione, selezionate il bordo della mappa immagine e trascinate.

   Consultare [Regolare la posizione, la forma e le dimensioni delle mappe immagine](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Eliminazione delle mappe immagine** : selezionate lo strumento Panning, selezionate la mappa immagine per selezionarla, quindi selezionate  **[!UICONTROL Elimina]**.

   Per rimuovere tutte le mappe immagine da un eCatalog, seleziona la scheda **[!UICONTROL Ordina pagine]** , quindi seleziona **[!UICONTROL Cancella mappe]**.

* **Gestione delle mappe immagine sovrapposte**  - Trascinate per modificare l’ordine delle mappe immagine nell’elenco Mappa immagine.

   Consulta [Gestire le mappe immagine sovrapposte](creating-image-maps.md#handling_overlapping_image_maps).

* **Copia delle mappe immagine in altre pagine**  - Seleziona  **[!UICONTROL Copia mappe in]**  (accertati di essere nella scheda Mappa pagine ). Nella schermata Seleziona immagini , seleziona la pagina o le pagine in cui desideri copiare le mappe immagine e seleziona **[!UICONTROL Seleziona]**.

   Consulta [Copia mappe immagine in altre immagini](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Oltre a copiare le mappe immagine in pagine diverse di un eCatalog, puoi copiare tutte le mappe immagine di un eCatalog in un altro eCatalog. Consulta [Copia mappe immagine tra eCatalog](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Rivedere e importare i dati della mappa immagine {#reviewing-and-importing-image-map-data}

La schermata Riepilogo mappe fornisce i metadati relativi all’eCatalog. Potete anche importare in batch i dati delle mappe immagine per l’eCatalog partendo dalla schermata Riepilogo mappe. L’importazione dei dati delle mappe immagine in questo modo consente di inserire in modo semplice gli URL delle mappe immagine e il testo di rollover.

Per visualizzare la schermata Riepilogo mappa, nella scheda Pagine mappa della schermata eCatalog, seleziona **[!UICONTROL Riepilogo]**.

### Rivedere il riepilogo dei dati delle mappe immagine {#review-image-map-data-summary}

1. Nella schermata Mappa pagine , seleziona **[!UICONTROL Riepilogo]**.

   Nella schermata Riepilogo mappe viene visualizzato il numero di mappe immagine, di URL, di descrizioni di testi di rollover e di altre azioni presenti nell’eCatalog.

1. In caso di errori con la chiave di rollover, seleziona l’errore nella colonna **[!UICONTROL Errore rollover_Key]** per vedere cosa deve cambiare nel foglio di calcolo per correggere l’errore. Potete selezionare e copiare il testo di questo messaggio e incollarlo nel foglio dati.
1. Seleziona **[!UICONTROL Anteprima]** per esaminare una pagina nel visualizzatore di eCatalog; seleziona la X per chiudere la schermata Riepilogo e tornare alla schermata Mappa pagine oppure seleziona **[!UICONTROL Chiudi]** per tornare a Sfoglia.

### Importare i dati per le mappe immagine {#import-image-map-data}

Invece di inserire i dati relativi alle mappe immagine in ciascuna pagina, potete importare i dati per l’intero eCatalog nella schermata Riepilogo mappe. Potete importare i dati delle mappe immagine come un file delimitato da tabulazioni o un file XML DTD. I campi presenti nel file devono essere nell’ordine visualizzato nella schermata Riepilogo mappe: Nome, Etichette di sommario, Mappe, URL, Testo di rollover, Altre azioni e Stringhe di ricerca. Importando i dati delle mappe immagine si evita di dover inserire i dati nell’elenco delle mappe immagine durante la creazione di ciascuna mappa immagine.

>[!NOTE]
>
>prima di importare i dati delle mappe immagine, dovete già aver creato le mappe immagine.

Nella schermata Riepilogo mappe, seguite queste istruzioni per importare i dati della mappa immagine per le mappe immagine create:

1. Seleziona **[!UICONTROL Importa dati mappa]**.
1. Nella finestra di dialogo Importa metadati, selezionare **[!UICONTROL Sfoglia]**, quindi selezionare il file DTD XML o delimitato da tabulazioni.
1. Nel campo Nome processo, digitate un nome per il file (fate attenzione a mantenere l’estensione).
1. Seleziona **[!UICONTROL Carica]**.

## Copiare mappe immagine tra gli eCatalogs {#copying-image-maps-between-ecatalogs}

Potete copiare tutte le mappe immagine di un eCatalog in un diverso eCatalog. Questo è utile ad esempio per copiare le mappe immagine tra versioni in lingue diverse di uno stesso eCatalog. Affinché la copia abbia successo, ad Adobe, Dynamic Media Classic consiglia di copiare tra eCatalogs con lo stesso numero di pagine e le stesse immagini.

>[!NOTE]
>
>se l’eCatalog in cui copiate le mappe immagine ne contiene già altre, queste ultime verranno sostituite a seguito della copia.

Per copiare tutte le mappe immagine di un eCatalog in un altro eCatalog, procedi come segue:

1. Seleziona l’eCatalog con le mappe immagine da copiare e fai clic sul pulsante rollover dell’eCatalog **[!UICONTROL Modifica]** .
1. Nella scheda Pagine ordine , seleziona **[!UICONTROL Copia mappe]**.
1. Nella finestra di dialogo Seleziona risorsa , seleziona l’eCatalog in cui desideri copiare le mappe immagine, quindi seleziona **[!UICONTROL Seleziona]**.

Ad Adobe, Dynamic Media Classic visualizza un messaggio di avviso se l’eCatalog di destinazione (l’eCatalog in cui copiate le mappe immagine) ha un numero diverso di pagine o immagini di dimensioni diverse. Seleziona **[!UICONTROL Continua]** per copiare le mappe immagine nonostante l&#39;avviso.
