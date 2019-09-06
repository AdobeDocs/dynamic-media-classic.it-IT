---
title: Impostazione amministrazione
seo-title: Impostazione amministrazione
description: 'null'
seo-description: Scoprite come configurare l'area di amministrazione di Dynamic Media Classic.
uuid: 16 ba 9 fed-b 5 c 6-4991-83 b 3-8 d 7 d 7129013 a
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 3 c 9 ee 4 ec-dd 37-498 d -98 d 6-1339 b 80177 ff
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Impostazione amministrazione{#administration-setup}

Le schermate Impostazione amministrazione consentono di gestire gli utenti di Scene7 Publishing System. Usate queste schermate per consentire agli utenti di lavorare in Scene7 Publishing System e per comunicare con gli utenti tramite e-mail.

1. To access Administration Setup options, click **Setup** &gt; **Personal Setup** &gt; **Administration Setup**.

## Amministrazione utente {#user-administration}

A tutti gli utenti Dynamic Media Classic viene assegnato un ruolo che ne determina privilegi e diritti di accesso alle funzioni di Scene 7 Publishing System. Gli amministratori specificano i diversi ruoli e responsabilità per le società a cui sono assegnati.

In genere, Dynamic Media Classic configura il primo gruppo di società e assegna un amministratore della società. L’amministratore della società imposta e gestisce quindi gli utenti di Scene7 Publishing System.

Scene7 Publishing System supporta tre ruoli utente. Tutti e tre i ruoli possono accedere alle società configurate per Scene7 Publishing System:

**Amministratore SPS** Può visualizzare e amministrare tutte le funzioni di Scene 7 Publishing System, nonché configurare società e aggiungere amministratori e utenti.

**Amministratore società** Può visualizzare e amministrare solo le proprie società. Un amministratore di società può inoltre eseguire tutte le funzioni amministrative, inclusa l’aggiunta di amministratori e utenti. Un amministrare società può aggiungere un utente agli account di amministrazione società SPS. Questo ruolo è il ruolo utente predefinito.

**Utente SPS** Può accedere alle società alle quali è stato assegnato; non è in grado di eseguire attività amministrative.

Dopo l’aggiunta di un utente, Scene7 Publishing System invia all’utente un messaggio e-mail di benvenuto, contenete la password e l’URL per accedere a Scene7 Publishing System.

### Aggiunta di un utente o di un amministratore {#adding-a-user-or-administrator}

1. Fate clic su Configurazione &gt; Impostazione applicazione &gt; Impostazione amministrazione &gt; Amministrazione utente.
1. Fate clic su Aggiungi. 
1. Immettete il nome e l’indirizzo e-mail dell’utente o amministratore da aggiungere, quindi fate clic su Avanti.

   >[!NOTE]
   >
   >gli indirizzi e-mail non possono contenere il carattere di apostrofo (').

1. Scegliete un ruolo da assegnare all’utente.

   Consultate [Ruoli utente e privilegi di Dynamic Media Classic](administration-setup.md#user_administration).

1. Selezionate un nome di società per aggiungere un utente a una società.
1. Per aggiungere l’utente a un gruppo (se state aggiungendo un utente o un collaboratore di Media Portal), fate clic su Avanti e aggiungete l’utente.
1. Fate clic su Salva per completare la configurazione dell’utente.

   Dopo il salvataggio, un messaggio chiede se desiderate aggiungere l’utente a un’altra società. Fate clic su Aggiungi per aggiungere l’utente a una società.

   A tutti i nuovi utenti viene assegnata una password generata in modo casuale, che dovrà essere modificata dagli utenti stessi al loro primo accesso a Scene7 Publishing System.

   Dopo essere stati aggiunti da un amministratore, i nuovi utenti ricevono un messaggio e-mail di benvenuto. Il messaggio contiene una password temporanea e le istruzioni per accedere a Scene7 Publishing System.

   Se l'utente non riceve il messaggio e-mail di benvenuto, chiedetegli di accedere alla pagina di accesso di SPS (https://s7sps1.scene7.com) e di fare clic su Forgot My Password (Password dimenticata). La password viene reimpostata e viene inviato un nuovo messaggio e-mail. Se l’utente non riceve l’e-mail (e se il messaggio non è stato inserito nella cartella della posta indesiderata), contattate il Supporto tecnico.

   Quando aggiungete nuovi utenti di Media Portal, potete anche accedere a Configurazione &gt; Impostazione applicazione &gt; Amministrazione utente, fare clic su Carica elenco utenti e selezionare un file .csv contenente un massimo di 500 utenti.

### Eliminazione di un utente {#deleting-a-user}

Potete eliminare utenti da Scene7 Publishing System impostandone lo stato su Non valido. Gli utenti con stato Non valido vengono eliminati dal sistema e da tutti gli account.

1. Fate clic su **Configurazione** &gt; **Impostazione applicazione** &gt; **Impostazione amministrazione** &gt; **Amministrazione utente**.
1. Selezionate un utente dall’elenco e fate clic su **Modifica**.
1. Deselezionate Valido.
1. Fate clic su **Salva**.

### Attivazione o disattivazione degli utenti {#activating-or-deactivating-users}

Gli utenti che sono stati disattivati non sono più autorizzati ad accedere all’account indicato all’inizio del menu Seleziona account per l’accesso.

1. Fate clic su **Configurazione** &gt; **Impostazione applicazione** &gt; **Impostazione amministrazione** &gt; **Amministrazione utente**.
1. Nell’elenco di utenti, selezionate o deselezionate l’opzione Attivo accanto al nome dell’utente.

### Modifica delle informazioni utente {#editing-user-information}

Le informazioni utente che potete modificare dipendono dal vostro ruolo di amministratore e dal ruolo assegnato all’utente di cui desiderate modificare le informazioni. Le opzioni che appaiono attenuate (non disponibili) non possono essere modificate.

1. Passate a **Configurazione** &gt; **Impostazione applicazione** &gt; **Impostazione amministrazione** &gt; **Amministrazione utente**.
1. Selezionate l’utente e fate clic su **Modifica**.
1. Selezionate nella tabella la voce corrispondente alla società per la quale desiderate modificare le autorizzazioni o l’accesso, quindi fate clic sul collegamento Gestisci società.
1. Selezionate il ruolo utente.
1. Se volete modificare l’iscrizione al gruppo dell’utente (se state modificando o aggiungendo un utente o un collaboratore di Media Portal), fate clic su Avanti e modificate l’iscrizione al gruppo.
1. Fate clic su **Salva**.

### Filtro e ordine dell’elenco degli utenti {#filtering-and-sorting-the-user-list}

Potete filtrare e ordinare l’elenco degli utenti per individuare un utente. Tutti gli utenti di tutti gli account da voi amministrati compaiono nell’elenco utenti, indipendentemente dall’account selezionato nel menu Seleziona account per l’accesso.

È possibile filtrare l’elenco di utenti con le seguenti tecniche:

**Filtra per gruppo** Selezionate il menu Per gruppo e scegliete un'opzione per limitare l'elenco agli utenti di un gruppo.

**Filtrare per ruolo** utente Selezionate il menu Per ruolo utente e scegliete un'opzione per limitare l'elenco a utenti o amministratori di tipi diversi.

**Filtra per nome campo** Selezionate l'opzione Attiva filtro per campo. Dal menu Per nome campo, scegliete una colonna per filtrare l’elenco; dal menu Filtra carattere, scegliete una lettera. L’elenco viene ridotto a una sola colonna in base alla lettera scelta. Per visualizzare di nuovo l’elenco completo, deselezionate l’opzione Attiva filtro per campo.

**Filtrare gli utenti non validi** Deseleziona l'opzione Includi non valido. Nei risultati della ricerca vengono visualizzati solo gli utenti presenti nel sistema. Gli utenti non validi sono quelli che avete eliminato dal sistema e dagli account da voi amministrati.

**Ordina per colonna:** fate clic su un'intestazione per ordinare tutti gli utenti in base al relativo stato, per nome, cognome o indirizzo e-mail, per ruolo utente o per stato valido/non valido.

Se nel sistema è presente un numero elevato di utenti, potete limitare le dimensioni dell’elenco specificando un numero nel menu Dimensione massima elenco.

### Collegamento di un'identità utente IMS a un account utente IPS Dynamic Media Classic {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

Potete collegare un'identità utente Adobe IMS a un account utente IPS Dynamic Media Classic, in modo da poter utilizzare SSO (Single Sign On) per accedere e avviare Scene 7 Publishing System da Adobe Marketing Cloud.

1. Adobe deve già aver configurato il vostro account con un'organizzazione Adobe Marketing Cloud e averlo collegato al contesto del prodotto Scene 7 Publishing System. Se questa configurazione non è ancora stata completata o non sei sicuro di averlo fatto, contatta l'Assistenza clienti Adobe.

   Al termine della configurazione, potete accedere ad Adobe Marketing Cloud e collegare l'identità Adobe Marketing Cloud all'account utente Dynamic Media Classic effettuando le seguenti operazioni.

1. In Adobe Marketing Cloud, andate alle impostazioni dell'account.
1. Fai clic **su Gestisci organizzazioni**.
1. Fate clic su **Collega account** o **su Ottieni accesso**.
1. Selezionate **Experience Manager**, quindi digitate le vostre credenziali.

   Le credenziali includono l'area dell'azienda IPS, l'indirizzo e-mail e la password.

1. Fate clic **su Collega**.
1. Quando il collegamento viene impostato, potete avviare Scene 7 Publishing System dall'interno di Adobe Marketing Cloud oppure avviarlo direttamente.

   Effettuate una delle seguenti operazioni:

   * Per avviare Dynamic Media Classic da Adobe Marketing Cloud, nella barra a sinistra di Adobe Marketing Cloud, fate clic **su Soluzioni** &gt; **Experience Manager**. Nella scheda Dynamic Media Classic, fate clic su **Avvia**.
   * Per accedere a Scene 7 Publishing System direttamente utilizzando le credenziali IMS, utilizzate il seguente sito Web:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Sostituite «N» nel percorso precedente con il numero dell'area della società IPS. Ovvero N = 1 per Nord America; 3 per EMEA; oppure 5 per JAPAC.

## Larghezza di banda e spazio di archiviazione {#bandwidth-storage}

Gli amministratori di SPS possono generare i rapporti su larghezza di banda, archiviazione e altri tipi di rapporti per le società che amministrano. Tali rapporti sono disponibili nella schermata Larghezza di banda e spazio di archiviazione. 

Per aprire questa schermata, fate clic su Configurazione &gt; Configurazione personale. Espandete Impostazione amministrazione e fate clic su Larghezza di banda e spazio di archiviazione.

### Tipi di rapporti {#types-of-reports}

La tabella seguente descrive i rapporti che potete generare dalla schermata Larghezza di banda e spazio di archiviazione:

| Rapporto | Informazioni | Utilizzo |
|:--- |:--- |:--- |
| Larghezza di banda | Larghezza di banda usata dalla società | Consente di tenere traccia dell’utilizzo di larghezza di banda da parte della società per specifici intervalli di date, al fine di determinare i pattern di traffico. |
| Archiviazione | Utilizzo dello spazio di archiviazione | Consente di tenere traccia della quantità di dati caricati dalla società. |
| Contenuti immagine | Quantità di richieste immagini per tipo | Consente di tenere traccia della quantità di richieste e volume per i diversi tipi di immagini. |
| Dominio | Quantità di richieste URL per dominio | Consente di tenere traccia dell’utilizzo di immagini in base al dominio delle richieste di immagini per una specifica società. (Dynamic Media Classic può fornire più di un dominio per account. Per ulteriori informazioni, rivolgetevi al supporto tecnico. |
| Streaming video | Utilizzo della larghezza di banda per lo streaming video | Consente di tenere traccia dell’utilizzo di streaming video da parte della società per specifici intervalli di date, al fine di determinare i pattern di traffico. |
| Contenuti video | Tempo di riproduzione di diversi video | Consente di individuare i video più visualizzati e quelli meno visualizzati. |


Il rapporto Contenuti immagine offre informazioni sulle richieste per i seguenti tipi di immagini:

**Richieste di richieste** di immagini per immagini.

**Richieste di richiesta** miniature per campioni o immagini alternative nei visualizzatori.

**Richieste di richieste** maschera a immagini che restituiscono maschere in scala di grigio.

**Richieste di** immagini affiancate per visualizzatore caricate da un visualizzatore.

**Richieste di rendering delle** immagini Vnt per l'oggetto che restituiscono un'immagine con oggetti specificati nelle vignettature richieste.

**Richieste di rendering delle** immagini Vnt Info che restituiscono informazioni relative alle vignettature richieste.

>[!NOTE]
>
>il rapporto Streaming video è applicabile solo ai video in streaming. Non tiene traccia della visualizzazione di video progressivi.

### Generazione di un rapporto {#generating-a-report}

Per generare un rapporto sulla larghezza di banda, l’archiviazione, i contenuti immagine, il dominio, lo streaming video o i contenuti video:

1. Fate clic su Configurazione &gt; Configurazione personale.
1. Espandete Impostazione amministrazione e fate clic su Larghezza di banda e spazio di archiviazione.
1. Fate clic su una scheda: Larghezza di banda, Archiviazione, Contenuto immagine, Dominio, Streaming video o Contenuto video.

   Consultate [Tipi di rapporti](administration-setup.md#types_of_reports).

### Visualizzazione dei dati in diversi modi {#viewing-data-in-different-ways}

Dopo la generazione di un rapporto dalla pagina Larghezza di banda e spazio di archiviazione, potete scegliere diverse opzioni per la visualizzazione delle informazioni. Potete scegliere come presentare le informazioni, se visualizzarle sotto forma di grafico o griglia, nonché specificare un periodo di tempo per i dati da acquisire. In visualizzazione Dati, potete inoltre ordinare le informazioni e riordinare le colonne.

**Visualizzazione dei dati sotto forma di grafico o griglia** di dati Fate clic sull'opzione Visualizzazione grafico per visualizzare i dati sotto forma di grafico; fare clic sull'opzione Visualizzazione dati per visualizzare i dati sotto forma di griglia.

**Scelta di un tipo di presentazione di rapporti** Nel menu Tipo rapporto, scegliete Riepilogo, Giornaliero o Mensile per organizzare i dati sotto forma di riepilogo, per giorno o per mese. Questa opzione non è disponibile per tutti i rapporti.

**Specificare un periodo di tempo** Scegliere le opzioni per definire un periodo di tempo per il rapporto, quindi fare clic su Aggiorna dopo aver definito un periodo di tempo:

**Periodo di tempo predefinito** nel menu Rapporto predefinito, scegliete un'opzione. Ad esempio, scegliete Ultimo mese per acquisire i dati a partire dall’ultimo mese.

**Periodo di tempo personalizzato** nel menu Rapporto predefinito, scegliete Personalizzato. Quindi scegliete una data dal menu Mese iniziale (o Data iniziale) e una dal menu N. di mesi (o N. di giorni). Per i rapporti Dominio e Contenuti video, potete scegliere una data iniziale e finale specifica per l’acquisizione delle informazioni per il rapporto.

**Ordinamento dei dati (solo visualizzazione Dati)** Per ordinare le informazioni in una colonna, fare clic sull'intestazione della colonna. Fate di nuovo clic per ordinare i dati in ordine discendente.

**Ridisporre le colonne (solo visualizzazione dati)** Per spostare una colonna altrove sulla griglia di dati, trascinatene l'intestazione.

### Esportazione e stampa dei rapporti {#exporting-and-printing-reports}

I rapporti generati possono essere esportati in modo da consentire l’utilizzo dei dati in fogli di calcolo e altre applicazioni. I rapporti possono inoltre essere stampati.

**Esportazione dei dati del report** in visualizzazione Dati, ordinamento e disposizione dei dati come necessario. Quindi aprite il menu Esporta e scegliete un formato: Delimitato da tabulazioni, Separato da virgola o Formato HTML. I dati vengono copiati negli Appunti nel formato scelto e li potete quindi incollare in un foglio di calcolo o in un’altra applicazione.

**Stampa di un rapporto** Fate clic su Stampa, scegliete le opzioni desiderate nella finestra di dialogo Stampa, quindi fate clic su OK.

## Errori immagini {#image-errors}

Gli amministratori SPS possono generare dei rapporti Errori immagini. Questi rapporti forniscono un elenco dei 20 errori più frequenti relativi alle immagini, per le ultime 24 ore, riferiti alla società a cui siete attualmente collegati. Per generare un rapporto Errori immagini, effettuate le seguenti operazioni:

1. Fate clic su Configurazione &gt; Configurazione personale.
1. Espandete Impostazione amministrazione e fate clic su Errori immagini.
1. (Facoltativo) Effettuate una o più delle operazioni seguenti:

   * Fate clic su un’intestazione per ordinare gli errori in base alle informazioni dell’intestazione. Per impostazione predefinita, gli errori vengono ordinati per numero di occorrenze, dalla più alta alla più bassa.
   * Portate il cursore sul campo Risposta di un errore per visualizzare il messaggio di errore specifico.
   * Portate il cursore sul campo URL o Referente per visualizzare il collegamento all’immagine o il sito Web del referente.
   * Fate clic su Copia URL nella colonna URL per copiare il collegamento all’immagine vera e propria. Potete quindi incollare il collegamento nel campo indirizzo della finestra di un browser per passare all’immagine ed esaminare l’errore.
   * Fate clic su Copia URL nella colonna Referente per copiare il collegamento alla pagina Web del referente.

Gli errori visualizzati si riferiscono alla società a cui siete attualmente connessi. Ciascun errore include le seguenti informazioni:

**ID** immagine dell'immagine che ha originato l'errore.

**Ora** L'intervallo di tempo della prima volta che l'errore è stato segnalato all'ultima volta in cui è stato segnalato l'errore, nell'arco delle ultime 24 ore.

**Conteggio** del numero di errori segnalati nell'immagine.

**Risposta** Il messaggio di errore specifico. Gli errori possono essere di tipo 4xx o 5xx.

**URL** Elenca l'URL dell'immagine in Scene 7.

**Referente** : specifica l'URL del sito Web da cui proveniva la richiesta iniziale. Il referente può essere qualsiasi sito Web contenente un collegamento all’immagine.

Alle colonne URL e Referente è stata associata la relativa funzione Copia URL per facilitare la verifica.
