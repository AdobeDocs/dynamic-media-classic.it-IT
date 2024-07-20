---
title: Gestire il contenuto del pannello informazioni nei cataloghi elettronici
description: Scopri come gestire il contenuto del pannello Info negli eCatalog in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 40%

---

# Gestire il contenuto del pannello informazioni nei cataloghi elettronici{#managing-info-panel-content-in-ecatalogs}

Oltre a usare il testo delle mappe immagine per i rollover nell’eCatalog, potete usare un pannello Info per aggiungere quantità maggiori di testo di rollover, inclusi i collegamenti. Puoi anche gestire il pannello Info utilizzando il caching temporizzato e pianificando gli aggiornamenti dei contenuti.

Potete gestire la configurazione e i dati del pannello Info utilizzando le seguenti funzioni di Adobe Dynamic Media Classic:

* Il pannello Impostazione InfoPanel consente di specificare il modello utilizzato per visualizzare il testo del pannello Info, una risposta predefinita per gli errori e il numero di ore in cui le informazioni vengono memorizzate nella cache. Inoltre, potete specificare se pubblicare automaticamente gli eCatalog.
* Il pannello Feed dati di InfoPanel consente di specificare un file CSV contenente il testo che si desidera visualizzare nel testo di rollover di InfoPanel e di programmare gli orari per l&#39;aggiornamento delle informazioni.
* La finestra di dialogo Importa metadati (accessibile dalla vista Pagine mappa ) consente di importare un file TXT delimitato da tabulazioni contenente le informazioni di testo di rollover. Con l’opzione file CSV puoi utilizzare questa opzione TXT o il pannello Feed dati per il testo di rollover.
* La vista Pagine mappa fornisce un’opzione per visualizzare in anteprima il codice xml visualizzato per mappe immagine specifiche.

## Impostare un modello di risposta per gli eCatalog {#set-up-a-response-template-for-ecatalogs}

Potete selezionare uno dei tre modelli di risposta predefiniti per la visualizzazione del testo in un pannello Info. I modelli di risposta predefiniti determinano come le informazioni vengono presentate nel pannello Info: il numero di colonne e righe, la dimensione dei caratteri, il font e così via. È possibile selezionare un modello di risposta predefinito o crearne uno personalizzato.

>[!NOTE]
>
>potete anche impostare il modello di risposta nel predefinito del visualizzatore. Per utilizzare il modello di risposta nel predefinito visualizzatore, aggiungi `fmt=1` alla fine dell&#39;URL del server informazioni nel predefinito visualizzatore.
>
>Vedere [Configurare i predefiniti visualizzatore eCatalog](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Fai doppio clic sull’eCatalog per aprirlo nella Vista dettagli.
1. Selezionare il pannello **[!UICONTROL Configurazione InfoPanel]**.
1. Selezionate un modello di risposta:

   * Selezionate un predefinito dal menu Modello risposta. Il codice XML per la creazione dei modelli viene visualizzato nella casella Modello utente.
   * Per creare un modello di risposta personalizzato, seleziona **[!UICONTROL Personalizzato]**. Digitate la definizione XML del modello nella casella Modello utente. Potete usare i modelli predefiniti come base per creare dei modelli personalizzati.

1. (Facoltativo) Nella casella Risposta predefinita digitare il testo che si desidera visualizzare se in Adobe Dynamic Media Classic si verifica un errore durante il recupero delle informazioni per una mappa immagine. Ad esempio, se il sistema riceve il nome di una società e il nome di un eCatalog, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.
1. Nella casella TTL di risposta viene visualizzato il numero di ore di attesa prima che i dati vengano memorizzati nella cache:

   * Con un valore basso i dati vengono aggiornati frequentemente nel corso della giornata.
   * Impostare un numero più alto se i dati sono relativamente stabili e non richiedono aggiornamenti frequenti nel corso della giornata. Il valore predefinito è dieci ore.

1. Seleziona **[!UICONTROL Publish]**.

## Importare contenuto sorgente per il pannello Info in eCatalog {#import-source-content-for-the-info-panel-in-ecatalogs}

Potete usare un file con valori separati da virgole (CSV) o delimitati da tabulazioni (TXT) per il testo sorgente per il pannello Info di un eCatalog. Per i file delimitati da tabulazioni è richiesta la codifica UTF16 (Unicode). È possibile importare diversi tipi di file utilizzando metodi diversi.

Durante la formattazione del contenuto sorgente, tenete presente i seguenti accorgimenti:

* Verificate che i dati delimitati da tabulazioni e virgole contengano il numero di colonne desiderato per il modello di rollover.
* Assicurati che il primo elemento o colonna di dati sia l’identificatore di rollover (associato al valore rollover_key dagli URL della mappa immagine).
* Assicurati che ogni elemento delimitato da tabulazioni o virgole dopo l’identificatore sia l’elemento da sostituire nel modello di risposta. Pertanto, la prima colonna viene sostituita da $1$, la seconda da $2$ e così via.

### Importare contenuti CSV in eCatalog da una posizione ospitata esternamente {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Fare doppio clic sull&#39;eCatalog per aprirlo in Vista dettagli.
1. Selezionare il pannello **[!UICONTROL Feed dati InfoPanel]**.
1. Inserite l’URL per il file CSV nel campo Posizione file CSV esterno (HTTP). Potete incollare l’URL in questo campo o digitarlo direttamente.
1. (Facoltativo) Specifica un orario per aggiornare il contenuto utilizzando il menu Pianifica aggiornamento e seleziona **[!UICONTROL Aggiungi]**. Potete selezionare più momenti temporali per l’aggiornamento. Ciascuno di essi viene visualizzato nella casella Orari aggiornamenti. Per rimuovere un&#39;ora, selezionarla e selezionare **[!UICONTROL Elimina]**.
1. (Facoltativo) Seleziona **[!UICONTROL Esegui aggiornamento ora]** per poter aggiornare immediatamente il contenuto.

### Importare un file CSV o delimitato da tabulazioni {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Fare doppio clic sull&#39;eCatalog per aprirlo in Vista dettagli.
1. Selezionare il pannello **[!UICONTROL Configurazione InfoPanel]**.
1. Selezionare **[!UICONTROL Carica contenuto S7Info]**.
1. Seleziona **[!UICONTROL Sfoglia]**, seleziona il file TXT, CSV o SSV delimitato da tabulazioni che desideri utilizzare e seleziona **[!UICONTROL Apri]**.
1. Seleziona **[!UICONTROL Carica]**.

Adobe Dynamic Media Classic ti invia un messaggio di posta elettronica che ti informa se il caricamento è stato eseguito correttamente o meno.

## Anteprima del testo chiave di rollover per una mappa immagine {#preview-rollover-key-text-for-an-image-map}

Dalla schermata Mappe pagine potete visualizzare facilmente il testo del pannello Info per le mappe immagine in una pagina specifica dell’eCatalog.

1. Seleziona il pulsante di rollover **[!UICONTROL Modifica]** del catalogo.
1. Seleziona **[!UICONTROL Mappa pagine]**.
1. Nella parte superiore della tabella, sul lato destro dello schermo, scegliere **[!UICONTROL Pannello Info]** dal menu Mostra.

   Il testo chiave di rollover viene visualizzato accanto a ogni mappa immagine che contiene il testo del pannello Info.
