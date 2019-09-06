---
title: Verifica dei file di processo
seo-title: Verifica dei file di processo
description: 'null'
seo-description: Scoprite come controllare i file di processo.
uuid: 8241 a 894-3014-4 a 5 c -96 ef -71 f 3 aaa 3716 a
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/upload_ and_ publish_ assets
discoiquuid: d 53 ae 5 dd -8 daf -4 d 87-b 9 a 6-3039 bad 30538
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Verifica dei file di processo{#checking-job-files}

Per monitorare i file caricati in Scene 7 Publishing System e i file pubblicati sui server Dynamic Media Classic, SPS offre la pagina Processi. Nella pagina Processi potete visualizzare i processi di caricamento e pubblicazione, controllarne lo stato e annullare i processi di pubblicazione. Potete anche pianificare i processi di caricamento e pubblicazione.

Quando caricate delle risorse, viene visualizzata un’icona rotante accanto al menu Processi a indicare che è in corso un processo; viene inoltre visualizzato il numero di file inclusi in tale processo. Potete fare clic sull’icona per visualizzare ulteriori informazioni sul processo attivo. 

>[!NOTE]
>
>nella pagina Attività recenti è disponibile un elenco dei processi pubblicati di recente. Per aprire tale pagina, fate clic su Recente nella barra di navigazione globale.

## La pagina Processi {#about-the-jobs-page}

Per aprire la pagina Processi, fate clic sul pulsante Processi nella barra di navigazione globale. Per impostazione predefinita, i processi più recenti vengono visualizzati all’inizio dell’elenco.

I processi vengono elencati in queste categorie nella scheda Cronologia della pagina Processi:

**Tipo processo** Un'icona indica il tipo di processo: I tipi di processi più comuni sono Caricamento e Pubblica.

**Nome processo** Il nome del processo. Il nome include la parte del nome immessa dall’utente e il timbro della data e dell’ora.

**Iniziato** all'avvio del processo.

**Totale** Il numero di file trasferiti.

**W (avvisi)** Il numero di avvertenze nel processo (se presenti). Le avvertenze indicano i problemi riscontrati durante il processo che tuttavia non ne hanno compromesso il completamento totale. Possono generalmente essere ignorate perché vengono segnalano file nascosti. Ad esempio, i file con estensione DS_store (Macintosh) e Thumbs.db (Windows) contengono informazioni sulla modalità di visualizzazione dei file immagine agli utenti. Le voci di avviso relative a questi file possono tuttavia essere ignorate perché non riguardano il modo in cui questi file vengono utilizzati in Dynamic Media Classic. Per visualizzare informazioni dettagliate sulle avvertenze di un processo, fate doppio clic sul nome corrispondente.

**E (Errori)** Elenca il numero di errori nel processo. Per visualizzare informazioni dettagliate sugli errori di un processo, fate doppio clic sul nome corrispondente.

**Durata** Tempo necessario per completare il processo.

**Stato** Mostra lo stato del processo.

**Destinazione** Per i processi di caricamento, il nome della società e la cartella in cui sono stati caricati i file. Questa categoria non può essere applicata ai processi di pubblicazione.

**Inviato da** Elenca gli utenti che hanno caricato le risorse.

***Nota**: Per annullare i processi di pubblicazione e caricamento in corso, fate clic sul pulsante Annulla accanto alla barra di avanzamento.*

## Modifica delle visualizzazioni nella pagina Processi {#changing-views-on-the-jobs-page}

Per ordinare i processi o modificare la visualizzazione della scheda Cronologia nella pagina Processi, effettuate le seguenti procedure:

**Ordinamento** Consente di selezionare un nome di colonna per ordinare l'elenco in base a una particolare colonna. Potete selezionare l’interruttore accanto al nome della colonna per impostare l’ordinamento ascendente o discendente.

**Intervallo** date Selezionate il menu Intervallo date e scegliete un'opzione per limitare l'elenco dei processi alla data corrente, alla settimana precedente o al mese precedente. Per immettere un intervallo date specifico, scegliete Intervallo di date personalizzato.

**Tipo processo** Selezionate il menu Tipo processo e scegliete Pubblica o Carica per limitare l'elenco ai processi di pubblicazione o di caricamento. Per visualizzare entrambi i tipi di processi, scegliete Tutto. 

**Scegliete** Mostra &gt; Processi personali o Mostra &gt; Tutti i processi per limitare l'elenco ai processi ordinati o ai processi ordinati dalla società aziendale.

## Visualizzazione, copia o stampa di un rapporto Dettagli processo {#viewing-copying-or-printing-a-job-details-report}

Per aprire la pagina Dettagli processo, fate doppio clic sul nome di un rapporto nella pagina Processi. Questa pagina fornisce un rapporto riassuntivo sui file inclusi nel processo. Fate clic su Visualizzazione dettagli per visualizzare l’ID SPS di una voce, il percorso di destinazione e le informazioni sul suo stato. Se avete caricato un file PDF o PostScript che richiede font non disponibili in SPS, nel rapporto vengono visualizzati i font mancanti.

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

**Editing a recurring job** Select the Edit button and enter schedule information in the Edit Scheduled Job dialog box. Per pianificare l’esecuzione del processo a un intervallo desiderato, scegliete Ripeti &gt; Personalizzato.

Consultate [Creazione di un intervallo personalizzato per un processo di caricamento o pubblicazione](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

**Deleting a recurring job** Select the Delete button.

**Pausing (and resuming) a recurring job** In the Active column, deselect a check box to pause a job; select a check box to resume a job that was paused.

### Creazione di un intervallo personalizzato per un processo di caricamento o pubblicazione {#creating-a-custom-upload-or-publish-job-time-interval}

Per creare un intervallo personalizzato per un processo di caricamento (Mediante FTP) o pubblicazione, scegliete Ripeti &gt; Personalizzato nella pagina Carica o Pubblica. Immettete quindi i numeri e i caratteri jolly nella casella Regola per descrivere un intervallo in cui eseguire i processi di caricamento o pubblicazione periodici. 

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
| Mese | 1-12 o Gen, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Sep, Ott, Nov | I valori seguono la distinzione tra maiuscole e minuscole. | , - * / |
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
| L | L maiuscola | Ultimo “giorno del mese” o “giorno della settimana” (disponibile solo per questi campi). Se ad esempio il mese è Gennaio, un valore L per il campo “giorno del mese” pianifica l’esecuzione del processo per il 31 gennaio.Per il campo “giorno della settimana” potete immettere solo questo carattere per pianificare il processo ogni sabato. Potete utilizzarlo con un numero (ad esempio, 6 L) per specificare l'ultimo venerdì del mese. Non specificate L con i caratteri jolly virgola o trattino. |
| # | Segno di numero | “Ennesimo” giorno del mese (disponibile solo per il campo “giorno della settimana”).Ad esempio, 6#3 nel campo “giorno della settimana” indica il terzo venerdì del mese. Il 6 indica “Venerdì” (il sesto giorno della settimana) e il 3 indica la terza occorrenza nel mese. |
| C | # C maiuscolo | Primo “giorno del mese” o “giorno della settimana” del calendario (disponibile solo per questi campi). Ad esempio, specificando un valore 1 C per «giorno del mese» si pianifica il primo giorno del calendario che si verifica entro o dopo la quinta. Per il campo «giorno della settimana», specificando 1 C si pianifica il primo giorno nel calendario che si verifica in base o dopo Domenica |

Nell’elenco seguente sono illustrati alcuni esempi che descrivono gli intervalli temporali nella casella Regola:

* 0 0 12 * * ?: tutti i giorni a mezzogiorno
* 0 15 10 ? * *: 10:15 di ogni giorno
* 0 0/5 14 * * ?: ogni 5 minuti tra le 14:00 e le 14:55 di ogni giorno
* 0 0/5 14,18 * * ?: ogni 5 minuti tra le 14:00 e le 14:55 di ogni giorno e ogni 5 minuti tra le 18:00 e le 18:55 di ogni giorno
* 0 10,44 14 ? 3: Wed alle 14:10 e alle 14:44 ogni mercoledì di marzo
* 0 15 10 ? *: Li-Fren alle 10:15 ogni giorno feriale
* 0 15 10 20 * ?: alle 10:15 il 20 di ogni mese
* 0 15 10 L * ?: alle 10:15 l’ultimo giorno di ogni mese
* 0 15 10 ? * 6L: alle 10:15 l’ultimo venerdì di ogni mese
* 0 15 10 * * 6#3: alle 10:15 il terzo venerdì di ogni mese

## Utilizzo di un processo di caricamento o pubblicazione come trigger {#using-an-upload-or-publish-job-as-a-trigger}

Quando caricate risorse mediante FTP o eseguite un processo di pubblicazione, potete pianificare l’inizio di un processo successivo subito dopo il termine del caricamento. Se all’ora specificata è pianificato l’inizio di altri processi, il processo impostato in questo campo verrà messo in coda. Il nuovo processo invia una notifica all’indirizzo specificato per poter attivare il codice nella posizione esatta. A questo processo di caricamento successivo viene assegnato lo stesso nome di quello corrente, con l’aggiunta del prefisso _Pub.

Per fare in modo che un processo di caricamento o pubblicazione ne attivi un altro, selezionate Avanzate nella pagina Carica o Pubblica. Immettete quindi l’URL nel campo di testo Notifica HTTP.
