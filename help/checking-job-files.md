---
title: Verifica dei file di processo
seo-title: Verifica dei file di processo
description: 'null'
seo-description: Scoprite come controllare i file di processo.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 71%

---


# Verifica dei file di processo{#checking-job-files}

Per monitorare i file caricati in Dynamic Media Classic e i file pubblicati sui server Dynamic Media Classic, la pagina Processi di Dynamic Media Classic è disponibile. Nella pagina Processi potete visualizzare i processi di caricamento e pubblicazione, controllarne lo stato e annullare i processi di pubblicazione. Potete anche pianificare i processi di caricamento e pubblicazione.

Quando caricate delle risorse, viene visualizzata un’icona rotante accanto al menu Processi a indicare che è in corso un processo; viene inoltre visualizzato il numero di file inclusi in tale processo. Potete fare clic sull’icona per visualizzare ulteriori informazioni sul processo attivo. 

>[!NOTE]
>
>nella pagina Attività recenti è disponibile un elenco dei processi pubblicati di recente. Per aprire tale pagina, fate clic su Recente nella barra di navigazione globale.

## La pagina Processi {#about-the-jobs-page}

Per aprire la pagina Processi, fate clic sul pulsante Processi nella barra di navigazione globale. Per impostazione predefinita, i processi più recenti vengono visualizzati all’inizio dell’elenco.

I processi vengono elencati in queste categorie nella scheda Cronologia della pagina Processi:

**Tipo** processo Un’icona indica il tipo di processo: Caricare e pubblicare sono i tipi di processi più comuni.

**Nome** processo Il nome del processo. Il nome include la parte del nome immessa dall’utente e il timbro della data e dell’ora.

**Avviato** All’inizio del processo.

**Totale** Il numero di file trasferiti.

**W (avvertenze)** Numero di eventuali avvertenze nel processo. Le avvertenze indicano i problemi riscontrati durante il processo che tuttavia non ne hanno compromesso il completamento totale. Possono generalmente essere ignorate perché vengono segnalano file nascosti. Ad esempio, i file con estensione DS_store (Macintosh) e Thumbs.db (Windows) contengono informazioni sulla modalità di visualizzazione dei file immagine agli utenti. Le voci di avviso relative a questi file, tuttavia, possono essere ignorate perché non riguardano la modalità di utilizzo di tali file in Dynamic Media Classic. Per visualizzare informazioni dettagliate sulle avvertenze di un processo, fate doppio clic sul nome corrispondente.

**E (errori)** Elenca il numero di eventuali errori nel processo. Per visualizzare informazioni dettagliate sugli errori di un processo, fate doppio clic sul nome corrispondente.

**Durata** : tempo necessario per completare il processo.

**Stato** Mostra lo stato del processo.

**Destinazione** Per i processi di caricamento, il nome della società e la cartella in cui sono stati caricati i file. Questa categoria non può essere applicata ai processi di pubblicazione.

**Inviato** da elenchi che hanno caricato le risorse.

***Nota **: Per annullare i processi di pubblicazione e caricamento in corso, fate clic sul pulsante Annulla accanto alla barra di avanzamento.*

## Modifica delle visualizzazioni nella pagina Processi {#changing-views-on-the-jobs-page}

Per ordinare i processi o modificare la visualizzazione della scheda Cronologia nella pagina Processi, effettuate le seguenti procedure:

**Ordinamento** Selezionare un nome di colonna per ordinare l&#39;elenco in base a una particolare colonna. Potete selezionare l’interruttore accanto al nome della colonna per impostare l’ordinamento ascendente o discendente.

**Intervallo** date Selezionate il menu Intervallo date e scegliete un’opzione per limitare l’elenco dei processi alla data corrente, alla settimana precedente o al mese precedente. Per immettere un intervallo date specifico, scegliete Intervallo di date personalizzato.

**Tipo** processo Selezionate il menu Tipo processo e scegliete Pubblica o Carica per limitare l’elenco ai soli processi di pubblicazione o caricamento. Per visualizzare entrambi i tipi di processi, scegliete Tutto. 

**Mostra** scegliere Mostra > Processi personali o Mostra > Tutti i processi per limitare l’elenco ai soli processi ordinati o ai processi ordinati dagli utenti della società.

## Visualizzazione, copia o stampa di un rapporto Dettagli lavoro {#viewing-copying-or-printing-a-job-details-report}

