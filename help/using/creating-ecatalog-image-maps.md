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
autotag-review: '2026-05-13T17:43:26.837Z'
TQID: 'https://experienceleague.adobe.com/E1qnvzD2WIqVHt0UAtIq7bZfYlPZbfG9Ye6F9ntX5Q4'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 23257d3c04ec0d662f382ffb55fd6c26454d39a2
workflow-type: tm+mt
source-wordcount: 1496
ht-degree: 18%

---

# Crea mappe immagine eCatalog{#creating-ecatalog-image-maps}

Una mappa immagine è un&#39;area di una pagina eCatalog che è possibile spostare con il mouse o selezionare per attivare azioni di vario tipo. Quando si sposta il puntatore su una mappa immagine, ad esempio, viene visualizzata una descrizione di testo di rollover di un elemento. Quando selezioni una mappa immagine, viene avviata un’altra azione. Ad esempio, è possibile aprire una pagina Web per consentire agli utenti di ottenere ulteriori informazioni su un elemento o acquistarlo, oppure è possibile avviare un video per visualizzare un elemento in uso.

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

   Per semplificare l&#39;immissione di URL (modelli HREF), selezionare **[!UICONTROL Modifica]** e immettere un modello.

Vedi [Utilizzare un modello per immettere JavaScript e URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Facoltativo) Nell&#39;elenco a discesa Mostra, selezionare **[!UICONTROL Testo di rollover]**, quindi immettere il testo che si desidera visualizzare sullo schermo quando si spostano i puntatori sulla mappa immagine.
1. (Facoltativo) Nell&#39;elenco a discesa Mostra, selezionare **[!UICONTROL Altre azioni]** e immettere un attributo per attivare un&#39;azione di sfocatura o attivazione quando gli utenti spostano i puntatori su una mappa immagine.

   Vedi [Definire altre azioni per le mappe immagine](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Seleziona **[!UICONTROL Salva]**.
1. (Facoltativo) Seleziona **[!UICONTROL Anteprima]** per visualizzare l&#39;eCatalog con il predefinito visualizzatore eCatalog predefinito.

Per eliminare una mappa immagine, selezionarne il nome nell&#39;elenco Mappa immagine e selezionare **[!UICONTROL Elimina]**. È possibile disattivare temporaneamente una mappa immagine in una pagina senza eliminarla. Selezionare l&#39;opzione Mappa immagine attivata nel pannello elenco Mappa immagine.

## Incorporare rich media in un eCatalog {#embedding-rich-media-in-an-ecatalog}

Puoi utilizzare l’opzione Rich Media dell’eCatalog per aggiungere video in formato MP4 o set 360 gradi alle mappe immagine aggiunte a un eCatalog. Quando un utente seleziona l’area Mappa immagine nell’eCatalog, viene visualizzato il set 360 gradi o il video associato. Questa funzionalità è particolarmente utile se si desidera che i clienti visualizzino un articolo durante l&#39;uso o che lo visualizzino da diverse angolazioni.

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

* **Regolare la posizione**: selezionare lo strumento Panning e spostare il puntatore vicino al bordo della mappa senza posizionarlo sulla mappa. Quando il puntatore mostra un&#39;icona a forma di freccia direzionale, trascinare l&#39;intera mappa immagine in una nuova posizione.

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
>Quando si copiano mappe immagine in pagine diverse di un eCatalog, è anche possibile copiare tutte le mappe immagine da un eCatalog a un altro. Vedi [Copia mappe immagine tra eCatalog](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Rivedere e importare i dati di Image Map {#reviewing-and-importing-image-map-data}

La schermata Riepilogo mappe fornisce i metadati relativi all’eCatalog. Potete anche importare in batch i dati delle mappe immagine per l’eCatalog partendo dalla schermata Riepilogo mappe. L’importazione dei dati della mappa immagine semplifica l’immissione degli URL della mappa immagine e del testo di rollover.

Per visualizzare la schermata Riepilogo mappa, nella scheda Pagine mappa della schermata eCatalog, selezionare **[!UICONTROL Riepilogo]**.

### Rivedere il riepilogo dei dati delle mappe immagine {#review-image-map-data-summary}

1. Nella schermata Mappa pagine selezionare **[!UICONTROL Riepilogo]**.

   Nella schermata Riepilogo mappe viene visualizzato il numero di mappe immagine, URL, descrizioni di testo di rollover e altre azioni presenti nell’eCatalog.

1. Se sono presenti errori di rollover, seleziona l&#39;errore nella colonna **[!UICONTROL Errore chiave di rollover]** per visualizzare gli elementi da aggiornare nel foglio di calcolo per correggerlo. Potete selezionare e copiare il testo di questo messaggio e incollarlo nel foglio dati.
1. Selezionare **[!UICONTROL Anteprima]** per esaminare una pagina nel visualizzatore eCatalog. Seleziona la X per chiudere la schermata Riepilogo e tornare alla schermata Mappa pagine, oppure seleziona **[!UICONTROL Chiudi]** per tornare a Sfoglia.

### Importare i dati per le mappe immagine {#import-image-map-data}

Anziché immettere i dati della mappa immagine in ogni pagina, è possibile importare i dati dell&#39;intero eCatalog nella schermata Riepilogo mappa. Potete importare i dati delle mappe immagine come un file delimitato da tabulazioni o un file XML DTD. I campi nel file devono seguire l’ordine mostrato nella schermata Riepilogo mappa: Nome, Etichette sommario, Mappe, URL, Testo di rollover, Altre azioni e Stringhe di ricerca. L&#39;importazione dei dati della mappa immagine elimina la necessità di immettere i dati nell&#39;elenco Mappa immagine durante la creazione di ogni mappa immagine.

>[!NOTE]
>
>prima di importare i dati delle mappe immagine, dovete già aver creato le mappe immagine.

Nella schermata Riepilogo mappe, seguite queste istruzioni per importare i dati della mappa immagine per le mappe immagine create:

1. Selezionare **[!UICONTROL Importa dati mappa]**.
1. Nella finestra di dialogo Importa metadati selezionare **[!UICONTROL Sfoglia]**, quindi selezionare il file DTD XML o delimitato da tabulazioni.
1. Nel campo Nome processo digitare un nome per il file, assicurandosi di mantenere l&#39;estensione.
1. Seleziona **[!UICONTROL Carica]**.

## Copiare mappe immagine tra eCatalog {#copying-image-maps-between-ecatalogs}

Potete copiare tutte le mappe immagine di un eCatalog in un diverso eCatalog. Copiare mappe immagine in questo modo è un metodo per copiare mappe immagine tra versioni localizzate dello stesso eCatalog. Affinché la copia abbia esito positivo, Adobe Dynamic Media Classic consiglia di copiare tra eCatalog con lo stesso numero di pagine e le stesse dimensioni di immagine.

>[!NOTE]
>
>se l’eCatalog in cui copiate le mappe immagine ne contiene già altre, queste ultime verranno sostituite a seguito della copia.

Per copiare tutte le mappe immagine in un eCatalog in un altro, effettuare le seguenti operazioni:

1. Seleziona l&#39;eCatalog con le mappe immagine da copiare, quindi fai clic sul pulsante di rollover **[!UICONTROL Modifica]** dell&#39;eCatalog.
1. Nella scheda Ordina pagine selezionare **[!UICONTROL Copia mappe]**.
1. Nella finestra di dialogo Seleziona risorsa, seleziona l&#39;eCatalog in cui desideri copiare le mappe immagine, quindi seleziona **[!UICONTROL Seleziona]**.

Adobe Dynamic Media Classic visualizza un messaggio di avviso se l’eCatalog di destinazione in cui si copiano le mappe immagine contiene un numero diverso di pagine o immagini di dimensioni diverse. Seleziona **[!UICONTROL Continua]** per copiare le mappe immagine nonostante l&#39;avviso.
