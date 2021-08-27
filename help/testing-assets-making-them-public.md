---
title: Verifica delle risorse prima di renderle pubbliche
description: Scopri come verificare le risorse prima di renderle pubbliche.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 37%

---

# Verifica delle risorse prima di renderle pubbliche {#testing-assets-before-making-them-public}

Il test protetto consente di definire un ambiente di test sicuro e di creare una solida soluzione B2B, basata su un set configurabile di indirizzi IP e intervalli. Questa funzionalità ti consente di abbinare le implementazioni Adobe Dynamic Media Classic all’architettura della gestione dei contenuti e del sistema aziendale.

La verifica protetta consente di visualizzare in anteprima una versione per uso interno del sito Web, con contenuti non ancora pubblicati.

Se lo desideri, crea un ambiente di staging anziché rendere le risorse disponibili al pubblico per i seguenti motivi:

* Anteprima di siti Web prima del lancio effettivo (pubblicazione protetta a scopo di verifica).
* Trasmissione di risorse per accesso limitato, ad esempio eCatalog che mostrano i prezzi in un’applicazione Web B2B.
* Utilizzo di risorse all’interno di un firewall come parte di un sistema di gestione delle informazioni sui prodotti, di un’applicazione per il servizio di assistenza clienti, di un sito di formazione e così via.

>[!NOTE]
>
>La verifica sicura non influisce sull’accesso ad Adobe Dynamic Media Classic. Ad Adobe, la sicurezza di Dynamic Media Classic rimane coerente e richiede le solite credenziali per l’accesso ad Adobe Dynamic Media Classic e ai servizi Web correlati.

## Funzionamento della verifica protetta {#how-secure-testing-works}

Per la maggior parte delle società le connessioni Internet avvengono mediante un firewall. L’accesso a Internet è possibile tramite alcuni indirizzamenti e in genere con una serie limitata di indirizzi IP pubblici.

Dalla rete aziendale, è possibile individuare l&#39;indirizzo IP pubblico utilizzando siti web come https://whatismyip.com o richiedere queste informazioni all&#39;organizzazione IT aziendale.

Con il test protetto, Adobe Dynamic Media Classic stabilisce un server di immagini dedicato per gli ambienti di staging o le applicazioni interne. Per tutte le richieste inviate a questo server viene controllato l’indirizzo IP di origine. Se la richiesta non proviene dall’elenco di indirizzi IP approvato, viene restituita una risposta di operazione non riuscita. L’amministratore della società Dynamic Media Classic Adobe configura l’elenco approvato di indirizzi IP per l’ambiente di test Secure della propria azienda.

Poiché la posizione della richiesta originale deve essere confermata, il traffico del servizio Secure Testing non viene instradato attraverso una rete di distribuzione del contenuto come il traffico pubblico di Dynamic Media Image Server. Le richieste al servizio Secure Testing hanno una latenza leggermente più elevata rispetto ai server immagini pubblici di Dynamic Media.

Le risorse non pubblicate sono immediatamente disponibili dai servizi di verifica protetta, senza dover essere pubblicati. In questo modo, puoi eseguire un’anteprima prima che le risorse vengano pubblicate sul server di immagini rivolto al pubblico.

>[!NOTE]
>
>I servizi di verifica protetta utilizzano il server di catalogo configurato con un contesto di pubblicazione interno. Pertanto, se la tua azienda è configurata per la pubblicazione su Secure Testing, tutte le risorse caricate in Adobe Dynamic Media Classic diventano immediatamente disponibili sui servizi Secure Testing. Questa funzionalità è valida anche se le risorse sono contrassegnate per la pubblicazione al momento del caricamento.

I servizi di verifica sicura supportano attualmente i seguenti tipi di risorse e funzionalità:

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
* Visualizzatori rich media standard di Adobe Dynamic Media Classic.
* Adobe pagine JSP Dynamic Media Classic OnDemand.
* Contenuto statico, ad esempio file PDF e video progressivi.
* Streaming video HTTP.
* Streaming di video progressivo.

I seguenti tipi di risorse e funzionalità non sono attualmente supportati:

* Streaming video RTMP
* Servizi UGC
* Web-stampa
* Adobe Informazioni di Dynamic Media Classic o ricerca eCatalog

