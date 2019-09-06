---
title: Gestione del contenuto del pannello Info negli ecatalog
seo-title: Gestione del contenuto del pannello Info negli ecatalog
description: 'null'
seo-description: Scoprite come gestire il contenuto del pannello Informazioni negli ecatalog.
uuid: 5 aa 634 f 9-0874-4 bb 5-a 3 d 9-8 ce 4 d 5577941
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/ecatalogs
discoiquuid: be 277831-77 cc -4011-ae 30-e 75 c 18 eec 99 b
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Gestione del contenuto del pannello Info negli ecatalog{#managing-info-panel-content-in-ecatalogs}

Oltre a usare il testo delle mappe immagine per i rollover nell’eCatalog, potete usare un pannello Info per aggiungere quantità maggiori di testo di rollover, inclusi i collegamenti. Potete anche gestire il pannello Info usando la cache a tempo e pianificando gli aggiornamenti dei contenuti.

Potete gestire l'impostazione e i dati del pannello Info utilizzando le seguenti funzioni in Dynamic Media Classic:

* Il pannello Impostazioni pannello Info consente di specificare il modello utilizzato per visualizzare il testo del pannello Info, una risposta predefinita in caso di errori e il numero di ore in cui le informazioni restano nella cache. Inoltre, potete specificare se pubblicare automaticamente gli eCatalog.
* Il pannello Feed di dati per pannello Info consente di specificare un file CSV contenente il testo che desiderate visualizzare nel testo di rollover del pannello Info, nonché i tempi di pianificazione per l’aggiornamento delle informazioni.
* La finestra di dialogo Importa metadati (a cui si accede dalla visualizzazione Mappe pagine) consente di importare un file TXT delimitato da tabulazioni contenente le informazioni del testo di rollover. Potete utilizzare questa opzione TXT o il pannello Feed di dati con l’opzione file CSV per il testo di rollover.
* La visualizzazione Mappe pagine fornisce un’opzione di anteprima del file xml visualizzato per mappe immagine specifiche.

## Configurare un modello di risposta per ecatalog {#set-up-a-response-template-for-ecatalogs}

Potete selezionare uno dei tre modelli di risposta predefiniti per la visualizzazione del testo in un pannello Info. I modelli di risposta predefiniti determinano come le informazioni vengono presentate nel pannello Info: il numero di colonne e righe, la dimensione dei caratteri, il font e così via. Potete selezionare un modello di risposta predefinito o crearne uno personalizzato.

>[!NOTE]
>
>potete anche impostare il modello di risposta nel predefinito del visualizzatore. To use the Response Template in the Viewer Preset instead, add `fmt=1` to the end of the Information Server URL in the Viewer Preset.
>
>Consultate [Impostazione dei predefiniti per il visualizzatore di eCatalog](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Fate doppio clic sull’eCatalog per aprirlo in visualizzazione dettagli.
1. Fate clic sul pannello Impostazioni pannello Info per aprirlo.
1. Selezionate un modello di risposta:

   * Selezionate un predefinito dal menu Modello risposta. Il codice XML per la creazione dei modelli viene visualizzato nella casella Modello utente.
   * Selezionate Personalizzato per creare un modello di risposta personale. Digitate la definizione XML del modello nella casella Modello utente. Potete usare i modelli predefiniti come base per creare dei modelli personalizzati.

1. (Facoltativo) Nella casella Risposta predefinita, digitate il testo da visualizzare se Dynamic Media Classic restituisce un errore durante il recupero delle informazioni per una mappa immagine. Ad esempio, se il sistema riceve il nome di una società e il nome di un eCatalog, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.
1. Nella casella TTL di risposta viene visualizzato il numero di ore di attesa prima che i dati vengano memorizzati nella cache:

   * Con un valore basso i dati vengono aggiornati frequentemente nel corso della giornata.
   * Con un valore più elevato i dati sono relativamente stabili e non richiedono un aggiornamento frequente durante il giorno. Il valore predefinito è dieci ore.

1. Click **Publish**.

## Import source content for the Info Panel in eCatalogs {#import-source-content-for-the-info-panel-in-ecatalogs}

Potete usare un file con valori separati da virgole (CSV) o delimitati da tabulazioni (TXT) per il testo sorgente per il pannello Info di un eCatalog. Per i file delimitati da tabulazioni è richiesta la codifica UTF16 (Unicode). Potete importare tipi di file diversi utilizzando metodi diversi.

Durante la formattazione del contenuto sorgente, tenete presente i seguenti accorgimenti:

* Verificate che i dati delimitati da tabulazioni e virgole contengano il numero di colonne desiderato per il modello di rollover.
* Verificate che il primo elemento o la prima colonna di dati sia un identificatore di rollover (associato al valore rollover_key degli URL della mappa immagine).
* Verificate che ciascun elemento delimitato da tabulazioni o virgole dopo l’identificatore sia l’elemento da sostituire nel modello di risposta (la prima colonna viene sostituita da $1$, la seconda colonna da $2$ e così via).

### Import CSV content into eCatalogs from an externally hosted location {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Fate doppio clic sull’eCatalog per aprirlo in visualizzazione dettagli.
1. Fate clic nel pannello Feed di dati per pannello Info per aprirlo.
1. Inserite l’URL per il file CSV nel campo Posizione file CSV esterno (HTTP). Potete incollare l’URL in questo campo o digitarlo direttamente.
1. (Facoltativo) Specificate quando aggiornare il contenuto mediante i menu Pianifica aggiornamento e fate clic su Aggiungi. Potete selezionare più momenti temporali per l’aggiornamento. Ciascuno di essi viene visualizzato nella casella Orari aggiornamenti. Per rimuovere un orario di aggiornamento, selezionatelo e fate clic su Elimina.
1. (Facoltativo) Fate clic su Esegui aggiornamento ora per aggiornare immediatamente il contenuto.

### Importare un file CSV o delimitato da tabulazioni {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Fate doppio clic sull’eCatalog per aprirlo in visualizzazione dettagli.
1. Fate clic sul pannello Impostazioni pannello Info per aprirlo.
1. **Fate clic su Carica contenuto S 7 Info**.
1. Click **Browse**, select the tab-delimited TXT file, CSV or SSV file you want to use, and click **Open**.
1. Fate clic su **Carica**.

Dynamic Media Classic invia un messaggio e-mail comunicandovi se il caricamento ha avuto esito positivo o meno.

## Anteprima del testo chiave di rollover per una mappa immagine {#preview-rollover-key-text-for-an-image-map}

Dalla schermata Mappe pagine potete visualizzare facilmente il testo del pannello Info per le mappe immagine in una pagina specifica dell’eCatalog.

1. Fate clic sul pulsante rollover Modifica dell’eCatalog.
1. Fate clic su Mappe pagine.
1. Nella parte superiore della tabella sul lato destro della schermata, scegliete Pannello Info dal menu Mostra.

   Il testo chiave di rollover viene visualizzato accanto a ogni mappa immagine che contiene il testo del pannello Info.

