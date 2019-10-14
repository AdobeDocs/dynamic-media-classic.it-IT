---
title: 'Pubblicazione di file '
seo-title: 'Pubblicazione di file '
description: 'null'
seo-description: Scoprite come pubblicare i file.
uuid: cdcf519b-4c1e-430b-b43a-2f20f75071b1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/Categories/upload_and_publish_assets
discoiquuid: 39099bc0-9228-46f0-9bee-3542059f4695
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Pubblicazione di file {#publishing-files}

Le risorse vengono pubblicate sui server immagini per file multimediali dinamici. Potete pubblicare le risorse una sola volta oppure fare in modo che Dynamic Media Classic le pubblichi su una pianificazione periodica. Dopo aver pubblicato le risorse, queste sono disponibili per la distribuzione. Potete copiare le richieste URL da Scene7 Publishing System e aggiungerle al sito Web o all’applicazione.

Scene7 Publishing System ora supporta la distribuzione di tutte le immagini e i video su HTTP/2. ossia un URL pubblicato o un codice da incorporare per l’immagine o il video può essere integrato con qualsiasi applicazione che accetta una risorsa ospitata. La risorsa pubblicata viene quindi distribuita tramite il protocollo HTTP/2. Questo metodo di distribuzione migliora il modo in cui i browser e i server comunicano, consentendo una migliore risposta e tempi di caricamento di tutte le risorse Dynamic Media Classic. Consultate [HTTP2 Delivery of Content FAQ](https://docs.adobe.com/content/docs/en/aem/6-2/administer/integration/marketing-cloud/scene7/http2faq.html)(Distribuzione HTTP2 di contenuti).

## Pubblica dopo il caricamento {#publish-after-uploading}

Risorse in stato pubblicato o non pubblicato. Per impostazione predefinita, tutte le risorse caricate in Dynamic Media Classic vengono contrassegnate automaticamente per la pubblicazione.

Per ulteriori informazioni, consultate il PDF [Avviso di pubblicazione](https://marketing.adobe.com/resources/help/en_US/s7/rendering-instant-publish-notification.pdf)istantanea.

Per contrassegnare le risorse per la pubblicazione, eseguite i seguenti metodi:

* **Pubblica dopo il caricamento** Nella pagina Carica, in basso, selezionate Pubblica dopo il caricamento. Per impostazione predefinita, questa opzione è selezionata.

* **Pubblica dopo il caricamento** Nella finestra di dialogo Opzioni processo, selezionate Pubblica dopo il caricamento. Per impostazione predefinita, questa opzione è selezionata.

Alcune risorse secondarie vengono contrassegnate automaticamente per la pubblicazione quando lo sono anche le relative risorse principali. Nella seguente tabella sono illustrate le risorse secondarie contrassegnate automaticamente per la pubblicazione.

| Elemento principale (gruppo) | Elementi secondari (membro) |
|--- |--- |
| Set di immagini | Immagini nel set. |
| Set di campioni | Campioni nel set. |
| Set 360 gradi | Immagini nel set. |
| Modelli | File, pagine e immagini di modello. |

Quando le immagini principali sono contrassegnate per la pubblicazione, vengono contrassegnate automaticamente anche le immagini derivate. Le immagini derivate includono le immagini modificate mediante le opzioni di modifica delle immagini. Potete visualizzare queste immagini derivate nella visualizzazione Dettagli in Generate e derivate.

## Creazione di un processo di pubblicazione {#creating-a-publish-job}

Potete creare un processo di pubblicazione per pubblicare le risorse che avete caricato sui server Dynamic Media Classic ma che non sono ancora state pubblicate automaticamente. Potete effettuare un processo di pubblicazione una tantum oppure pianificare processi periodici. Dynamic Media Classic offre opzioni di pubblicazione avanzate per la pubblicazione su server specifici e opzioni per la ripubblicazione di risorse già pubblicate.

**Per creare un processo di pubblicazione**

1. Nella barra di navigazione globale, fate clic su **Pubblica**.
1. Nella finestra di dialogo per la pubblicazione, scegliete se effettuare un processo di pubblicazione una tantum o periodico.

   Consultate [Creazione di un processo di pubblicazione una tantum](publishing-files.md#creating_a_one_time_publish_job) e [Creazione di un processo di pubblicazione periodico](publishing-files.md#creating_a_recurring_publish_job).

1. Immettete un nome per il processo.
1. Facoltativamente potete visualizzare le opzioni Avanzate e selezionarle. 

   Consultate [Opzioni di pubblicazione avanzate](publishing-files.md#advanced_publish_options).

1. Fate clic su **Invia pubblicazione**.

Scene Publishing System tiene traccia dei processi di pubblicazione nella pagina Processi. In questa pagina potete controllare i processi di pubblicazione.

>[!NOTE]
>
>le risorse ripubblicate (ovvero quelle che sono già state pubblicate) non vengono visualizzate subito sul sito Web a causa del sistema di Web caching sulla rete per la distribuzione dei contenuti (CDN). Consultate [Risorse ripubblicate e ritardi CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Creazione di un processo di pubblicazione una tantum {#creating-a-one-time-publish-job}

Per creare un processo di pubblicazione una tantum, selezionate l’opzione Una tantum nella pagina Pubblica.

Per pubblicare un processo di pubblicazione da eseguire in una data successiva, selezionate il menu Quando e scegliete Pianifica per un momento successivo. Usate quindi il cursore Calendar and Time per selezionare un giorno e un’ora in cui eseguire il processo di pubblicazione.

### Creazione di un processo di pubblicazione periodico {#creating-a-recurring-publish-job}

Per creare un processo di pubblicazione periodico, selezionate l’opzione Periodico nella pagina Pubblica.

Scegliete quindi un’opzione di Ripeti: Quotidianamente, Settimanalmente, Mensilmente o Personalizzato, per specificare quando eseguire il processo di pubblicazione. Dynamic Media Classic presenta gli strumenti calendario per pianificare il processo di pubblicazione periodico. Potete scegliere l’opzione Personalizzato e immettere una regola nella casella Regola in cui descrivere un intervallo per il processo personalizzato. 

Consultate [Creazione di un intervallo personalizzato per un processo di caricamento o pubblicazione](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>i processi di pubblicazione (e caricamento) periodici vengono visualizzati nella pagina Processi. Per modificare o eliminare un processo pianificato, usate la scheda Pianificati della pagina Processi.

### Opzioni di pubblicazione avanzate {#advanced-publish-options}

Potete visualizzare le Opzioni avanzate nella pagina Pubblica e sceglierle per gestire un processo di pubblicazione:

* **Pubblica su** Scegliete un tipo di server per pubblicare le risorse solo su un server specifico, non su tutti i server.

* **Per impostazione predefinita,** in SPS vengono pubblicate solo le risorse nuove e non ancora pubblicate in precedenza (opzione Nuovo dall’ultima pubblicazione). Potete tuttavia scegliere Pubblicazione completa per pubblicare anche le risorse aggiornate o modificate dopo l’ultima pubblicazione. Scegliete Completa con dati di ricerca se pubblicate un eCatalog e desiderate consentire ai lettori di effettuare ricerche in base alla parola chiave.

* **Esegui processo come** Scegliere un nome utente dall’elenco. Potete ordinare i processi in base al nome utente nella pagina Processi. Scegliendo un nome, verrà associato un processo di pubblicazione a un utente.

**Notifica** HTTP Inserite un URL per attivare i processi di pubblicazione successivi.

Consultate [Uso di un processo di caricamento o pubblicazione come trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).

## Annullamento di un processo di pubblicazione {#canceling-a-publish-job}

Potete annullare un processo di pubblicazione in corso. Se siete un amministratore, potete inoltre annullare un processo di pubblicazione in corso dalla pagina Processi della società.

Per annullare un processo di pubblicazione, aprite la pagina Processi e fate clic su pulsante Annulla. Nella scheda Pianificati della pagina Processi potete sospendere o ripristinare un processo deselezionando o selezionando la casella di controllo nella colonna Attivo del processo.

>[!NOTE]
>
>quando annullate un processo di pubblicazione, il relativo stato diventa “interruzione in corso” finché il processo raggiunge il punto in cui può essere interrotto in maniera sicura. Se il processo di pubblicazione viene interrotto durante il recupero dei dati dal database, l’interruzione può richiedere alcuni minuti.

## Pubblicazione manuale di risorse {#manually-publishing-assets}

Potete pubblicare manualmente singole risorse anziché creare un processo di pubblicazione. Quando pubblicate dei set, ad esempio un set di immagini o un set video adattivo, vengono pubblicati sia il set (“elemento principale”) sia tutti i membri (“elementi secondari”) all’interno del set.

Le risorse non pubblicate sono indicate nell’interfaccia utente tramite un’icona rotonda grigia sbarrata con una barra (stato Non pubblicato) a sinistra del nome. Dopo la pubblicazione, l’icona della risorsa diventa verde e presenta un segno di spunta bianco al centro (stato Pubblicato).

**Per pubblicare le risorse manualmente**

1. Effettuate una delle seguenti operazioni:

   * Nelle visualizzazioni Griglia, Elenco o Dettagli, usate i metodi di selezione file standard per selezionare uno o più video dal set.

      Nella barra di navigazione globale, fate clic su **File &gt; Pubblica**.

   * Nelle visualizzazioni Griglia, Elenco o Dettagli, fate clic sull’icona rotonda grigia barrata a sinistra del nome della risorsa.

## Annullamento manuale della pubblicazione di risorse {#manually-unpublishing-assets}

Potete annullare la pubblicazione di singole risorse manualmente. Quando si annulla la pubblicazione di un set, ad esempio un set di campioni o un eCatalog, il set (“elemento principale”) diventa Non pubblicato. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Le risorse pubblicate sono indicate nell’interfaccia utente tramite un’icona rotonda verde con un segno di spunta bianco al centro (stato Pubblicato) a sinistra del nome. Dopo l’annullamento della pubblicazione, l’icona della risorsa diventa grigia e barrata (stato Non pubblicato).

**Per esportare manualmente le risorse non pubblicate**

1. Effettuate una delle seguenti operazioni:

   * Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate una o più risorse pubblicate.

      On the Global Navigation Bar, click **File &gt; **Unpublish**.

   * Nelle visualizzazioni Griglia, Elenco o Dettagli, fate clic sull’icona verde rotonda con il segno di spunta a sinistra del nome della risorsa.

## Visualizzazione della cronologia di pubblicazione di una risorsa {#getting-an-asset-s-publish-history}

L’ultima data di pubblicazione di una risorsa viene visualizzata nella visualizzazione Dettagli nella parte superiore del pannello. Per visualizzare ulteriori dettagli sulla cronologia di pubblicazione, aprite il pannello Server per cronologia e pubblicati nella visualizzazione Dettagli. Questo pannello mostra la data di pubblicazione della risorsa e i server su cui è stata pubblicata.

## Risorse pubblicate e ritardi CDN {#republished-assets-and-cdn-delays}

Le risorse Dynamic Media Classic sono distribuite sulla rete di distribuzione dei contenuti (CDN). Una rete CDN è un sistema di computer server collegati tra di loro per collaborare in maniera trasparente alla distribuzione di contenuti, specialmente contenuti multimediali di grandi dimensioni, agli utenti finali. Nel sistema CDN il contenuto Web viene archiviato nelle cache Web di Internet (chiamata rete di edge caching). Il contenuto Web viene distribuito agli utenti finali da queste cache Web per accelerare le operazioni.

La prima volta che un utente scarica una pagina Web, le risorse vengono distribuite su un server cache Web CDN. Le risorse vengono quindi archiviate su questo server in modo che la prossima volta che un utente nella stessa area accede alla pagina Web, è possibile distribuire più velocemente lo stesso contenuto memorizzato nella cache. Il contenuto viene distribuito più velocemente perché si trova più vicino all’utente finale. La rete CDN assicura visualizzazioni di pagine Web più veloci. Una rete CDN diminuisce le esigenze di larghezza di banda sul server centrale perché il contenuto viene distribuito dalla rete di edge caching e non da un server centrale in ogni istanza.

Il contenuto Dynamic Media Classic appena pubblicato è disponibile immediatamente per l'utente finale e popola rapidamente la rete di edge caching. Tuttavia, il contenuto appena ripubblicato, ovvero le immagini con nomi identici a quelli delle immagini pubblicate precedentemente su un server di immagini, non viene aggiornato sulla rete CDN per almeno dieci ore. Gli utenti finali invece visualizzano il contenuto di una cache Web sulla rete CDN. Per questo motivo, le risorse ripubblicate di Dynamic Media Classic potrebbero non essere visualizzate agli utenti finali per dieci ore.

Per rendere disponibili le risorse appena ripubblicate prima che sia trascorso questo intervallo di dieci ore, potete cancellare le cache Web sulla rete CDN. La cancellazione delle cache Web rimuove i vecchi contenuti dalle cache Web della rete CDN e li sostituisce con le risorse pubblicate più di recente.

Per cancellare la cache, scegliete File &gt; Annulla validità CDN. Tutti i file selezionati vengono rimossi dalla cache. Se non vi sono risorse pubblicate, o se non siete un amministratore di società, l’opzione Rimuovi da CDN non è disponibile.

>[!MORELIKETHIS]
>
>* [Verifica dei file di processo](checking-job-files.md)
>* [Modifica, eliminazione, sospensione e ripristino di processi periodici](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

