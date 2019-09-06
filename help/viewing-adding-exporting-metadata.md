---
title: Visualizzazione, aggiunta ed esportazione di metadati
seo-title: Visualizzazione, aggiunta ed esportazione di metadati
description: 'null'
seo-description: Scoprite come visualizzare, aggiungere ed esportare i metadati.
uuid: a 5254 c 51-9 e 04-45 ae -8236-3 eab 2925 e 5 fc
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: 5414 b 4 f 5-6 e 05-468 c -8725-385423596342
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Visualizzazione, aggiunta ed esportazione di metadati{#viewing-adding-and-exporting-metadata}

Potete memorizzare informazioni specifiche sui file usati in Scene7 Publishing System; tali informazioni sono dette *metadati*. Potete usare i metadati in Dynamic Media Classic per organizzare, cercare, filtrare e ordinare le risorse.

I metadati vengono visualizzati in visualizzazione Dettagli insieme alle informazioni generate da Dynamic Media Classic, ad esempio data di creazione file, data di pubblicazione e parole chiave. Per visualizzare i metadati, aprite la risorsa in visualizzazione Dettagli e selezionate il pannello Metadati. In visualizzazione Dettagli potete immettere e modificare i metadati.

Alcuni metadati sono incorporati direttamente in un file. Se un file contiene tali metadati, Dynamic Media Classic lo carica automaticamente con il file. Potete incorporare i metadati nelle risorse sorgente in Adobe Photoshop, indesign, Illustrator e altre applicazioni; Dynamic Media Classic riconosce tali metadati. Potete inoltre aggiungere metadati ai singoli file nel pannello Metadati in visualizzazione Dettagli. Per assicurare coerenza tra le diverse risorse, gli amministratori della società possono creare dei modelli di metadati che forniscono i campi di metadati da compilare.

For more information about embedded metadata, see [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Visualizzare i metadati {#view-metadata}

Per visualizzare i metadati di una risorsa, apritela in visualizzazione Dettagli e fate clic sul pannello Metadati. Quindi scegliete un’opzione nel menu Visualizzazioni metadati per selezionare un set di campi di metadati. Dynamic Media Classic offre queste visualizzazioni metadati:

**Vista compatta** Un elenco di valori di base.

**Valori IPTC** come definiti dall'International Press Telecommunications Council.

**Valori XMP** come definiti dall'extensible metadata platform.

Gli amministratori possono creare ulteriori visualizzazioni di metadati, che vengono aggiunte al menu Visualizzazioni metadati. Per informazioni sulla creazione di visualizzazioni di metadati, consultate [Visualizzazione metadati](application-setup.md#metadata_views).

## Immettere manualmente i metadati per una risorsa {#manually-enter-metadata-for-an-asset}

1. Aprite la risorsa in visualizzazione Dettagli.
1. Aprite il pannello Metadati ed effettuate una delle seguenti operazioni:

   * Scegliete una visualizzazione metadati per determinare quali campi di metadati sono disponibili nel pannello.
   * Scegliete un valore predefinito e fate clic su Applica per compilare i campi dei metadati con i valori impostati nel predefinito. I valori dei predefiniti vengono impostati dagli amministratori di società.

1. Immettete i valori nel pannello Metadati.

>[!NOTE]
>
>Per modificare i metadati di più risorse alla volta, selezionate le risorse e scegliete File &gt; Modifica info. Le modifiche effettuate ai metadati nella finestra Modifica info vengono applicate a tutte le risorse selezionate.

## Aggiungere o modificare le parole chiave {#add-or-edit-keywords}

Oltre ai metadati, potete facilitare la ricerca e la gestione delle risorse mediante l’uso di parole chiave.

Se durante la sessione di lavoro corrente avete aggiunto delle parole chiave ad altri file o ne avete rimosse alcune dall’elenco, queste vengono visualizzate nella tabella Suggerimenti parole chiave.

1. Aprite il file in visualizzazione Dettagli.
1. Fate clic su Parole chiave.
1. Per aggiungere delle parole chiave, effettuate una delle seguenti operazioni:

   * Digitate una parola chiave nella casella di testo e fate clic su Aggiungi.
   * Fate clic su una parola chiave nell’elenco Suggerimenti parole chiave.

1. Per rimuovere una parola chiave, selezionatela e fate clic su Rimuovi. Viene spostata nella tabella Suggerimenti parole chiave.

>[!NOTE]
Potete aggiungere parole chiave ai file mentre le caricate in Dynamic Media Classic. Nella finestra di dialogo Opzioni processo di caricamento, scegliete Metadati aggiunti e immettete le parole chiave. Consultate [Opzioni di caricamento](uploading-files.md#upload_options).

## Importare i metadati {#import-metadata}

Invece di immettere manualmente i metadati per una risorsa alla volta, potete importare i metadati per diverse risorse da un file XML o delimitato da tabulazioni. L’immissione dei metadati in un file XML o delimitato da tabulazioni e l’importazione di tale file risulta più rapida rispetto all’immissione dei metadati in singole risorse. Nella prima riga del file delimitato da tabulazioni, inserite l’ID e i nomi dei campi per i quali desiderate registrare i metadati. In ogni riga successiva, immettete il nome dell’ID della risorsa seguito dai valori di metadati. I campi non inclusi nel file XML o delimitato da tabulazioni non vengono modificati. Per importare metadati da un file XML, accertatevi che sia conforme al DTD.

>[!NOTE]
potete creare un modello per l’immissione dei metadati per facilitarne l’importazione corretta in Scene7 Publishing System. Una volta creato il modello, utilizzatelo per immettere i metadati. Consultate [Creare un modello per l’immissione di metadati da caricare](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Puoi trovare ulteriori informazioni su proprietà standardizzate all'indirizzo: https://www.adobe.com/devnet/xmp.html

1. Nel pannello Sfoglia, selezionate le immagini a cui desiderate aggiungere dei metadati da un file XML o delimitato da tabulazioni.
1. Fate clic su **File** &gt; **Importa metadati**.
1. Nella finestra di dialogo **Carica metadati**, fate clic su **Sfoglia**.
1. Nella finestra di dialogo **Seleziona file da caricare**, selezionate un file XML o delimitato da tabulazioni.
1. Immettete un nome per il processo.
1. Fate clic su **Carica**.

**Identificazione di tipi di metadati diversi in fase di importazione**

Tenete sempre presente quanto segue per identificare i diversi tipi di metadati da importare:

* I campi definiti dall’utente sono identificati dal relativo nome, creato in Configurazione &gt; Impostazione applicazione &gt; Metadati &gt; Campi definiti dall’utente. Utilizzate la funzionalità di generazione file per ottenere un elenco di tutti i campi definiti dall’utente nel formato corretto di importazione.
* Il nome delle proprietà di metadati XMP deve essere preceduto dal relativo prefisso XMP. Il prefisso e il nome sono separati dal segno due punti (:). Il prefisso XMP si trova in Configurazione &gt; Impostazione applicazione &gt; Metadati &gt; Schema metadati. I nomi tecnici si trovano nella documentazione del relativo schema XMP. I nomi delle proprietà XMP non vengono visualizzati nella funzione Genera file.
* Il nome delle proprietà Schema metadati deve essere preceduto dal relativo prefisso. Il prefisso e il nome sono separati dal segno due punti (:). Il prefisso e i nomi delle proprietà sono definiti nell’editor Schema metadati. I nomi delle proprietà Schema metadati non vengono visualizzati nella funzione Genera file.

Ad esempio: la proprietà XMP per le parole chiave è composta dal prefisso “dc” dello schema XMP “Dublin Core” e dal nome tecnico XMP “subject”. Il prefisso e il nome tecnico XMP vengono combinati per ottenere il nome proprietà completo “dc:subject”. Nel formato di importazione di metadati XML, “dc.subject” deve essere il nome della proprietà. Nel formato delimitato da tabulazioni, queste deve essere usato come intestazione di colonna.

**Importare parole chiave**

Le parole chiave possono essere importate come un elenco separato da virgole. Se una virgola è utilizzata in uno dei valori, deve essere preceduta da una barra rovesciata (\). Un segno di barra rovesciata deve essere invece riportato come doppia barra rovesciata (\\).

Ad esempio, un file di importazione di metadati contenente il valore “Hello\, World!,back\\slash,foo” per “dc:subject” imposta tre parole chiave XMP sulla risorsa: “Hello, World!”, “back\slash” e “foo”.

**Importare file XMP di metadati XMP e Schema metadati**

L’importazione XML accetta solo dati XML validi. Quando importate dei campi XMP o Schema metadati, il prefisso dello spazio nomi viene aggiunto e si comporta come uno spazio nomi XMP. Questo spazio nomi deve essere dichiarato, ad esempio nel tag di primo livello.

Ad esempio:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Importare file delimitati da tabulazioni per metadati XMP e Schema metadati**

Il prefisso deve essere aggiunto alla relativa intestazione di colonna del campo da importare.

## Importare metadati (tramite FTP) {#import-metadata-via-ftp}

Per importare metadati relativi a più file, immetteteli nel file XML o delimitato da tabulazioni e selezionate Elabora file di metadati nella schermata Carica (tramite FTP).

Accertatevi che i dati presenti nel file XML o delimitato da tabulazioni siano nel formato corretto. Nella prima riga, immettete il campo ID seguito dai nomi dei campi di metadati da modificare. In ogni riga successiva, immettete il nome dell’ID della risorsa seguito dai valori di metadati. I campi non inclusi nel file XML o delimitato da tabulazioni non vengono modificati.

Fate clic sul pulsante Carica nella barra di navigazione globale e, nella schermata Processi, selezionate la scheda Mediante FTP per importare i metadati. Quindi fate clic su Opzioni processo. Nella finestra di dialogo Opzioni processo di caricamento, selezionate Elabora file di metadati.

## Rinominare gli ID in batch tramite metadati {#batch-rename-ids-using-metadata}

Utilizzando i metadati importati da un file XML o delimitato da tabulazioni potete rinominare gli ID di Scene7 Publishing System. I metadati importati vengono applicati solo alle immagini specificate nel file di metadati. Non occorre quindi selezionare le immagini nel pannello Sfoglia.

To rename an image’s Scene7 Publishing System ID, add a column labeled *newipsid* to the tab-delimited file, or add a field called* new_vc_objectname* to the XML data.

Ad esempio:

| ipsid | newipsid |
|--- |--- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |


Nel registro dei processi relativo al processo Metadati verranno visualizzati gli ID rinominati correttamente e quelli per i quali l’operazione non è riuscita.

## Creare un modello per l’immissione di metadati da caricare. {#create-a-template-for-entering-metadata-to-upload}

Dynamic Media Classic offre un comando per creare un modello per la registrazione di metadati. Quando si utilizza un modello, si è certi che i metadati immessi sono nel formato corretto e possono quindi essere caricati correttamente in Scene7 Publishing System. Per creare un modello per la registrazione e l’importazione di metadati in Scene7 Publishing System, effettuate le seguenti operazioni:

1. Selezionate le risorse immagini contenenti i campi di metadati che desiderate inserire nel modello.
1. Scegliete File &gt; Importa metadati.
1. Per il tipo di proprietà risorsa, selezionate Immagine.
1. Nel menu Genera file scegliete Modello delimitato da tabulazioni, Metadati XML della risorsa o DTD XML.
1. Fate clic su Genera.
1. Nella finestra di dialogo risultante, copiate i dati. Utilizzate tali dati per definire il modello.

## Operazioni con gli schemi di metadati {#working-with-metadata-schemas}

Un amministratore di società può visualizzare un elenco di tutti gli schemi disponibili. Aprite Impostazione applicazione &gt; Metadati &gt; Schema metadati.

Inizialmente, gli schemi standard globali come XMP sono nascosti. Per visualizzarli, usate la casella di selezione in fondo all’elenco.

L’amministratore di società può creare un nuovo schema personalizzato, oppure modificare uno schema personalizzato esistente.

Potete utilizzare l’Editor schema metadati per effettuare le operazioni seguenti:

| Azione | Descrizione |
|--- |--- |
| Aggiungi | Aggiunge una nuova proprietà allo schema. Una finestra di dialogo modale raccoglie le informazioni: ID, Etichetta, Struttura e Tipo di dati. |
| Aggiungi valore di scelta | Aggiunge una nuova scelta selezionabile a una proprietà con struttura Scelta aperta o Scelta chiusa. Tutti i valori di scelta sono dello stesso tipo. Per attivare il pulsante è necessario selezionare la proprietà stessa. |
| Modifica | Modifica l’etichetta di una proprietà o di un valore di scelta. Potete modificare solo le informazioni di Etichetta e ID; Tipo non è modificabile. |
| Sposta in alto/Sposta in basso | L’ordine impostato nello schema viene rispecchiato nell’interfaccia utente. Per modificare l’ordine, selezionate una proprietà o un valore di scelta e utilizzate questi pulsanti. Al momento non è possibile trascinare. |
| Elimina | Elimina dallo schema una proprietà o un valore di scelta. Questa operazione non elimina i valori dal blocco XMP o dal database. La proprietà non è più disponibile per le visualizzazioni di metadati e viene rimossa dalla vista dei dettagli delle risorse. Se la proprietà è stata pubblicata nel server di metadati, eseguite una pubblicazione forzata per rimuovere i dati dal server di metadati rivolto al pubblico. |

Il sistema genera automaticamente uno schema personalizzato per i campi definiti dall’utente con il prefisso “s7udf”. Questi sono i campi esistenti definiti dall’utente e possono essere modificati nella relativa sezione Configurazione.

>[!NOTE]
le modifiche apportate allo schema non modificano mai i metadati stessi delle risorse. Tuttavia, una volta modificati non sono più visibili nelle funzioni SPS e server di metadati e non è più possibile accedervi. Inoltre, se i metadati sono stati usati per una risorsa, la creazione dello schema corrispondente rende i metadati utilizzabili in SPS e nel server di metadati.

L’Editor schema metadati offre un metodo grafico per aggiungere o modificare uno schema personalizzato della società in SPS. Uno schema è definito da un prefisso, uno spazio nomi e un elenco di proprietà.

* Nome

   Nome dello schema per l’interfaccia utente. Utilizzato per identificare le proprietà in nelle visualizzazioni metadati e in Ricerca avanzata. Simile alle sezioni XMP come ad esempio Base, IPTC, PDF.

* Prefisso

   Identificatore univoco tecnico per lo schema. È possibile utilizzare solo lettere a-z e A-Z. Il prefisso non è visibile nell’interfaccia utente di SPS, ma viene utilizzato quando i metadati di una risorsa vengono salvati nel blocco XMP e nel database. Il prefisso viene utilizzato per identificare in modo univoco i campi di metadati per le ricerche metadati nel server metadati o per l’importazione.

* Spazio nome

   Identificatore univoco tecnico per lo schema, in genere un URL nel modulo `https://your.company.com/name/version/`. Per degli esempi, consultate l’elenco degli schemi standard. Lo spazio nomi non è visibile nell’interfaccia utente di SPS, ma viene utilizzato per archiviare i metadati nel blocco XMP.

* Descrizione

   Descrizione libera dello schema.

>[!NOTE]
il prefisso e lo spazio nomi non possono essere modificati. Per modificare queste proprietà, è necessario eliminare e ricreare lo schema.

Le proprietà descrivono i metadati che possono essere memorizzati con questo schema nel blocco XMP. Una proprietà è costituita da:

| Proprietà | Descrizione |
|--- |--- |
| ID | Identificatore tecnico della proprietà. L’ID non è visibile nell’interfaccia utente di SPS, ma è utilizzato quando i metadati di una risorsa vengono memorizzati nel blocco XMP e nel database. L’ID viene utilizzato per creare query di ricerca nel server metadati. L’ID presenta alcune restrizioni: <ul><li>Non può contenere spazi</li><li>Non può contenere ".", ":", "$"</li><li>Non può contenere un numero come primo carattere</li><li>Come primo carattere si consiglia di utilizzare una lettera a-z o A-Z</li></ul> <br>Una volta creato, l’ID non può essere modificato. |
| Etichetta | Nome della proprietà per l’interfaccia utente. |
| Struttura | Determina il tipo di proprietà e il tipo di dati. La struttura può essere:<ul><li>Tipo semplice: valore singolo di tipo di dati</li><li>Sequenza: elenco di valori dello stesso tipo di dati</li><li>Scelta aperta: selezionate una voce da un elenco di valori predefiniti, oppure immettete del testo a scelta. Può essere solo di tipo Stringa o Intero</li><li>Scelta chiusa: selezionate una voce da un elenco di valori predefiniti (casella a comparsa o elenco di scelta)</li></ul> |
| Tipo di dati | Selezionate tra i seguenti tipi disponibili: <ul><li>Stringa</li><li>Intero</li><li>Virgola mobile</li><li>Sì/No (booleano)</li><li>Data</li></ul> |


Quando la struttura della proprietà è Scelta aperta o Scelta chiusa, immettete almeno un valore di scelta. Un valore di Scelta aperta può essere modificato. Un valore di Scelta chiusa non può essere modificato. Tutti i valori di scelta hanno lo stesso tipo di dati della proprietà.

| Proprietà | Descrizione |
|--- |--- |
| ID | Identificatore tecnico del valore. L’ID non è visibile nell’interfaccia utente di SPS, ma è utilizzato quando i metadati di una risorsa vengono memorizzati nel blocco XMP e nel database. L’ID viene utilizzato nelle query di ricerca nel server metadati. L’ID non può contenere spazi. Una volta creato, l’ID non può essere modificato. |
| Etichetta | Nome del valore per l’interfaccia utente. |

>[!MORELIKETHIS]
* [Predefiniti per visualizzatori](application-setup.md#viewer_presets)
* [Predefiniti per metadati](application-setup.md#metadata_presets)
