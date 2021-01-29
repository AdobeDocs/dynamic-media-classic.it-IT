---
title: Creazione di mappe immagine
description: Scopri come creare mappe immagine.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '2440'
ht-degree: 75%

---


# Creazione di mappe immagine{#creating-image-maps}

Una mappa immagine è un’area su un’immagine, una pagina di eCatalog o un’immagine di un set 360 gradi, che visualizza un pannello di rollover con del testo. Quando l’utente fa clic su una mappa immagine, viene attivata un’azione. Ad esempio, può essere avviata una pagina Web contenente ulteriori informazioni su un prodotto. Per richiamare l’attenzione su queste mappe, la mappa immagine viene delineata da un contorno quando l’utente ci passa sopra con il puntatore del mouse.

Oltre alla possibilità di creare una mappa immagine in Dynamic Media Classic, potete anche creare mappe immagine quando progettate un catalogo in  Adobe Acrobat o  Adobe InDesign.

Quando create le mappe immagine potete effettuare le seguenti operazioni:

* Immettere testo di rollover.
* Immettere JavaScript e URL per avviare pagine Web.
* Creare modelli URL per le mappe immagine.
* Copiare le mappe immagine in altre immagini, pagine di eCatalog o set 360 gradi.
* Esportare le mappe immagine in CSV o XML.
* Importare i metadati immagine da un file delimitato da tabulazioni o XML.
* Definire altre azioni secondo quanto stabilito dal World Wide Web Consortium.
* Visualizzare l’anteprima delle mappe immagine.

## Disegno e regolazione di una mappa immagine  {#drawing-and-adjusting-an-image-map}

1. Effettuate una delle seguenti operazioni:

   * Se state lavorando con un’immagine in visualizzazione Griglia o Elenco, fate clic su **Mappa immagine** nell’elenco a discesa Modifica. In alternativa, apritela in visualizzazione Dettagli e fate clic su **Mappa immagine** sopra l’immagine.
   * Se state lavorando con un set 360 gradi in visualizzazione Griglia o Elenco, fate clic su **Modifica**. In alternativa, apritela in visualizzazione Dettagli e fate clic su **Modifica**. Selezionate una risorsa immagine, quindi fate clic su **Mappa immagine**.
   * Se state lavorando con un eCatalog, in visualizzazione Griglia, Elenco e Dettagli fate clic su **Modifica**. Fare clic sulla scheda **Mappe pagine**.

   ![](assets/ma_image_map.png)

1. Disegnate una mappa immagine rettangolare o poligonale:

   **Mappa rettangolare:** selezionate lo strumento rettangolo per mappe immagine e trascinate sulla pagina per creare il rettangolo. Per aggiungere un punto a una mappa rettangolare (facendola così diventare una mappa poligonale), premete Ctrl, quindi portate lo strumento di inserimento nella posizione desiderata e fate clic.

   **Mappa poligonale:** selezionate lo strumento poligono per mappe immagine e fate clic sui punti del perimetro dell’area dell’immagine da includere. Usate il cursore di densità del poligono per variare la densità dei punti nel poligono. La densità originale viene ricordata se selezionate altre mappe. Se un punto del poligono viene aggiunto, eliminato o spostato, la densità originale viene perduta e il cursore viene reimpostato sul valore massimo.

1. Se lo desiderate, potete immettere un nome per la mappa immagine nell’elenco Mappa immagine. Dopo aver disegnato una mappa immagine, Dynamic Media Classic le assegna un nome.

   Per creare il nome, Dynamic Media Classic aggiunge un numero sequenziale al nome dell’immagine o della pagina di eCatalog con cui state lavorando. Potete immettere un nome di vostra scelta.

