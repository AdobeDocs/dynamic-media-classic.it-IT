---
title: Verifica file di processo
description: Scopri come controllare i file di processo in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
topic: Administration, Content Management
level: Intermediate
source-git-commit: bb229047c0c9b3855453ea15dcd1f9754bc65cef
workflow-type: tm+mt
source-wordcount: '1622'
ht-degree: 23%

---

# Verifica file di processo{#checking-job-files}

Per monitorare i caricamenti di file in Adobe Dynamic Media Classic e i file pubblicati sui server Adobe Dynamic Media Classic, Adobe Dynamic Media Classic offre la pagina Processi. Nella pagina Processi è possibile rivedere, caricare e pubblicare i processi, controllare lo stato dei processi e annullare la pubblicazione dei processi. Potete anche pianificare i processi di caricamento e pubblicazione.

Quando caricate delle risorse, viene visualizzata un’icona rotante accanto al menu Processi a indicare che è in corso un processo; viene inoltre visualizzato il numero di file inclusi in tale processo. Puoi selezionare l’icona per visualizzare ulteriori informazioni sul processo attivo.

>[!NOTE]
>
>nella pagina Attività recenti è disponibile un elenco dei processi pubblicati di recente. Seleziona **[!UICONTROL Recente]** sulla barra di navigazione globale.

## La pagina Processi {#about-the-jobs-page}

Seleziona **[!UICONTROL Processi]** sulla barra di navigazione globale, in modo che venga visualizzata la pagina Processi. Per impostazione predefinita, i processi più recenti vengono visualizzati all’inizio dell’elenco.

I processi vengono elencati in queste categorie nella scheda Cronologia della pagina Processi:

* **[!UICONTROL Tipo di processo]**: un’icona indica il tipo di processo: Carica e Pubblica sono i tipi di processo più comuni.

* **[!UICONTROL Nome processo]**: nome del processo. Il nome include la parte del nome immessa dall&#39;utente e la data e l&#39;ora.

* **[!UICONTROL Avviato]**: all’avvio del processo.

* **[!UICONTROL Totale]**: numero di file trasferiti.

* **[!UICONTROL W (avvisi)]**: numero di avvisi nel processo (se presenti). Le avvertenze indicano i problemi riscontrati durante il processo che tuttavia non ne hanno compromesso il completamento totale. Possono generalmente essere ignorate perché vengono segnalano file nascosti. Ad esempio: `.DS_store` I file (Mac) e i file Thumbs.db (Windows®) contengono informazioni su come visualizzare i file di immagine agli utenti. Le voci di avviso relative a questi file, tuttavia, possono essere ignorate perché non riguardano il modo in cui questi file vengono utilizzati in Adobe Dynamic Media Classic. Per visualizzare informazioni dettagliate sulle avvertenze di un processo, fate doppio clic sul nome corrispondente.

* **[!UICONTROL E (errori)]**: elenca il numero di errori nel processo (se presenti). Per visualizzare informazioni dettagliate sugli errori di un processo, fate doppio clic sul nome corrispondente.

* **[!UICONTROL Durata]**: tempo necessario per completare il processo.

* **[!UICONTROL Stato]**: mostra lo stato del processo.

* **[!UICONTROL Destinazione]**: per i processi di caricamento, la destinazione è il nome della società e la cartella in cui sono stati caricati i file. Questa categoria non si applica ai processi per la pubblicazione.

* **[!UICONTROL Inviato da]**: elenca chi ha caricato le risorse.

>[!NOTE]
>
>Puoi annullare i processi di pubblicazione e caricamento in corso selezionando la **[!UICONTROL Annulla]** accanto alla barra di avanzamento.

## Modificare le visualizzazioni nella pagina Processi {#changing-views-on-the-jobs-page}

Per ordinare i processi o modificare la visualizzazione della scheda Cronologia nella pagina Processi, effettuate le seguenti procedure:

* **[!UICONTROL Ordinamento]**: seleziona il nome di una colonna per ordinare l’elenco in base a una determinata colonna. Potete selezionare l’interruttore accanto al nome della colonna per impostare l’ordinamento ascendente o discendente.

* **[!UICONTROL Intervallo date]**: seleziona la **[!UICONTROL Intervallo date]** e scegliere un&#39;opzione per limitare l&#39;elenco dei job alla data corrente, alla settimana precedente o al mese precedente. Seleziona **[!UICONTROL Intervallo date personalizzato]**, quindi inserisci un intervallo di date specifico.

* **[!UICONTROL Tipo di processo]**: seleziona la **[!UICONTROL Tipo di processo]** e scegliere **[!UICONTROL Pubblica]** o **[!UICONTROL Carica]** restringere l&#39;elenco per la pubblicazione dei processi o il caricamento dei processi. Seleziona **[!UICONTROL Tutti]** per visualizzare entrambi i tipi di job.

