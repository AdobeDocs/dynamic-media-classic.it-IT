---
title: Controllare i file di processo
description: Scopri come controllare i file di lavoro in Adobe Dynamic Media Classic.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1592'
ht-degree: 40%

---

# Controllare i file di processo{#checking-job-files}

Per monitorare i caricamenti di file nell’Adobe Dynamic Media Classic e i file pubblicati nei server Adobe Dynamic Media Classic, la pagina Processi è disponibile in Adobe Dynamic Media Classic. Nella pagina Processi potete visualizzare i processi di caricamento e pubblicazione, controllarne lo stato e annullare i processi di pubblicazione. Potete anche pianificare i processi di caricamento e pubblicazione.

Quando caricate delle risorse, viene visualizzata un’icona rotante accanto al menu Processi a indicare che è in corso un processo; viene inoltre visualizzato il numero di file inclusi in tale processo. Puoi selezionare l’icona per visualizzare ulteriori informazioni sul processo attivo.

>[!NOTE]
>
>nella pagina Attività recenti è disponibile un elenco dei processi pubblicati di recente. Seleziona **[!UICONTROL Recente]** nella barra di navigazione globale.

## La pagina Processi {#about-the-jobs-page}

Seleziona **[!UICONTROL Processi]** nella barra di navigazione globale per aprire la pagina Processi . Per impostazione predefinita, i processi più recenti vengono visualizzati all’inizio dell’elenco.

I processi vengono elencati in queste categorie nella scheda Cronologia della pagina Processi:

* **[!UICONTROL Tipo di processo]**  - Un&#39;icona indica il tipo di processo: Caricare e pubblicare sono i tipi di lavoro più comuni.

* **[!UICONTROL Nome processo]** : il nome del processo. Il nome include la parte del nome inserita dall’utente e la data e l’ora.

* **[!UICONTROL Avviato]** : all&#39;avvio del processo.

* **[!UICONTROL Totale]**  - Il numero di file trasferiti.

* **[!UICONTROL W (avvisi)]**  - Il numero di avvisi nel processo (se presenti). Le avvertenze indicano i problemi riscontrati durante il processo che tuttavia non ne hanno compromesso il completamento totale. Possono generalmente essere ignorate perché vengono segnalano file nascosti. Ad esempio, i file `.DS_store` (Macintosh) e i file Thumbs.db (Windows®) contengono informazioni su come visualizzare i file immagine agli utenti. Le voci di avviso relative a questi file, tuttavia, possono essere ignorate perché non riguardano il modo in cui questi file vengono utilizzati in Adobe Dynamic Media Classic. Per visualizzare informazioni dettagliate sulle avvertenze di un processo, fate doppio clic sul nome corrispondente.

* **[!UICONTROL E (errori)]**  - Elenca il numero di errori nel processo (se presenti). Per visualizzare informazioni dettagliate sugli errori di un processo, fate doppio clic sul nome corrispondente.

* **[!UICONTROL Durata]**  - Quanto tempo è necessario per completare il lavoro.

* **[!UICONTROL Stato]**  - Mostra lo stato del processo.

* **[!UICONTROL Destinazione]** : per i processi di caricamento, il nome dell’azienda e la cartella in cui sono stati caricati i file. Questa categoria non può essere applicata ai processi di pubblicazione.

* **[!UICONTROL Inviato da]** : elenca gli utenti che hanno caricato le risorse.

>[!NOTE]
>
>Per annullare i processi di pubblicazione e caricamento in corso, seleziona il pulsante **[!UICONTROL Annulla]** accanto alla barra di avanzamento.

## Modificare le visualizzazioni nella pagina Processi {#changing-views-on-the-jobs-page}

Per ordinare i processi o modificare la visualizzazione della scheda Cronologia nella pagina Processi, effettuate le seguenti procedure:

* **[!UICONTROL Ordinamento]** : consente di selezionare un nome di colonna per ordinare l’elenco in base a una particolare colonna. Potete selezionare l’interruttore accanto al nome della colonna per impostare l’ordinamento ascendente o discendente.

* **[!UICONTROL Intervallo date]** : seleziona il menu  **[!UICONTROL Intervallo]** date e scegli un’opzione per limitare l’elenco dei processi alla data corrente, alla settimana precedente o al mese precedente. Seleziona **[!UICONTROL Intervallo date personalizzato]**, quindi inserisci un intervallo di date specifico.

* **[!UICONTROL Tipo di lavoro]** : seleziona il  **[!UICONTROL menu]** Tipo di lavoro e scegli  **** Editore o  **** Carica per restringere l’elenco in modo da pubblicare i lavori o caricare i lavori. Seleziona **[!UICONTROL Tutto]** per visualizzare entrambi i tipi di processi.

