---
title: Verifica delle risorse prima di renderle pubbliche
seo-title: Verifica delle risorse prima di renderle pubbliche
description: 'null'
seo-description: Scoprite come verificare le risorse prima di renderle pubbliche.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 54%

---


# Verifica delle risorse prima di renderle pubbliche {#testing-assets-before-making-them-public}

La funzione di verifica consente di definire un ambiente di verifica protetto e di creare una solida soluzione B2B, in base a una serie di indirizzi e intervalli IP configurabili. Questa funzionalità consente di far corrispondere le distribuzioni Dynamic Media Classic all&#39;architettura della piattaforma di gestione dei contenuti e di e-commerce.

La verifica protetta consente di visualizzare in anteprima una versione per uso interno del sito Web, con contenuti non ancora pubblicati.

Può essere preferibile creare un ambiente di pubblicazione protetta per solo uso interno anziché rendere le risorse disponibili pubblicamente per i seguenti motivi:

* Anteprima di siti Web prima del lancio effettivo (pubblicazione protetta a scopo di verifica).
* Trasmissione di risorse per accesso limitato, ad esempio eCatalog che mostrano i prezzi in un’applicazione Web B2B.
* Utilizzo di risorse all’interno di un firewall come parte di un sistema di gestione delle informazioni sui prodotti, di un’applicazione per il servizio di assistenza clienti, di un sito di formazione e così via.

>[!NOTE]
>
>La verifica protetta non influisce sull&#39;accesso ad Dynamic Media Classic. La protezione di Dynamic Media Classic rimane coerente e richiede le normali credenziali per l&#39;accesso ad Dynamic Media Classic e ai servizi Web correlati.

## Funzionamento della verifica protetta {#how-secure-testing-works}

Per la maggior parte delle società le connessioni Internet avvengono mediante un firewall. L’accesso a Internet è possibile tramite alcuni indirizzamenti e in genere con una serie limitata di indirizzi IP pubblici.

Dalla rete aziendale, potete risalire all’indirizzo IP pubblico utilizzando siti Web come https://whatismyip.com o richiedendo tali informazioni all’organizzazione IT aziendale.

Con la verifica protetta, Dynamic Media Classic stabilisce un server di immagini dedicato per gli ambienti di pubblicazione protetta o le applicazioni interne. Per tutte le richieste inviate a questo server viene controllato l’indirizzo IP di origine. Se la richiesta non proviene dall’elenco di indirizzi IP approvato, viene restituita una risposta di operazione non riuscita. L’amministratore di Dynamic Media Classic Company configura l’elenco approvato di indirizzi IP per l’ambiente di verifica protetta della propria azienda.

Poiché la posizione della richiesta originale deve essere confermata, il traffico del servizio di verifica protetta non viene instradato attraverso una rete di distribuzione del contenuto come il traffico pubblico del server immagini Dynamic Media. Le richieste al servizio di verifica protetta potrebbero presentare una latenza leggermente superiore rispetto ai server immagini pubblici di Dynamic Media.

Le risorse non pubblicate sono immediatamente disponibili dai servizi di verifica protetta, senza dover essere pubblicati. Potete così visualizzare un’anteprima delle risorse prima che vengano pubblicate sul server immagine pubblico.

***nota **: I servizi di verifica protetta utilizzano il server catalogo configurato con contesto di pubblicazione interno. Pertanto, se la società è configurata per la pubblicazione in modalità di verifica protetta, tutte le risorse caricate in Dynamic Media Classic diventano immediatamente disponibili nei servizi di verifica protetta. Questa funzionalità è valida sia per le risorse contrassegnate per la pubblicazione al momento del caricamento che per quelle che non lo sono.*

I servizi di verifica protetta al momento supportano i seguenti tipi di risorse e funzionalità:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Immagini.
* Vignettature (richieste per il server di rendering).
* Richieste del server di rendering (supportate, ma richieste esplicitamente dal cliente).
* Set, compresi i set di immagini, eCatalog, set di rendering e set di file multimediali.
* Visualizzatori Dynamic Media Classic per contenuti multimediali avanzati standard.
* Pagine Dynamic Media Classic OnDemand JSP.
* Contenuto statico, ad esempio file PDF e video progressivi.
* Streaming video HTTP.
* Streaming di video progressivo.

I seguenti tipi di risorse e funzionalità non sono attualmente supportati:

* Streaming video RTMP
* Servizi UGC
* Web-stampa
* Ricerca in informazioni classiche Dynamic Media o eCatalog