1. Se volete che venga aperta una nuova pagina Web quando gli utenti fanno clic sulla mappa immagine, immettete l’URL nell’elenco Mappa immagine. 

   Consultate [ per inserire JavaScript e URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Per visualizzare un testo di rollover quando gli utenti passano il puntatore su una mappa immagine, immettete il testo nell’elenco Mappa immagine. Nell’elenco Mappa immagine, selezionate il menu Mostra e scegliete Testo di rollover. A questo punto, immettete il testo che verrà presentato agli utenti. Potete scrivere il testo in un elaboratore testi e copiarlo nel campo di testo Rollover.
1. Per attivare un’altra azione quando gli utenti passano il mouse su una mappa immagine, definite l’azione desiderata. Nell’elenco a discesa Mostra, fate clic su Altre azioni. Immettete gli attributi dell’azione. Per creare sia un testo di rollover che un’azione per una mappa immagine, fate clic su Mostra > Entrambi.

   Consultate [Definizione di altre azioni per le mappe immagine](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Facoltativo) Effettuate una o più delle operazioni seguenti:

   * Fate clic su Anteprima per vedere in anteprima le mappe immagine.
   * Per eliminare un vertice della mappa immagine o del poligono, selezionate una forma sull’immagine e fate clic su Elimina. Oppure, per un eCatalog, nella scheda Ordina pagine, fate clic su Cancella mappe per rimuovere le mappe immagine da tutte le pagine.
   * Per rimuovere temporaneamente una mappa immagine da un’immagine, una pagina di eCatalog o un’immagine di un set 360 gradi senza eliminarla, deselezionate la relativa opzione Attivato nell’elenco Mappa immagine.

1. Fate clic su Salva.

### Regolazione della posizione, forma e dimensione delle mappe immagine  {#adjusting-the-position-shape-and-size-of-image-maps}

Per cambiare posizione, forma e dimensione alla mappa immagine, fate clic sul pulsante Mappa immagine . Selezionate quindi lo strumento scorrimento e seguite le istruzioni seguenti:

**Modifica della** posizioneSpostate il puntatore accanto ma non sopra il bordo della mappa immagine. Quando viene visualizzata l’icona con la freccia a quattro punte, trascinate la mappa nella nuova posizione.

**Modifica delle dimensioni e della** formaLa modalità di modifica della forma e delle dimensioni di una mappa immagine dipende dal tipo di mappa immagine (rettangolare o poligonale) in uso:

***Suggerimento **: Potete trascinare il cursore Dimensione nella parte inferiore della schermata per cambiare le viste e ottenere un’immagine migliore della mappa immagine.*

**Mappa** immagine rettangolare: portate il puntatore su un lato o un angolo della mappa immagine. Quando viene visualizzata l’icona con la freccia a due punte, iniziate a trascinare. Tenete premuto il tasto Maiusc mentre trascinate per cambiare le dimensioni ma mantenere le stesse proporzioni (forma).

**Mappa immagine poligonale:** trascinate una maniglia di selezione quadrata. Per creare una maniglia di selezione, fate clic sul bordo della mappa immagine e iniziate a trascinare.

### Gestione delle mappe immagine sovrapposte {#handling-overlapping-image-maps}

Se l’immagine o la pagina di eCatalog include più mappe immagine che si sovrappongono, potete gestirne la sovrapposizione cambiando l’ordine delle mappe nell’elenco Mappa immagine. Trascinate i nomi delle mappe verso l’alto o il basso nell’elenco. Le mappe immagine si sovrappongono l’una sull’altra in base all’ordine dei relativi nomi in questo elenco, dall’alto al basso.

### Importazione di dati per le mappe immagine  {#importing-image-map-data}

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

### Copia delle mappe immagine  {#copying-image-maps}

Potete copiare le mappe immagine da un’immagine o una pagina di eCatalog all’altra, per facilitare la creazione di nuove mappe immagine o per ricrearle in immagini o pagine che condividono lo stesso layout o la stessa struttura di mappatura. 

Ad esempio, può essere utile copiare tutte le mappe immagine di un eCatalog per le versioni nelle diverse lingue dello stesso eCatalog. Per risultati ottimali, si consiglia di copiare tra diversi eCatalog con lo stesso numero di pagine e le stesse immagini. Se l’eCatalog in cui copiate le mappe immagine ne contiene già altre, queste ultime verranno sostituite a seguito della copia.

**Per copiare le mappe immagine**

1. Passate alla pagina Editor mappa immagine (per le immagini o le immagini in set 360 gradi) o alla scheda Mappe pagine della schermata di modifica di un eCatalog.
1. Fate clic su Copia mappe in.
1. Per copiare le mappe immagine da altre immagini o per copiarle da un eCatalog, effettuate una delle seguenti operazioni:

   * (Immagini) Nella schermata Seleziona immagini, selezionate le immagini nelle quali desiderate copiare le mappe immagine.
   * (Immagini) Nella schermata Seleziona risorsa, selezionate le immagini o le pagine eCatalog nelle quali desiderate copiare le mappe immagine.

1. Fate clic su Seleziona.

## Utilizzo di un modello per inserire JavaScript e URL  {#using-a-template-to-enter-javascript-and-urls}

Potete definire un modello URL (detto anche modello Href) per facilitare e migliorare l’immissione degli URL delle mappe immagine. La definizione di un modello URL risulta utile se la maggior parte degli URL della mappa immagine hanno uno stesso formato fisso. Immettendo la parte fissa dell’URL come modello URL non sarà necessario reimmetterla ogni volta che create una mappa immagine. Il modello URL può contenere anche parametri, nomi di percorso e comandi JavaScript. Per impostazione predefinita, il modello URL contiene un handler JavaScript proprietario di Dynamic Media Classic denominato `loadProduct` che apre l&#39;immagine in una nuova finestra.

>[!NOTE]
>
>Tenete presente che quando aggiungete il codice JavaScript nell’attributo HREF della mappa immagine, il codice viene eseguito sul computer client. Accertatevi quindi che il codice JavaScript sia sicuro.

### I modelli URL  {#about-url-templates}

In un modello URL il contenuto della colonna URL nell’elenco Mappa immagine è sostituito da un doppio simbolo di dollaro (‘$$’):

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Nel modello URL vanno inseriti tutti i valori che restano invariati nelle diverse mappe immagine. Nella colonna URL dell’elenco Mappa immagine vanno invece aggiunti solo i valori che variano da mappa immagine a mappa immagine. Ad esempio:

* Modello URL: j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* Valore URL: `product.htm`
* URL effettivo generato: `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Per impostazione predefinita, il modello URL include un handler JavaScript proprietario di Dynamic Media Classic denominato `loadProduct` che apre una nuova finestra con la destinazione URL. Tuttavia, è possibile utilizzare qualsiasi codice JavaScript per sostituire questo handler JavaScript o utilizzare uno dei seguenti handler Dynamic Media Classic:

* `loadProductCW`

   visualizza la destinazione URL specificata nella colonna URL nella finestra corrente. Questo handler è indicato soprattutto per gli eCatalog integrati in una pagina di un sito Web.

* `loadProductPW`

   visualizza la destinazione URL specificata nella colonna URL nella finestra principale (la pagina che ha aperto quella corrente). La finestra corrente resta aperta, ma quella principale cambia per visualizzare la destinazione URL.

   ***nota **: Il gestore  `loadProductPW` non supporta i visualizzatori DHTML e HTML5.*

### Creazione di un modello URL {#creating-a-url-template}

Per creare un modello URL:

1. Nella schermata Editor mappa (per le immagini e i set 360 gradi) o nella scheda Mappe pagine della schermata eCatalog (per gli eCatalog), selezionate Modifica accanto all’opzione Modello URL. Viene visualizzata la finestra di dialogo Modifica modello mappa.
1. Immettete il codice JavaScript e l’URL completo (con la porzione variabile sostituita dai segni di dollaro [$$]). Potete incollare il codice facendo clic con il pulsante destro del mouse e scegliendo Incolla.
1. Fate clic sul pulsante Salva.

### Gestione dei modelli URL  {#handling-url-templates}

La pagina Editor mappa (per le immagini e i set 360 gradi) e la scheda Mappe pagine della schermata eCatalog (per gli eCatalog) offrono i seguenti comandi per gestire i modelli URL:

**Opzione Modello URL:** selezionate l’opzione Modello URL per applicare il modello URL a tutte le mappe immagine di un’immagine o di una pagina di eCatalog.

**Opzione Modello:** Deselezionate un’opzione Modello nell’elenco Mappa immagine URL se non desiderate che il modello URL sia utilizzato da una singola mappa immagine.

## Definizione di altre azioni per le mappe immagine {#defining-other-actions-for-image-maps}

Per attivare azioni diverse dal testo di rollover o dall’avvio di pagine Web, scegliete Altre azioni dal menu Mostra. Potete fare sì che un’azione venga avviata quando l’utente passa il puntatore su una mappa immagine. Queste azioni sono attributi definiti per le mappe immagine sul lato client dalle specifiche HTML del World Wide Web Consortium. Includono:

**tasto di** accessoAttiva un&#39;azione quando l&#39;utente preme un tasto designato sulla tastiera.

**** onfocusAttiva un evento quando la mappa immagine viene resa attiva (tramite cursore, tasto di tabulazione o tasto di accesso). Ad esempio, è possibile avviare una pagina Web quando la mappa immagine viene resa attiva e chiuderla quando la mappa è resa inattiva.

**** onblurAttiva un evento quando la mappa immagine perde lo stato attivo, tramite cursore o tasto di tabulazione.

**Per definire altre azioni per le mappe immagine**

1. Nella schermata Editor mappa (per le immagini e i set 360 gradi) o nella scheda Mappe pagine della schermata eCatalog (per gli eCatalog), scegliete Altre azioni dal menu Mostra.
1. Usando la sintassi indicata dalle specifiche HTML del World Wide Web Consortium, aggiungete gli attributi supportati nella colonna Altre azioni dell’elenco Mappa immagine.
1. Fate clic su **Salva**.

Per associare una mappa immagine sia a un testo di rollover che a un’azione, scegliete Entrambi dal menu Mostra.

## Creazione di mappe immagine in Adobe Acrobat o Adobe InDesign  {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Potete creare le mappe immagine mentre create un eCatalog in Adobe Acrobat o Adobe InDesign.

In Acrobat o InDesign, inserite i riferimenti ipertestuali in corrispondenza delle mappe immagine desiderate e specificate i percorsi URL per le mappe immagine. Quando si seleziona l’opzione Estrai collegamenti durante il caricamento del file PDF in Dynamic Media Classic, i collegamenti vengono convertiti automaticamente in mappe immagine.

Per ulteriori informazioni, consultate la guida di Acrobat o di InDesign.

### Per creare mappe immagine in Adobe InDesign  {#to-create-image-maps-in-adobe-indesign}

1. In InDesign, scegliete Finestra > Interattivo > Collegamenti ipertestuali per aprire il pannello Collegamenti ipertestuali.
1. Selezionate il testo, la cornice o l’elemento grafico da convertire in mappa immagine.
1. Nel menu del pannello Collegamenti ipertestuali, scegliete Nuovo collegamento ipertestuale.
1. Nella finestra di dialogo Nuovo collegamento ipertestuale, scegliete URL dal menu Collega a.
1. Digitate o incollate l’ID del prodotto nella casella URL e fate clic su OK. Dynamic Media Classic completa l’URL con il modello URL mappa immagine.

   >[!NOTE]
   >
   >non è necessario impostare le opzioni di aspetto in InDesign. Potete specificare l&#39;aspetto in Dynamic Media Classic.

1. Ripetete i passaggi da 2 a 5 per tutte le mappe immagine da creare.
1. Esportate il file come PDF.
1. Caricate il PDF in Dynamic Media Classic e selezionate Estrai collegamenti dalle opzioni PDF.

### Per creare mappe immagine in Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. In Acrobat, scegliete Strumenti > Modifica avanzata > Strumento Link.
1. Trascinate per creare la mappa immagine. Viene visualizzata la finestra Crea link.
1. Selezionate Link personalizzato e fate clic su Avanti.

   ***nota **: Non è necessario impostare le opzioni di aspetto in  Acrobat. È possibile specificare l&#39;aspetto in Dynamic Media Classic.*

1. Nella finestra Proprietà link, fate clic su Azioni.
1. Selezionate Apri un link Web dal menu Seleziona azione e fate clic su Aggiungi.
1. Digitate l’ID del prodotto per la mappa immagine nella casella Modifica URL e fate clic su OK. Dynamic Media Classic completa l’URL utilizzando il modello URL della mappa immagine.
1. Ripetete i passaggi da 1 a 7 per tutte le mappe immagine da creare.
1. Salvate il file.
1. Caricate il PDF in Dynamic Media Classic e selezionate Estrai collegamenti dalle opzioni PDF.