Per aprire la pagina Dettagli processo, fate doppio clic sul nome di un rapporto nella pagina Processi. Questa pagina fornisce un rapporto riassuntivo sui file inclusi nel processo. Fate clic su Visualizza dettaglio per visualizzare l’ID Dynamic Media Classic di una voce, il percorso di destinazione e le informazioni sullo stato. Se avete caricato un file PDF o PostScript che richiede font non disponibili in Dynamic Media Classic, nel rapporto vengono elencati i font mancanti.

Potete copiare queste informazioni negli Appunti.

1. Per aprire la pagina Dettagli processo, fate doppio clic sul nome di un rapporto nella pagina Processi. 
1. Per visualizzare un rapporto dettagliato su una voce del rapporto, fate clic su Visualizza dettaglio.
1. Fate clic su Copia negli appunti.

## Gestione di processi di caricamento e pubblicazione periodici {#handling-recurring-upload-and-publish-jobs}

I processi di caricamento e pubblicazione periodici creati nelle pagine Carica e Pubblica sono visualizzati nella scheda Pianificati della pagina Processi. In questa schermata potete modificare ed eliminare i processi periodici.

Per modificare ed eliminare i processi periodici, fate clic sul pulsante Processi nella barra di navigazione globale e selezionate la scheda Pianificati nella pagina Processi.

>[!NOTE]
>
>per filtrare l’elenco dei processi nella scheda Pianificati, selezionate i menu Tipo processo e Mostra. Per restringere l’elenco includendo solo i processi di pubblicazione di un determinato tipo, scegliete Tipo processo. Per visualizzare i processi creati da voi o da qualsiasi utente aziendale, scegliete l’opzione Mostra.

### Modifica, eliminazione, sospensione e ripristino di processi periodici {#editing-deleting-pausing-and-resuming-recurring-jobs}

Selezionate un processo periodico nella pagina Processi e seguite le seguenti istruzioni per modificarlo o eliminarlo:

**Modifica di un processo** periodico Selezionare il pulsante Modifica e immettere le informazioni sulla pianificazione nella finestra di dialogo Modifica processo pianificato. Per pianificare l’esecuzione del processo a un intervallo desiderato, scegliete Ripeti > Personalizzato.