* **[!UICONTROL Spettacolo]**: vai a **[!UICONTROL Spettacolo]** > **[!UICONTROL Processi personali]** o **[!UICONTROL Spettacolo]** > **[!UICONTROL Tutti i processi]** per restringere l&#39;elenco ai processi ordinati dall&#39;utente o ai processi ordinati dagli utenti della società.

## Visualizzare, copiare o stampare un rapporto Dettagli lavoro {#viewing-copying-or-printing-a-job-details-report}

Fare doppio clic sul nome di un report nella pagina Job per aprire la pagina Dettagli job. Questa pagina fornisce un rapporto riassuntivo sui file inclusi nel processo. Seleziona **[!UICONTROL Visualizza dettagli]** in modo da visualizzare l&#39;ID Adobe Dynamic Media Classic, il percorso di destinazione e le informazioni sullo stato di una voce. Se avete caricato un file PDF o PostScript che richiede font non disponibili in Adobe Dynamic Media Classic, il report elenca i font mancanti.

Potete copiare queste informazioni negli Appunti.

1. Fare doppio clic sul nome di un report nella pagina Processi.
1. Nella pagina Dettagli processo, seleziona **[!UICONTROL Visualizza dettagli]** per ottenere un rapporto dettagliato su una voce.
1. Seleziona **[!UICONTROL Copia negli Appunti]**.

## Gestire i processi di caricamento e pubblicazione ricorrenti {#handling-recurring-upload-and-publish-jobs}

I processi di caricamento e pubblicazione ricorrenti, creati nelle pagine Carica e Pubblica, sono elencati nella scheda Pianificato della pagina Processi. In questa schermata potete modificare ed eliminare i processi periodici.

Selezionare il pulsante Processi sulla barra di navigazione globale e nella pagina Processi selezionare **[!UICONTROL Pianificato]** in modo da poter modificare ed eliminare i processi ricorrenti.

>[!NOTE]
>
>Puoi filtrare l’elenco dei processi in base a **[!UICONTROL Pianificato]** scheda con **[!UICONTROL Tipo di processo]** e **[!UICONTROL Spettacolo]** menu. Selezionare un tipo di processo in modo da restringere l&#39;elenco in modo da pubblicare processi di un tipo specifico. Seleziona un **[!UICONTROL Spettacolo]** opzione che consente di visualizzare i processi creati o quelli creati da tutti gli utenti della società.

### Modifica, elimina, sospendi e riprendi processi ricorrenti {#editing-deleting-pausing-and-resuming-recurring-jobs}

Selezionare un job ricorrente nella pagina Job e seguire queste istruzioni se si desidera modificarlo o eliminarlo:

* **Modificare un processo ricorrente**: seleziona la **[!UICONTROL Modifica]** e immettere le informazioni sulla programmazione nella finestra di dialogo Modifica OdL programmato. Se si desidera che il processo ricorra a un intervallo desiderato, passare a **[!UICONTROL Ripeti]** > **[!UICONTROL Personalizzato]**.

