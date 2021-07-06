---
title: Creazione di mappe immagine
description: Scopri come creare mappe immagine.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Gestione risorse
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '2427'
ht-degree: 62%

---

# Creazione di mappe immagine{#creating-image-maps}

Una mappa immagine è un’area su un’immagine, una pagina di eCatalog o un’immagine di un set 360 gradi, che visualizza un pannello di rollover con del testo. Quando l’utente fa clic su una mappa immagine, viene attivata un’azione. Ad esempio, può essere avviata una pagina Web contenente ulteriori informazioni su un prodotto. Quando l’utente sposta il puntatore su una mappa immagine, viene visualizzato un contorno intorno a una mappa immagine.

Oltre alla possibilità di creare mappe immagine in Dynamic Media Classic, puoi anche creare mappe immagine quando progetti un catalogo in Adobe Acrobat o Adobe InDesign.

Quando create le mappe immagine, potete effettuare una delle seguenti operazioni:

* Immettere testo di rollover.
* Immetti JavaScript™ e gli URL per l&#39;avvio di pagine web.
* Creare modelli URL per le mappe immagine.
* Copiare le mappe immagine in altre immagini, pagine di eCatalog o set 360 gradi.
* Esportare le mappe immagine in CSV o XML.
* Importa metadati immagine da un file delimitato da tabulazioni o da un file XML.
* Definire altre azioni secondo quanto stabilito dal World Wide Web Consortium.
* Visualizzare l’anteprima delle mappe immagine.

## Disegno e regolazione di una mappa immagine {#drawing-and-adjusting-an-image-map}

1. Effettuate una delle seguenti operazioni:

   * Se si lavora con un&#39;immagine nella Vista a griglia o nella Vista a elenco, nell&#39;elenco a discesa Modifica fare clic su **Mappa immagine**. In alternativa, aprilo in Vista dettagli e fai clic su **Mappa immagine** sopra l&#39;immagine.
   * Se si utilizza un Set 360 gradi nella visualizzazione Griglia o Elenco, fare clic su **Modifica**. In alternativa, aprilo in Vista dettagli e fai clic su **Modifica**. Seleziona una risorsa immagine, quindi fai clic su **Mappa immagine**.
   * Se si utilizza un eCatalog, in Vista griglia, Vista elenco, Vista dettagli fare clic su **Modifica**. Fai clic sulla scheda **Mappa pagine** .

   ![](assets/ma_image_map.png)

1. Disegnate una mappa immagine rettangolare o poligonale:

   **Mappa rettangolareSeleziona lo strumento Mappa immagine rettangolare e trascina sulla pagina per creare il rettangolo.** Per aggiungere un punto a una mappa rettangolare (facendola così diventare una mappa poligonale), premete Ctrl, quindi portate lo strumento di inserimento nella posizione desiderata e fate clic.

   **Mappa poligonaleSelezionate lo strumento Mappa immagine poligonale e fate clic sui punti sul perimetro dell&#39;area dell&#39;immagine che desiderate racchiudere.** Usate il cursore di densità del poligono per variare la densità dei punti nel poligono. La densità originale viene ricordata se selezionate altre mappe. Se un punto del poligono viene aggiunto, eliminato o spostato, la densità originale viene perduta e il cursore viene reimpostato sul valore massimo.

1. Se lo desiderate, potete immettere un nome per la mappa immagine nell’elenco Mappa immagine. Dopo aver disegnato una mappa immagine, Dynamic Media Classic le assegna un nome.

   Per creare il nome, Dynamic Media Classic aggiunge un numero sequenziale al nome dell&#39;immagine o della pagina eCatalog con cui si sta lavorando. Potete immettere un nome di vostra scelta.

