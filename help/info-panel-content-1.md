---
title: Gestione del contenuto del pannello Info in Set di immagini
seo-title: Gestione del contenuto del pannello Info in Set di immagini
description: 'null'
seo-description: Scoprite come gestire il contenuto del pannello Info in Set di immagini.
uuid: ed 7 b 4344-f 180-41 fc-a 95 a -62 a 9767 dc 056
contentOwner: rbrough
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
content-type: riferimento
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/image_ sets
discoiquuid: ba 5 d 1 fb 1-af 54-471 c-a 471-853 ace 7 f 72 fd
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Gestione del contenuto del pannello Info in Set di immagini{#managing-info-panel-content-in-image-sets}

Oltre a usare il testo delle mappe immagine per i rollover in set di immagini, potete usare un pannello Info per aggiungere quantità maggiori di testo di rollover, inclusi i collegamenti. Potete anche gestire il pannello Info usando la cache a tempo e pianificando gli aggiornamenti dei contenuti.

Potete gestire l’impostazione e i dati del pannello Info utilizzando le seguenti funzioni di Scene7 Publishing System:

* Il pannello Impostazioni pannello Info consente di specificare il modello utilizzato per visualizzare il testo del pannello Info, una risposta predefinita in caso di errori e il numero di ore in cui le informazioni restano nella cache. Inoltre, potete specificare se pubblicare automaticamente il set di immagini.
* Il pannello Feed di dati per pannello Info consente di specificare un file CSV contenente il testo che desiderate visualizzare nel testo di rollover del pannello Info, nonché i tempi di pianificazione per l’aggiornamento delle informazioni.
* La finestra di dialogo Importa metadati consente di importare un file TXT delimitato da tabulazioni contenente le informazioni per il testo di rollover. Potete utilizzare questa opzione TXT o il pannello Info con l’opzione file CSV per il testo di rollover.

## Configurare un modello di risposta per i set di immagini {#set-up-a-response-template-for-image-sets}

Potete selezionare uno dei tre modelli di risposta predefiniti per la visualizzazione del testo in un pannello Info. I modelli di risposta predefiniti determinano come le informazioni vengono presentate nel pannello Info: il numero di colonne e righe, la dimensione dei caratteri, il font e così via. Potete selezionare un modello di risposta predefinito o crearne uno personalizzato.

**Per configurare un modello di risposta**

1. Fate doppio clic sul set di immagini per aprirlo in visualizzazione Dettagli.
1. Click **InfoPanel Setup** to unfold the panel.
1. Dall’elenco a discesa Modello risposta, effettuate una delle seguenti operazioni:

   * Selezionate Predefinito per utilizzare la risposta predefinita. Il codice XML per la creazione dei modelli viene visualizzato in modo attenuato nella casella Modello utente.
   * Selezionate Personalizzato per creare un modello di risposta personale. Nella casella di testo Modello utente, digitate la definizione XML del modello. Come base, potete usare il modello predefinito che è già definito nella casella di testo.

1. (Facoltativo) Nella casella Risposta predefinita, digitate il testo da visualizzare se Dynamic Media Classic restituisce un errore durante il recupero delle informazioni per una mappa immagine. Ad esempio, se il sistema riceve il nome di una società e il nome di un set di immagini, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.
1. Nel campo TTL di risposta viene visualizzato il numero di ore di attesa prima che i dati vengano memorizzati nella cache.

   * Con un valore basso i dati vengono aggiornati frequentemente nel corso della giornata.
   * Con un valore più elevato i dati sono relativamente stabili e non richiedono un aggiornamento frequente durante il giorno. Il valore predefinito è dieci ore.

1. Click **Upload** to upload info panel content, based on the rollover_key values, to s7info.
1. In the S7Info Upload dialog box, browse to the file that you want to use, and then click **Upload**.

   I formati file supportati sono file delimitati da tabulazioni con codifica UTF-16 e file CSV con codifica ASCII. Per i file CSV, i caratteri non ASCII devono essere codificati in HTML.

1. In the InfoPanel Setup panel, click **Publish**.

## Importare il contenuto sorgente per il pannello Info in Set di immagini {#import-source-content-for-the-info-panel-in-image-sets}

Per il testo sorgente per il pannello Info di un set di immagini, potete usare un file CSV (separato da virgole) con codifica ASCII (i caratteri non ASCII devono essere codificati in HTML) o un file delimitato da tabulazioni. Per i file delimitati da tabulazioni è richiesta la codifica UTF-16 (Unicode). Potete importare tipi di file diversi utilizzando metodi diversi.

Durante la formattazione del contenuto sorgente, tenete presente i seguenti accorgimenti:

* I dati delimitati da tabulazioni e virgole devono contenere tutte le colonne desiderate per il modello di rollover.
* Il primo elemento o la prima colonna di dati deve essere l’identificatore di rollover (associato al valore rollover_key degli URL della mappa immagine).
* Verificate che ciascun elemento delimitato da tabulazioni o virgole dopo l’identificatore sia l’elemento da sostituire nel modello di risposta (la prima colonna viene sostituita da $1$, la seconda colonna da $2$ e così via).

### Importazione di contenuto CSV in set di immagini da un percorso esterno {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Fate doppio clic sul set di immagini per aprirlo in visualizzazione Dettagli.
1. Click **InfoPanel Datafeed** to unfold the panel.
1. Nel campo Posizione file CSV esterno (HTTP), immettete l’URL del file CSV.
1. (Optional) In the Schedule Update fields, specify a time to update the content, and then click **Add**.

   Potete selezionare più momenti temporali per l’aggiornamento. Ciascuno di essi viene visualizzato nella casella Orari aggiornamenti. To remove a scheduled time, select it, and then click **Delete**.

1. (Optional) Click **Run Update** to immediately update the content.

