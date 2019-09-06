---
title: Verifica delle risorse prima di renderle pubbliche
seo-title: Verifica delle risorse prima di renderle pubbliche
description: 'null'
seo-description: Scoprite come testare le risorse prima di renderle pubbliche.
uuid: 5 e 8 f 3 bec -6 cf 1-408 e -8 ea 1-aebde 0012 a 70
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/upload_ and_ publish_ assets
discoiquuid: 52 fadf 99-7 d 11-46 f 7-8483-a 9 f 87 ffc 2 f 67
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Verifica delle risorse prima di renderle pubbliche {#testing-assets-before-making-them-public}

La funzione di verifica consente di definire un ambiente di verifica protetto e di creare una solida soluzione B2B, in base a una serie di indirizzi e intervalli IP configurabili. Questa funzionalità vi consente di far corrispondere le implementazioni Dynamic Media Classic all'architettura della vostra piattaforma di gestione dei contenuti e di commerce.

La verifica protetta consente di visualizzare in anteprima una versione per uso interno del sito Web, con contenuti non ancora pubblicati.

Può essere preferibile creare un ambiente di pubblicazione protetta per solo uso interno anziché rendere le risorse disponibili pubblicamente per i seguenti motivi:

* Anteprima di siti Web prima del lancio effettivo (pubblicazione protetta a scopo di verifica).
* Trasmissione di risorse per accesso limitato, ad esempio eCatalog che mostrano i prezzi in un’applicazione Web B2B.
* Utilizzo di risorse all’interno di un firewall come parte di un sistema di gestione delle informazioni sui prodotti, di un’applicazione per il servizio di assistenza clienti, di un sito di formazione e così via.

>[!NOTE]
>
>la verifica protetta non influisce sull’accesso a Scene7 Publishing System. La protezione SPS rimane coerente e richiede le normali credenziali per l’accesso a SPS e ai servizi Web correlati.

## Funzionamento della verifica protetta {#how-secure-testing-works}

Per la maggior parte delle società le connessioni Internet avvengono mediante un firewall. L’accesso a Internet è possibile tramite alcuni indirizzamenti e in genere con una serie limitata di indirizzi IP pubblici.

Dalla rete aziendale, potete risalire all'indirizzo IP pubblico utilizzando siti Web come https://whatismyip.com o richiedendo tali informazioni al reparto IT aziendale.

Con la verifica protetta, Dynamic Media Classic stabilisce un server immagine dedicato per ambienti di staging o applicazioni interne. Per tutte le richieste inviate a questo server viene controllato l’indirizzo IP di origine. Se la richiesta non proviene dall’elenco di indirizzi IP approvato, viene restituita una risposta di operazione non riuscita. L'amministratore della società Dynamic Media Classic configura l'elenco di indirizzi IP approvati per l'ambiente di verifica protetta della propria azienda.

Poiché la posizione della richiesta originale deve essere confermata, il traffico del servizio di verifica protetta non viene instradato attraverso una rete di distribuzione dei contenuti come il traffico pubblico del server immagini Dynamic Media. Le richieste al servizio di verifica protetta potrebbero avere una latenza leggermente superiore rispetto ai server immagini Dynamic Media.

Le risorse non pubblicate sono immediatamente disponibili dai servizi di verifica protetta, senza dover essere pubblicati. Potete così visualizzare un’anteprima delle risorse prima che vengano pubblicate sul server immagine pubblico.

***Nota**: I servizi di verifica protetta utilizzano il server catalogo configurato con contesto di pubblicazione interna. Di conseguenza, se la società è configurata per la pubblicazione sul servizio di verifica protetta, eventuali risorse caricate in Scene7 Publishing System diventano immediatamente disponibili nei servizi di verifica protetta. Questa funzionalità è valida sia per le risorse contrassegnate per la pubblicazione al momento del caricamento che per quelle che non lo sono.*

I servizi di verifica protetta al momento supportano i seguenti tipi di risorse e funzionalità:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Immagini.
* Vignettature (richieste per il server di rendering).
* Richieste server di rendering (supportate, ma richieste esplicitamente dal cliente).
* Set, compresi i set di immagini, eCatalog, set di rendering e set di file multimediali.
* Visualizzatori Rich Media Classic standard per contenuti multimediali diversi.
* Pagine Dynamic Media Classic ondemand JSP.
* Contenuto statico, ad esempio file PDF e video progressivi.
* Streaming video HTTP.
* Streaming di video progressivo.

I seguenti tipi di risorse e funzionalità non sono attualmente supportati:

* Streaming video RTMP
* Servizi UGC
* Web-stampa
* Ricerca Dynamic Media Classic o ecatalog

## Verifica del servizio di verifica protetta {#testing-the-secure-testing-service}

È consigliabile verificare il servizio di verifica protetta per controllare che funzioni correttamente.

**Preparare l’account**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Contattate l’assistenza tecnica e richiedete l’attivazione del servizio di verifica protetta per il vostro account.
1. In Scene7 Publishing System, fate clic su **Configurazione** &gt; **Configurazione pubblicazione** &gt; **Image Server**.
1. Nella pagina Pubblica su Image Server, nell’elenco a discesa Contesto di pubblicazione, selezionate l’opzione per la **verifica del server immagini**.
1. Per Filtro indirizzi client, fate clic su **Aggiungi**.
1. Selezionate la casella di controllo per attivare l’indirizzo e digitate un indirizzo IP e una maschera di rete nei rispettivi campi.
1. Ripete questi due passaggi per aggiungere altri indirizzi IP. In caso contrario, continuate con il passaggio successivo.
1. In basso a sinistra nella pagina Pubblica su Image Server, fate clic su **Salva**
1. Caricate le immagini desiderate nel vostro account Scene7 Publishing System.

   Consultate [Caricamento dei file](uploading-files.md#uploading_files).

1. Accertatevi che alcune delle immagini siano contrassegnate per la pubblicazione e altre non lo siano, quindi inviate il processo di pubblicazione.

   Consultate [Pubblicazione](publishing-files.md#publishing_files).

1. Determinate il nome del servizio di verifica protetta facendo clic su **Configurazione** &gt; **Impostazione applicazione** &gt; **Impostazioni generali**.
1. Nella pagina Impostazioni generali applicazione, nella sezione Server, individuate il nome a destra di **Nome server contesto pubblicazione di prova**.

Se il nome del server risulta mancante o se gli URL del server non funzionano, rivolgetevi all’assistenza tecnica.

**Preparare le varianti del sito Web**

È necessario disporre di due varianti di un sito Web, con collegamenti alle risorse pubblicate e a quelle non pubblicate:

* Versione pubblica: Collegare le risorse utilizzando la normale sintassi URL Dynamic Media Classic
* Versione di verifica: collegate le risorse con la stessa sintassi, ma con il nome del sito di verifica protetta

**Eseguire le verifiche**

Eseguite le seguenti verifiche:

1. Controllate che le risorse siano visibili nella rete aziendale.

   Dall’interno della rete aziendale identificata dall’intervallo di indirizzi IP precedentemente definito, nella versione di verifica del sito Web devono essere visualizzate tutte le immagini, sia quelle contrassegnate per la pubblicazione che quelle che non lo sono. Questo vi permette di effettuare la verifica senza correre il rischio rendere le immagini disponibili prima dell’approvazione o del lancio di un prodotto.

   Confermate che la versione pubblica del sito contenga le risorse pubblicate come descritto precedentemente con Dynamic Media Classic.

1. Dall’esterno della rete aziendale, verificate che non sia possibile a terzi accedere alle risorse non pubblicate (cioè quelle non contrassegnate per la pubblicazione).

   Accedete alla rete dall’esterno (ad esempio, dal vostro computer di casa o da una connessione 3G), quindi verificate che la versione pubblica del sito contenga tutte le risorse pubblicate ma nessuno dei contenuti non pubblicati.

   Confermate che la versione di verifica non contenga alcuna risorsa, poiché state tentando di accedere al servizio di verifica protetta da un indirizzo IP non autorizzato.