* **[!UICONTROL Mostra]**  - Vai a  **[!UICONTROL Mostra]**  >  **[!UICONTROL My]** Jobsor  **[!UICONTROL Show]** >  **[!UICONTROL Tutti i]** Jobsto restringere l&#39;elenco ai lavori ordinati o ai lavori ordinati dalle persone della tua azienda.

## Visualizzare, copiare o stampare un rapporto Dettagli lavoro {#viewing-copying-or-printing-a-job-details-report}

Fare doppio clic sul nome di un rapporto nella pagina Processi per aprire la pagina Dettagli processo. Questa pagina fornisce un rapporto riassuntivo sui file inclusi nel processo. Seleziona **[!UICONTROL Visualizza dettagli]** per visualizzare l’Adobe Dynamic Media Classic ID di una voce, il percorso di destinazione e le informazioni sullo stato. Se hai caricato un file PDF o PostScript che richiede font non disponibili in Adobe Dynamic Media Classic, il rapporto elenca i font mancanti.

Potete copiare queste informazioni negli Appunti.

1. Fare doppio clic sul nome di un rapporto nella pagina Processi.
1. Nella pagina Dettagli processo, seleziona **[!UICONTROL Visualizza dettaglio]** per ottenere un rapporto dettagliato su una voce.
1. Selezionare **[!UICONTROL Copia negli Appunti]**.

## Gestire processi di caricamento e pubblicazione ricorrenti {#handling-recurring-upload-and-publish-jobs}

I processi di caricamento e pubblicazione periodici creati nelle pagine Carica e Pubblica sono visualizzati nella scheda Pianificati della pagina Processi. In questa schermata potete modificare ed eliminare i processi periodici.

Seleziona il pulsante Processi nella barra di navigazione globale e, nella pagina Processi, seleziona la scheda **[!UICONTROL Pianificato]** in modo da poter modificare ed eliminare i lavori ricorrenti.

>[!NOTE]
>
>È possibile filtrare l&#39;elenco dei processi nella scheda **[!UICONTROL Pianificato]** con i menu **[!UICONTROL Tipo di lavoro]** e **[!UICONTROL Mostra]**. Seleziona un tipo di processo in modo da restringere l’elenco per pubblicare lavori di un tipo specifico. Seleziona un&#39;opzione **[!UICONTROL Mostra]** se desideri visualizzare i lavori creati o quelli creati da tutti gli utenti dell&#39;azienda.

### Modificare, eliminare, mettere in pausa e riprendere i processi ricorrenti {#editing-deleting-pausing-and-resuming-recurring-jobs}

Seleziona un processo ricorrente nella pagina Processi e segui queste istruzioni se desideri modificarlo o eliminarlo:

* **Modifica un processo ricorrente** : seleziona il pulsante  **** Modifica e inserisci le informazioni sulla pianificazione nella finestra di dialogo Modifica processo pianificato. Se desideri che il processo si ripeta a un intervallo desiderato, passa a **[!UICONTROL Ripeti]** > **[!UICONTROL Personalizzato]**.

