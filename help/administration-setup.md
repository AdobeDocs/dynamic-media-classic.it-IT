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
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 64%

---


<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Impostazione amministrazione{#administration-setup}

Le schermate Impostazione amministrazione sono riservate agli utenti di Dynamic Media Classic. Usate queste schermate per consentire agli utenti di lavorare in Dynamic Media Classic e per comunicare tramite e-mail con gli utenti.

1. Per accedere alle opzioni di impostazione amministrazione, fate clic su **Configurazione** > **Configurazione personale** > **Impostazione amministrazione**.

## Amministrazione utente {#user-administration}

A tutti gli utenti di Dynamic Media Classic viene assegnato un ruolo che ne determina privilegi e diritti di accesso alle funzioni di Dynamic Media Classic. Gli amministratori specificano i diversi ruoli e responsabilità per le società a cui sono assegnati.

In genere, Dynamic Media Classic configura il primo gruppo di società e assegna un amministratore di società. L’amministratore della società, quindi, configura e amministra gli utenti di Dynamic Media Classic.

Dynamic Media Classic supporta diversi ruoli utente. Questi ruoli possono accedere alle società configurate per Dynamic Media Classic:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic** UserPuò accedere alle società a cui è stato assegnato; non può eseguire alcuna attività amministrativa.

**Adobe Dynamic Media Classic Company** AdminPuò visualizzare e amministrare solo le proprie società. Un amministratore di società può inoltre eseguire tutte le funzioni amministrative, inclusa l’aggiunta di amministratori e utenti. Un amministratore società può aggiungere un utente agli account di amministrazione società DMC. Questo ruolo è il ruolo utente predefinito.

Dopo aver aggiunto un utente, Dynamic Media Classic invia all’utente un messaggio e-mail di benvenuto. Il messaggio include una password e l&#39;URL Dynamic Media Classic.

### Aggiunta di un utente o di un amministratore {#adding-a-user-or-administrator}

1. Fate clic su Configurazione > Impostazione applicazione > Impostazione amministrazione > Amministrazione utente.
1. Fate clic su Aggiungi. 
1. Immettete il nome e l’indirizzo e-mail dell’utente o amministratore da aggiungere, quindi fate clic su Avanti.

   >[!NOTE]
   >
   >gli indirizzi e-mail non possono contenere il carattere di apostrofo (&#39;).

1. Scegliete un ruolo da assegnare all’utente.

   Consultate [Ruoli utente e privilegi di Dynamic Media Classic](administration-setup.md#user_administration).

1. Selezionate un nome di società per aggiungere un utente a una società.
1. Per aggiungere l’utente a un gruppo (se state aggiungendo un utente o un collaboratore di Media Portal), fate clic su Avanti e aggiungete l’utente.
1. Fate clic su Salva per completare la configurazione dell’utente.

   Dopo il salvataggio, un messaggio chiede se desiderate aggiungere l’utente a un’altra società. Fate clic su Aggiungi per aggiungere l’utente a una società.

   A tutti i nuovi utenti viene assegnata una password generata in modo casuale; gli utenti devono cambiare la password al loro primo accesso ad Dynamic Media Classic.

   Dopo essere stati aggiunti da un amministratore, i nuovi utenti ricevono un messaggio e-mail di benvenuto. Il messaggio contiene una password temporanea e le istruzioni per accedere a Scene7 Publishing System.

   Se l’utente non riceve il messaggio e-mail di benvenuto, chiedetegli di passare alla pagina di accesso di Dynamic Media Classic (https://s7sps1.scene7.com) e di fare clic su Password dimenticata. La password viene reimpostata e viene inviato un nuovo messaggio e-mail. Se l’utente non riceve l’e-mail (e se il messaggio non è stato inserito nella cartella della posta indesiderata), contattate il Supporto tecnico.

   Quando aggiungete nuovi utenti di Media Portal, potete anche accedere a Configurazione > Impostazione applicazione > Amministrazione utente, fare clic su Carica elenco utenti e selezionare un file .csv contenente un massimo di 500 utenti.

### Eliminazione di un utente  {#deleting-a-user}

Puoi eliminare gli utenti da Dynamic Media Classic impostandone la modalità non valida. Gli utenti con stato Non valido vengono eliminati dal sistema e da tutti gli account.

1. Fate clic su **Configurazione** > **Impostazione applicazione** > **Impostazione amministrazione** > **Amministrazione utente**.
1. Selezionate un utente dall’elenco e fate clic su **Modifica**.
1. Deselezionate Valido.
1. Fate clic su **Salva**.

### Attivazione o disattivazione degli utenti  {#activating-or-deactivating-users}

Gli utenti che sono stati disattivati non sono più autorizzati ad accedere all’account indicato all’inizio del menu Seleziona account per l’accesso.

1. Fate clic su **Configurazione** > **Impostazione applicazione** > **Impostazione amministrazione** > **Amministrazione utente**.
1. Nell’elenco di utenti, selezionate o deselezionate l’opzione Attivo accanto al nome dell’utente.

### Modifica delle informazioni utente  {#editing-user-information}

Le informazioni utente che potete modificare dipendono dal vostro ruolo di amministratore e dal ruolo assegnato all’utente di cui desiderate modificare le informazioni. Le opzioni che appaiono attenuate (non disponibili) non possono essere modificate.

1. Passate a **Configurazione** > **Impostazione applicazione** > **Impostazione amministrazione** > **Amministrazione utente**.
1. Selezionate l’utente e fate clic su **Modifica**.
1. Selezionate nella tabella la voce corrispondente alla società per la quale desiderate modificare le autorizzazioni o l’accesso, quindi fate clic sul collegamento Gestisci società.
1. Selezionate il ruolo utente.
1. Se volete modificare l’iscrizione al gruppo dell’utente (se state modificando o aggiungendo un utente o un collaboratore di Media Portal), fate clic su Avanti e modificate l’iscrizione al gruppo.
1. Fate clic su **Salva**.

### Filtro e ordine dell’elenco degli utenti  {#filtering-and-sorting-the-user-list}

Potete filtrare e ordinare l’elenco degli utenti per individuare un utente. Tutti gli utenti di tutti gli account da voi amministrati compaiono nell’elenco utenti, indipendentemente dall’account selezionato nel menu Seleziona account per l’accesso.

È possibile filtrare l’elenco di utenti con le seguenti tecniche:

**Filtrare per** gruppoSelezionate il menu Per gruppo e scegliete un’opzione per limitare l’elenco agli utenti di un gruppo.

**Filtrare per** ruolo utenteSelezionate il menu Per ruolo utente e scegliete un’opzione per limitare l’elenco a utenti o amministratori di tipi diversi.

**Filtrare per** nome campoSelezionare l&#39;opzione Attiva filtro per campo. Dal menu Per nome campo, scegliete una colonna per filtrare l’elenco; dal menu Filtra carattere, scegliete una lettera. L’elenco viene ridotto a una sola colonna in base alla lettera scelta. Per visualizzare di nuovo l’elenco completo, deselezionate l’opzione Attiva filtro per campo.

**Escludere** gli utenti non validiDeselezionare l&#39;opzione Includi non validi. Nei risultati della ricerca vengono visualizzati solo gli utenti presenti nel sistema. Gli utenti non validi sono quelli che avete eliminato dal sistema e dagli account da voi amministrati.

**Ordina per** intestazione di colonnaFate clic su un’intestazione per ordinare tutti gli utenti in base al loro stato, in ordine alfabetico per nome, cognome o e-mail, per ruolo utente o per stato valido/non valido.

Se nel sistema è presente un numero elevato di utenti, potete limitare le dimensioni dell’elenco specificando un numero nel menu Dimensione massima elenco.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to a Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to a Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Click **Manage Organizations**.
1. Click **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Click **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, click **Solutions** > **Experience Manager**. Under the Dynamic Media Classic card, click **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Larghezza di banda e spazio di archiviazione  {#bandwidth-storage}

Gli amministratori di Dynamic Media Classic possono generare larghezza di banda, archiviazione e altri tipi di rapporti per le aziende che amministrano. Tali rapporti sono disponibili nella schermata Larghezza di banda e spazio di archiviazione. 

Per aprire questa schermata, fate clic su Configurazione > Configurazione personale. Espandete Impostazione amministrazione e fate clic su Larghezza di banda e spazio di archiviazione.

### Tipi di rapporti  {#types-of-reports}

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

**Image** RequestRequests per le immagini.

**Thumbnail** RequestRequest per campioni o immagini alternative nei visualizzatori.

**Maschera** richiesta: le immagini che restituiscono maschere in scala di grigio.

**Richieste** RequestImage per la sezione del visualizzatore caricate da un visualizzatore.

**Richieste di rendering Vnt Object** RequestImage che restituiscono un&#39;immagine con oggetti specificati nelle vignettature richieste.

**Richieste di rendering Vnt Info** RequestImage che restituiscono informazioni sulle vignettature richieste.

>[!NOTE]
>
>il rapporto Streaming video è applicabile solo ai video in streaming. Non tiene traccia della visualizzazione di video progressivi.

### Generazione di un rapporto  {#generating-a-report}

Per generare un rapporto sulla larghezza di banda, l’archiviazione, i contenuti immagine, il dominio, lo streaming video o i contenuti video:

1. Fate clic su Configurazione > Configurazione personale.
1. Espandete Impostazione amministrazione e fate clic su Larghezza di banda e spazio di archiviazione.
1. Fate clic su una scheda: Larghezza di banda, Archiviazione, Contenuto immagine, Dominio, Streaming video o Contenuto video.

   Consultate [Tipi di rapporti](administration-setup.md#types_of_reports).

### Visualizzazione dei dati in diversi modi  {#viewing-data-in-different-ways}

Dopo la generazione di un rapporto dalla pagina Larghezza di banda e spazio di archiviazione, potete scegliere diverse opzioni per la visualizzazione delle informazioni. Potete scegliere come presentare le informazioni, se visualizzarle sotto forma di grafico o griglia, nonché specificare un periodo di tempo per i dati da acquisire. In visualizzazione Dati, potete inoltre ordinare le informazioni e riordinare le colonne.

**Visualizzazione dei dati in un grafico o in una** griglia di datiFare clic sull&#39;opzione Visualizzazione grafico per visualizzare i dati in un grafico; fare clic sull&#39;opzione Visualizzazione dati per visualizzare i dati sotto forma di griglia.

**Scelta di un** tipo di presentazione del rapportoNel menu Tipo rapporto, scegliete Riepilogo, Giornaliero o Mensile per organizzare i dati in forma di riepilogo, per giorno o per mese. Questa opzione non è disponibile per tutti i rapporti.

**Specifica di un** periodo di tempo: scegli le opzioni per definire un periodo di tempo per il rapporto, quindi fai clic su Aggiorna dopo aver definito un periodo di tempo:

**Periodo** di tempo predefinitoScegliere un’opzione dal menu Rapporto predefinito. Ad esempio, scegliete Ultimo mese per acquisire i dati a partire dall’ultimo mese.

**Periodo** di tempo personalizzatoScegliere Personalizzato dal menu Rapporto predefinito. Quindi scegliete una data dal menu Mese iniziale (o Data iniziale) e una dal menu N. di mesi (o N. di giorni). Per i rapporti Dominio e Contenuti video, potete scegliere una data iniziale e finale specifica per l’acquisizione delle informazioni per il rapporto.

**Ordinamento dei dati (solo in visualizzazione Dati)** Per ordinare le informazioni in una colonna, fare clic sull’intestazione della colonna. Fate di nuovo clic per ordinare i dati in ordine discendente.

**Ridisposizione delle colonne (solo in visualizzazione Dati)** Per spostare una colonna in un&#39;altra posizione nella griglia di dati, trascinarne l&#39;intestazione.

### Esportazione e stampa dei rapporti {#exporting-and-printing-reports}

I rapporti generati possono essere esportati in modo da consentire l’utilizzo dei dati in fogli di calcolo e altre applicazioni. I rapporti possono inoltre essere stampati.

**Esportazione** dei dati del rapportoNella visualizzazione Dati, ordinare e disporre i dati in base alle esigenze. Quindi aprite il menu Esporta e scegliete un formato: Delimitato da tabulazioni, Separato da virgola o Formato HTML. I dati vengono copiati negli Appunti nel formato scelto e li potete quindi incollare in un foglio di calcolo o in un’altra applicazione.

**Stampa di un** rapportoFare clic su Stampa, scegliere le opzioni desiderate nella finestra di dialogo Stampa, quindi fare clic su OK.

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

**ID immagine** per l’immagine che ha originato l’errore.

**** Ora: intervallo di tempo della prima volta in cui l’errore è stato segnalato all’ultima volta che l’errore è stato segnalato, entro le ultime 24 ore.

**** Conteggio: il numero di errori segnalati sull’immagine.

**** Risposta: il messaggio di errore specifico. Gli errori possono essere di tipo 4xx o 5xx.

**URLs** Elenca l’URL dell’immagine in Scene7.

**** Referente: specifica l’URL del sito Web da cui proveniva la richiesta iniziale. Il referente può essere qualsiasi sito Web contenente un collegamento all’immagine.

Alle colonne URL e Referente è stata associata la relativa funzione Copia URL per facilitare la verifica.