## Verifica del servizio di verifica protetta {#testing-the-secure-testing-service}

Verifica che il servizio di test sicuro funzioni come previsto.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]*** - If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### Preparare l’account

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Contatta l’Assistenza clienti Adobe e richiedi l’abilitazione del test protetto sul tuo account.
1. In Adobe Dynamic Media Classic, nella barra di navigazione globale, fate clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazioni di pubblicazione]** > **[!UICONTROL Server immagini]**.
1. Nella pagina Pubblica su Image Server, nell&#39;elenco a discesa **[!UICONTROL Contesto pubblicazione]**, selezionare **[!UICONTROL Test Image Serving]**.
1. Per Filtro indirizzi client, fate clic su **[!UICONTROL Aggiungi]**.
1. Selezionare la casella di controllo in modo che l&#39;indirizzo sia abilitato (attivato), quindi digitare un indirizzo IP e una maschera di rete nei rispettivi campi di testo.

   >[!NOTE]
   >
   >Se aggiungi un indirizzo IP singolo e una maschera di rete, tale indirizzo può effettuare chiamate alle risorse. Tuttavia, non è consentito effettuare chiamate alle risorse ad altri indirizzi IP e maschere di rete aggiunti. Per disattivare la possibilità di specificare un indirizzo IP e una maschera di rete, disattiva la casella di controllo del passaggio precedente. In questo modo, tutti gli indirizzi IP *tutti* possono effettuare chiamate alle risorse e vengono visualizzati.

1. Effettuate una delle seguenti operazioni:
   * Ripeti i due passaggi precedenti se devi aggiungere altri indirizzi IP.
   * Procedi al passaggio successivo.
1. In basso a sinistra della pagina Pubblicazione su Image Server, fai clic su **[!UICONTROL Salva]**
1. Carica le immagini desiderate nel tuo account Adobe Dynamic Media Classic.

   Consultate [Caricamento dei file](uploading-files.md#uploading_files).

1. Accertatevi che alcune delle immagini siano contrassegnate per la pubblicazione e altre non lo siano, quindi inviate il processo di pubblicazione.

   Consultate [Pubblicazione](publishing-files.md#publishing_files).

1. Determinate il nome del servizio di verifica protetta facendo clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali]**.
1. Nella pagina Impostazioni generali applicazione, nella sezione Server, individuate il nome a destra di **[!UICONTROL Nome server contesto pubblicazione di prova]**.

Se il nome del server è mancante o se gli URL del server non funzionano, contatta l’Assistenza Adobe.

### Preparare le varianti del sito Web

È necessario disporre di due varianti di un sito Web, con collegamenti alle risorse pubblicate e a quelle non pubblicate:

* Versione pubblica : collega le risorse utilizzando la sintassi URL tradizionale di Dynamic Media Classic di Adobe.
* Versione di staging : collega le risorse utilizzando la stessa sintassi ma con il nome del sito di Secure Testing.

### Eseguire le verifiche

Eseguite le seguenti verifiche:

1. Controllate che le risorse siano visibili nella rete aziendale.

   Dall&#39;interno della rete aziendale identificata dall&#39;intervallo di indirizzi IP precedentemente definito, la versione di staging del sito web visualizza tutte le immagini, contrassegnate per la pubblicazione o meno. Puoi eseguire il test senza rendere accidentalmente disponibili le immagini prima dell’approvazione dell’anteprima o del lancio del prodotto.

   Conferma che la versione pubblica del sito mostri le risorse pubblicate come precedentemente sperimentato con Adobe Dynamic Media Classic.

1. Dall’esterno della rete aziendale, verificate che non sia possibile a terzi accedere alle risorse non pubblicate (cioè quelle non contrassegnate per la pubblicazione).

   Accedete alla rete dall’esterno (ad esempio, dal vostro computer di casa o da una connessione 3G), quindi verificate che la versione pubblica del sito contenga tutte le risorse pubblicate ma nessuno dei contenuti non pubblicati.

   Confermate che la versione di verifica non contenga alcuna risorsa, poiché state tentando di accedere al servizio di verifica protetta da un indirizzo IP non autorizzato.