Consulta [Creare un intervallo di tempo del processo di caricamento o pubblicazione personalizzato](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Eliminazione di un processo ricorrente**: seleziona la **[!UICONTROL Elimina]** pulsante.

* **Sospensione (e ripresa) di un processo ricorrente**: nella colonna Attivo deselezionare una casella di controllo per sospendere un processo; selezionare una casella di controllo per riprendere un processo sospeso.

### Creare un intervallo di tempo del processo di caricamento o pubblicazione personalizzato {#creating-a-custom-upload-or-publish-job-time-interval}

Per creare un intervallo di tempo personalizzato per un caricamento (tramite FTP) o per un processo di pubblicazione, nella pagina Caricamento o Pubblicazione vai a **[!UICONTROL Ripeti]** > **[!UICONTROL Personalizzato]**. Quindi immetti numeri e caratteri jolly nella casella Regola che descrive un intervallo di tempo per la ricorrenza dei processi di caricamento o pubblicazione.

La sintassi per la descrizione degli intervalli personalizzati di caricamento e pubblicazione nella casella Regola è la seguente:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Ad esempio: `0 15 10 * * ?` pianifica un processo alle 10:15.00 ogni giorno.

Nelle tabelle e nell’elenco seguenti viene illustrato come specificare un intervallo temporale nella casella Regola.

In questa tabella vengono visualizzati gli incrementi temporali, i relativi valori consentiti e i caratteri jolly supportati:

| Incrementi temporali  | Valori consentiti | Commenti | Caratteri jolly supportati |
|--- |--- |--- |--- |
| Secondi | 0-59 |  | `,: * /` |
| Minuti | 0-59 |  | `,: * /` |
| Ore | 0-23 | Notare l’uso dell’orologio costituito da 24 ore. | `,: * /` |
| Giorno del mese | 1-31 | Non è possibile specificare un valore numerico per &quot;giorno del mese&quot; e &quot;giorno della settimana&quot;. Uno di questi campi deve utilizzare un `?` carattere jolly. | `,: * / ? L C` |
| Mese | 1-12 o Gen, Feb, Mar, Apr, Mag, Giu, Lug, Ago, Set, Ott, Nov, Dic | I valori fanno distinzione tra maiuscole e minuscole. | `,: * /` |
| Giorno della settimana | Lun, Mar, Mer, Gio, Ven, Sab, Dom | I valori fanno distinzione tra maiuscole e minuscole. Non è possibile specificare un valore numerico per &quot;giorno del mese&quot; e &quot;giorno della settimana&quot;. Uno di questi campi deve utilizzare un `?` carattere jolly. | `,: * / ? L C #` |
| Anno (facoltativo) | Vuoto o 1970-2099 |  | `,: * /` |


Nella tabella seguente sono illustrati i caratteri jolly consentiti nella casella Regola e come usarli:

| Carattere jolly | Nome | Descrizione |
| --- | --- | --- |
| `*` | Asterisco | Tutti i valori (ad esempio, &quot;ogni minuto&quot;). |
| `?` | Punto interrogativo | Nessun valore specifico, ad esempio &quot;qualsiasi minuto entro l’ora specificata&quot;. |
| `,` | Virgola | Altri valori (ad esempio, &quot;Lunedì e mercoledì&quot;). |
| `-` | Trattino | Intervallo di valori (ad esempio, &quot;da lunedì a venerdì&quot;). |
| `/` | Barra | Incrementi (ad esempio, &quot;ogni 15 minuti&quot;). |
| `L` | L maiuscola | Ultimo &quot;giorno del mese&quot; o &quot;giorno della settimana&quot; (disponibile solo per questi campi). Ad esempio, se il mese è gennaio, un valore L per il campo &quot;giorno del mese&quot; pianifica il processo per il 31 gennaio. Per il campo &quot;giorno della settimana&quot;, è possibile immettere questo carattere solo per pianificare il lavoro il sabato. Puoi utilizzarlo con un numero (ad esempio, `6L`) per specificare l&#39;ultimo venerdì del mese. Non specificare `L` con i caratteri jolly virgola o trattino. |
| `#` | Segno di numero | &quot;Nth&quot; weekend day of the month (disponibile solo per il campo &quot;day of the week&quot;). Ad esempio: `6#3` nel campo &quot;giorno della settimana&quot; è specificato il terzo venerdì del mese. Il `6` indica &quot;Friday&quot; (il sesto giorno della settimana) e il `3` indica la terza occorrenza del mese. |
| `C` | # C maiuscolo | Primo calendario &quot;giorno del mese&quot; o &quot;giorno della settimana&quot; (disponibile solo per questi campi). Ad esempio, specificando un valore di `1C` per &quot;giorno del mese&quot; pianifica il primo giorno del calendario che si verifica il o dopo il quinto. Per il campo &quot;giorno della settimana&quot;, specificare `1C` pianifica il primo giorno del calendario che si verifica la domenica o dopo la domenica. |

Nell’elenco seguente sono illustrati alcuni esempi che descrivono gli intervalli temporali nella casella Regola:

* `0 0 12 * * ?` : mezzogiorno ogni giorno
* `0 15 10 ? * *` : 10:15 ogni giorno
* `0 0/5 14 * * ?`: ogni 5 minuti tra le 14:00 e le 14:55 ogni giorno
* `0 0/5 14,18 * * ?` : ogni 5 minuti tra le 14:00 e le 14:55 e ogni 5 minuti tra le 18:00 e le 18:55 ogni giorno
* `0 10,44 14 ? 3` : mercoledì alle 14:10 e alle 14:44 ogni mercoledì di marzo
* `0 15 10 ? *` : lunedì alle 10:15 tutti i giorni feriali
* `0 15 10 20 * ?` : alle 10:15 del 20 di ogni mese
* `0 15 10 L * ?` : alle 10:15 dell’ultimo giorno di ogni mese
* `0 15 10 ? * 6L` : alle 10:15 dell’ultimo venerdì di ogni mese
* `0 15 10 * * 6#3` : alle 10:15 del terzo venerdì di ogni mese

## Utilizzare un processo di caricamento o pubblicazione come attivatore {#using-an-upload-or-publish-job-as-a-trigger}

Quando carichi le risorse tramite FTP o esegui un processo di pubblicazione, puoi pianificare l’inizio di un processo successivo al termine del caricamento. Se è stato pianificato l&#39;inizio di altri processi, il processo pianificato in questa posizione verrà messo in coda dietro di essi. Il nuovo processo invia una notifica all&#39;indirizzo specificato in modo che il codice in tale posizione possa essere attivato. A questo processo di caricamento successivo viene assegnato lo stesso nome di quello corrente, con l’aggiunta del prefisso _Pub.

Per fare in modo che un processo di caricamento o pubblicazione attivi un altro processo, seleziona **[!UICONTROL Avanzate]** nella pagina Carica o Pubblica. Immettete quindi l’URL nel campo di testo Notifica HTTP.
