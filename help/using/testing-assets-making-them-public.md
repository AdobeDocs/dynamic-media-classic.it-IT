---
title: Testare le risorse prima di renderle pubbliche
description: Scopri come testare le risorse in Adobe Dynamic Media Classic prima di renderle pubbliche.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 19%

---

# Testare le risorse prima di renderle pubbliche {#testing-assets-before-making-them-public}

Secure Testing consente di definire un ambiente di test sicuro e di creare una soluzione B2B solida, basata su un set configurabile di indirizzi IP e intervalli. Questa funzionalità consente di abbinare le implementazioni di Adobe Dynamic Media Classic all&#39;architettura del sistema di gestione dei contenuti e del sistema aziendale.

La verifica protetta consente di visualizzare in anteprima una versione per uso interno del sito Web, con contenuti non ancora pubblicati.

Se lo desideri, crea un ambiente di staging anziché rendere le risorse disponibili al pubblico per i seguenti motivi:

* Anteprima di siti Web prima del lancio effettivo (pubblicazione protetta a scopo di verifica).
* Distribuisci le risorse che richiedono un accesso limitato, ad esempio i cataloghi elettronici che mostrano i prezzi in un’applicazione web B2B.
* Utilizza le risorse dietro un firewall come parte di un sistema di gestione delle informazioni sui prodotti, di un&#39;applicazione di assistenza clienti, di un sito di formazione e così via.

>[!NOTE]
>
>Il test protetto non influisce sull’accesso a Adobe Dynamic Media Classic. La sicurezza di Adobe Dynamic Media Classic rimane coerente e richiede le credenziali abituali per accedere a Adobe Dynamic Media Classic e ai servizi Web correlati.

## Funzionamento della verifica protetta {#how-secure-testing-works}

Per la maggior parte delle società le connessioni Internet avvengono mediante un firewall. L’accesso a Internet è possibile tramite alcuni indirizzamenti e in genere con una serie limitata di indirizzi IP pubblici.

Dalla rete aziendale è possibile individuare l&#39;indirizzo IP pubblico utilizzando siti Web come [https://www.whatismyip.com](https://www.whatismyip.com/) o richiedere queste informazioni all&#39;organizzazione IT aziendale.

Con il Secure Testing, Adobe Dynamic Media Classic crea un server immagini dedicato per ambienti di staging o applicazioni interne. Per tutte le richieste inviate a questo server viene controllato l’indirizzo IP di origine. Se la richiesta in ingresso non si trova nell’elenco approvato di indirizzi IP, viene restituita una risposta di errore. L’amministratore aziendale di Adobe Dynamic Media Classic configura l’elenco approvato di indirizzi IP per l’ambiente di test protetto della propria azienda.

Poiché la posizione della richiesta originale deve essere confermata, il traffico del servizio di test protetto non viene instradato attraverso una rete di distribuzione del contenuto come il traffico pubblico del server immagini di Dynamic Medie. Le richieste al servizio di test sicuro hanno una latenza leggermente superiore rispetto ai server immagini Dynamic Medie pubblici.

Le risorse non pubblicate sono immediatamente disponibili dai servizi di verifica protetta, senza dover essere pubblicati. In questo modo, puoi eseguire un’anteprima prima che le risorse vengano pubblicate sul loro server immagini rivolto al pubblico.

>[!NOTE]
>
>I servizi di test sicuri utilizzano il server di catalogo configurato con un contesto di pubblicazione interno. Pertanto, se l’azienda è configurata per la pubblicazione su Secure Testing, tutte le risorse caricate in Adobe Dynamic Media Classic sono immediatamente disponibili su Secure Testing Services. Questa funzionalità è true indipendentemente dal fatto che le risorse siano contrassegnate per la pubblicazione al caricamento.

I servizi di test sicuro supportano attualmente i seguenti tipi di risorse e funzionalità:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved "Render Server requests" from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Immagini.
* Vignettature (richieste per il server di rendering).
* Richieste di rendering del server (supportate, ma il cliente deve richiederle esplicitamente)
* Set, compresi i set di immagini, eCatalog, set di rendering e set di file multimediali.
* Visualizzatori rich media Adobe Dynamic Media Classic standard.
* Pagine JSP di Adobe Dynamic Media Classic OnDemand.
* Contenuto statico, ad esempio file PDF e video progressivi.
* Streaming video HTTP.
* Streaming di video progressivo.

I seguenti tipi di risorse e funzionalità non sono attualmente supportati:

* Ricerca in Adobe Dynamic Media Classic Info o eCatalog
* Streaming video RTMP
* Web-stampa
* Servizi UGC (User-Generated Content)

>[!IMPORTANT]
>
>Il supporto per risorse di immagini vettoriali UGC nuove o esistenti in Adobe Dynamic Media Classic è terminato il 30 settembre 2021.

## Test del servizio di test protetto {#testing-the-secure-testing-service}

Esegui il test del servizio di test protetto in modo da assicurarti che funzioni come previsto.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]***: If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### Preparare l’account

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under "Prepare your account" 9/10/2012</p>

 -->

1. Contatta l’Assistenza clienti Adobe e richiedi l’abilitazione di Secure Testing sul tuo account.
1. In Adobe Dynamic Media Classic, sulla barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Installazione di Publish]** > **[!UICONTROL Server immagini]**.
1. Nella pagina Publish di Image Server selezionare **[!UICONTROL Test Image Server]** dall&#39;elenco a discesa **[!UICONTROL `Publish Context`]**.
1. Per Filtro indirizzi client, selezionare **[!UICONTROL Aggiungi]**.
1. Selezionare la casella di controllo in modo che l&#39;indirizzo sia attivato, quindi digitare un indirizzo IP e una maschera di rete nei rispettivi campi di testo.

   >[!NOTE]
   >
   >Se aggiungi un singolo indirizzo IP e una maschera di rete, tale indirizzo può effettuare chiamate alle risorse. Tuttavia, gli altri indirizzi IP e le maschere di rete aggiunti non possono effettuare chiamate alle risorse. È pertanto consigliabile disattivare (disattivare) la casella di controllo del passaggio precedente per disattivare la possibilità di specificare un indirizzo IP e una maschera di rete. In questo modo, *tutti* gli indirizzi IP possono effettuare chiamate alle risorse e vengono visualizzati tutti.

1. Effettuate una delle seguenti operazioni:
   * Se devi aggiungere altri indirizzi IP, ripeti i due passaggi precedenti.
   * Procedi al passaggio successivo.
1. Nella parte inferiore sinistra della pagina Image Server Publish, seleziona **[!UICONTROL Salva]**
1. Carica le immagini desiderate sul tuo account Adobe Dynamic Media Classic.

   Vedi [Carica file](uploading-files.md#uploading_files).

1. Assicurarsi che alcune immagini siano contrassegnate per la pubblicazione e altre non siano contrassegnate, quindi inviare il processo di pubblicazione.

   Vedi [file Publish](publishing-files.md#publishing_files).

1. Determinare il nome del servizio di test protetto scegliendo **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Impostazioni generali]**.
1. Nella pagina Impostazioni generali applicazione, nella sezione Server, individuate il nome a destra di **[!UICONTROL Nome server contesto pubblicazione di prova]**.

Contatta l’Assistenza Adobe se il nome del server non è presente o se gli URL del server non funzionano.

### Preparare le varianti del sito Web

È necessario disporre di due varianti di un sito Web, con collegamenti alle risorse pubblicate e a quelle non pubblicate:

* Versione pubblica: collega le risorse utilizzando la sintassi URL tradizionale di Adobe Dynamic Media Classic.
* Versione di staging: collega le risorse utilizzando la stessa sintassi ma con il nome del sito di test protetto.

### Eseguire le verifiche

Eseguite le seguenti verifiche:

1. Controllate che le risorse siano visibili nella rete aziendale.

   All’interno della rete aziendale identificata dall’intervallo di indirizzi IP definito in precedenza, nella versione di staging del sito web vengono visualizzate tutte le immagini, contrassegnate per la pubblicazione o meno. Di conseguenza, è possibile eseguire il test senza rendere accidentalmente disponibili le immagini prima dell’approvazione in anteprima o del lancio del prodotto.

   Verifica che la versione pubblica del sito mostri le risorse pubblicate come precedentemente fatto con Adobe Dynamic Media Classic.

1. All’esterno della rete aziendale, verifica che le risorse non pubblicate (ossia, non contrassegnate per la pubblicazione) siano protette dall’accesso di terze parti.

   Accedi alla rete dall’esterno (ad esempio dal computer di casa o tramite una connessione 3G), quindi verifica che nella versione pubblica del sito siano visualizzate tutte le risorse pubblicate ma nessun contenuto non pubblicato.

   Confermate che la versione di verifica non contenga alcuna risorsa, poiché state tentando di accedere al servizio di verifica protetta da un indirizzo IP non autorizzato.