Consulta [Creare un intervallo personalizzato di caricamento o pubblicazione dei processi](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Eliminazione di un processo**  ricorrente - Selezionare il pulsante  **** Elimina.

* **Sospensione (e ripresa) di un processo**  ricorrente - Nella colonna Attivo deselezionare una casella di controllo per mettere in pausa un processo; selezionare una casella di controllo per riprendere un processo in pausa.

### Crea un intervallo personalizzato per il processo di caricamento o pubblicazione {#creating-a-custom-upload-or-publish-job-time-interval}

Per creare un intervallo di tempo personalizzato per un caricamento (tramite FTP) o un processo di pubblicazione, nella pagina Carica o Pubblica , passa a **[!UICONTROL Ripeti]** > **[!UICONTROL Personalizzato]**. Quindi inserisci numeri e caratteri jolly nella casella Regola che descrivono un intervallo di tempo per i processi di caricamento o pubblicazione da ripetere.

La sintassi per la descrizione degli intervalli personalizzati di caricamento e pubblicazione nella casella Regola è la seguente:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Ad esempio, `0 15 10 * * ?` pianifica un lavoro alle 10:15.00 ogni giorno.

Nelle tabelle e nell’elenco seguenti viene illustrato come specificare un intervallo temporale nella casella Regola.

In questa tabella vengono visualizzati gli incrementi temporali, i relativi valori consentiti e i caratteri jolly supportati:

| Incrementi temporali  | Valori consentiti | Commenti | Caratteri jolly supportati |
|--- |--- |--- |--- |
| Secondi | 0-59 |  | `, - * /` |
| Minuti | 0-59 |  | `, - * /` |
| Ore | 0-23 | Notare l’uso dell’orologio costituito da 24 ore. | `, - * /` |
| Giorno del mese | 1-31 | Per “giorno del mese” e “giorno della settimana” non potete specificare valori numerici. Uno di questi campi deve utilizzare un carattere jolly `?`. | `, - * / ? L C` |
| Mese | 1-12 o gen, feb, mar, Apr, May, Jun, Jul, Aug, Set, Set, ott, nov, Dec | I valori sono sensibili all’uso di maiuscole e minuscole. | `, - * /` |
| Giorno della settimana | Lun, Mar, Mer, Gio, Ven, Sab, Dom | I valori sono sensibili all’uso di maiuscole e minuscole. Per “giorno del mese” e “giorno della settimana” non potete specificare valori numerici. Uno di questi campi deve utilizzare un carattere jolly `?`. | `, - * / ? L C #` |
| Anno (facoltativo) | Vuoto o 1970-2099 |  | `, - * /` |


Nella tabella seguente sono illustrati i caratteri jolly consentiti nella casella Regola e come usarli:

| Carattere jolly | Nome | Descrizione |
|--- |--- |--- |
| `*` | Asterisco | Tutti i valori (ad esempio “ogni minuto”). |
| `?` | Punto interrogativo | Nessun valore specifico (ad esempio, “un minuto qualsiasi nell’ora specificata”). |
| `,` | Virgola | Altri valori (ad esempio, &quot;Lunedì e Mercoledì&quot;). |
| `-` | Trattino | Intervallo di valori (ad esempio “Da lunedì a venerdì”). |
| `/` | Barra | Incrementi (ad esempio, “ogni 15 minuti”). |
| `L` | L maiuscola | Ultimo “giorno del mese” o “giorno della settimana” (disponibile solo per questi campi). Se ad esempio il mese è Gennaio, un valore L per il campo “giorno del mese” pianifica l’esecuzione del processo per il 31 gennaio. Per il campo “giorno della settimana” potete immettere solo questo carattere per pianificare il processo ogni sabato. È possibile utilizzarlo con un numero (ad esempio, `6L`) per specificare l’ultimo venerdì del mese. Non specificare `L` con i caratteri jolly virgola o trattino. |
| `#` | Segno di numero | “Ennesimo” giorno del mese (disponibile solo per il campo “giorno della settimana”). Ad esempio, `6#3` nel campo &quot;giorno della settimana&quot; specifica il terzo venerdì del mese. Il `6` indica &quot;Friday&quot; (il sesto giorno della settimana) e il `3` indica la terza occorrenza del mese. |
| `C` | # C maiuscolo | Primo “giorno del mese” o “giorno della settimana” del calendario (disponibile solo per questi campi). Ad esempio, specificando un valore di `1C` per &quot;giorno del mese&quot; si pianifica il primo giorno del calendario che si verifica a partire dal quinto. Per il campo &quot;giorno della settimana&quot;, specificando `1C` si pianifica il primo giorno del calendario che si verifica la domenica o dopo tale data |

Nell’elenco seguente sono illustrati alcuni esempi che descrivono gli intervalli temporali nella casella Regola:

* `0 0 12 * * ?` : tutti i giorni a mezzogiorno
* `0 15 10 ? * *` : 10:15 di ogni giorno
* `0 0/5 14 * * ?`: ogni 5 minuti tra le 14:00 e le 14:55 di ogni giorno
* `0 0/5 14,18 * * ?` : ogni 5 minuti tra le 14:00 e le 14:55 di ogni giorno e ogni 5 minuti tra le 18:00 e le 18:55 di ogni giorno
* `0 10,44 14 ? 3` : Wed alle 14:10 e alle 14:44 ogni mercoledì di marzo
* `0 15 10 ? *` : Venerdì alle 10:15 di ogni giorno feriale
* `0 15 10 20 * ?` : alle 10:15 il 20 di ogni mese
* `0 15 10 L * ?` : alle 10:15 l’ultimo giorno di ogni mese
* `0 15 10 ? * 6L` : alle 10:15 l’ultimo venerdì di ogni mese
* `0 15 10 * * 6#3` : alle 10:15 il terzo venerdì di ogni mese

## Utilizzare un processo di caricamento o pubblicazione come attivatore {#using-an-upload-or-publish-job-as-a-trigger}

Quando carichi le risorse tramite FTP o esegui un processo di pubblicazione, puoi pianificare un processo successivo affinché inizi una volta completato il caricamento. (Se sono programmati altri lavori per l&#39;inizio, il lavoro pianificato viene messo in coda dietro di essi.) Il nuovo processo invia una notifica all’indirizzo specificato per poter attivare il codice nella posizione esatta. A questo processo di caricamento successivo viene assegnato lo stesso nome di quello corrente, con l’aggiunta del prefisso _Pub.

Per fare in modo che un processo di caricamento o pubblicazione attivi un altro processo, seleziona **[!UICONTROL Avanzate]** nella pagina Carica o Pubblica . Immettete quindi l’URL nel campo di testo Notifica HTTP.
