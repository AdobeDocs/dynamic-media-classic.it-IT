---
title: File Publish
description: Scopri come pubblicare le risorse sui server immagini Dynamic Medie.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1674'
ht-degree: 21%

---

# File Publish{#publishing-files}

Le risorse vengono pubblicate sui server immagini Dynamic Medie. Puoi pubblicare le risorse una tantum o fare in modo che Adobe Dynamic Media Classic pubblichi le risorse in base a una pianificazione ricorrente. Dopo aver pubblicato le risorse, queste sono disponibili per la distribuzione. Puoi copiare le chiamate URL da Adobe Dynamic Media Classic e aggiungerle al sito web o all’applicazione.

Adobe Dynamic Media Classic ora supporta la distribuzione di tutte le immagini e i video tramite HTTP/2. In altre parole, è disponibile un URL pubblicato o un codice di incorporamento per l’immagine o il video da integrare con qualsiasi applicazione che accetta una risorsa in hosting. La risorsa pubblicata utilizza il protocollo HTTP/2 per distribuirla. Questo metodo di distribuzione migliora il modo in cui browser e server comunicano, consentendo tempi di risposta e di caricamento migliori per tutte le risorse Adobe Dynamic Media Classic. Consulta [Domande frequenti sulla distribuzione HTTP2 dei contenuti](https://experienceleague.adobe.com/it/docs/experience-manager-65/content/assets/dynamic/http2).

## Pubblica dopo il caricamento {#publish-after-uploading}

Risorse in stato pubblicato o non pubblicato. Per impostazione predefinita, tutte le risorse caricate in Adobe Dynamic Media Classic vengono automaticamente contrassegnate per la pubblicazione.

Per ulteriori informazioni, vedere [Instant Publish Notice PDF](/help/using/assets/rendering-instant-publish-notification.pdf).

Per contrassegnare le risorse per la pubblicazione, utilizzare le tecniche riportate di seguito.

* **[!UICONTROL Publish dopo il caricamento]**: nella pagina Caricamento, in basso, selezionare **[!UICONTROL Publish dopo il caricamento]**. Per impostazione predefinita, questa opzione è selezionata.

* **[!UICONTROL Publish dopo il caricamento]**: nella finestra di dialogo Opzioni processo selezionare **[!UICONTROL Publish dopo il caricamento]**. Per impostazione predefinita, questa opzione è selezionata.

Alcune risorse secondarie vengono contrassegnate automaticamente per la pubblicazione quando lo sono anche le relative risorse principali. In questa tabella sono elencate le risorse figlie contrassegnate automaticamente per la pubblicazione.

| Elemento principale (gruppo) | Elementi secondari (membro) |
| --- | --- |
| Set di immagini | Immagini nel set. |
| Set di campioni | Campioni nel set. |
| Set 360 gradi | Immagini nel set. |
| Modelli | File modello, pagine e immagini. |

Le immagini derivate vengono inoltre contrassegnate automaticamente per la pubblicazione quando vengono pubblicate le immagini padre. Le immagini derivate includono le immagini modificate mediante le opzioni di modifica delle immagini. Puoi vedere queste immagini derivate nella sezione Visualizzazione dettagli in Generato e derivati.

## Creare un processo di pubblicazione {#creating-a-publish-job}

Crea un processo di pubblicazione per pubblicare le risorse caricate sui server Adobe Dynamic Media Classic ma non vuoi che vengano pubblicate automaticamente al momento. È possibile eseguire un job di pubblicazione una tantum o pianificare job da riutilizzare regolarmente. Adobe Dynamic Media Classic offre opzioni di pubblicazione avanzate per la pubblicazione su server specifici e opzioni per la ripubblicazione delle risorse già pubblicate.

**Per creare un processo di pubblicazione:**

1. Sulla barra di spostamento globale, selezionare **[!UICONTROL Publish]**.
1. Nella finestra di dialogo Pubblicazione scegliere se si desidera eseguire un processo di pubblicazione una tantum o ricorrente.

   Consulta [Creare un processo di pubblicazione una tantum](publishing-files.md#creating_a_one_time_publish_job) e [Creare un processo di pubblicazione ricorrente](publishing-files.md#creating_a_recurring_publish_job).

1. Immettete un nome per il processo.
1. Facoltativamente potete visualizzare le opzioni Avanzate e selezionarle. 

   Consultate [Opzioni di pubblicazione avanzate](publishing-files.md#advanced_publish_options).

1. Selezionare **[!UICONTROL Invia Publish]**.

Adobe Dynamic Media Classic tiene traccia dei processi di pubblicazione nella pagina Processi. In questa pagina potete controllare i processi di pubblicazione.

>[!NOTE]
>
>Assets che hai ripubblicato (che hai già pubblicato in precedenza) non viene visualizzato immediatamente sul sito web a causa del meccanismo di web-caching sulla rete CDN (content delivery network). Consultate [Risorse ripubblicate e ritardi CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Creare un processo di pubblicazione una tantum {#creating-a-one-time-publish-job}

Crea un processo di pubblicazione una tantum selezionando l&#39;opzione **[!UICONTROL Una tantum]** nella pagina Pubblicazione.

Se si desidera che il processo di pubblicazione venga eseguito in un secondo momento, nella pagina Pubblicazione selezionare **[!UICONTROL Una tantum]**. Dall&#39;elenco a discesa, selezionare **[!UICONTROL Pianifica per dopo]**. Utilizza il Calendario e il cursore Ora per selezionare un giorno e un’ora per eseguire il processo di pubblicazione.

### Creare un processo di pubblicazione ricorrente {#creating-a-recurring-publish-job}

Creare un processo di pubblicazione ricorrente selezionando **[!UICONTROL Ricorrente]** nella pagina Pubblicazione.

Quindi scegli un&#39;opzione di ripetizione di **[!UICONTROL Giornaliero]**, **[!UICONTROL Settimanale]**, **[!UICONTROL Mensile]** o **[!UICONTROL Personalizzato]**, quindi specifica quando desideri che il processo di pubblicazione ricorra nuovamente. Adobe Dynamic Media Classic presenta gli strumenti del calendario per la pianificazione del processo di pubblicazione ricorrente. È possibile selezionare l&#39;opzione **[!UICONTROL Personalizzato]** e immettere una regola nel campo di testo Regola per descrivere un intervallo di processo personalizzato.

Vedere [Intervallo di tempo caricamento o pubblicazione personalizzato](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>i processi di pubblicazione (e caricamento) periodici vengono visualizzati nella pagina Processi. Per modificare o eliminare un processo pianificato, usate la scheda Pianificati della pagina Processi.

### Opzioni avanzate di pubblicazione {#advanced-publish-options}

Puoi visualizzare le opzioni Avanzate nella pagina Pubblicazione e scegliere le seguenti opzioni per la gestione di un processo di pubblicazione:

* **[!UICONTROL Publish in]**: per pubblicare le risorse solo in un server specifico, scegliere un tipo di server.

* **[!UICONTROL Publish]**: per impostazione predefinita, Adobe Dynamic Media Classic pubblica solo le risorse nuove e non ancora pubblicate (opzione Nuovo dall&#39;ultimo Publish). Tuttavia, è possibile selezionare **[!UICONTROL Full Publish]** in modo da poter pubblicare anche le risorse aggiornate o modificate dall&#39;ultima pubblicazione. Selezionare **[!UICONTROL Completo con dati di ricerca]** se si pubblica un eCatalog e si desidera che i lettori possano eseguire ricerche per parola chiave.

* **[!UICONTROL Esegui processo come]**: scegliere un nome utente dall&#39;elenco. Potete ordinare i processi in base al nome utente nella pagina Processi. Scegliendo un nome, si associa un processo di pubblicazione a un utente.

**[!UICONTROL Notifica HTTP]**: immettere un URL per attivare i processi di pubblicazione successivi.

Vedi [Utilizzare un processo di caricamento o pubblicazione come trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Annullare un processo di pubblicazione {#canceling-a-publish-job}

È possibile annullare un processo di pubblicazione in corso. Se siete un amministratore, potete inoltre annullare un processo di pubblicazione in corso dalla pagina Processi della società.

Per annullare un processo di pubblicazione, passare alla pagina Processi e selezionare **[!UICONTROL Annulla]**. Nella scheda Pianificato della pagina Processi è possibile sospendere o riprendere un processo deselezionando o selezionando la casella di controllo nella colonna Attivo del processo.

>[!NOTE]
>
>Dopo aver annullato un processo di pubblicazione, il relativo stato diventa &quot;arresto&quot; finché il processo non raggiunge un punto in cui può essere interrotto in modo sicuro. L&#39;arresto di un processo di pubblicazione può richiedere del tempo se il processo è in fase di recupero dei dati dal database.

## Risorse Publish manualmente {#manually-publishing-assets}

Potete pubblicare manualmente singole risorse anziché creare un processo di pubblicazione. Quando pubblichi dei set, ad esempio un set di immagini o un set di video adattivi, vengono pubblicati il set (o &quot;principale&quot;) e tutti i membri (o &quot;secondari&quot;) al suo interno.

Le risorse non pubblicate sono indicate nell’interfaccia utente da un’icona rotonda grigia con una barra (&quot;stato non pubblicato&quot;) a sinistra del nome della risorsa. Dopo la pubblicazione, l’icona della risorsa diventa verde e presenta un segno di spunta bianco al centro (stato Pubblicato).

**Per pubblicare manualmente le risorse:**

1. Effettuate una delle seguenti operazioni:

   * Nelle visualizzazioni Griglia, Elenco o Dettagli, usate i metodi di selezione file standard per selezionare uno o più video dal set.

     Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Publish]**.

   * Nella Vista griglia, Vista elenco o Vista dettagli, seleziona l’icona grigia arrotondata con una barra che la attraversa, a sinistra del nome della risorsa.

## Annullare la pubblicazione manuale delle risorse {#manually-unpublishing-assets}

Potete annullare la pubblicazione di singole risorse manualmente. Quando annulli la pubblicazione di un set, ad esempio un set di campioni o un eCatalog, il set (o &quot;principale&quot;) passa a uno stato non pubblicato. Tuttavia, i membri (o &quot;figli&quot;) all&#39;interno di quel set non sono interessati; invece, ciascuno di essi mantiene il proprio stato pubblicato o non pubblicato esistente.

Le risorse pubblicate sono indicate nell’interfaccia utente da un’icona rotonda, verde, con un segno di spunta bianco al centro (stato di pubblicazione), a sinistra del nome della risorsa. Dopo aver annullato la pubblicazione di una risorsa, l’icona diventa grigia con una barra (&quot;stato non pubblicato&quot;);

**Per annullare la pubblicazione manuale delle risorse:**

1. Effettuate una delle seguenti operazioni:

   * In Vista griglia, Vista elenco o Vista dettagli, seleziona una o più risorse pubblicate.

     Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Annulla pubblicazione]**.

   * Nella Vista griglia, Vista elenco o Vista dettagli, seleziona l’icona a forma di segno di spunta arrotondato e verde a sinistra del nome della risorsa.

## Ottenere la cronologia di pubblicazione di una risorsa {#getting-an-asset-s-publish-history}

La data dell’ultima pubblicazione di una risorsa viene visualizzata in Vista dettagli, nella parte superiore del pannello. Per ulteriori dettagli sulla cronologia di pubblicazione, apri il pannello Cronologia e server pubblicati in Vista dettagli. Questo pannello mostra la data di pubblicazione della risorsa e i server su cui è stata pubblicata.

## Risorse pubblicate e ritardi CDN {#republished-assets-and-cdn-delays}

Le risorse Adobe Dynamic Media Classic vengono distribuite sulla rete CDN (Content Delivery Network). Una rete CDN è un sistema di computer server collegati tra di loro per collaborare in maniera trasparente alla distribuzione di contenuti, specialmente contenuti multimediali di grandi dimensioni, agli utenti finali. Nel sistema CDN, il contenuto Web viene memorizzato nelle cache Web in Internet (rete di cache Edge). I contenuti web vengono consegnati dalle cache web agli utenti finali per velocizzare le consegne.

La prima volta che un utente scarica una pagina web, le risorse vengono inviate a un server di cache web CDN. Questo server le memorizza in modo che, al successivo accesso alla pagina Web da parte di un utente nella stessa area, lo stesso contenuto memorizzato nella cache venga distribuito più rapidamente. Il contenuto viene distribuito più velocemente perché si trova più vicino all’utente finale. La rete CDN consente una visualizzazione più rapida delle pagine web. Una rete CDN diminuisce le esigenze di larghezza di banda sul server centrale perché il contenuto viene distribuito dalla rete di edge caching e non da un server centrale in ogni istanza.

Il contenuto Adobe Dynamic Media Classic appena pubblicato è immediatamente disponibile per l’utente finale e popola rapidamente la rete della cache edge. Tuttavia, i contenuti ripubblicati, ovvero le immagini con gli stessi nomi di quelle pubblicate in precedenza su un server immagini, non vengono aggiornati sulla rete CDN per un massimo di dieci ore. Al contrario, gli utenti finali visualizzano ciò che si trova in una cache web sulla rete CDN. Per questo motivo, le risorse Adobe Dynamic Media Classic ripubblicate non vengono visualizzate agli utenti finali per dieci ore.

Se desideri che le nuove risorse immagine ripubblicate siano disponibili prima del ritardo di dieci ore, puoi eseguire il flushing delle cache web su CDN. Il flushing di queste cache web rimuove il contenuto obsoleto dalle cache web CDN e lo sostituisce con le risorse pubblicate più di recente.

Per svuotare la cache, sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Annulla validità CDN]**. Tutti i file selezionati vengono rimossi dalla cache. Se non vi sono risorse pubblicate, o se non siete un amministratore di società, l’opzione Rimuovi da CDN non è disponibile.

>[!MORELIKETHIS]
>
>* [Verifica file di processo](checking-job-files.md)
>* [Modifica, elimina, sospendi e riprendi processi ricorrenti](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
