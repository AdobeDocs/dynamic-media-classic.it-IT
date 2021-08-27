---
title: Gestire il contenuto del pannello informazioni negli eCatalog
description: Scopri come gestire il contenuto del pannello Info negli eCatalog in Adobe Dynamic Media Classic.
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 59%

---

# Gestire il contenuto del pannello informazioni negli eCatalog{#managing-info-panel-content-in-ecatalogs}

Oltre a usare il testo delle mappe immagine per i rollover nell’eCatalog, potete usare un pannello Info per aggiungere quantità maggiori di testo di rollover, inclusi i collegamenti. Potete anche gestire il pannello Info usando la cache a tempo e pianificando gli aggiornamenti dei contenuti.

Puoi gestire la configurazione e i dati del pannello Info utilizzando le seguenti funzioni in Adobe Dynamic Media Classic:

* Il pannello Impostazioni pannello Info consente di specificare il modello utilizzato per visualizzare il testo del pannello Info, una risposta predefinita in caso di errori e il numero di ore in cui le informazioni restano nella cache. Inoltre, potete specificare se pubblicare automaticamente gli eCatalog.
* Il pannello Feed di dati InfoPanel consente di specificare un file CSV contenente il testo da visualizzare nel testo di rollover InfoPanel e i tempi di pianificazione per l’aggiornamento delle informazioni.
* La finestra di dialogo Importa metadati (a cui si accede dalla visualizzazione Mappe pagine) consente di importare un file TXT delimitato da tabulazioni contenente le informazioni del testo di rollover. Potete utilizzare questa opzione TXT o il pannello Feed di dati con l’opzione file CSV per il testo di rollover.
* La visualizzazione Mappe pagine fornisce un’opzione di anteprima del file xml visualizzato per mappe immagine specifiche.

## Configurare un modello di risposta per gli eCatalogs {#set-up-a-response-template-for-ecatalogs}

Potete selezionare uno dei tre modelli di risposta predefiniti per la visualizzazione del testo in un pannello Info. I modelli di risposta predefiniti determinano come le informazioni vengono presentate nel pannello Info: il numero di colonne e righe, la dimensione dei caratteri, il font e così via. Potete selezionare un modello di risposta predefinito o crearne uno personalizzato.

>[!NOTE]
>
>potete anche impostare il modello di risposta nel predefinito del visualizzatore. Per utilizzare invece il modello di risposta nel predefinito visualizzatore, aggiungi `fmt=1` alla fine dell’URL del server informazioni nel predefinito visualizzatore.
>
>Consulta [Configurazione predefiniti visualizzatore di eCatalog](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Fate doppio clic sull&#39;eCatalog in modo che si apra nella visualizzazione dettagli.
1. Selezionare il pannello **[!UICONTROL InfoPanel Setup]**.
1. Selezionate un modello di risposta:

   * Selezionate un predefinito dal menu Modello risposta. Il codice XML per la creazione dei modelli viene visualizzato nella casella Modello utente.
   * Per creare un modello di risposta personalizzato, seleziona **[!UICONTROL Personalizzato]**. Digitate la definizione XML del modello nella casella Modello utente. Potete usare i modelli predefiniti come base per creare dei modelli personalizzati.

1. (Facoltativo) Nella casella Risposta predefinita, digitare il testo che si desidera visualizzare se in Adobe Dynamic Media Classic viene rilevato un errore nel recupero delle informazioni per una mappa immagine. Ad esempio, se il sistema riceve il nome di una società e il nome di un eCatalog, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.
1. Nella casella TTL di risposta viene visualizzato il numero di ore di attesa prima che i dati vengano memorizzati nella cache:

   * Con un valore basso i dati vengono aggiornati frequentemente nel corso della giornata.
   * Con un valore più elevato i dati sono relativamente stabili e non richiedono un aggiornamento frequente durante il giorno. Il valore predefinito è dieci ore.

1. Seleziona **[!UICONTROL Pubblica]**.

## Importare il contenuto sorgente per il pannello Informazioni negli eCatalogs {#import-source-content-for-the-info-panel-in-ecatalogs}

Potete usare un file con valori separati da virgole (CSV) o delimitati da tabulazioni (TXT) per il testo sorgente per il pannello Info di un eCatalog. Per i file delimitati da tabulazioni è richiesta la codifica UTF16 (Unicode). Potete importare tipi di file diversi utilizzando metodi diversi.

Durante la formattazione del contenuto sorgente, tenete presente i seguenti accorgimenti:

* Verificate che i dati delimitati da tabulazioni e virgole contengano il numero di colonne desiderato per il modello di rollover.
* Verificate che il primo elemento o la prima colonna di dati sia un identificatore di rollover (associato al valore rollover_key degli URL della mappa immagine).
* Assicurati che ogni elemento delimitato da tabulazioni o virgole dopo l’identificatore sia l’elemento da sostituire nel modello di risposta. Quindi, la prima colonna viene sostituita in $1$, la seconda colonna in $2$, e così via.

### Importare contenuti CSV in eCatalog da una posizione ospitata esternamente {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Fate doppio clic sull&#39;eCatalog in modo che si apra nella visualizzazione dettagli.
1. Selezionare il pannello **[!UICONTROL InfoPanel Datafeed]**.
1. Inserite l’URL per il file CSV nel campo Posizione file CSV esterno (HTTP). Potete incollare l’URL in questo campo o digitarlo direttamente.
1. (Facoltativo) Specifica l&#39;ora in cui aggiornare il contenuto utilizzando i menu Pianifica aggiornamento e seleziona **[!UICONTROL Aggiungi]**. Potete selezionare più momenti temporali per l’aggiornamento. Ciascuno di essi viene visualizzato nella casella Orari aggiornamenti. (Per rimuovere un’ora, selezionala e seleziona **[!UICONTROL Elimina]**.)
1. (Facoltativo) Seleziona **[!UICONTROL Esegui aggiornamento ora]** per aggiornare immediatamente il contenuto.

### Importare un file CSV o delimitato da tabulazioni {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Fate doppio clic sull&#39;eCatalog in modo che venga aperto in visualizzazione dettagli.
1. Selezionare il pannello **[!UICONTROL InfoPanel Setup]**.
1. Seleziona **[!UICONTROL Carica contenuto S7Info]**.
1. Seleziona **[!UICONTROL Sfoglia]**, seleziona il file TXT, CSV o SSV delimitato da tabulazioni da utilizzare e seleziona **[!UICONTROL Apri]**.
1. Seleziona **[!UICONTROL Carica]**.

Adobe Dynamic Media Classic ti invia un messaggio e-mail che ti informa se il caricamento è stato eseguito correttamente o meno.

## Anteprima del testo chiave di rollover per una mappa immagine {#preview-rollover-key-text-for-an-image-map}

Dalla schermata Mappe pagine potete visualizzare facilmente il testo del pannello Info per le mappe immagine in una pagina specifica dell’eCatalog.

1. Selezionare il pulsante rollover del catalogo **[!UICONTROL Modifica]**.
1. Seleziona **[!UICONTROL Mappa pagine]**.
1. Nella parte superiore della tabella sul lato destro dello schermo, scegliere **[!UICONTROL Pannello informazioni]** dal menu Mostra.

   Il testo della chiave di rollover viene visualizzato accanto a ogni mappa immagine che contiene il testo del Pannello Informazioni.