## Verifica del servizio di verifica protetta {#testing-the-secure-testing-service}

È consigliabile verificare il servizio di verifica protetta per controllare che funzioni correttamente.

Nota: Se non viene indicato alcun IP in Configurazione > Impostazione pubblicazione > Server immagini > Test Image Service
se aggiungete solo un IP, l’IP sarà in grado di chiamare le risorse e nessun altro IP potrà effettuare le chiamate. Finché non viene menzionato alcun IP in quella sezione, tutti gli IP possono effettuare le chiamate per le risorse e verranno visualizzati.

**Preparare l’account**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Contattate l’assistenza tecnica e richiedete l’attivazione del servizio di verifica protetta per il vostro account.
1. In Dynamic Media Classic, fate clic su **Configurazione** > **Impostazione pubblicazione** > **Server immagini**.
1. Nella pagina Pubblica su Image Server, nell’elenco a discesa Contesto di pubblicazione, selezionate l’opzione per la **verifica del server immagini**.
1. Per Filtro indirizzi client, fate clic su **Aggiungi**.
1. Selezionate la casella di controllo per attivare l’indirizzo e digitate un indirizzo IP e una maschera di rete nei rispettivi campi.

   >[!NOTE]
   >
   >Se aggiungete un indirizzo IP singolo e una maschera di rete, tale indirizzo può effettuare chiamate alle risorse. Tuttavia, a tutti gli altri indirizzi IP e maschere di rete aggiunti non è consentito effettuare chiamate di risorse. È quindi possibile disattivare (disattivare) la casella di controllo del passaggio precedente per disattivare la possibilità di specificare un indirizzo IP e una maschera di rete. In questo modo, tutti gli indirizzi *tutti* IP possono effettuare chiamate alle risorse e verranno visualizzati.

1. Effettuate una delle seguenti operazioni:
   * Ripete questi due passaggi per aggiungere altri indirizzi IP.
   * Passate al passaggio successivo.
1. In basso a sinistra nella pagina Pubblica su Image Server, fate clic su **Salva**
1. Caricate le immagini desiderate nel vostro account Dynamic Media Classic.

   Consultate [Caricamento dei file](uploading-files.md#uploading_files).

1. Accertatevi che alcune delle immagini siano contrassegnate per la pubblicazione e altre non lo siano, quindi inviate il processo di pubblicazione.

   Consultate [Pubblicazione](publishing-files.md#publishing_files).

1. Determinate il nome del servizio di verifica protetta facendo clic su **Configurazione** > **Impostazione applicazione** > **Impostazioni generali**.
1. Nella pagina Impostazioni generali applicazione, nella sezione Server, individuate il nome a destra di **Nome server contesto pubblicazione di prova**.

Contatta  Adobe se il nome del server risulta mancante o se gli URL del server non funzionano.

**Preparare le varianti del sito Web**

È necessario disporre di due varianti di un sito Web, con collegamenti alle risorse pubblicate e a quelle non pubblicate:

* Versione pubblica - Collegate le risorse utilizzando la normale sintassi URL di Dynamic Media Classic.
* Versione di verifica: collegate le risorse con la stessa sintassi ma con il nome del sito di verifica protetta.

**Eseguire le verifiche**

Eseguite le seguenti verifiche:

1. Controllate che le risorse siano visibili nella rete aziendale.

   Dall’interno della rete aziendale identificata dall’intervallo di indirizzi IP precedentemente definito, nella versione di verifica del sito Web devono essere visualizzate tutte le immagini, sia quelle contrassegnate per la pubblicazione che quelle che non lo sono. Questo vi permette di effettuare la verifica senza correre il rischio rendere le immagini disponibili prima dell’approvazione o del lancio di un prodotto.

   Verificate che la versione pubblica del sito contenga le risorse pubblicate come precedentemente sperimentato con Dynamic Media Classic.

1. Dall’esterno della rete aziendale, verificate che non sia possibile a terzi accedere alle risorse non pubblicate (cioè quelle non contrassegnate per la pubblicazione).

   Accedete alla rete dall’esterno (ad esempio, dal vostro computer di casa o da una connessione 3G), quindi verificate che la versione pubblica del sito contenga tutte le risorse pubblicate ma nessuno dei contenuti non pubblicati.

   Confermate che la versione di verifica non contenga alcuna risorsa, poiché state tentando di accedere al servizio di verifica protetta da un indirizzo IP non autorizzato.

