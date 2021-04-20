---
title: Visualizzazione, aggiunta ed esportazione di metadati
description: Scopri come visualizzare, aggiungere ed esportare i metadati.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic,Asset Management,Metadata
role: Business Practitioner
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '2250'
ht-degree: 63%

---


# Visualizzazione, aggiunta ed esportazione di metadati{#viewing-adding-and-exporting-metadata}

È possibile memorizzare informazioni specifiche per i file con cui si lavora in Dynamic Media Classic; queste informazioni sono denominate *metadata*. In Dynamic Media Classic puoi utilizzare i metadati per organizzare, cercare, filtrare e ordinare le risorse.

I metadati vengono visualizzati in visualizzazione Dettagli insieme alle informazioni generate da Dynamic Media Classic, ad esempio la data di creazione del file, la data di pubblicazione e le parole chiave. Per visualizzare i metadati, aprite la risorsa in visualizzazione Dettagli e selezionate il pannello Metadati. In visualizzazione Dettagli potete immettere e modificare i metadati.

Alcuni metadati sono incorporati direttamente in un file. Se un file contiene questi metadati, Dynamic Media Classic li carica automaticamente con il file . È possibile incorporare i metadati nelle risorse di origine in Adobe Photoshop, InDesign, Illustrator e altre applicazioni; Dynamic Media Classic riconosce questi metadati. Potete inoltre aggiungere metadati ai singoli file nel pannello Metadati in visualizzazione Dettagli. Per assicurare coerenza tra le diverse risorse, gli amministratori della società possono creare dei modelli di metadati che forniscono i campi di metadati da compilare.

