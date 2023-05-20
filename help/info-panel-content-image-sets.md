---
title: Gestisci contenuto del pannello Info in Immagine set
description: Scopri come gestire contenuto del pannello Info in Immagine set in Adobe Systems Dynamic Media Classic.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 51%

---

# Gestisci contenuto del pannello Info in Immagine set{#managing-info-panel-content-in-image-sets}

Oltre a usare il testo delle mappe immagine per i rollover in set di immagini, potete usare un pannello Info per aggiungere quantità maggiori di testo di rollover, inclusi i collegamenti. Potete anche gestire il pannello Info usando la cache a tempo e pianificando gli aggiornamenti dei contenuti.

Puoi gestire la configurazione e i dati del tuo InfoPanel utilizzando le seguenti funzioni di Adobe Systems Dynamic Media Classic:

* Il pannello Impostazioni pannello Info consente di specificare il modello utilizzato per visualizzare il testo del pannello Info, una risposta predefinita in caso di errori e il numero di ore in cui le informazioni restano nella cache. Inoltre, potete specificare se pubblicare automaticamente il set di immagini.
* Il pannello datafeed di InfoPanel consente di specificare un file CSV contenente il testo da visualizzare nel testo di rollover del pannello Info e programmare volte ad aggiornare le informazioni.
* La finestra di dialogo Importa metadati consente di importare un file TXT delimitato da tabulazioni contenente le informazioni per il testo di rollover. Potete utilizzare questa opzione TXT o il pannello feed dati dell&#39;InfoPanel con l&#39;opzione file CSV per il testo di rollover.

## Impostare un modello di risposta per i set di Immagine {#set-up-a-response-template-for-image-sets}

Potete selezionare uno dei tre modelli di risposta predefiniti per la visualizzazione del testo in un pannello Info. I modelli di risposta predefiniti determinano come le informazioni vengono presentate nel pannello Info: il numero di colonne e righe, la dimensione dei caratteri, il font e così via. Potete selezionare un modello di risposta predefinito o crearne uno personalizzato.

**Per impostare un modello di risposta per i set di Immagine:**

1. Fai doppio clic sul tuo Immagine insieme in modo che si apra in dettaglio Visualizza.
1. Seleziona **[!UICONTROL Impostazione InfoPanel]**.
1. Dall’elenco a discesa Modello risposta, effettuate una delle seguenti operazioni:

   * Per utilizzare la risposta predefinita, selezionare **[!UICONTROL predefinito]** . Il codice XML per la creazione dei modelli viene visualizzato in modo attenuato nella casella Modello utente.
   * Per creare un modello di risposta personale, selezionare **[!UICONTROL personalizzato]** . Nella casella di testo Modello utente, digitate la definizione XML del modello. Come base, potete usare il modello predefinito che è già definito nella casella di testo.

1. Facoltativo Nella casella risposta predefinita, digitate il testo che desiderate visualizzare se Adobe Systems Dynamic Media Classic incontra un errore nel recupero delle informazioni per una mappa immagine. Ad esempio, se il sistema riceve il nome di una società e il nome di un set di immagini, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.
1. Nel campo TTL di risposta viene visualizzato il numero di ore di attesa prima che i dati vengano memorizzati nella cache.

   * Con un valore basso i dati vengono aggiornati frequentemente nel corso della giornata.
   * Con un valore più elevato i dati sono relativamente stabili e non richiedono un aggiornamento frequente durante il giorno. Il valore predefinito è dieci ore.

1. Seleziona **[!UICONTROL carica]** per caricare il pannello informazioni contenuto, in base ai valori rollover_key, a S7Info.
1. Nella finestra di dialogo Carica S7Info, individuate il file da utilizzare e fate clic **[!UICONTROL su carica]** .

   I formati di file supportati sono file delimitati da tabulazioni con codifica UTF-16 e file CSV con codifica ASCII. Per i file CSV, i caratteri non ASCII devono essere codificati in HTML.

1. Nel pannello impostazioni InfoPanel, selezionate **[!UICONTROL Publish]** .

## Importa contenuto di origine per il pannello Info nei set di Immagine {#import-source-content-for-the-info-panel-in-image-sets}

Per il testo sorgente per il pannello Info di un set di immagini, potete usare un file CSV (separato da virgole) con codifica ASCII (i caratteri non ASCII devono essere codificati in HTML) o un file delimitato da tabulazioni. Per i file delimitati da tabulazioni è richiesta la codifica UTF-16 (Unicode). Potete importare tipi di file diversi utilizzando metodi diversi.

Durante la formattazione del contenuto sorgente, tenete presente i seguenti accorgimenti:

* I dati di scheda e delimitati da virgole possono contenere tutte le colonne necessarie per il modello di rollover.
* Il primo elemento o colonna di dati è l&#39;identificatore di rollover (associato al valore rollover_key dagli URL della mappa immagine).
* Assicurati che ogni elemento delimitato da scheda o da virgole dopo l&#39;identificatore sia l&#39;elemento che desideri sostituire nel modello di risposta. Quindi, la prima colonna viene sostituita in $1 $, la seconda colonna in $2 $ e così via).

### Importare contenuti CSV in set di immagini da una posizione ospitata esternamente {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Fate doppio clic sul Immagine insieme in modo che si apra in dettaglio Visualizza.
1. Seleziona **[!UICONTROL InfoPanel datafeed]** .
1. Nel campo Posizione file CSV esterno (HTTP), immettete l’URL del file CSV.
1. Facoltativo Nei campi Pianifica aggiornamento, specificate un orario per aggiornare le contenuto e fate clic **[!UICONTROL su Aggiungi]** .

   Potete selezionare più momenti temporali per l’aggiornamento. Ciascuno di essi viene visualizzato nella casella Orari aggiornamenti. Per rimuovere un&#39;ora pianificata, selezionatela, quindi selezionate **[!UICONTROL Elimina]** .

1. Facoltativo Seleziona **[!UICONTROL Esegui aggiornamento]** per aggiornare immediatamente il contenuto.
