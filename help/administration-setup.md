---
title: Impostazione amministrazione
seo-title: Impostazione amministrazione
description: 'null'
seo-description: Scopri come impostare l'area di amministrazione di Dynamic Media Classic.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 56%

---


<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Impostazione amministrazione{#administration-setup}

Le schermate Impostazione amministrazione sono riservate agli utenti di Dynamic Media Classic. Usate queste schermate per consentire agli utenti di lavorare in Dynamic Media Classic e per comunicare tramite e-mail con gli utenti.

1. To access Administration Setup options, click **Setup** > **Personal Setup** > **Administration Setup**.

## Amministrazione utente {#user-administration}

A tutti gli utenti di Dynamic Media Classic viene assegnato un ruolo che ne determina privilegi e diritti di accesso alle funzioni di Dynamic Media Classic. Gli amministratori specificano i diversi ruoli e responsabilità per le società a cui sono assegnati.

In genere, Dynamic Media Classic configura il primo gruppo di società e assegna un amministratore di società. L’amministratore della società, quindi, configura e amministra gli utenti di Dynamic Media Classic.

Dynamic Media Classic supporta diversi ruoli utente. Questi ruoli possono accedere alle società configurate per Dynamic Media Classic:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic User** Può accedere alle società a cui è stato assegnato; non può eseguire alcuna attività amministrativa.

**Adobe Dynamic Media Classic Company Admin** Può visualizzare e amministrare solo le proprie società. Un amministratore di società può inoltre eseguire tutte le funzioni amministrative, inclusa l’aggiunta di amministratori e utenti. Un amministratore società può aggiungere un utente agli account di amministrazione società DMC. Questo ruolo è il ruolo utente predefinito.

Dopo aver aggiunto un utente, Dynamic Media Classic invia all’utente un messaggio e-mail di benvenuto. Il messaggio include una password e l&#39;URL Dynamic Media Classic.

### Aggiunta di un utente o di un amministratore {#adding-a-user-or-administrator}

1. Fate clic su Configurazione > Impostazione applicazione > Impostazione amministrazione > Amministrazione utente.
1. Fate clic su Aggiungi. 
1. Immettete il nome e l’indirizzo e-mail dell’utente o amministratore da aggiungere, quindi fate clic su Avanti.

   >[!NOTE]
   >
   >gli indirizzi e-mail non possono contenere il carattere di apostrofo (&#39;).

1. Scegliete un ruolo da assegnare all’utente.

   Consultate Ruoli utente e privilegi di [Dynamic Media Classic](administration-setup.md#user_administration).

1. Selezionate un nome di società per aggiungere un utente a una società.
1. Per aggiungere l’utente a un gruppo (se state aggiungendo un utente o un collaboratore di Media Portal), fate clic su Avanti e aggiungete l’utente.
1. Fate clic su Salva per completare la configurazione dell’utente.

   Dopo il salvataggio, un messaggio chiede se desiderate aggiungere l’utente a un’altra società. Fate clic su Aggiungi per aggiungere l’utente a una società.

   A tutti i nuovi utenti viene assegnata una password generata in modo casuale; gli utenti devono cambiare la password al loro primo accesso ad Dynamic Media Classic.

   Dopo essere stati aggiunti da un amministratore, i nuovi utenti ricevono un messaggio e-mail di benvenuto. Il messaggio contiene una password temporanea e le istruzioni per accedere a Scene7 Publishing System.

   Se l’utente non riceve il messaggio e-mail di benvenuto, chiedetegli di passare alla pagina di accesso di Dynamic Media Classic (https://s7sps1.scene7.com) e di fare clic su Password dimenticata. La password viene reimpostata e viene inviato un nuovo messaggio e-mail. Se l’utente non riceve l’e-mail (e se il messaggio non è stato inserito nella cartella della posta indesiderata), contattate il Supporto tecnico.

   Quando aggiungete nuovi utenti di Media Portal, potete anche accedere a Configurazione > Impostazione applicazione > Amministrazione utente, fare clic su Carica elenco utenti e selezionare un file .csv contenente un massimo di 500 utenti.

### Eliminazione di un utente {#deleting-a-user}

Puoi eliminare gli utenti da Dynamic Media Classic impostandone la modalità non valida. Gli utenti con stato Non valido vengono eliminati dal sistema e da tutti gli account.

1. Fate clic su **Configurazione** > **Impostazione applicazione** > **Impostazione amministrazione** > **Amministrazione utente**.
1. Selezionate un utente dall’elenco e fate clic su **Modifica**.
1. Deselezionate Valido.
1. Fate clic su **Salva**.

### Attivazione o disattivazione degli utenti {#activating-or-deactivating-users}

Gli utenti che sono stati disattivati non sono più autorizzati ad accedere all’account indicato all’inizio del menu Seleziona account per l’accesso.

1. Fate clic su **Configurazione** > **Impostazione applicazione** > **Impostazione amministrazione** > **Amministrazione utente**.
1. Nell’elenco di utenti, selezionate o deselezionate l’opzione Attivo accanto al nome dell’utente.

### Modifica delle informazioni utente {#editing-user-information}

Le informazioni utente che potete modificare dipendono dal vostro ruolo di amministratore e dal ruolo assegnato all’utente di cui desiderate modificare le informazioni. Le opzioni che appaiono attenuate (non disponibili) non possono essere modificate.

1. Passate a **Configurazione** > **Impostazione applicazione** > **Impostazione amministrazione** > **Amministrazione utente**.
1. Selezionate l’utente e fate clic su **Modifica**.
1. Selezionate nella tabella la voce corrispondente alla società per la quale desiderate modificare le autorizzazioni o l’accesso, quindi fate clic sul collegamento Gestisci società.
1. Selezionate il ruolo utente.
1. Se volete modificare l’iscrizione al gruppo dell’utente (se state modificando o aggiungendo un utente o un collaboratore di Media Portal), fate clic su Avanti e modificate l’iscrizione al gruppo.
1. Fate clic su **Salva**.

### Filtro e ordine dell’elenco degli utenti {#filtering-and-sorting-the-user-list}

Potete filtrare e ordinare l’elenco degli utenti per individuare un utente. Tutti gli utenti di tutti gli account da voi amministrati compaiono nell’elenco utenti, indipendentemente dall’account selezionato nel menu Seleziona account per l’accesso.

È possibile filtrare l’elenco di utenti con le seguenti tecniche:

**Filtrare per gruppo** Selezionate il menu Per gruppo e scegliete un’opzione per limitare l’elenco agli utenti di un gruppo.

**Filtrare per ruolo** utente Selezionate il menu Per ruolo utente e scegliete un’opzione per limitare l’elenco a utenti o amministratori di tipi diversi.

**Filtrare per nome** campo Selezionare l&#39;opzione Attiva filtro per campo. Dal menu Per nome campo, scegliete una colonna per filtrare l’elenco; dal menu Filtra carattere, scegliete una lettera. L’elenco viene ridotto a una sola colonna in base alla lettera scelta. Per visualizzare di nuovo l’elenco completo, deselezionate l’opzione Attiva filtro per campo.

**Escludere gli utenti** non validi Deselezionare l&#39;opzione Includi non validi. Nei risultati della ricerca vengono visualizzati solo gli utenti presenti nel sistema. Gli utenti non validi sono quelli che avete eliminato dal sistema e dagli account da voi amministrati.

**Ordina per intestazione** di colonna Fare clic su un&#39;intestazione per ordinare tutti gli utenti in base al loro stato, in ordine alfabetico per nome, cognome o e-mail, per ruolo utente o per stato valido/non valido.

Se nel sistema è presente un numero elevato di utenti, potete limitare le dimensioni dell’elenco specificando un numero nel menu Dimensione massima elenco.

### Collegamento di un&#39;identità utente IMS a un account utente Dynamic Media Classic IPS {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

Potete collegare un’identità utente Adobe IMS a un account utente Dynamic Media Classic IPS in modo da poter utilizzare SSO (Single Sign On) per accedere e avviare Scene7 Publishing System dall’interno  Adobe Marketing Cloud.

1. Adobe deve già aver configurato l’account con un’organizzazione  Adobe Marketing Cloud e averlo collegato al contesto di prodotto Scene7 Publishing System. Se la configurazione non è ancora stata completata o non sei sicuro se è già stata completata, contatta l&#39;Assistenza clienti Adobe.

   Una volta completata la configurazione, potete accedere  Adobe Marketing Cloud e collegare l&#39;identità del Adobe Marketing Cloud  al vostro account utente Dynamic Media Classic effettuando le seguenti operazioni.

1. In  Adobe Marketing Cloud, andate alle impostazioni dell&#39;account.
1. Fate clic su **Gestisci organizzazioni**.
1. Fate clic su **Collega account** o su **Ottieni accesso**.
1. Selezionare **Experience Manager**, quindi digitare le credenziali.

   Le credenziali includono l&#39;area geografica della società IPS, l&#39;indirizzo e-mail e la password.

1. Fate clic su **Collega**.
1. Quando il collegamento è impostato, potete avviare Scene7 Publishing System dall’interno  Adobe Marketing Cloud oppure avviarlo direttamente.

   Effettuate una delle seguenti operazioni:

   * Per avviare Dynamic Media Classic dall&#39;interno  Adobe Marketing Cloud, nella barra a sinistra di  Adobe Marketing Cloud, fate clic su **Soluzioni** > **Experience Manager**. Nella scheda Dynamic Media Classic, fate clic su **Avvia**.
   * Per accedere direttamente a Scene7 Publishing System utilizzando le credenziali IMS, usate il seguente sito Web:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Sostituisci &quot;N&quot; nel percorso precedente con il numero per la tua regione della società IPS. Ovvero, N = 1 per l&#39;America del Nord; 3 per l&#39;EMEA; oppure 5 per il GIAPPONE.

## Larghezza di banda e spazio di archiviazione {#bandwidth-storage}

Gli amministratori di Dynamic Media Classic possono generare larghezza di banda, archiviazione e altri tipi di rapporti per le aziende che amministrano. Tali rapporti sono disponibili nella schermata Larghezza di banda e spazio di archiviazione. 

Per aprire questa schermata, fate clic su Configurazione > Configurazione personale. Espandete Impostazione amministrazione e fate clic su Larghezza di banda e spazio di archiviazione.

### Tipi di rapporti {#types-of-reports}

La tabella seguente descrive i rapporti che potete generare dalla schermata Larghezza di banda e spazio di archiviazione:

| Rapporto | Informazioni | Utilizzo |
|:--- |:--- |:--- |
| Larghezza di banda | Larghezza di banda usata dalla società | Consente di tenere traccia dell’utilizzo di larghezza di banda da parte della società per specifici intervalli di date, al fine di determinare i pattern di traffico. |
| Archiviazione | Utilizzo dello spazio di archiviazione | Consente di tenere traccia della quantità di dati caricati dalla società. |
| Contenuti immagine | Quantità di richieste immagini per tipo | Consente di tenere traccia della quantità di richieste e volume per i diversi tipi di immagini. |
| Dominio | Quantità di richieste URL per dominio | Consente di tenere traccia dell’utilizzo di immagini in base al dominio delle richieste di immagini per una specifica società. (Dynamic Media Classic può fornire più domini per account. Per ulteriori informazioni, rivolgetevi al supporto tecnico. |
| Streaming video | Utilizzo della larghezza di banda per lo streaming video | Consente di tenere traccia dell’utilizzo di streaming video da parte della società per specifici intervalli di date, al fine di determinare i pattern di traffico. |
| Contenuti video | Tempo di riproduzione di diversi video | Consente di individuare i video più visualizzati e quelli meno visualizzati. |


Il rapporto Contenuti immagine offre informazioni sulle richieste per i seguenti tipi di immagini:

**Richieste** di immagini per le immagini.

**Richieste** di miniature per campioni o immagini alternative nei visualizzatori.

**Richieste di maschere** alle immagini che restituiscono maschere in scala di grigio.

**Richieste** di immagini per la sezione del visualizzatore caricate da un visualizzatore.

**Richieste** di rendering di immagini Vnt Object che restituiscono un&#39;immagine con oggetti specificati nelle vignettature richieste.

**Richieste** di rendering di immagini Vnt Info che restituiscono informazioni sulle vignettature richieste.

>[!NOTE]
>
>il rapporto Streaming video è applicabile solo ai video in streaming. Non tiene traccia della visualizzazione di video progressivi.

### Generazione di un rapporto {#generating-a-report}

Per generare un rapporto sulla larghezza di banda, l’archiviazione, i contenuti immagine, il dominio, lo streaming video o i contenuti video:

1. Fate clic su Configurazione > Configurazione personale.
1. Espandete Impostazione amministrazione e fate clic su Larghezza di banda e spazio di archiviazione.
1. Fate clic su una scheda: Larghezza di banda, Archiviazione, Contenuto immagine, Dominio, Streaming video o Contenuto video.

   Consultate [Tipi di rapporti](administration-setup.md#types_of_reports).

### Visualizzazione dei dati in diversi modi {#viewing-data-in-different-ways}

Dopo la generazione di un rapporto dalla pagina Larghezza di banda e spazio di archiviazione, potete scegliere diverse opzioni per la visualizzazione delle informazioni. Potete scegliere come presentare le informazioni, se visualizzarle sotto forma di grafico o griglia, nonché specificare un periodo di tempo per i dati da acquisire. In visualizzazione Dati, potete inoltre ordinare le informazioni e riordinare le colonne.

**Visualizzazione dei dati in un grafico o in una griglia** di dati Fare clic sull&#39;opzione Visualizzazione grafico per visualizzare i dati in un grafico; fare clic sull&#39;opzione Visualizzazione dati per visualizzare i dati sotto forma di griglia.

**Scelta di un tipo** di presentazione del rapporto Nel menu Tipo rapporto, scegliere Riepilogo, Giornaliero o Mensile per organizzare i dati in forma di riepilogo, per giorno o per mese. Questa opzione non è disponibile per tutti i rapporti.

**Specificare un periodo** di tempo Scegliere le opzioni per definire un periodo di tempo per il rapporto, quindi fare clic su Aggiorna dopo aver definito un periodo di tempo:

**Periodo** di tempo predefinito Scegliere un&#39;opzione dal menu Rapporto predefinito. Ad esempio, scegliete Ultimo mese per acquisire i dati a partire dall’ultimo mese.

**Periodo** di tempo personalizzato Scegliere Personalizzato dal menu Rapporto predefinito. Quindi scegliete una data dal menu Mese iniziale (o Data iniziale) e una dal menu N. di mesi (o N. di giorni). Per i rapporti Dominio e Contenuti video, potete scegliere una data iniziale e finale specifica per l’acquisizione delle informazioni per il rapporto.

**Ordinamento dei dati (solo in visualizzazione Dati)** Per ordinare le informazioni in una colonna, fare clic sull’intestazione della colonna. Fate di nuovo clic per ordinare i dati in ordine discendente.

**Ridisposizione delle colonne (solo in visualizzazione Dati)** Per spostare una colonna in un&#39;altra posizione nella griglia di dati, trascinarne l&#39;intestazione.

### Esportazione e stampa dei rapporti {#exporting-and-printing-reports}

I rapporti generati possono essere esportati in modo da consentire l’utilizzo dei dati in fogli di calcolo e altre applicazioni. I rapporti possono inoltre essere stampati.

**Esportazione dei dati** del rapporto In visualizzazione Dati, ordinare e disporre i dati in base alle esigenze. Quindi aprite il menu Esporta e scegliete un formato: Delimitato da tabulazioni, Separato da virgola o Formato HTML. I dati vengono copiati negli Appunti nel formato scelto e li potete quindi incollare in un foglio di calcolo o in un’altra applicazione.

**Per stampare un rapporto** , fare clic su Stampa, scegliere le opzioni desiderate nella finestra di dialogo Stampa, quindi fare clic su OK.

## Errori immagini {#image-errors}

Gli amministratori di Dynamic Media Classic possono generare rapporti Errori immagini. Questi rapporti forniscono un elenco dei 20 errori più frequenti relativi alle immagini, per le ultime 24 ore, riferiti alla società a cui siete attualmente collegati. Per generare un rapporto Errori immagini, effettuate le seguenti operazioni:

1. Fate clic su Configurazione > Configurazione personale.
1. Espandete Impostazione amministrazione e fate clic su Errori immagini.
1. (Facoltativo) Effettuate una o più delle operazioni seguenti:

   * Fate clic su un’intestazione per ordinare gli errori in base alle informazioni dell’intestazione. Per impostazione predefinita, gli errori vengono ordinati per numero di occorrenze, dalla più alta alla più bassa.
   * Portate il cursore sul campo Risposta di un errore per visualizzare il messaggio di errore specifico.
   * Portate il cursore sul campo URL o Referente per visualizzare il collegamento all’immagine o il sito Web del referente.
   * Fate clic su Copia URL nella colonna URL per copiare il collegamento all’immagine vera e propria. Potete quindi incollare il collegamento nel campo indirizzo della finestra di un browser per passare all’immagine ed esaminare l’errore.
   * Fate clic su Copia URL nella colonna Referente per copiare il collegamento alla pagina Web del referente.

Gli errori visualizzati si riferiscono alla società a cui siete attualmente connessi. Ciascun errore include le seguenti informazioni:

**ID** immagine per l’immagine che ha originato l’errore.

**Ora** L’intervallo di tempo della prima volta in cui l’errore è stato segnalato all’ultima volta che l’errore è stato segnalato, entro le ultime 24 ore.

**Conteggio** Il numero di errori segnalati sull’immagine.

**Risposta** Il messaggio di errore specifico. Gli errori possono essere di tipo 4xx o 5xx.

**URL** Elenca l’URL dell’immagine in Scene7.

**Referente** Specifica l&#39;URL del sito Web da cui proveniva la richiesta iniziale. Il referente può essere qualsiasi sito Web contenente un collegamento all’immagine.

Alle colonne URL e Referente è stata associata la relativa funzione Copia URL per facilitare la verifica.