1. Se volete che venga aperta una nuova pagina Web quando gli utenti fanno clic sulla mappa immagine, immettete l’URL nell’elenco Mappa immagine. 

   Consulta [per inserire JavaScript™ e URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Per visualizzare un testo di rollover quando gli utenti passano il puntatore su una mappa immagine, immettete il testo nell’elenco Mappa immagine. Nell’elenco Mappa immagine, selezionate il menu Mostra e scegliete Testo di rollover. A questo punto, immettete il testo che verrà presentato agli utenti. Potete scrivere il testo in un elaboratore testi e copiarlo nel campo di testo Rollover.
1. Per attivare un’altra azione quando gli utenti passano il mouse su una mappa immagine, definite l’azione desiderata. Nell’elenco a discesa Mostra, fate clic su Altre azioni. Immettete gli attributi dell’azione. Per creare sia un testo di rollover che un’azione per una mappa immagine, fate clic su Mostra > Entrambi.

   Consultate [Definizione di altre azioni per le mappe immagine](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Facoltativo) Effettuate una o più delle operazioni seguenti:

   * Per visualizzare in anteprima le mappe immagine, fai clic su **[!UICONTROL Anteprima]**.
   * Per eliminare una mappa immagine o un vertice poligonale, selezionare una forma sull&#39;immagine, quindi fare clic su **[!UICONTROL Elimina]**. Oppure, per un eCatalog, nella scheda Pagine ordine fai clic su **[!UICONTROL Cancella mappe]** per rimuovere le mappe immagine da tutte le pagine.
   * Per rimuovere temporaneamente una mappa immagine da un’immagine, una pagina di eCatalog o un’immagine di un set 360 gradi senza eliminarla, deselezionate la relativa opzione Attivato nell’elenco Mappa immagine.

1. Fate clic su **[!UICONTROL Salva]**.

### Regolazione della posizione, forma e dimensione delle mappe immagine {#adjusting-the-position-shape-and-size-of-image-maps}

Per cambiare posizione, forma e dimensione alla mappa immagine, fate clic sul pulsante Mappa immagine . Quindi, seleziona lo strumento **[!UICONTROL Pan]** e segui queste istruzioni:

**Modifica della posizione** : sposta il puntatore vicino al bordo della mappa immagine ma non sopra di esso. Quando viene visualizzata l’icona con la freccia a quattro punte, trascinate la mappa nella nuova posizione.

**Modifica delle dimensioni e della forma**  - La modalità di modifica della forma e delle dimensioni di una mappa immagine dipende dal fatto che si stia utilizzando una mappa immagine rettangolare o poligonale:

>[!TIP]
>
>Potete trascinare il cursore Dimensione in fondo alla schermata per cambiare le visualizzazioni e avere una visione migliore della mappa immagine.

**Mappa immagine rettangolare** : sposta il puntatore su un lato o un angolo della mappa immagine. Quando viene visualizzata l’icona con la freccia a due punte, iniziate a trascinare. Tenete premuto il tasto Maiusc mentre trascinate per cambiare le dimensioni ma mantenere le stesse proporzioni (forma).

**Mappa immagine poligonale** : consente di trascinare una maniglia di selezione quadrata. Per creare una maniglia di selezione, fate clic sul bordo della mappa immagine e iniziate a trascinare.

### Gestione delle mappe immagine sovrapposte {#handling-overlapping-image-maps}

Se l’immagine o la pagina di eCatalog include più mappe immagine che si sovrappongono, potete gestirne la sovrapposizione cambiando l’ordine delle mappe nell’elenco Mappa immagine. Trascinate i nomi delle mappe verso l’alto o il basso nell’elenco. Le mappe immagine si sovrappongono l’una sull’altra in base all’ordine dei relativi nomi in questo elenco, dall’alto al basso.

### Importazione di dati per le mappe immagine {#importing-image-map-data}

Invece di inserire i dati relativi alle mappe immagine in ciascuna pagina, potete importare i dati per l’immagine, il set 360 gradi o l’eCatalog nella schermata Riepilogo mappe. Potete importare i dati delle mappe immagine come un file delimitato da tabulazioni o un file XML DTD. I campi presenti nel file devono essere nell’ordine visualizzato nella schermata Riepilogo mappe: Nome, Etichette di sommario, Mappe, URL, Testo di rollover, Altre azioni e Stringhe di ricerca. Importando i dati delle mappe immagine si evita di dover inserire i dati nell’elenco delle mappe immagine durante la creazione di ciascuna mappa immagine.

**Per importare i dati per le mappe immagine**

1. Passate alla pagina Editor mappa immagine (per le immagini o le immagini in set 360 gradi) o alla scheda Mappe pagine della schermata di modifica di un eCatalog.
1. Fate clic su Importa metadati.
1. Nella finestra di dialogo Carica metadati, fate clic su Immagine o Mappa immagine per caricare metadati dal tipo di proprietà desiderato.
1. Dall’elenco a discesa Genera file, selezionate il tipo di file da creare.
1. (Facoltativo) Fate clic su Genera per visualizzare un’anteprima dei dati risultanti in base al tipo di file che si desidera creare. Fate clic su Chiudi per tornare alla finestra di dialogo Carica metadati.
1. Individuate il file da caricare. Nel campo di testo Nome file, specificate il nome del file generato.
1. (Facoltativo) Nel campo Nome processo, specificate un nome per il processo di caricamento dei metadati.
1. Fate clic su Carica.

### Copia delle mappe immagine {#copying-image-maps}

Potete copiare le mappe immagine da un’immagine o una pagina di eCatalog all’altra, Utilizza **[!UICONTROL Copia mappa immagine]** per ottenere un primo inizio nella creazione di tali immagini. o per ricrearle in immagini o pagine che condividono lo stesso layout o la stessa struttura di mappatura. 

Ad esempio, può essere utile copiare tutte le mappe immagine di un eCatalog per le versioni nelle diverse lingue dello stesso eCatalog. Per risultati ottimali, si consiglia di copiare tra diversi eCatalog con lo stesso numero di pagine e le stesse immagini. Se l’eCatalog in cui copiate contiene già delle mappe immagine, queste vengono eliminate quando create la copia.

**Per copiare le mappe immagine**

1. Passate alla pagina Editor mappa immagine (per le immagini o le immagini in set 360 gradi) o alla scheda Mappe pagine della schermata di modifica di un eCatalog.
1. Fate clic su Copia mappe in.
1. Per copiare le mappe immagine da altre immagini o per copiarle da un eCatalog, effettuate una delle seguenti operazioni:

   * (Immagini) Nella schermata Seleziona immagini, selezionate le immagini nelle quali desiderate copiare le mappe immagine.
   * (Immagini) Nella schermata Seleziona risorsa, selezionate le immagini o le pagine eCatalog nelle quali desiderate copiare le mappe immagine.

1. Fate clic su Seleziona.

## Utilizzo di un modello per immettere JavaScript™ e URL {#using-a-template-to-enter-javascript-and-urls}

Potete definire un modello URL (detto anche modello Href) per facilitare e migliorare l’immissione degli URL delle mappe immagine. La definizione di un modello URL risulta utile se la maggior parte degli URL della mappa immagine hanno uno stesso formato fisso. Immettendo la parte fissa dell’URL come modello URL non sarà necessario reimmetterla ogni volta che create una mappa immagine. Il modello URL può anche contenere comandi, nomi percorso e parametri JavaScript™. Per impostazione predefinita, il modello URL contiene un gestore JavaScript™ proprietario di Dynamic Media Classic denominato `loadProduct` che apre l’immagine in una nuova finestra.

>[!NOTE]
>
>Quando si aggiunge il codice JavaScript™ all&#39;attributo HREF della mappa immagine, il codice viene eseguito sul computer del client. Assicurati pertanto che il codice JavaScript™ sia sicuro.

### I modelli URL {#about-url-templates}

In un modello URL il contenuto della colonna URL nell’elenco Mappa immagine è sostituito da un doppio simbolo di dollaro (‘$$’):

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Inserisci tutti i valori che non cambiano tra le mappe immagine nel modello URL. Nella colonna URL dell’elenco Mappa immagine vanno invece aggiunti solo i valori che variano da mappa immagine a mappa immagine. Ad esempio:

* Modello URL: j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* Valore URL: `product.htm`
* URL effettivo generato: `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Per impostazione predefinita, il modello URL include un gestore JavaScript™ proprietario di Dynamic Media Classic denominato `loadProduct` che apre una nuova finestra con la destinazione URL. Tuttavia, è possibile utilizzare qualsiasi codice JavaScript™ per sostituire questo gestore JavaScript™ o utilizzare uno dei seguenti gestori Dynamic Media Classic:

* `loadProductCW`

   visualizza la destinazione URL specificata nella colonna URL nella finestra corrente. Questo handler è indicato soprattutto per gli eCatalog integrati in una pagina di un sito Web.

* `loadProductPW`

   visualizza la destinazione URL specificata nella colonna URL nella finestra principale (la pagina che ha aperto quella corrente). La finestra corrente resta aperta, ma quella principale cambia per visualizzare la destinazione URL.

   >[!NOTE]
   >
   >L’handler `loadProductPW` non supporta i visualizzatori DHTML e HTML5.

### Creazione di un modello URL {#creating-a-url-template}

Per creare un modello URL:

1. Nella schermata Editor mappa (per le immagini e i set 360 gradi) o nella scheda Mappe pagine della schermata eCatalog (per gli eCatalog), selezionate Modifica accanto all’opzione Modello URL. Viene visualizzata la finestra di dialogo Modifica modello mappa.
1. Immetti il codice JavaScript™ e l&#39;URL completo (con la porzione di variabile sostituita dal simbolo del dollaro [$]). Potete incollare il codice facendo clic con il pulsante destro del mouse e scegliendo Incolla.
1. Fate clic sul pulsante Salva.

### Gestione dei modelli URL {#handling-url-templates}

La pagina Editor mappa (per le immagini e i set 360 gradi) e la scheda Mappe pagine della schermata eCatalog (per gli eCatalog) offrono i seguenti comandi per gestire i modelli URL:

* **Opzione** Modello URLSeleziona l’opzione Modello URL per applicare il modello URL a tutte le mappe immagine di un’immagine o di una pagina di eCatalog.

* **Opzione** ModelloDeseleziona un’opzione Modello nell’elenco URL mappa immagine se non desideri che una singola mappa immagine utilizzi il modello URL.

## Definizione di altre azioni per le mappe immagine {#defining-other-actions-for-image-maps}

Per attivare azioni diverse dal testo di rollover o dall’avvio di pagine Web, scegliete Altre azioni dal menu Mostra. Potete fare sì che un’azione venga avviata quando l’utente passa il puntatore su una mappa immagine. Queste azioni sono attributi definiti per le mappe immagine sul lato client dalle specifiche HTML del World Wide Web Consortium. Includono:

* **accesskey** : attiva un’azione quando l’utente preme un tasto designato sulla tastiera.

* **onfocus**  - Attiva un evento quando la mappa immagine diventa attiva, tramite il cursore, la tabulazione o premendo un tasto di accesso. Ad esempio, è possibile avviare una pagina Web quando la mappa immagine viene resa attiva e chiuderla quando la mappa è resa inattiva.

* **onblur** : attiva un evento quando la mappa immagine diventa inattiva, tramite il cursore o con il tasto di tabulazione.

**Per definire altre azioni per le mappe immagine:**

1. Nella schermata Editor mappa (per le immagini e i set 360 gradi) o nella scheda Mappe pagine della schermata eCatalog (per gli eCatalog), scegliete Altre azioni dal menu Mostra.
1. Usando la sintassi indicata dalle specifiche HTML del World Wide Web Consortium, aggiungete gli attributi supportati nella colonna Altre azioni dell’elenco Mappa immagine.
1. Fate clic su **[!UICONTROL Salva]**.

Seleziona il menu **[!UICONTROL Mostra]** e scegli **[!UICONTROL Entrambi]** se desideri che una mappa immagine includa testo di rollover e un’azione.

## Creazione di mappe immagine in Adobe Acrobat o Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Potete creare le mappe immagine mentre create un eCatalog in Adobe Acrobat o Adobe InDesign.

In Acrobat o InDesign, inserite i riferimenti ipertestuali in corrispondenza delle mappe immagine desiderate e specificate i percorsi URL per le mappe immagine. Quando si seleziona l’opzione Estrai collegamenti durante il caricamento del file PDF in Dynamic Media Classic, i collegamenti vengono automaticamente convertiti in mappe immagine.

Per ulteriori informazioni, consulta la Guida di Adobe InDesign o la Guida di Adobe Acrobat.

### Per creare mappe immagine in Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. In InDesign, fai clic su **[!UICONTROL Windows®]** > **[!UICONTROL Interattivo]** > **[!UICONTROL Collegamenti ipertestuali]** per aprire il pannello Collegamenti ipertestuali.
1. Selezionate il testo, la cornice o l’elemento grafico da convertire in mappa immagine.
1. Nel pannello Collegamenti ipertestuali, fate clic su **[!UICONTROL Nuovo collegamento ipertestuale]** nel menu del pannello.
1. Nella finestra di dialogo Nuovo collegamento ipertestuale, scegliere **[!UICONTROL URL]** dal menu Collega a.
1. Digita o incolla l&#39;ID prodotto nella casella URL e fai clic su **[!UICONTROL OK]**. (Dynamic Media Classic completa l’URL utilizzando il modello URL della mappa immagine.)

   >[!NOTE]
   >
   >Non è necessario impostare le opzioni di aspetto in Adobe InDesign. Puoi specificare l’aspetto in Dynamic Media Classic.

1. Ripetete i passaggi da 2 a 5 per tutte le mappe immagine da creare.
1. Esportate il file come PDF.
1. Carica il PDF in Dynamic Media Classic e seleziona Estrai collegamenti dalle opzioni PDF.

### Per creare mappe immagine in Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. In Acrobat, fai clic su **[!UICONTROL Strumenti]** > **[!UICONTROL Modifica avanzata]** > **[!UICONTROL Strumento di collegamento]**.
1. Trascinate per creare la mappa immagine. Viene visualizzata la finestra Crea link.
1. Seleziona **[!UICONTROL Collegamento personalizzato]**, quindi fai clic su **[!UICONTROL Avanti]**.

>[!NOTE]
>
>Non è necessario impostare le opzioni di aspetto in Adobe Acrobat. Puoi specificare l’aspetto in Dynamic Media Classic.

1. Nella casella Proprietà collegamento fare clic su **[!UICONTROL Azioni]**.
1. Selezionare **[!UICONTROL Apri un collegamento web]** dal menu Seleziona azione, quindi fare clic su **[!UICONTROL Aggiungi]**.
1. Digita l&#39;ID prodotto per la mappa immagine nella casella Modifica URL e fai clic su **[!UICONTROL OK]**. (Dynamic Media Classic completa l&#39;URL utilizzando il modello URL della mappa immagine.)
1. Ripetete i passaggi da 1 a 7 per tutte le mappe immagine da creare.
1. Salvate il file.
1. Carica il PDF in Dynamic Media Classic e seleziona Estrai collegamenti dalle opzioni PDF.
