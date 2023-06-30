---
title: Creare mappe immagine
description: Scopri come creare mappe immagine in Adobe Dynamic Media Classic.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '2430'
ht-degree: 49%

---

# Creare mappe immagine {#creating-image-maps}

Una mappa immagine è un’area su un’immagine, una pagina di eCatalog o un’immagine di un set 360 gradi, che visualizza un pannello di rollover con del testo. Quando l’utente seleziona una mappa immagine, viene attivata un’azione di qualche tipo. Ad esempio, può essere avviata una pagina Web contenente ulteriori informazioni su un prodotto. Quando l&#39;utente sposta il puntatore su una mappa immagine, viene visualizzata una struttura.

Oltre alla possibilità di creare mappe immagine in Adobe Dynamic Media Classic, puoi anche creare mappe immagine durante la progettazione di un catalogo in Adobe Acrobat o Adobe InDesign.

Quando create le mappe immagine, potete effettuare una delle seguenti operazioni:

* Immettere testo di rollover.
* Immettere JavaScript e URL per avviare pagine Web.
* Creare modelli URL per le mappe immagine.
* Copiare le mappe immagine in altre immagini, pagine di eCatalog o set 360 gradi.
* Esportare le mappe immagine in CSV o XML.
* Importa i metadati dell&#39;immagine da un file delimitato da tabulazioni o da un file XML.
* Definire altre azioni secondo quanto stabilito dal World Wide Web Consortium.
* Visualizzare l’anteprima delle mappe immagine.

## Disegnare e regolare una mappa immagine {#drawing-and-adjusting-an-image-map}

1. Effettuate una delle seguenti operazioni:

   * Se si utilizza un&#39;immagine nella visualizzazione griglia o nella visualizzazione elenco, nell&#39;elenco a discesa Modifica selezionare **[!UICONTROL Mappa immagine]**. In alternativa, aprirlo in Vista dettagli, quindi selezionare **[!UICONTROL Mappa immagine]** sopra l&#39;immagine.
   * Se utilizzate un set 360 gradi nella vista griglia o nella vista elenco, selezionate **[!UICONTROL Modifica]**. In alternativa, aprirlo in Vista dettagli, quindi selezionare **[!UICONTROL Modifica]**. Seleziona una risorsa di immagine, quindi fai clic su **[!UICONTROL Mappa immagine]**.
   * Se si utilizza un eCatalog, nella visualizzazione griglia, nella visualizzazione elenco, nella visualizzazione dettagli selezionare **[!UICONTROL Modifica]**. Seleziona la **[!UICONTROL Mappa pagine]** scheda.

   ![Immagine mappa immagine](assets/ma_image_map.png)

1. Disegnate una mappa immagine rettangolare o poligonale:

   * **Mappa rettangolare** - Selezionare lo strumento Mappa immagine rettangolo e trascinare sulla pagina per creare il rettangolo. Per aggiungere un punto a una mappa rettangolare (trasformandola in una mappa poligonale), premete Ctrl, quindi posizionate lo strumento di inserimento nella posizione desiderata e selezionate.

   * **Mappa poligonale** - Selezionate lo strumento mappa immagine poligonale (Polygon Image Map) e selezionate i punti sul perimetro dell&#39;area dell&#39;immagine da racchiudere. Usate il cursore di densità del poligono per variare la densità dei punti nel poligono. La densità originale viene ricordata se selezionate altre mappe. Se un punto del poligono viene aggiunto, eliminato o spostato, la densità originale viene perduta e il cursore viene reimpostato sul valore massimo.

1. Se lo desiderate, potete immettere un nome per la mappa immagine nell’elenco Mappa immagine. Dopo aver disegnato una mappa immagine, Adobe Dynamic Media Classic le assegna un nome.

   Per creare il nome, Adobe Dynamic Media Classic aggiunge un numero sequenziale al nome dell&#39;immagine o della pagina eCatalog che si sta utilizzando. Potete immettere un nome di vostra scelta.