Consultate [Creazione di un intervallo personalizzato per un processo di caricamento o pubblicazione](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

**Eliminazione di un processo** periodico Fate clic sul pulsante Elimina.

**Sospensione (e ripristino) di un processo** periodico Nella colonna Attivo, deselezionate una casella di controllo per sospendere un processo; selezionate una casella di controllo per riprendere un processo in pausa.

### Creazione di un intervallo personalizzato per un processo di caricamento o pubblicazione {#creating-a-custom-upload-or-publish-job-time-interval}

Per creare un intervallo personalizzato per un processo di caricamento (Mediante FTP) o pubblicazione, scegliete Ripeti > Personalizzato nella pagina Carica o Pubblica. Immettete quindi i numeri e i caratteri jolly nella casella Regola per descrivere un intervallo in cui eseguire i processi di caricamento o pubblicazione periodici. 

La sintassi per la descrizione degli intervalli personalizzati di caricamento e pubblicazione nella casella Regola è la seguente:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

For example, `0 15 10 * * ?` schedules a job at 10:15.00 every day.

Nelle tabelle e nell’elenco seguenti viene illustrato come specificare un intervallo temporale nella casella Regola.

In questa tabella vengono visualizzati gli incrementi temporali, i relativi valori consentiti e i caratteri jolly supportati:

| Incrementi temporali  | Valori consentiti | Commenti | Caratteri jolly supportati |
|--- |--- |--- |--- |
| Secondi | 0-59 |  | , - * / |
| Minuti | 0-59 |  | , - * / |
| Ore | 0-23 | Notare l’uso dell’orologio costituito da 24 ore. | , - * / |
| Giorno del mese | 1-31 | Per “giorno del mese” e “giorno della settimana” non potete specificare valori numerici. Uno di questi campi deve usare un carattere jolly ? . | , - * / ? L C |
| Mese | 1-12 o gen, feb, mar, Apr, May, Jun, Jul, Aug, set, set, ott, nov, dic | I valori seguono la distinzione tra maiuscole e minuscole. | , - * / |
| Giorno della settimana | Lun, Mar, Mer, Gio, Ven, Sab, Dom | I valori seguono la distinzione tra maiuscole e minuscole. Per “giorno del mese” e “giorno della settimana” non potete specificare valori numerici. Uno di questi campi deve usare un carattere jolly ? . | , - * / ? L C # |
| Anno (facoltativo) | Vuoto o 1970-2099 |  | , - * / |


Nella tabella seguente sono illustrati i caratteri jolly consentiti nella casella Regola e come usarli:

| Carattere jolly | Nome | Descrizione |
|--- |--- |--- |
| * | Asterisco | Tutti i valori (ad esempio “ogni minuto”). |
| ? | Punto interrogativo | Nessun valore specifico (ad esempio, “un minuto qualsiasi nell’ora specificata”). |
| , | Virgola | Valori aggiuntivi (ad esempio “Lunedì e Mercoledì”). |
| - | Trattino | Intervallo di valori (ad esempio “Da lunedì a venerdì”). |
| / | Barra | Incrementi (ad esempio, “ogni 15 minuti”). |
| L | L maiuscola | Ultimo “giorno del mese” o “giorno della settimana” (disponibile solo per questi campi). Se ad esempio il mese è Gennaio, un valore L per il campo “giorno del mese” pianifica l’esecuzione del processo per il 31 gennaio.Per il campo “giorno della settimana” potete immettere solo questo carattere per pianificare il processo ogni sabato. È possibile utilizzarlo con un numero (ad esempio, 6L) per specificare l&#39;ultimo venerdì del mese. Non specificare L con i caratteri jolly virgola o trattino. |
| # | Segno di numero | “Ennesimo” giorno del mese (disponibile solo per il campo “giorno della settimana”).Ad esempio, 6#3 nel campo “giorno della settimana” indica il terzo venerdì del mese. Il 6 indica “Venerdì” (il sesto giorno della settimana) e il 3 indica la terza occorrenza nel mese. |
| C | # C maiuscolo | Primo “giorno del mese” o “giorno della settimana” del calendario (disponibile solo per questi campi). Ad esempio, se si specifica un valore di 1C per &quot;giorno del mese&quot;, il primo giorno del calendario viene pianificato il quinto o dopo il quinto. Per il campo &quot;giorno della settimana&quot;, specificando 1C il primo giorno del calendario viene pianificato il primo giorno del calendario che si verifica o dopo la domenica |

Nell’elenco seguente sono illustrati alcuni esempi che descrivono gli intervalli temporali nella casella Regola:

* 0 0 12 * * ?: tutti i giorni a mezzogiorno
* 0 15 10 ? * *: 10:15 di ogni giorno
* 0 0/5 14 * * ?: ogni 5 minuti tra le 14:00 e le 14:55 di ogni giorno
* 0 0/5 14,18 * * ?: ogni 5 minuti tra le 14:00 e le 14:55 di ogni giorno e ogni 5 minuti tra le 18:00 e le 18:55 di ogni giorno
* 0 10,44 14 ? 3: Wed alle 14:10 e alle 14:44 ogni mercoledì di marzo
* 0 15 10 ? *: Da lun a ven alle 10:15 di ogni giorno feriale
* 0 15 10 20 * ?: alle 10:15 il 20 di ogni mese
* 0 15 10 L * ?: alle 10:15 l’ultimo giorno di ogni mese
* 0 15 10 ? * 6L: alle 10:15 l’ultimo venerdì di ogni mese
* 0 15 10 * * 6#3: alle 10:15 il terzo venerdì di ogni mese

## Utilizzo di un processo di caricamento o pubblicazione come trigger {#using-an-upload-or-publish-job-as-a-trigger}

Quando caricate risorse mediante FTP o eseguite un processo di pubblicazione, potete pianificare l’inizio di un processo successivo subito dopo il termine del caricamento. Se all’ora specificata è pianificato l’inizio di altri processi, il processo impostato in questo campo verrà messo in coda. Il nuovo processo invia una notifica all’indirizzo specificato per poter attivare il codice nella posizione esatta. A questo processo di caricamento successivo viene assegnato lo stesso nome di quello corrente, con l’aggiunta del prefisso _Pub.

Per fare in modo che un processo di caricamento o pubblicazione ne attivi un altro, selezionate Avanzate nella pagina Carica o Pubblica. Immettete quindi l’URL nel campo di testo Notifica HTTP.
