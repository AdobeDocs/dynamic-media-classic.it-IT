---
title: Visualizzare, aggiungere ed esportare metadati
description: Scopri come visualizzare, aggiungere ed esportare metadati in Adobe Dynamic Media Classic.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
topic: Content Management
level: Intermediate
source-git-commit: 1b90beb99b161b76da81403f5aed9755b3a92c8b
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 45%

---

# Visualizzare, aggiungere ed esportare metadati{#viewing-adding-and-exporting-metadata}

È possibile memorizzare informazioni specifiche dei file utilizzati in Adobe Dynamic Media Classic; tali informazioni sono denominate *metadati*. Puoi utilizzare i metadati in Adobe Dynamic Media Classic per organizzare, cercare, filtrare e ordinare le risorse.

I metadati vengono visualizzati in visualizzazione dettagli insieme alle informazioni generate da Adobe Dynamic Media Classic, ad esempio la data di creazione del file, la data di pubblicazione e le parole chiave. Per visualizzare i metadati, apri la risorsa in Vista dettagli, quindi seleziona il pannello Metadati. In visualizzazione Dettagli potete immettere e modificare i metadati.

Alcuni metadati sono incorporati direttamente in un file. Se un file contiene questi metadati, Adobe Dynamic Media Classic li carica automaticamente con il file. Puoi incorporare i metadati nelle risorse sorgente in Adobe Photoshop, InDesign, Illustrator e altre applicazioni; Adobe Dynamic Media Classic riconosce tali metadati. Potete anche aggiungere metadati a singoli file nel pannello Metadati in Vista dettagli. Per assicurare coerenza tra le diverse risorse, gli amministratori della società possono creare dei modelli di metadati che forniscono i campi di metadati da compilare.