1. Se si desidera che gli utenti aprano una nuova pagina Web quando selezionano Mappa immagine, immettere l&#39;URL nell&#39;elenco Mappa immagine.

   Consultate [ per inserire JavaScript e URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Per visualizzare un testo di rollover quando gli utenti passano il puntatore su una mappa immagine, immettete il testo nell’elenco Mappa immagine. Nell&#39;elenco Mappa immagine selezionare **[!UICONTROL Spettacolo]** menu e seleziona **[!UICONTROL Testo di rollover]**. Immettere quindi il testo che si desidera visualizzare sullo schermo. Potete scrivere il testo in un elaboratore testi e copiarlo nel campo di testo Rollover.

1. Per attivare un’altra azione quando gli utenti passano il mouse su una mappa immagine, definite l’azione desiderata. In **[!UICONTROL Spettacolo]** elenco a discesa, seleziona **[!UICONTROL Altre azioni]**. Immettete gli attributi dell’azione. (Vai a **[!UICONTROL Spettacolo]** > **[!UICONTROL Entrambi]** per creare testo di rollover e un&#39;azione per una mappa immagine.)

   Consulta [Definire altre azioni per le mappe immagine](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Facoltativo) Effettuate una o più delle operazioni seguenti:

   * Per visualizzare in anteprima le mappe immagine, seleziona **[!UICONTROL Anteprima]**.
   * Per eliminare una mappa immagine o un vertice di poligono, selezionare una forma nell&#39;immagine, quindi selezionare **[!UICONTROL Elimina]**. In alternativa, per un eCatalog, nella scheda Ordina pagine, selezionare **[!UICONTROL Cancella mappe]** per rimuovere le mappe immagine da tutte le pagine.
   * Per rimuovere temporaneamente una mappa immagine da un’immagine, una pagina di eCatalog o un’immagine di un set 360 gradi senza eliminarla, deselezionate la relativa opzione Attivato nell’elenco Mappa immagine.

1. Seleziona **[!UICONTROL Salva]**.

### Regolare la posizione, la forma e le dimensioni delle mappe immagine {#adjusting-the-position-shape-and-size-of-image-maps}

Per cambiare posizione, forma e dimensione alla mappa immagine, fate clic sul pulsante Mappa immagine . Quindi, seleziona la **[!UICONTROL Panoramica]** e seguire queste istruzioni:

* **Cambia posizione** : sposta il puntatore vicino al bordo della mappa immagine, ma non oltre. Quando viene visualizzata l’icona con la freccia a quattro punte, trascinate la mappa nella nuova posizione.

* **Modificare dimensioni e forma** - La modalità di modifica della forma e delle dimensioni di una mappa immagine dipende dal fatto che si utilizzi una mappa immagine rettangolare o poligonale:

>[!TIP]
>
>Potete trascinare il cursore Dimensione in fondo alla schermata per cambiare le visualizzazioni e avere una visione migliore della mappa immagine.

* **Mappa immagine rettangolare** - Spostare il puntatore su un lato o un angolo della mappa immagine. Quando viene visualizzata l’icona con la freccia a due punte, iniziate a trascinare. Tenete premuto il tasto Maiusc mentre trascinate per cambiare le dimensioni ma mantenere le stesse proporzioni (forma).

* **Mappa immagine poligonale** - Trascinare un punto di manipolazione di selezione quadrato. Per creare un punto di manipolazione di selezione, seleziona il bordo della mappa immagine e inizia a trascinare.

### Gestire le mappe immagine sovrapposte {#handling-overlapping-image-maps}

Se l’immagine o la pagina di eCatalog include più mappe immagine che si sovrappongono, potete gestirne la sovrapposizione cambiando l’ordine delle mappe nell’elenco Mappa immagine. Trascinate i nomi delle mappe verso l’alto o il basso nell’elenco. Le mappe immagine si sovrappongono l’una sull’altra in base all’ordine dei relativi nomi in questo elenco, dall’alto al basso.

### Importare i dati per le mappe immagine {#importing-image-map-data}

Invece di inserire i dati relativi alle mappe immagine in ciascuna pagina, potete importare i dati per l’immagine, il set 360 gradi o l’eCatalog nella schermata Riepilogo mappe. Potete importare i dati delle mappe immagine come un file delimitato da tabulazioni o un file XML DTD. I campi presenti nel file devono essere nell’ordine visualizzato nella schermata Riepilogo mappe: Nome, Etichette di sommario, Mappe, URL, Testo di rollover, Altre azioni e Stringhe di ricerca. Importando i dati delle mappe immagine si evita di dover inserire i dati nell’elenco delle mappe immagine durante la creazione di ciascuna mappa immagine.

**Per importare i dati per le mappe immagine:**

1. Passate alla pagina Editor mappa immagine (per le immagini o le immagini in set 360 gradi) o alla scheda Mappe pagine della schermata di modifica di un eCatalog.
1. Seleziona **[!UICONTROL Importa metadati]**.
1. Nella finestra di dialogo Carica metadati, seleziona Immagine o Mappa immagine per caricare i metadati dal tipo di proprietà della risorsa desiderata.
1. Dall’elenco a discesa Genera file, selezionate il tipo di file da creare.
1. (Facoltativo) Seleziona **[!UICONTROL Genera]** per visualizzare in anteprima i dati risultanti in base al tipo di file da creare. Seleziona **[!UICONTROL Chiudi]** per tornare alla finestra di dialogo Carica metadati.
1. Individuate il file da caricare. Nel campo di testo Nome file, specificate il nome del file generato.
1. (Facoltativo) Nel campo Nome processo, specificate un nome per il processo di caricamento dei metadati.
1. Seleziona **[!UICONTROL Carica]**.

### Copia mappe immagine {#copying-image-maps}

Potete copiare le mappe immagine da un’immagine o una pagina di eCatalog all’altra, Utilizzare **[!UICONTROL Copia mappa immagine]** per iniziare subito a crearli. È inoltre possibile copiare mappe immagine per ricrearle in immagini o pagine che condividono layout o strutture di mappatura.

Ad esempio, può essere utile copiare tutte le mappe immagine di un eCatalog per le versioni nelle diverse lingue dello stesso eCatalog. Per risultati ottimali, si consiglia di copiare tra diversi eCatalog con lo stesso numero di pagine e le stesse immagini. Se l&#39;eCatalog in cui si effettua la copia contiene già mappe immagine, queste ultime vengono eliminate al momento della copia.

**Per copiare le mappe immagine:**

1. Passate alla pagina Editor mappa immagine (per le immagini o le immagini in set 360 gradi) o alla scheda Mappe pagine della schermata di modifica di un eCatalog.
1. Seleziona **[!UICONTROL Copia mappe in]**.
1. Per copiare le mappe immagine da altre immagini o per copiarle da un eCatalog, effettuate una delle seguenti operazioni:

   * (Immagini) Nella schermata Seleziona immagini, selezionate le immagini nelle quali desiderate copiare le mappe immagine.
   * (Immagini) Nella schermata Seleziona risorsa, selezionate le immagini o le pagine eCatalog nelle quali desiderate copiare le mappe immagine.

1. Scegli **[!UICONTROL Seleziona]**.

## Utilizza un modello per immettere JavaScript e URL {#using-a-template-to-enter-javascript-and-urls}

Potete definire un modello URL (detto anche modello Href) per facilitare e migliorare l’immissione degli URL delle mappe immagine. La definizione di un modello URL risulta utile se la maggior parte degli URL della mappa immagine hanno uno stesso formato fisso. Immettendo la parte fissa dell’URL come modello URL non sarà necessario reimmetterla ogni volta che create una mappa immagine. Il modello URL può contenere anche parametri, nomi di percorso e comandi JavaScript. Adobe Dynamic Media Classic Per impostazione predefinita, il modello URL contiene un gestore JavaScript proprietario denominato `loadProduct` che apre l&#39;immagine in una nuova finestra.

>[!NOTE]
>
>Quando si aggiunge il codice JavaScript all&#39;attributo HREF della mappa immagine, il codice viene eseguito sul computer del client. Di conseguenza, assicurati che il codice JavaScript sia sicuro.

### I modelli URL {#about-url-templates}

In un modello URL il contenuto della colonna URL nell’elenco Mappa immagine è sostituito da un doppio simbolo di dollaro (‘$$’):

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Inserisci tutti i valori che non cambiano tra le mappe immagine nel modello URL. Nella colonna URL dell’elenco Mappa immagine vanno invece aggiunti solo i valori che variano da mappa immagine a mappa immagine. Ad esempio:

* Modello URL - `javascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* Valore URL - `product.htm`
* URL effettivo generato - `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Adobe Dynamic Media Classic Per impostazione predefinita, il modello URL include un gestore JavaScript proprietario denominato `loadProduct` che apre una nuova finestra con la destinazione URL. Tuttavia, puoi utilizzare qualsiasi codice JavaScript per sostituire questo gestore JavaScript o uno dei seguenti gestori Adobe Dynamic Media Classic:

* `loadProductCW` - visualizza la destinazione URL specificata nella colonna URL nella finestra corrente. Questo handler è indicato soprattutto per gli eCatalog integrati in una pagina di un sito Web.

* `loadProductPW` - visualizza la destinazione URL specificata nella colonna URL nella finestra principale (la pagina che ha aperto quella corrente). La finestra corrente resta aperta, ma quella principale cambia per visualizzare la destinazione URL.

  >[!NOTE]
  >
  >L’handler `loadProductPW` non supporta i visualizzatori DHTML e HTML5.

### Creare un modello URL {#creating-a-url-template}

1. Nella schermata Editor mappa (per le immagini e i set 360 gradi) o nella scheda Mappe pagine della schermata eCatalog (per gli eCatalog), selezionate Modifica accanto all’opzione Modello URL. Viene visualizzata la finestra di dialogo Modifica modello mappa.
1. Immettete il codice JavaScript e l’URL completo (con la porzione variabile sostituita dai segni di dollaro [$$]). Puoi incollare il codice facendo clic con il pulsante destro del mouse e scegliendo **[!UICONTROL Incolla]**.
1. Seleziona **[!UICONTROL Salva]**.

### Gestire i modelli URL {#handling-url-templates}

La pagina Editor mappa (per le immagini e i set 360 gradi) e la scheda Mappe pagine della schermata eCatalog (per gli eCatalog) offrono i seguenti comandi per gestire i modelli URL:

* **Opzione modello URL** : seleziona l’opzione Modello URL per applicare il modello URL a tutte le mappe immagine su un’immagine o una pagina eCatalog.

* **Opzione modello** : deseleziona un’opzione Modello nell’elenco URL Image Map (Mappa immagine URL) se non desideri che una singola mappa immagine utilizzi il modello URL.

## Definire altre azioni per le mappe immagine {#defining-other-actions-for-image-maps}

È possibile selezionare **[!UICONTROL Spettacolo]** e scegliere **[!UICONTROL Altre azioni]** per attivare azioni diverse dal rollover di testo e dagli avvii di pagine web. Potete fare sì che un’azione venga avviata quando l’utente passa il puntatore su una mappa immagine. Queste azioni sono attributi definiti per le mappe immagine sul lato client dalle specifiche HTML del World Wide Web Consortium. Includono:

* **`accesskey`** - Attiva un’azione quando l’utente preme un determinato tasto della tastiera.

* **`onfocus`** - Attiva un evento quando la mappa immagine viene attivata dal cursore, dalla tabulazione o premendo un tasto di accesso. Ad esempio, è possibile avviare una pagina Web quando la mappa immagine viene resa attiva e chiuderla quando la mappa è resa inattiva.

* **`onblur`** - Attiva un evento quando la mappa immagine viene resa inattiva tramite cursore o tasto di tabulazione.

**Per definire altre azioni per le mappe immagine:**

1. Nella schermata Map Editor (immagini e set 360 gradi) o Map Pages (Mappa pagine) della schermata eCatalog (eCatalog), seleziona la **[!UICONTROL Spettacolo]** menu e seleziona **[!UICONTROL Altre azioni]**.
1. Usando la sintassi indicata dalle specifiche HTML del World Wide Web Consortium, aggiungete gli attributi supportati nella colonna Altre azioni dell’elenco Mappa immagine.
1. Seleziona **[!UICONTROL Salva]**.

Seleziona la **[!UICONTROL Spettacolo]** menu e seleziona **[!UICONTROL Entrambi]** se desideri che una mappa immagine contenga testo di rollover e un’azione.

## Creare mappe immagine in Adobe Acrobat o Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Potete creare le mappe immagine mentre create un eCatalog in Adobe Acrobat o Adobe InDesign.

In Adobe Acrobat o Adobe InDesign, crea i riferimenti ai collegamenti ipertestuali nel punto in cui desideri visualizzare le mappe immagine e specifica le posizioni URL per la mappa immagine. Selezionando l’opzione Estrai collegamenti durante il caricamento del file PDF in Adobe Dynamic Media Classic, i collegamenti vengono automaticamente convertiti in mappe immagine.

Per ulteriori informazioni, consulta la Guida di Adobe InDesign o Adobe Acrobat.

### Per creare mappe immagine in Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. In Adobe InDesign, vai a **[!UICONTROL Windows®]** > **[!UICONTROL Interattiva]** > **[!UICONTROL Collegamenti ipertestuali]**.
1. Nel pannello Collegamenti ipertestuali, selezionate il testo, la cornice o l&#39;elemento grafico da trasformare in una mappa immagine.
1. Seleziona **[!UICONTROL Nuovo collegamento ipertestuale]** dal menu del pannello.
1. Nella finestra di dialogo Nuovo collegamento ipertestuale, da **[!UICONTROL Collega a]** menu, scegliere **[!UICONTROL URL]**.
1. Digita o incolla l’ID prodotto nella casella URL.
1. Seleziona **[!UICONTROL OK]**. (Adobe Dynamic Media Classic completa l’URL utilizzando il modello URL della mappa immagine).

   >[!NOTE]
   >
   >Non è necessario impostare le opzioni di aspetto in Adobe InDesign. È possibile specificare l&#39;aspetto in Adobe Dynamic Media Classic.

1. Ripetete i passaggi da 2 a 6 per tutte le mappe immagine da creare.
1. Esportate il file come PDF.
1. Carica il PDF in Adobe Dynamic Media Classic.
1. In entrata **[!UICONTROL Opzioni PDF]**, seleziona **[!UICONTROL Estrai collegamenti]**.

### Per creare mappe immagine in Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. In Adobe Acrobat, vai a **[!UICONTROL Strumenti]** > **[!UICONTROL Modifica avanzata]** > **[!UICONTROL Strumento Collega]**.
1. Trascinate per creare la mappa immagine.
1. Nella casella Crea collegamento, seleziona **[!UICONTROL Collegamento personalizzato]**, e seleziona **[!UICONTROL Successivo]**.

>[!NOTE]
>
>Non è necessario impostare le opzioni di aspetto in Adobe Acrobat. È possibile specificare l&#39;aspetto in Adobe Dynamic Media Classic.

1. Nella casella Proprietà collegamento, seleziona **[!UICONTROL Azioni]**.
1. Seleziona **[!UICONTROL Apri Un Collegamento Web]** dal menu Seleziona azione, quindi selezionare **[!UICONTROL Aggiungi]**.
1. Digita l’ID prodotto per la mappa immagine nella casella Modifica URL e seleziona **[!UICONTROL OK]**. (Adobe Dynamic Media Classic completa l’URL utilizzando il modello URL della mappa immagine).
1. Ripetete i passaggi da 1 a 7 per tutte le mappe immagine da creare.
1. Salvate il file.
1. Carica il PDF in Adobe Dynamic Media Classic e seleziona Estrai collegamenti dalle opzioni PDF.