Per ulteriori informazioni sui metadati incorporati, consulta [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Visualizzare i metadati {#view-metadata}

Per visualizzare i metadati di una risorsa, apri la risorsa in visualizzazione Dettagli e tocca il pannello Metadati . Per selezionare un set di campi di metadati, scegliete un’opzione dal menu Visualizzazione metadati. Dynamic Media Classic offre le seguenti visualizzazioni metadati:

* **Visualizzazione**
compattaElenco di valori di base.

* ****
IPTCValues come definito dal Consiglio internazionale delle telecomunicazioni per la stampa.

* ****
XMPValues come definito dalla piattaforma di metadati estensibile.

Gli amministratori possono creare ulteriori visualizzazioni di metadati, che vengono aggiunte al menu Visualizzazioni metadati. Per informazioni sulla creazione di visualizzazioni di metadati, consultate [Visualizzazione metadati](application-setup.md#metadata_views).

## Immettere manualmente i metadati per una risorsa  {#manually-enter-metadata-for-an-asset}

1. Aprite la risorsa in visualizzazione Dettagli.
1. Aprite il pannello Metadati ed effettuate una delle seguenti operazioni:

   * Scegliete una visualizzazione metadati per determinare quali campi di metadati sono disponibili nel pannello.
   * Scegliete un valore predefinito e fate clic su Applica per compilare i campi dei metadati con i valori impostati nel predefinito. I valori dei predefiniti vengono impostati dagli amministratori di società.

1. Immettete i valori nel pannello Metadati.

>[!NOTE]
>
>Per modificare i metadati di più risorse alla volta, selezionate le risorse e scegliete File > Modifica info. Le modifiche effettuate ai metadati nella finestra Modifica info vengono applicate a tutte le risorse selezionate.

## Aggiungere o modificare le parole chiave  {#add-or-edit-keywords}

Oltre ai metadati, è possibile utilizzare parole chiave per facilitare la ricerca e la gestione delle risorse.

Se durante la sessione di lavoro corrente avete aggiunto delle parole chiave ad altri file o ne avete rimosse alcune dall’elenco, queste vengono visualizzate nella tabella Suggerimenti parole chiave.

1. Aprite il file in visualizzazione Dettagli.
1. Fate clic su Parole chiave.
1. Per aggiungere delle parole chiave, effettuate una delle seguenti operazioni:

   * Digitate una parola chiave nella casella di testo e fate clic su Aggiungi.
   * Fate clic su una parola chiave nell’elenco Suggerimenti parole chiave.

1. Per rimuovere una parola chiave, selezionatela e fate clic su Rimuovi. Viene spostata nella tabella Suggerimenti parole chiave.

>[!NOTE]
>
>È possibile aggiungere parole chiave ai file durante il caricamento in Dynamic Media Classic. Nella finestra di dialogo Opzioni processo di caricamento, scegliete Metadati aggiunti e immettete le parole chiave. Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

## Importare i metadati  {#import-metadata}

Invece di immettere manualmente i metadati per una risorsa alla volta, potete importare i metadati per diverse risorse da un file XML o delimitato da tabulazioni. L’immissione dei metadati in un file XML o delimitato da tabulazioni e l’importazione di tale file risulta più rapida rispetto all’immissione dei metadati in singole risorse. Nella prima riga del file delimitato da tabulazioni, inserite l’ID e i nomi dei campi per i quali desiderate registrare i metadati. In ogni riga successiva, immettete il nome dell’ID della risorsa seguito dai valori di metadati. I campi non inclusi nel file XML o delimitato da tabulazioni non vengono modificati. Per importare metadati da un file XML, accertatevi che sia conforme al DTD.

>[!NOTE]
>
>Puoi creare un modello per l’immissione dei metadati in modo che possano essere importati correttamente in Dynamic Media Classic. Una volta creato il modello, utilizzatelo per immettere i metadati. Consultate [Creare un modello per l’immissione di metadati da caricare](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Per ulteriori informazioni sulle proprietà standardizzate, consulta: https://www.adobe.com/devnet/xmp.html

1. Nel pannello Sfoglia, selezionate le immagini a cui desiderate aggiungere dei metadati da un file XML o delimitato da tabulazioni.
1. Fate clic su **File** > **Importa metadati**.
1. Nella finestra di dialogo **Carica metadati**, fate clic su **Sfoglia**.
1. Nella finestra di dialogo **Seleziona file da caricare**, selezionate un file XML o delimitato da tabulazioni.
1. Immettete un nome per il processo.
1. Fate clic su **Carica**.

**Identificazione di tipi di metadati diversi in fase di importazione**

Tenete sempre presente quanto segue per identificare i diversi tipi di metadati da importare:

* I campi definiti dall’utente sono identificati dal nome creato in Configurazione > Impostazione applicazione > Metadati > Campi definiti dall’utente. Utilizzate la funzionalità di generazione file per ottenere un elenco di tutti i campi definiti dall’utente nel formato corretto di importazione.
* Il nome delle proprietà di metadati XMP deve essere preceduto dal relativo prefisso XMP. Il prefisso e il nome sono separati dal segno due punti (:). Il prefisso XMP si trova in Configurazione > Impostazione applicazione > Metadati > Schema metadati. I nomi tecnici si trovano nella documentazione del relativo schema XMP. I nomi delle proprietà XMP non vengono visualizzati nella funzione Genera file.
* Il nome delle proprietà Schema metadati deve essere preceduto dal relativo prefisso. Il prefisso e il nome sono separati dal segno due punti (:). Il prefisso e i nomi delle proprietà sono definiti nell’editor Schema metadati. I nomi delle proprietà dello schema metadati non vengono visualizzati nella funzione Genera file.

Ad esempio: la proprietà XMP per le parole chiave è composta dal prefisso “dc” dello schema XMP “Dublin Core” e dal nome tecnico XMP “subject”. Il prefisso e il nome tecnico XMP vengono combinati per ottenere il nome proprietà completo “dc:subject”. Nel formato di importazione di metadati XML, “dc.subject” deve essere il nome della proprietà. Nel formato di importazione delimitato da tabulazioni, deve essere l’intestazione della colonna.

**Importare parole chiave**

Le parole chiave possono essere importate come elenco separato da virgole. Se una virgola viene visualizzata in uno qualsiasi dei singoli valori, deve essere preceduta da una barra inversa (\). Un segno di barra rovesciata deve essere invece riportato come doppia barra rovesciata (\\).

Ad esempio, un file di importazione di metadati contenente il valore “Hello\, World!,back\\slash,foo” per “dc:subject” imposta tre parole chiave XMP sulla risorsa: “Hello, World!”, “back\slash” e “foo”.

**Importare file XMP di metadati XMP e Schema metadati**

L’importazione XML accetta solo dati XML validi. Quando si importano campi XMP o Schema metadati, il prefisso dello spazio dei nomi viene aggiunto e si comporta in questo modo come uno spazio dei nomi XMP. Questo spazio dei nomi deve essere dichiarato. Ad esempio, nel tag di primo livello.

Ad esempio:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Importare file delimitati da tabulazioni per metadati XMP e Schema metadati**

Il prefisso deve essere aggiunto alla relativa intestazione di colonna del campo da importare.

## Importare metadati (tramite FTP)  {#import-metadata-via-ftp}

Per importare metadati relativi a più file, immetteteli nel file XML o delimitato da tabulazioni e selezionate Elabora file di metadati nella schermata Carica (tramite FTP).

Accertatevi che i dati presenti nel file XML o delimitato da tabulazioni siano nel formato corretto. Nella prima riga, immettete il campo ID seguito dai nomi dei campi di metadati da modificare. In ogni riga successiva, immettete il nome dell’ID della risorsa seguito dai valori di metadati. I campi non inclusi nel file XML o delimitato da tabulazioni non vengono modificati.

Fai clic sul pulsante Carica nella barra di navigazione globale. Per importare i metadati, nella schermata Processi selezionare la scheda **[!UICONTROL Tramite FTP]**, quindi fare clic su **[!UICONTROL Opzioni processo]**. Nella finestra di dialogo Opzioni processo di caricamento , scegli Elabora file di metadati.

## Rinominare gli ID in batch tramite metadati {#batch-rename-ids-using-metadata}

Utilizzando i metadati importati da un file o file XML con valori delimitati da tabulazioni, puoi rinominare gli ID di Dynamic Media Classic. I metadati importati vengono applicati solo alle immagini specificate nel file di metadati. Non occorre quindi selezionare le immagini nel pannello Sfoglia.

Per rinominare l’ID Dynamic Media Classic di un’immagine, aggiungi una colonna con etichetta *newipsid* al file delimitato da tabulazioni oppure aggiungi un campo denominato* new_vc_objectname* ai dati XML.

Ad esempio:

| ipsid | newipsid |
|--- |--- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

Il registro dei processi per il processo Metadati mostra quali ID sono stati rinominati correttamente e quali no.

## Creare un modello per l’immissione di metadati da caricare.{#create-a-template-for-entering-metadata-to-upload}

Dynamic Media Classic offre un comando per la creazione di un modello per la registrazione dei metadati. L’utilizzo del modello assicura che i metadati siano immessi nel formato corretto e possano essere caricati correttamente in Dynamic Media Classic. Per creare un modello da utilizzare per la registrazione e l’importazione di metadati in Dynamic Media Classic, effettua le seguenti operazioni:

1. Selezionate le risorse immagini contenenti i campi di metadati che desiderate inserire nel modello.
1. Scegliete File > Importa metadati.
1. Per il tipo di proprietà risorsa, selezionate Immagine.
1. Nel menu Genera file scegliete Modello delimitato da tabulazioni, Metadati XML della risorsa o DTD XML.
1. Fate clic su Genera.
1. Nella finestra di dialogo risultante, copiate i dati. Utilizzate tali dati per definire il modello.

## Operazioni con gli schemi di metadati {#working-with-metadata-schemas}

Un amministratore di società può visualizzare un elenco di tutti gli schemi disponibili. Aprite Impostazione applicazione > Metadati > Schema metadati.

Inizialmente, l’elenco degli schemi standard globali come XMP è nascosto. Per visualizzarli, usate la casella di selezione in fondo all’elenco.

L’amministratore dell’azienda può creare uno schema personalizzato o modificare uno schema personalizzato esistente.

Potete utilizzare l’Editor schema metadati per effettuare le operazioni seguenti:

| Azione | Descrizione |
|--- |--- |
| Aggiungi | Aggiunge una proprietà allo schema. Una finestra di dialogo modale raccoglie le informazioni: ID, etichetta, struttura e tipo di dati. |
| Aggiungi valore di scelta | Aggiunge una nuova scelta selezionabile a una proprietà con struttura Scelta aperta o Scelta chiusa. Tutti i valori di scelta sono dello stesso tipo. Seleziona la proprietà stessa per abilitare il pulsante. |
| Modifica | Modifica l’etichetta di una proprietà o di un valore di scelta. Potete modificare solo le informazioni di Etichetta e ID; Tipo non è modificabile. |
| Sposta in alto/Sposta in basso | L’ordine impostato nello schema viene rispecchiato nell’interfaccia utente. Per modificare l’ordine, selezionate una proprietà o un valore di scelta e utilizzate questi pulsanti. Al momento il trascinamento non è supportato. |
| Elimina | Elimina dallo schema una proprietà o un valore di scelta. Non elimina i valori dal blocco XMP o dal database. La proprietà non è più disponibile per le visualizzazioni metadati e viene rimossa dalla vista Dettagli risorsa. Se la proprietà è stata pubblicata sul server metadati, eseguire una pubblicazione forzata per rimuovere i dati dal server metadati rivolto al pubblico. |

Il sistema genera automaticamente uno schema personalizzato per i campi definiti dall’utente con il prefisso “s7udf”. Si tratta di campi definiti dall’utente esistenti e vengono modificati nella relativa sezione Configurazione.

>[!NOTE]
>
>le modifiche apportate allo schema non modificano mai i metadati stessi delle risorse. Tuttavia, non sono visibili per tutte le funzionalità di Dynamic Media Classic e del server metadati e non è possibile accedervi dopo la modifica. Analogamente, se esistono metadati per una risorsa, la creazione dello schema corrispondente rende i metadati utilizzabili in Dynamic Media Classic e nel server metadati.

L’Editor schema metadati offre un modo grafico per aggiungere o modificare uno schema aziendale personalizzato in Dynamic Media Classic. Uno schema è definito da un prefisso, uno spazio nomi e un elenco di proprietà.

* Nome

   Nome dello schema per l’interfaccia utente. Utilizzato per identificare le proprietà in nelle visualizzazioni metadati e in Ricerca avanzata. Simile alle sezioni XMP come ad esempio Base, IPTC, PDF.

* Prefisso

   Identificatore univoco tecnico per lo schema. Limitato alle lettere a-z e A-Z. Il prefisso non è visibile nell’interfaccia utente di Dynamic Media Classic, ma viene utilizzato quando i metadati di una risorsa vengono memorizzati nel blocco XMP e nel database. Il prefisso viene utilizzato per identificare in modo univoco i campi di metadati per le ricerche metadati nel server metadati o per l’importazione.

* Spazio nome

   Identificatore univoco tecnico per lo schema, in genere un URL nel modulo `https://your.company.com/name/version/`. Per degli esempi, consultate l’elenco degli schemi standard. Lo spazio dei nomi non è visibile nell’interfaccia utente di Dynamic Media Classic, ma viene utilizzato per memorizzare i metadati nel blocco XMP.

* Descrizione

   Descrizione libera dello schema.

>[!NOTE]
>
>il prefisso e lo spazio nomi non possono essere modificati. Per modificare queste proprietà, è necessario eliminare e ricreare lo schema.

Le proprietà descrivono i metadati che possono essere memorizzati con questo schema nel blocco XMP. Una proprietà è costituita da:

| Proprietà | Descrizione |
|--- |--- |
| ID | Identificatore tecnico della proprietà. L’ID non è visibile nell’interfaccia utente di Dynamic Media Classic, ma viene utilizzato quando i metadati di una risorsa vengono memorizzati nel blocco XMP e nel database. L’ID viene utilizzato per creare query di ricerca nel server metadati. L’ID presenta alcune restrizioni: <ul><li>Non può contenere spazi</li><li>Non può contenere &quot;.&quot;, &quot;:&quot;, &quot;$&quot;</li><li>Non può contenere un numero come primo carattere</li><li>Come primo carattere si consiglia di utilizzare una lettera a-z o A-Z</li></ul> <br>Una volta creato, l’ID non può essere modificato. |
| Etichetta | Nome della proprietà per l’interfaccia utente. |
| Struttura | Determina il tipo di proprietà e il tipo di dati. La struttura può essere:<ul><li>Tipo semplice: valore singolo di tipo di dati</li><li>Sequenza: elenco di valori dello stesso tipo di dati</li><li>Scelta aperta: selezionate una voce da un elenco di valori predefiniti, oppure immettete del testo a scelta. Può essere solo di tipo Stringa o Intero</li><li>Scelta chiusa: selezionate una voce da un elenco di valori predefiniti (casella a comparsa o elenco di scelta)</li></ul> |
| Tipo di dati | Selezionate tra i seguenti tipi disponibili: <ul><li>Stringa</li><li>Intero</li><li>Virgola mobile</li><li>Sì/No (booleano)</li><li>Data</li></ul> |


Quando la struttura della proprietà è Scelta aperta o Scelta chiusa, immettete almeno un valore di scelta. Un valore di Scelta aperta può essere modificato. Un valore di Scelta chiusa non può essere modificato. Tutti i valori di scelta hanno lo stesso tipo di dati della proprietà.

| Proprietà | Descrizione |
|--- |--- |
| ID | Identificatore tecnico del valore. L’ID non è visibile nell’interfaccia utente di Dynamic Media Classic, ma viene utilizzato quando i metadati di una risorsa vengono memorizzati nel blocco XMP e nel database. L’ID viene utilizzato nelle query di ricerca nel server metadati. L’ID non può contenere spazi. Una volta creato, l’ID non può essere modificato. |
| Etichetta | Nome del valore per l’interfaccia utente. |

>[!MORELIKETHIS]
>
>* [Predefiniti per visualizzatori](application-setup.md#viewer_presets)
>* [Predefiniti per metadati](application-setup.md#metadata_presets)

