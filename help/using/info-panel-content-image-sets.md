---
title: Gestire il contenuto del pannello informazioni nei set di immagini
description: Scopri come gestire il contenuto del pannello informazioni nei set di immagini in Adobe Dynamic Media Classic.
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
topic: Content Management
level: Intermediate
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 34%

---

# Gestire il contenuto del pannello informazioni nei set di immagini{#managing-info-panel-content-in-image-sets}

Oltre a utilizzare il testo della mappa immagine per i rollover nei set di immagini, è possibile utilizzare un pannello Info per aggiungere grandi quantità di testo di rollover, inclusi i collegamenti. È inoltre possibile gestire il pannello Info utilizzando il caching temporale e pianificando gli aggiornamenti dei contenuti.

Potete gestire la configurazione e i dati del pannello Info utilizzando le seguenti funzioni di Adobe Dynamic Media Classic:

* Il pannello di configurazione del pannello Info consente di specificare il modello utilizzato per visualizzare il testo del pannello Info, una risposta predefinita per gli errori e il numero di ore in cui le informazioni vengono memorizzate nella cache. Inoltre, potete specificare se pubblicare automaticamente il set di immagini.
* Il pannello Feed dati del pannello Info consente di specificare un file CSV contenente il testo da visualizzare nel testo di rollover del pannello Info e di pianificare gli orari per l&#39;aggiornamento delle informazioni.
* La finestra di dialogo Importa metadati consente di importare un file TXT delimitato da tabulazioni contenente le informazioni di testo di rollover. Potete utilizzare questa opzione TXT o il pannello Feed dati di InfoPanel con l&#39;opzione File CSV per il testo di rollover.

## Impostare un modello di risposta per i set di immagini {#set-up-a-response-template-for-image-sets}

Potete selezionare uno dei tre modelli di risposta predefiniti per la visualizzazione del testo in un pannello Info. I modelli di risposta predefiniti determinano come le informazioni vengono presentate nel pannello Info: il numero di colonne e righe, la dimensione dei caratteri, il font e così via. Potete selezionare un modello di risposta predefinito o crearne uno personalizzato.

**Per impostare un modello di risposta per i set di immagini:**

1. Fai doppio clic sul set di immagini per aprirlo nella vista dei dettagli.
1. Selezionare **[!UICONTROL Configurazione InfoPanel]**.
1. Dall’elenco a discesa Modello risposta, effettuate una delle seguenti operazioni:

   * Per utilizzare la risposta predefinita, selezionare **[!UICONTROL Predefinito]**. Il codice XML per la creazione dei modelli viene visualizzato in modo attenuato nella casella Modello utente.
   * Per creare un modello di risposta personalizzato, seleziona **[!UICONTROL Personalizzato]**. Nella casella di testo Modello utente, digitate la definizione XML del modello. Come base, potete usare il modello predefinito che è già definito nella casella di testo.

1. (Facoltativo) Nella casella Risposta predefinita digitare il testo che si desidera visualizzare se in Adobe Dynamic Media Classic si verifica un errore durante il recupero delle informazioni per una mappa immagine. Ad esempio, se il sistema riceve il nome di una società e il nome di un set di immagini, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.
1. Nel campo TTL di risposta viene visualizzato il numero di ore di attesa prima che i dati vengano memorizzati nella cache.

   * Con un valore basso i dati vengono aggiornati frequentemente nel corso della giornata.
   * Con un valore più elevato i dati sono relativamente stabili e non richiedono un aggiornamento frequente durante il giorno. Il valore predefinito è dieci ore.

1. Seleziona **[!UICONTROL Carica]** per caricare in s7info il contenuto del pannello informazioni, in base al valore rollover_key.
1. Nella finestra di dialogo Caricamento S7Info individuare il file che si desidera utilizzare e quindi selezionare **[!UICONTROL Caricamento]**.

   I formati di file supportati sono file delimitati da tabulazioni con codifica UTF-16 e file CSV con codifica ASCII. Per i file CSV, i caratteri non ASCII devono essere codificati in HTML.

1. Nel pannello InfoPanel Setup, selezionare **[!UICONTROL Publish]**.

## Importare il contenuto sorgente del pannello Info nei set di immagini {#import-source-content-for-the-info-panel-in-image-sets}

È possibile utilizzare un file CSV (Comma-Separated Value) con codifica ASCII (i caratteri non ASCII devono essere codificati da HTML) o un file delimitato da tabulazioni per il testo sorgente di un pannello Info per un set di immagini. Per i file delimitati da tabulazioni è richiesta la codifica UTF-16 (Unicode). È possibile importare diversi tipi di file utilizzando metodi diversi.

Durante la formattazione del contenuto sorgente, tenete presente i seguenti accorgimenti:

* I dati delimitati da tabulazioni e virgole possono contenere tutte le colonne necessarie per il modello di rollover.
* La prima voce o colonna di dati è l’identificatore di rollover (associato al valore rollover_key dagli URL della mappa immagine).
* Assicurati che ogni elemento delimitato da tabulazioni o virgole dopo l’identificatore sia l’elemento che desideri sostituire nel modello di risposta. Pertanto, la prima colonna viene sostituita da $1$, la seconda da $2$ e così via).

### Importare contenuti CSV in set di immagini da una posizione ospitata esternamente {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Fate doppio clic sul set di immagini per aprirlo nella vista dei dettagli.
1. Seleziona **[!UICONTROL Feed dati InfoPanel]**.
1. Nel campo Posizione file CSV esterno (HTTP), immettete l’URL del file CSV.
1. (Facoltativo) Nel campo Pianifica aggiornamento, specificare l&#39;ora in cui aggiornare il contenuto, quindi selezionare **[!UICONTROL Aggiungi]**.

   Potete selezionare più momenti temporali per l’aggiornamento. Ciascuno di essi viene visualizzato nella casella Orari aggiornamenti. Per rimuovere un orario pianificato, selezionarlo, quindi selezionare **[!UICONTROL Elimina]**.

1. (Facoltativo) Seleziona **[!UICONTROL Esegui aggiornamento]** per poter aggiornare immediatamente il contenuto.