Per ulteriori informazioni sui metadati incorporati, consulta [Piattaforma metadati estensibile](https://www.adobe.com/products/xmp.html).

## Visualizzare i metadati {#view-metadata}

Per visualizzare i metadati di una risorsa, apri la risorsa in Vista dettagli e tocca il pannello Metadati. Per selezionare un set di campi di metadati, scegliere un&#39;opzione dal menu Visualizzazione metadati. Adobe Dynamic Media Classic offre le seguenti visualizzazioni metadati:

* **Vista compatta** - Un elenco di base di valori.

* **IPTC** - Valori definiti dal Consiglio internazionale delle telecomunicazioni di stampa.

* **XMP** - Valori definiti dal programma di metadati estensibili.

Gli amministratori possono creare ulteriori visualizzazioni di metadati, che vengono aggiunte al menu Visualizzazioni metadati.

Consulta [Visualizzazioni metadati](application-setup.md#metadata_views) per informazioni sulla creazione di visualizzazioni metadati.

## Immettere manualmente i metadati per una risorsa {#manually-enter-metadata-for-an-asset}

1. Apri la risorsa in Vista dettagli.
1. Aprite il pannello Metadati ed effettuate una delle seguenti operazioni:

   * Scegliete una visualizzazione metadati per determinare quali campi di metadati sono disponibili nel pannello.
   * Scegliete un valore predefinito, quindi selezionate **[!UICONTROL Applica]** per popolare i campi di metadati con valori preimpostati. I valori dei predefiniti vengono impostati dagli amministratori di società.

1. Immettete i valori nel pannello Metadati.

>[!NOTE]
>
>Per modificare i metadati di più risorse contemporaneamente, seleziona le risorse e passa a **[!UICONTROL File]** > **[!UICONTROL Modifica informazioni]**. Le modifiche effettuate ai metadati nella finestra Modifica info vengono applicate a tutte le risorse selezionate.

## Aggiungere o modificare le parole chiave {#add-or-edit-keywords}

Oltre ai metadati, puoi utilizzare le parole chiave per facilitare la ricerca e la gestione delle risorse.

Le parole chiave aggiunte ad altri file durante questa sessione o rimosse dall&#39;elenco vengono visualizzate nella tabella Suggerimenti parole chiave.

1. Aprite il file in visualizzazione Dettagli.
1. Seleziona **[!UICONTROL Parole chiave]**.
1. Per aggiungere delle parole chiave, effettuate una delle seguenti operazioni:

   * Digitate una parola chiave nella casella di testo e selezionate **[!UICONTROL Aggiungi]**.
   * Selezionare una parola chiave in **[!UICONTROL Suggerimenti parole chiave]** tabella.

1. Per rimuovere una parola chiave, selezionarla e selezionare **[!UICONTROL Rimuovi]**. Viene spostata nella tabella Suggerimenti parole chiave.

>[!NOTE]
>
>È possibile aggiungere parole chiave ai file durante il caricamento in Adobe Dynamic Media Classic. Nella finestra di dialogo Opzioni processo di caricamento, scegli **[!UICONTROL Metadati aggiuntivi]** e immettere le parole chiave.
>Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

## Importare i metadati {#import-metadata}

Invece di immettere manualmente i metadati per una risorsa alla volta, potete importare i metadati per diverse risorse da un file XML o delimitato da tabulazioni. L’immissione dei metadati in un file XML o delimitato da tabulazioni e l’importazione di tale file risulta più rapida rispetto all’immissione dei metadati in singole risorse. Nella prima riga del file delimitato da tabulazioni, inserite l’ID e i nomi dei campi per i quali desiderate registrare i metadati. In ogni riga successiva, immettete il nome dell’ID della risorsa seguito dai valori di metadati. I campi non inclusi nel file XML o delimitato da tabulazioni non vengono modificati. Per importare metadati da un file XML, accertatevi che sia conforme al DTD.

>[!NOTE]
>
>Puoi creare un modello per l’immissione dei metadati, in modo che possano essere importati correttamente in Adobe Dynamic Media Classic. Una volta creato il modello, utilizzatelo per immettere i metadati.
>Consultate [Creare un modello per l’immissione di metadati da caricare](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Per ulteriori informazioni sulle proprietà standardizzate, consulta [Centro per sviluppatori XMP Adobe](https://www.adobe.com/devnet/xmp.html).

1. Nel pannello Sfoglia, selezionate le immagini a cui desiderate aggiungere dei metadati da un file XML o delimitato da tabulazioni.
1. Vai a **[!UICONTROL File]** > **[!UICONTROL Importa metadati]**.
1. In **[!UICONTROL Carica metadati]** finestra di dialogo, seleziona **[!UICONTROL Sfoglia]**.
1. Nella finestra di dialogo **[!UICONTROL Seleziona file da caricare]**, selezionate un file XML o delimitato da tabulazioni.
1. Immettete un nome per il processo.
1. Seleziona **[!UICONTROL Carica]**.

### Identificare diversi tipi di metadati nell’importazione

Tenete sempre presente quanto segue per identificare i diversi tipi di metadati da importare:

* I campi definiti dall&#39;utente sono identificati dal relativo nome creato in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Campi definiti dall&#39;utente]**. Utilizzate la funzionalità di generazione file per ottenere un elenco di tutti i campi definiti dall’utente nel formato corretto di importazione.
* Il nome delle proprietà di metadati XMP deve essere preceduto dal relativo prefisso XMP. Il prefisso e il nome sono separati dal segno due punti (:). Il prefisso XMP si trova in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Schema metadati]** editor. I nomi tecnici si trovano nella documentazione del relativo schema XMP. I nomi delle proprietà XMP non vengono visualizzati nella funzione Genera file.
* Il nome delle proprietà Schema metadati deve essere preceduto dal relativo prefisso. Il prefisso e il nome sono separati dal segno due punti (:). Il prefisso e i nomi delle proprietà sono definiti nell’editor Schema metadati. I nomi delle proprietà dello schema metadati non vengono visualizzati nella funzione Genera file.

Ad esempio: la proprietà XMP per le parole chiave è lo schema XMP &quot;Dublin Core&quot; con il prefisso `dc` e `subject` è il nome tecnico dell’XMP. Il prefisso e il nome tecnico dell’XMP sono combinati nel `dc:subject` nome completo della proprietà. Nel formato di importazione dei metadati XML, `dc.subject` deve essere il nome della proprietà. Nel formato di importazione delimitato da tabulazioni, deve essere l’intestazione della colonna.

### Importare parole chiave

Le parole chiave possono essere importate come elenco separato da virgole. Se una virgola appare in uno qualsiasi dei singoli valori, deve essere preceduta da una barra rovesciata (\). Un segno di barra rovesciata deve essere invece riportato come doppia barra rovesciata (\\).

Ad esempio, un file di importazione dei metadati contenente il valore `Hello\, World!,back\\slash,foo` per `dc:subject` imposta tre parole chiave XMP sulla risorsa: `Hello, World!,` `back\slash,` e `foo`.

### Importare file XMP di metadati XMP e Schema metadati

L’importazione XML accetta solo dati XML validi. Quando si importano campi XMP o schema metadati, viene aggiunto il prefisso dello spazio dei nomi e qui si comporta come uno spazio dei nomi XMP. Questo spazio dei nomi deve essere dichiarato. Ad esempio, nel tag di livello superiore.

Ad esempio:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### Importare file delimitati da schede di metadati di XMP e schema metadati

Il prefisso deve essere aggiunto alla relativa intestazione di colonna del campo da importare.

## Importare metadati (tramite FTP) {#import-metadata-via-ftp}

È possibile importare metadati per più file immettendo i metadati in un file XML o delimitato da tabulazioni e selezionando **[!UICONTROL Elabora file di metadati]** nella pagina Carica opzioni processo (tramite la scheda FTP).

Accertatevi che i dati presenti nel file XML o delimitato da tabulazioni siano nel formato corretto. Nella prima riga, immettete il campo ID seguito dai nomi dei campi di metadati da modificare. In ogni riga successiva, immettete il nome dell’ID della risorsa seguito dai valori di metadati. I campi non inclusi nel file XML o delimitato da tabulazioni non vengono modificati.

Sulla barra di navigazione globale, seleziona **[!UICONTROL Carica]**. Per importare i metadati, nella pagina Carica seleziona la **[!UICONTROL Tramite FTP]** , quindi seleziona **[!UICONTROL Opzioni processo]**. Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Processo]**, quindi seleziona **[!UICONTROL Elabora file di metadati]** casella di controllo.

## Rinominare gli ID in batch tramite metadati {#batch-rename-ids-using-metadata}

Utilizzando i metadati importati da un file delimitato da tabulazioni o da un file XML, è possibile rinominare gli ID Adobe Dynamic Media Classic. I metadati importati vengono applicati solo alle immagini specificate nel file di metadati. Non importa se le immagini sono selezionate nel pannello Sfoglia.

Per rinominare l&#39;ID Adobe Dynamic Media Classic di un&#39;immagine, aggiungi una colonna etichettata *newipsid* nel file delimitato da tabulazioni oppure aggiungere un campo denominato `new_vc_objectname` ai dati XML.

Ad esempio:

| | newipsid |
| --- | --- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

Il registro dei processi per il processo Metadati mostra quali ID sono stati rinominati correttamente e quali no.

## Creare un modello per l’immissione di metadati da caricare. {#create-a-template-for-entering-metadata-to-upload}

Adobe Dynamic Media Classic offre un comando per la creazione di un modello per la registrazione dei metadati. L’utilizzo del modello assicura che i metadati vengano immessi nel formato corretto in modo da poter essere caricati correttamente in Adobe Dynamic Media Classic. Per creare un modello da utilizzare per la registrazione e l&#39;importazione di metadati in Adobe Dynamic Media Classic, effettuare le seguenti operazioni:

1. Seleziona le risorse immagine con i campi di metadati desiderati per il modello.
1. Vai a **[!UICONTROL File]** > **[!UICONTROL Importa metadati]**.
1. Per **[!UICONTROL Tipo di proprietà risorsa]**, seleziona **[!UICONTROL Immagine]**.
1. Dalla sezione **[!UICONTROL Genera file]** elenco a discesa, scegliere **[!UICONTROL Modello delimitato da tabulazioni]**, **[!UICONTROL Metadati XML della risorsa]**, o **[!UICONTROL DTD XML]**.
1. Seleziona **[!UICONTROL Genera]**.
1. Nella finestra di dialogo risultante, copiate i dati. Utilizzate tali dati per definire il modello.

## Operazioni con gli schemi di metadati {#working-with-metadata-schemas}

Un amministratore di società può visualizzare un elenco di tutti gli schemi disponibili. Sulla barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Metadati]** > **[!UICONTROL Schema metadati]**.

Inizialmente, l&#39;elenco degli schemi standard globali come l&#39;XMP è nascosto. Per visualizzarli, usate la casella di selezione in fondo all’elenco.

L’amministratore della società può creare uno schema personalizzato o modificarne uno esistente.

Potete utilizzare l’Editor schema metadati per effettuare le operazioni seguenti:

| Azione | Descrizione |
| --- | --- |
| Aggiungi | Aggiunge una proprietà allo schema. Una finestra di dialogo modale raccoglie le informazioni: ID, Etichetta, Struttura e Tipo di dati. |
| Aggiungi valore di scelta | Aggiunge una nuova scelta selezionabile a una proprietà con struttura Scelta aperta o Scelta chiusa. Tutti i valori di scelta sono dello stesso tipo. Seleziona la proprietà stessa per abilitare il pulsante. |
| Modifica | Modifica l’etichetta di una proprietà o di un valore di scelta. Potete modificare solo le informazioni di Etichetta e ID; Tipo non è modificabile. |
| Sposta in alto/Sposta in basso | L’ordine impostato nello schema viene rispecchiato nell’interfaccia utente. Per modificare l’ordine, selezionate una proprietà o un valore di scelta e utilizzate questi pulsanti. Il trascinamento della selezione non è attualmente supportato. |
| Elimina | Elimina dallo schema una proprietà o un valore di scelta. Non elimina i valori dal blocco XMP o dal database. La proprietà non è più disponibile per le visualizzazioni metadati e viene rimossa dalla visualizzazione Dettagli risorsa. Se la proprietà è stata pubblicata sul server metadati, esegui una pubblicazione forzata per rimuovere i dati dal server metadati rivolto al pubblico. |

Il sistema genera automaticamente uno schema personalizzato per i campi definiti dall&#39;utente con il prefisso `s7udf`. Si tratta di campi definiti dall&#39;utente esistenti che vengono modificati nella sezione Configurazione.

>[!NOTE]
>
>le modifiche apportate allo schema non modificano mai i metadati stessi delle risorse. Tuttavia, non sono visibili per tutte le funzionalità di Adobe Dynamic Media Classic e del server di metadati e non sono accessibili dopo la modifica. Allo stesso modo, se esistono metadati per una risorsa, la creazione dello schema corrispondente rende i metadati utilizzabili in Adobe Dynamic Media Classic e nel server di metadati.

L’Editor schema metadati offre una modalità grafica per aggiungere o modificare uno schema aziendale personalizzato all’interno di Adobe Dynamic Media Classic. Uno schema è definito da un prefisso, uno spazio nomi e un elenco di proprietà.

* **[!UICONTROL Nome]** - Nome interfaccia utente per lo schema. Utilizzato per identificare le proprietà in nelle visualizzazioni metadati e in Ricerca avanzata. Simile alle sezioni XMP come ad esempio Base, IPTC, PDF.

* **[!UICONTROL Prefisso]** - Identificatore univoco tecnico dello schema. Limitato alle lettere a-z e A-Z. Il prefisso non è visibile nell’interfaccia utente di Adobe Dynamic Media Classic, ma viene utilizzato quando i metadati di una risorsa vengono memorizzati nel blocco XMP e nel database. Il prefisso viene utilizzato per identificare in modo univoco i campi di metadati per le ricerche metadati nel server metadati o per l’importazione.

* **[!UICONTROL Namespace]** - Identificatore univoco tecnico per lo schema, in genere un URL nel modulo `https://your.company.com/name/version/`. Per degli esempi, consultate l’elenco degli schemi standard. Lo spazio dei nomi non è visibile nell’interfaccia utente di Adobe Dynamic Media Classic, ma viene utilizzato per memorizzare i metadati nel blocco XMP.

* **[!UICONTROL Descrizione]** - Descrizione in forma libera dello schema.

>[!NOTE]
>
>il prefisso e lo spazio nomi non possono essere modificati. Per modificare queste proprietà, è necessario eliminare e ricreare lo schema.

Le proprietà descrivono i metadati che possono essere memorizzati con questo schema nel blocco XMP. Una proprietà è costituita da:

| Proprietà | Descrizione |
| --- | --- |
| ID | Identificatore tecnico della proprietà. L’ID non è visibile nell’interfaccia utente di Adobe Dynamic Media Classic, ma viene utilizzato quando i metadati di una risorsa vengono memorizzati nel blocco XMP e nel database. L’ID viene utilizzato per creare query di ricerca nel server metadati. L’ID presenta alcune restrizioni: <ul><li>Non può contenere spazi</li><li>Non può contenere &quot;.&quot;, &quot;:&quot;, &quot;$&quot;</li><li>Non può contenere un numero come primo carattere</li><li>Come primo carattere si consiglia di utilizzare una lettera a-z o A-Z</li></ul> <br>Una volta creato, l’ID non può essere modificato. |
| Etichetta | Nome della proprietà per l’interfaccia utente. |
| Struttura | Determina il tipo di proprietà e il tipo di dati. La struttura può essere:<ul><li>Tipo semplice: valore singolo di tipo di dati</li><li>Sequenza: elenco di valori dello stesso tipo di dati</li><li>Scelta aperta: selezionate una voce da un elenco di valori predefiniti, oppure immettete del testo a scelta. Può essere solo di tipo Stringa o Intero</li><li>Scelta chiusa: selezionate una voce da un elenco di valori predefiniti (casella a comparsa o elenco di scelta)</li></ul> |
| Tipo di dati | Selezionate tra i seguenti tipi disponibili: <ul><li>Stringa</li><li>Intero</li><li>Virgola mobile</li><li>Sì/No (booleano)</li><li>Data</li></ul> |

Quando la struttura della proprietà è Scelta aperta o Scelta chiusa, immettete almeno un valore di scelta. Un valore di Scelta aperta può essere modificato. Un valore di Scelta chiusa non può essere modificato. Tutti i valori di scelta hanno lo stesso tipo di dati della proprietà.

| Proprietà | Descrizione |
| --- | --- |
| ID | Identificatore tecnico del valore. L’ID non è visibile nell’interfaccia utente di Adobe Dynamic Media Classic, ma viene utilizzato quando i metadati di una risorsa vengono memorizzati nel blocco XMP e nel database. L’ID viene utilizzato nelle query di ricerca nel server metadati. L’ID non può contenere spazi. Una volta creato, l’ID non può essere modificato. |
| Etichetta | Nome del valore per l’interfaccia utente. |

>[!MORELIKETHIS]
>
>* [Predefiniti per visualizzatori](application-setup.md#viewer_presets)
>* [Predefiniti per metadati](application-setup.md#metadata_presets)
