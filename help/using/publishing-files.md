---
title: Pubblicare i file
description: "Scopri come pubblicare le risorse sui server immagini Dynamic Media. Puoi pubblicare le risorse una tantum o fare in modo che Adobe Dynamic Media Classic pubblichi le risorse in base a una pianificazione ricorrente. Dopo aver pubblicato le risorse, queste sono disponibili per la distribuzione. Puoi copiare le chiamate URL da Adobe Dynamic Media Classic e aggiungerle al sito web o all’applicazione."
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 45%

---

# Pubblicare i file{#publishing-files}

Le risorse vengono pubblicate sui server immagini Dynamic Media. Puoi pubblicare le risorse una tantum o fare in modo che Adobe Dynamic Media Classic pubblichi le risorse in base a una pianificazione ricorrente. Dopo aver pubblicato le risorse, queste sono disponibili per la distribuzione. Puoi copiare le chiamate URL da Adobe Dynamic Media Classic e aggiungerle al sito web o all’applicazione.

Adobe Dynamic Media Classic ora supporta la distribuzione di tutte le immagini e i video tramite HTTP/2. In altre parole, è disponibile un URL pubblicato o un codice di incorporamento per l’immagine o il video da integrare con qualsiasi applicazione che accetta una risorsa in hosting. La risorsa pubblicata viene quindi distribuita tramite il protocollo HTTP/2. Questo metodo di distribuzione migliora il modo in cui browser e server comunicano, consentendo tempi di risposta e di caricamento migliori per tutte le risorse Adobe Dynamic Media Classic. Consulta [Domande frequenti sulla distribuzione dei contenuti HTTP2](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## Pubblica dopo il caricamento {#publish-after-uploading}

Risorse in stato pubblicato o non pubblicato. Per impostazione predefinita, tutte le risorse caricate in Adobe Dynamic Media Classic vengono automaticamente contrassegnate per la pubblicazione.

Per ulteriori informazioni, vedere [Instant Publish Notice PDF](/help/using/assets/rendering-instant-publish-notification.pdf).

Per contrassegnare le risorse per la pubblicazione, eseguite i seguenti metodi:

* **[!UICONTROL Pubblica dopo il caricamento]** - Nella pagina Carica, in basso, seleziona **[!UICONTROL Pubblica dopo il caricamento]**. Per impostazione predefinita, questa opzione è selezionata.

* **[!UICONTROL Pubblica dopo il caricamento]** - Nella finestra di dialogo Opzioni job, selezionare **[!UICONTROL Pubblica dopo il caricamento]**. Per impostazione predefinita, questa opzione è selezionata.

Alcune risorse secondarie vengono contrassegnate automaticamente per la pubblicazione quando lo sono anche le relative risorse principali. Nella seguente tabella sono illustrate le risorse secondarie contrassegnate automaticamente per la pubblicazione.

| Elemento principale (gruppo) | Elementi secondari (membro) |
| --- | --- |
| Set di immagini | Immagini nel set. |
| Set di campioni | Campioni nel set. |
| Set 360 gradi | Immagini nel set. |
| Modelli | File, pagine e immagini di modello. |

Quando le immagini principali sono contrassegnate per la pubblicazione, vengono contrassegnate automaticamente anche le immagini derivate. Le immagini derivate includono le immagini modificate mediante le opzioni di modifica delle immagini. Puoi vedere queste immagini derivate nella sezione Visualizzazione dettagli in Generato e derivati.

## Creare un processo di pubblicazione {#creating-a-publish-job}

Crea un processo di pubblicazione per pubblicare le risorse caricate sui server Adobe Dynamic Media Classic ma non desideri ancora pubblicarle automaticamente. Puoi eseguire un processo di pubblicazione una tantum o pianificare i processi in modo che ricorrano regolarmente. Adobe Dynamic Media Classic offre opzioni di pubblicazione avanzate per la pubblicazione su server specifici e opzioni per la ripubblicazione delle risorse già pubblicate.

**Per creare un processo di pubblicazione:**

1. Sulla barra di navigazione globale, seleziona **[!UICONTROL Pubblica]**.
1. Nella finestra di dialogo per la pubblicazione, scegliete se effettuare un processo di pubblicazione una tantum o periodico.

   Consulta [Creare un processo di pubblicazione una tantum](publishing-files.md#creating_a_one_time_publish_job) e [Creare un processo di pubblicazione ricorrente](publishing-files.md#creating_a_recurring_publish_job).

1. Immettete un nome per il processo.
1. Facoltativamente potete visualizzare le opzioni Avanzate e selezionarle. 

   Consultate [Opzioni di pubblicazione avanzate](publishing-files.md#advanced_publish_options).

1. Seleziona **[!UICONTROL Invia pubblicazione]**.

Adobe Dynamic Media Classic tiene traccia dei processi di pubblicazione nella pagina Processi. In questa pagina potete controllare i processi di pubblicazione.

>[!NOTE]
>
>Le risorse che ripubblichi (che hai già pubblicato) non vengono visualizzate immediatamente sul sito web a causa del meccanismo di web-caching sulla rete CDN (Content Delivery Network). Consultate [Risorse ripubblicate e ritardi CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Creare un processo di pubblicazione una tantum {#creating-a-one-time-publish-job}

Creare un processo di pubblicazione una tantum selezionando la **[!UICONTROL Una tantum]** nella pagina Pubblica.

Se desideri che il processo di pubblicazione avvenga in un secondo momento, nella pagina Pubblica seleziona **[!UICONTROL Una tantum]**, quindi seleziona **[!UICONTROL Pianifica per un momento successivo]** a discesa. Utilizza il Calendario e il cursore Ora per selezionare un giorno e un’ora per eseguire il processo di pubblicazione.

### Creare un processo di pubblicazione ricorrente {#creating-a-recurring-publish-job}

Creare un processo di pubblicazione ricorrente selezionando **[!UICONTROL Ricorrente]** nella pagina Pubblica.

Quindi scegliete un&#39;opzione Ripeti di **[!UICONTROL Giornaliero]**, **[!UICONTROL Ogni settimana]**, **[!UICONTROL Mensile]**, o **[!UICONTROL Personalizzato]**, quindi specifica quando desideri che il processo di pubblicazione ricorra. Adobe Dynamic Media Classic presenta gli strumenti del calendario per pianificare il processo di pubblicazione ricorrente. Puoi selezionare **[!UICONTROL Personalizzato]** e immettere una regola nel campo di testo Regola per descrivere un intervallo di processo personalizzato.

Consulta [Creare un intervallo di tempo del processo di caricamento o pubblicazione personalizzato](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>i processi di pubblicazione (e caricamento) periodici vengono visualizzati nella pagina Processi. Per modificare o eliminare un processo pianificato, usate la scheda Pianificati della pagina Processi.

### Opzioni avanzate di pubblicazione {#advanced-publish-options}

Potete visualizzare le Opzioni avanzate nella pagina Pubblica e sceglierle per gestire un processo di pubblicazione:

* **[!UICONTROL Pubblica in]** : per pubblicare le risorse solo su un server specifico, scegli un tipo di server.

* **[!UICONTROL Pubblica]** - Per impostazione predefinita, Adobe Dynamic Media Classic pubblica solo le risorse nuove e non ancora pubblicate (opzione Nuova dall’ultima pubblicazione). Tuttavia, puoi selezionare **[!UICONTROL Pubblicazione completa]** per pubblicare anche le risorse aggiornate o modificate dall&#39;ultima pubblicazione. Seleziona **[!UICONTROL Completa con dati di ricerca]** se si pubblica un eCatalog e si desidera che i lettori possano eseguire ricerche per parola chiave.

* **[!UICONTROL Esegui processo come]** - Scegliere un nome utente dall&#39;elenco. Potete ordinare i processi in base al nome utente nella pagina Processi. Scegliendo un nome, verrà associato un processo di pubblicazione a un utente.

**[!UICONTROL Notifica HTTP]** - Immetti un URL per attivare i processi di pubblicazione successivi.

Consulta [Utilizzare un processo di caricamento o pubblicazione come attivatore](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Annullare un processo di pubblicazione {#canceling-a-publish-job}

È possibile annullare un processo di pubblicazione in corso. Se siete un amministratore, potete inoltre annullare un processo di pubblicazione in corso dalla pagina Processi della società.

Per annullare un processo di pubblicazione, vai alla pagina Processi e seleziona **[!UICONTROL Annulla]**. Nella scheda Pianificati della pagina Processi potete sospendere o ripristinare un processo deselezionando o selezionando la casella di controllo nella colonna Attivo del processo.

>[!NOTE]
>
>quando annullate un processo di pubblicazione, il relativo stato diventa “interruzione in corso” finché il processo raggiunge il punto in cui può essere interrotto in maniera sicura. Se il processo di pubblicazione viene interrotto durante il recupero dei dati dal database, l’interruzione può richiedere alcuni minuti.

## Pubblicare manualmente le risorse {#manually-publishing-assets}

Potete pubblicare manualmente singole risorse anziché creare un processo di pubblicazione. Quando pubblicate dei set, ad esempio un set di immagini o un set video adattivo, vengono pubblicati sia il set (“elemento principale”) sia tutti i membri (“elementi secondari”) all’interno del set.

Le risorse non pubblicate sono indicate nell’interfaccia utente da un’icona rotonda grigia con una barra (&quot;stato non pubblicato&quot;) a sinistra del nome della risorsa. Dopo la pubblicazione, l’icona della risorsa diventa verde e presenta un segno di spunta bianco al centro (stato Pubblicato).

**Per pubblicare le risorse manualmente:**

1. Effettuate una delle seguenti operazioni:

   * Nelle visualizzazioni Griglia, Elenco o Dettagli, usate i metodi di selezione file standard per selezionare uno o più video dal set.

     Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Pubblica]**.

   * Nella Vista griglia, Vista elenco o Vista dettagli, seleziona l’icona grigia rotonda con una barra che la attraversa, a sinistra del nome della risorsa.

## Annullare la pubblicazione manuale delle risorse {#manually-unpublishing-assets}

Potete annullare la pubblicazione di singole risorse manualmente. Quando si annulla la pubblicazione di un set, ad esempio un set di campioni o un eCatalog, il set (“elemento principale”) diventa Non pubblicato. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Le risorse pubblicate sono indicate nell’interfaccia utente tramite un’icona rotonda verde con un segno di spunta bianco al centro (stato Pubblicato) a sinistra del nome. Dopo aver annullato la pubblicazione di una risorsa, l’icona diventa grigia con una barra (&quot;stato non pubblicato&quot;);

**Per esportare manualmente le risorse non pubblicate:**

1. Effettuate una delle seguenti operazioni:

   * In Vista griglia, Vista elenco o Vista dettagli, seleziona una o più risorse pubblicate.

     Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Annulla pubblicazione]**.

   * Nella Vista griglia, Vista elenco o Vista dettagli, seleziona l’icona a forma di segno di spunta arrotondato e verde a sinistra del nome della risorsa.

## Ottenere la cronologia di pubblicazione di una risorsa {#getting-an-asset-s-publish-history}

La data dell’ultima pubblicazione di una risorsa viene visualizzata in Vista dettagli, nella parte superiore del pannello. Per ulteriori dettagli sulla cronologia di pubblicazione, apri il pannello Cronologia e server pubblicati in Vista dettagli. Questo pannello mostra la data di pubblicazione della risorsa e i server su cui è stata pubblicata.

## Risorse pubblicate e ritardi CDN {#republished-assets-and-cdn-delays}

Le risorse Adobe Dynamic Media Classic vengono distribuite sulla rete CDN (Content Delivery Network). Una rete CDN è un sistema di computer server collegati tra di loro per collaborare in maniera trasparente alla distribuzione di contenuti, specialmente contenuti multimediali di grandi dimensioni, agli utenti finali. Nel sistema CDN il contenuto Web viene archiviato nelle cache Web di Internet (chiamata rete di edge caching). I contenuti web vengono consegnati dalle cache web agli utenti finali per velocizzare le consegne.

La prima volta che un utente scarica una pagina Web, le risorse vengono distribuite su un server cache Web CDN. Le risorse vengono quindi archiviate su questo server in modo che la prossima volta che un utente nella stessa area accede alla pagina Web, è possibile distribuire più velocemente lo stesso contenuto memorizzato nella cache. Il contenuto viene distribuito più velocemente perché si trova più vicino all’utente finale. La rete CDN assicura visualizzazioni di pagine Web più veloci. Una rete CDN diminuisce le esigenze di larghezza di banda sul server centrale perché il contenuto viene distribuito dalla rete di edge caching e non da un server centrale in ogni istanza.

Il contenuto Adobe Dynamic Media Classic appena pubblicato è immediatamente disponibile per l’utente finale e popola rapidamente la rete della cache edge. Tuttavia, il contenuto appena ripubblicato, ovvero le immagini con nomi identici a quelli delle immagini pubblicate precedentemente su un server di immagini, non viene aggiornato sulla rete CDN per almeno dieci ore. Gli utenti finali invece visualizzano il contenuto di una cache Web sulla rete CDN. Per questo motivo, le risorse Adobe Dynamic Media Classic ripubblicate non vengono visualizzate agli utenti finali per dieci ore.

Per rendere disponibili le risorse appena ripubblicate prima che sia trascorso questo intervallo di dieci ore, potete cancellare le cache Web sulla rete CDN. La cancellazione delle cache Web rimuove i vecchi contenuti dalle cache Web della rete CDN e li sostituisce con le risorse pubblicate più di recente.

Per svuotare la cache, nella barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Annulla validità CDN]**. Tutti i file selezionati vengono rimossi dalla cache. Se non vi sono risorse pubblicate, o se non siete un amministratore di società, l’opzione Rimuovi da CDN non è disponibile.

>[!MORELIKETHIS]
>
>* [Verifica file di processo](checking-job-files.md)
>* [Modifica, elimina, sospendi e riprendi processi ricorrenti](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
