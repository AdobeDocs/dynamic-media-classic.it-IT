---
title: 'Pubblicazione di file '
description: '"Scopri come pubblicare le risorse sui server di immagini Dynamic Media. Puoi pubblicare le risorse una tantum oppure fare in modo che Dynamic Media Classic pubblichi le risorse secondo una pianificazione periodica. Dopo aver pubblicato le risorse, queste sono disponibili per la distribuzione. Puoi copiare le chiamate URL da Adobe Dynamic Media Classic e aggiungerle al tuo sito web o applicazione."'
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1722'
ht-degree: 56%

---

# Pubblicazione di file {#publishing-files}

Le risorse vengono pubblicate sui server di immagini Dynamic Media. Puoi pubblicare le risorse una tantum oppure fare in modo che Dynamic Media Classic pubblichi le risorse secondo una pianificazione periodica. Dopo aver pubblicato le risorse, queste sono disponibili per la distribuzione. Puoi copiare le chiamate URL da Adobe Dynamic Media Classic e aggiungerle al tuo sito web o applicazione.

Adobe Dynamic Media Classic ora supporta la distribuzione di tutte le immagini e i video su HTTP/2. In altre parole, è disponibile un URL o un codice di incorporamento pubblicato per l’immagine o il video da integrare con qualsiasi applicazione che accetta una risorsa in hosting. La risorsa pubblicata viene quindi distribuita tramite il protocollo HTTP/2. Questo metodo di consegna migliora il modo in cui i browser e i server comunicano, consentendo una migliore risposta e tempi di caricamento di tutte le risorse Adobe Dynamic Media Classic. Consulta [Domande frequenti sulla distribuzione dei contenuti HTTP2](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## Pubblica dopo il caricamento {#publish-after-uploading}

Risorse in stato pubblicato o non pubblicato. Per impostazione predefinita, tutte le risorse caricate in Adobe Dynamic Media Classic vengono contrassegnate automaticamente per la pubblicazione.

Per ulteriori informazioni, consulta [Avviso di pubblicazione istantanea PDF](/help/assets/rendering-instant-publish-notification.pdf).

Per contrassegnare le risorse per la pubblicazione, eseguite i seguenti metodi:

* **Pubblica dopo il caricamento** : nella pagina Carica, in basso, seleziona Pubblica dopo il caricamento. Per impostazione predefinita, questa opzione è selezionata.

* **Pubblica dopo il caricamento** : nella finestra di dialogo Opzioni processo, seleziona Pubblica dopo il caricamento. Per impostazione predefinita, questa opzione è selezionata.

Alcune risorse secondarie vengono contrassegnate automaticamente per la pubblicazione quando lo sono anche le relative risorse principali. Nella seguente tabella sono illustrate le risorse secondarie contrassegnate automaticamente per la pubblicazione.

| Elemento principale (gruppo) | Elementi secondari (membro) |
|--- |--- |
| Set di immagini | Immagini nel set. |
| Set di campioni | Campioni nel set. |
| Set 360 gradi | Immagini nel set. |
| Modelli | File, pagine e immagini di modello. |

Quando le immagini principali sono contrassegnate per la pubblicazione, vengono contrassegnate automaticamente anche le immagini derivate. Le immagini derivate includono le immagini modificate mediante le opzioni di modifica delle immagini. Puoi vedere queste immagini derivate in Vista dettagli in Costruito e derivate.

## Creazione di un processo di pubblicazione {#creating-a-publish-job}

Crea un processo di pubblicazione per pubblicare le risorse caricate sui server Adobe Dynamic Media Classic, ma scegli di non pubblicarle ancora automaticamente. È possibile eseguire un processo di pubblicazione una tantum o pianificare i processi da eseguire regolarmente. Adobe Dynamic Media Classic offre opzioni di pubblicazione avanzate per la pubblicazione su server specifici e opzioni per la ripubblicazione delle risorse già pubblicate.

**Per creare un processo di pubblicazione:**

1. Nella barra di navigazione globale, fate clic su **[!UICONTROL Pubblica]**.
1. Nella finestra di dialogo per la pubblicazione, scegliete se effettuare un processo di pubblicazione una tantum o periodico.

   Consultate [Creazione di un processo di pubblicazione una tantum](publishing-files.md#creating_a_one_time_publish_job) e [Creazione di un processo di pubblicazione periodico](publishing-files.md#creating_a_recurring_publish_job).

1. Immettete un nome per il processo.
1. Facoltativamente potete visualizzare le opzioni Avanzate e selezionarle. 

   Consultate [Opzioni di pubblicazione avanzate](publishing-files.md#advanced_publish_options).

1. Fate clic su **[!UICONTROL Invia pubblicazione]**.

Ad Adobe, Dynamic Media Classic tiene traccia dei lavori di pubblicazione nella pagina Processi. In questa pagina potete controllare i processi di pubblicazione.

>[!NOTE]
>
>le risorse ripubblicate (ovvero quelle che sono già state pubblicate) non vengono visualizzate subito sul sito Web a causa del sistema di Web caching sulla rete per la distribuzione dei contenuti (CDN). Consultate [Risorse ripubblicate e ritardi CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Creazione di un processo di pubblicazione una tantum {#creating-a-one-time-publish-job}

Per creare un processo di pubblicazione una tantum, selezionate l’opzione Una tantum nella pagina Pubblica.

Se desideri che il processo di pubblicazione si verifichi in un secondo momento, nella pagina Pubblica seleziona **[!UICONTROL Una tantum]**, quindi fai clic sul menu a discesa **[!UICONTROL Pianifica per un momento successivo]** . Utilizza il Calendario e il cursore Ora per selezionare un giorno e un’ora per eseguire il processo di pubblicazione.

### Creazione di un processo di pubblicazione periodico {#creating-a-recurring-publish-job}

Crea un processo di pubblicazione ricorrente selezionando **[!UICONTROL Ricorrente]** nella pagina Pubblica .

Quindi scegli un&#39;opzione Ripeti di **[!UICONTROL Giornaliero]**, **[!UICONTROL Settimanale]**, **[!UICONTROL Mensile]** o **[!UICONTROL Personalizzato]**, quindi specifica quando riattivare il processo di pubblicazione. Ad Adobe, Dynamic Media Classic presenta gli strumenti di calendario per la pianificazione del processo di pubblicazione ricorrente. È possibile fare clic sull&#39;opzione **[!UICONTROL Personalizzato]** e immettere una regola nel campo di testo Regola per descrivere un intervallo di lavoro personalizzato.

Consultate [Creazione di un intervallo personalizzato per un processo di caricamento o pubblicazione](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>i processi di pubblicazione (e caricamento) periodici vengono visualizzati nella pagina Processi. Per modificare o eliminare un processo pianificato, usate la scheda Pianificati della pagina Processi.

### Opzioni di pubblicazione avanzate {#advanced-publish-options}

Potete visualizzare le Opzioni avanzate nella pagina Pubblica e sceglierle per gestire un processo di pubblicazione:

* **Pubblica in** : per pubblicare le risorse solo su un server specifico, scegli un tipo di server.

* **Pubblica** : per impostazione predefinita, in Adobe Dynamic Media Classic vengono pubblicate solo le risorse nuove e non ancora pubblicate (opzione Nuova dall’ultima pubblicazione). Tuttavia, puoi fare clic su **[!UICONTROL Pubblicazione completa]** per pubblicare anche le risorse che sono state aggiornate o modificate dopo l’ultima pubblicazione. Seleziona **[!UICONTROL Completo con dati di ricerca]** se pubblichi un eCatalog e desideri che i lettori siano in grado di cercarlo per parola chiave.

* **Esegui processo come** : scegli un nome utente dall’elenco. Potete ordinare i processi in base al nome utente nella pagina Processi. Scegliendo un nome, verrà associato un processo di pubblicazione a un utente.

**Notifica HTTP**  - Inserisci un URL per attivare i processi di pubblicazione successivi.

Consultate [Uso di un processo di caricamento o pubblicazione come trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).

## Annullamento di un processo di pubblicazione {#canceling-a-publish-job}

Potete annullare un processo di pubblicazione in corso. Se siete un amministratore, potete inoltre annullare un processo di pubblicazione in corso dalla pagina Processi della società.

Per annullare un processo di pubblicazione, vai alla pagina Processi e fai clic su **[!UICONTROL Annulla]**. Nella scheda Pianificati della pagina Processi potete sospendere o ripristinare un processo deselezionando o selezionando la casella di controllo nella colonna Attivo del processo.

>[!NOTE]
>
>quando annullate un processo di pubblicazione, il relativo stato diventa “interruzione in corso” finché il processo raggiunge il punto in cui può essere interrotto in maniera sicura. Se il processo di pubblicazione viene interrotto durante il recupero dei dati dal database, l’interruzione può richiedere alcuni minuti.

## Pubblicazione manuale di risorse {#manually-publishing-assets}

Potete pubblicare manualmente singole risorse anziché creare un processo di pubblicazione. Quando pubblicate dei set, ad esempio un set di immagini o un set video adattivo, vengono pubblicati sia il set (“elemento principale”) sia tutti i membri (“elementi secondari”) all’interno del set.

Le risorse non pubblicate sono indicate nell’interfaccia utente da un’icona rotonda grigia con una barra (stato non pubblicato) a sinistra del nome della risorsa. Dopo la pubblicazione, l’icona della risorsa diventa verde e presenta un segno di spunta bianco al centro (stato Pubblicato).

**Per pubblicare le risorse manualmente:**

1. Effettuate una delle seguenti operazioni:

   * Nelle visualizzazioni Griglia, Elenco o Dettagli, usate i metodi di selezione file standard per selezionare uno o più video dal set.

      Nella barra di navigazione globale, fate clic su **[!UICONTROL File]** > **[!UICONTROL Pubblica]**.

   * Nella vista Griglia, Elenco o Dettagli, fai clic sull’icona rotonda grigia con una barra a sinistra del nome della risorsa.

## Annullamento manuale della pubblicazione di risorse {#manually-unpublishing-assets}

Potete annullare la pubblicazione di singole risorse manualmente. Quando si annulla la pubblicazione di un set, ad esempio un set di campioni o un eCatalog, il set (“elemento principale”) diventa Non pubblicato. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Le risorse pubblicate sono indicate nell’interfaccia utente tramite un’icona rotonda verde con un segno di spunta bianco al centro (stato Pubblicato) a sinistra del nome. Una volta annullata la pubblicazione di una risorsa, l’icona diventa grigia a causa di una barra (stato non pubblicato),

**Per esportare manualmente le risorse non pubblicate:**

1. Effettuate una delle seguenti operazioni:

   * In Vista a griglia, Vista a elenco o Vista dettagli, selezionate una o più risorse pubblicate.

      Nella barra di navigazione globale, fate clic su **[!UICONTROL File]** > **[!UICONTROL Annulla pubblicazione]**.

   * Nelle visualizzazioni Griglia, Elenco o Dettagli, fate clic sull’icona verde rotonda con il segno di spunta a sinistra del nome della risorsa.

## Visualizzazione della cronologia di pubblicazione di una risorsa {#getting-an-asset-s-publish-history}

L’ultima data di pubblicazione di una risorsa viene visualizzata in Vista dettagli nella parte superiore del pannello. Per ottenere ulteriori dettagli sulla cronologia delle pubblicazioni, apri il pannello Server precedenti e pubblicati in Vista dettagli. Questo pannello mostra la data di pubblicazione della risorsa e i server su cui è stata pubblicata.

## Risorse pubblicate e ritardi CDN {#republished-assets-and-cdn-delays}

Adobe, le risorse Dynamic Media Classic sono distribuite sulla rete CDN (Content Delivery Network). Una rete CDN è un sistema di computer server collegati tra di loro per collaborare in maniera trasparente alla distribuzione di contenuti, specialmente contenuti multimediali di grandi dimensioni, agli utenti finali. Nel sistema CDN il contenuto Web viene archiviato nelle cache Web di Internet (chiamata rete di edge caching). Il contenuto web viene distribuito dalle cache web agli utenti finali per consentire consegne più veloci.

La prima volta che un utente scarica una pagina Web, le risorse vengono distribuite su un server cache Web CDN. Le risorse vengono quindi archiviate su questo server in modo che la prossima volta che un utente nella stessa area accede alla pagina Web, è possibile distribuire più velocemente lo stesso contenuto memorizzato nella cache. Il contenuto viene distribuito più velocemente perché si trova più vicino all’utente finale. La rete CDN assicura visualizzazioni di pagine Web più veloci. Una rete CDN diminuisce le esigenze di larghezza di banda sul server centrale perché il contenuto viene distribuito dalla rete di edge caching e non da un server centrale in ogni istanza.

Il contenuto di Adobe Classic recentemente pubblicato è disponibile immediatamente per l’utente finale e popola rapidamente la rete della cache edge. Tuttavia, il contenuto appena ripubblicato, ovvero le immagini con nomi identici a quelli delle immagini pubblicate precedentemente su un server di immagini, non viene aggiornato sulla rete CDN per almeno dieci ore. Gli utenti finali invece visualizzano il contenuto di una cache Web sulla rete CDN. Per questo motivo, le risorse ripubblicate in Dynamic Media Classic di Adobe non vengono visualizzate agli utenti finali per dieci ore.

Per rendere disponibili le risorse appena ripubblicate prima che sia trascorso questo intervallo di dieci ore, potete cancellare le cache Web sulla rete CDN. La cancellazione delle cache Web rimuove i vecchi contenuti dalle cache Web della rete CDN e li sostituisce con le risorse pubblicate più di recente.

Per svuotare la cache, nella barra di navigazione globale fai clic su **[!UICONTROL File]** > **[!UICONTROL Annulla validità CDN]**. Tutti i file selezionati vengono rimossi dalla cache. Se non vi sono risorse pubblicate, o se non siete un amministratore di società, l’opzione Rimuovi da CDN non è disponibile.

>[!MORELIKETHIS]
>
>* [Verifica dei file di processo](checking-job-files.md)
>* [Modifica, eliminazione, sospensione e ripristino di processi periodici](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

