---
title: Configurazione dell'amministrazione
description: Scopri come impostare l’area di amministrazione di Adobe Dynamic Media Classic.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1969'
ht-degree: 33%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Impostazione amministrazione{#administration-setup}

Le schermate di Configurazione amministrazione sono per l&#39;amministrazione degli utenti Adobe Dynamic Media Classic. Utilizzare queste schermate per consentire agli utenti di lavorare in Adobe Dynamic Media Classic e di comunicare tramite e-mail con gli utenti.

1. Per accedere alle opzioni di Impostazione amministrazione, vai a **Configurazione** > **Configurazione personale** > **Impostazione amministrazione**.

## Amministrazione utente {#user-administration}

A tutti gli utenti di Adobe Dynamic Media Classic viene assegnato un ruolo che determina i loro privilegi e diritti di accesso alle funzioni di Adobe Dynamic Media Classic. Gli amministratori specificano i diversi ruoli e responsabilità per le società a cui sono assegnati.

In genere, Adobe Dynamic Media Classic configura il primo set di società e assegna un amministratore aziendale. L’amministratore della società configura e amministra gli utenti Adobe Dynamic Media Classic.

Adobe Dynamic Media Classic supporta diversi ruoli utente. Questi ruoli possono accedere alle società configurate per Adobe Dynamic Media Classic:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Utente Adobe Dynamic Media Classic** possono accedere alle società alle quali sono state assegnate; non può svolgere alcuna attività amministrativa.

**Amministratore società Adobe Dynamic Media Classic** Possono visualizzare e amministrare solo le proprie aziende. Un amministratore di società può inoltre eseguire tutte le funzioni amministrative, inclusa l’aggiunta di amministratori e utenti. Un amministratore società può aggiungere un utente agli account di amministrazione dell’azienda DMC. Questo ruolo è il ruolo utente predefinito.

Dopo aver aggiunto un utente, Adobe Dynamic Media Classic invia all’utente un messaggio e-mail di benvenuto. Il messaggio include una password e l’URL Adobe Dynamic Media Classic.

### Aggiungi un utente o un amministratore {#adding-a-user-or-administrator}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Seleziona **[!UICONTROL Aggiungi]**.
1. Immettere il nome e l&#39;indirizzo e-mail dell&#39;utente o dell&#39;amministratore che si desidera aggiungere, quindi selezionare **[!UICONTROL Successivo]**.

   >[!NOTE]
   >
   >Il carattere apostrofo (`‘`) non è consentito negli indirizzi e-mail.

1. Per assegnare un ruolo all’utente, scegli un’opzione Ruolo .

   Vedi [Ruoli e privilegi utente di Adobe Dynamic Media Classic](administration-setup.md#user_administration).

1. Per aggiungere un utente a una società, seleziona un nome società.
1. Se desideri aggiungere l’utente a un gruppo (se aggiungi un utente o un collaboratore di Media Portal), seleziona **[!UICONTROL Successivo]** e aggiungi l&#39;utente.
1. Seleziona **[!UICONTROL Salva]** per completare la configurazione utente.

   Dopo il salvataggio, un messaggio chiede se desiderate aggiungere l’utente a un’altra società. Seleziona **[!UICONTROL Aggiungi]** se desideri aggiungere l’utente a una società.

   A tutti i nuovi utenti viene assegnata una password generata in modo casuale; gli utenti devono cambiare la password al primo accesso all’applicazione desktop Adobe Dynamic Media Classic.

   Dopo essere stati aggiunti da un amministratore, i nuovi utenti ricevono un messaggio e-mail di benvenuto. L’e-mail fornisce una password temporanea e spiega come accedere a Adobe Dynamic Media Classic.

   Se l’utente non riceve l’e-mail di benvenuto, chiedi all’utente di passare alla pagina di accesso Adobe Dynamic Media Classic (https://s7sps1.scene7.com) e seleziona **[!UICONTROL Password dimenticata]**. La password viene reimpostata e viene inviato un nuovo messaggio e-mail. Se l’utente non riceve l’e-mail (e se il messaggio non è stato inserito nella cartella della posta indesiderata), contattate il Supporto tecnico.

   Quando aggiungi nuovi utenti di Media Portal, puoi anche passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Amministrazione utente]**, quindi seleziona **[!UICONTROL Carica elenco utenti]** e seleziona un file .csv contenente non più di 500 utenti.

### Eliminare un utente {#deleting-a-user}

È possibile eliminare gli utenti da Adobe Dynamic Media Classic rendendoli non validi. Gli utenti con stato Non valido vengono eliminati dal sistema e da tutti gli account.

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Seleziona un utente dall’elenco, quindi seleziona **[!UICONTROL Modifica]**.
1. Deselezionate Valido.
1. Seleziona **[!UICONTROL Salva]**.

### Attivare o disattivare gli utenti {#activating-or-deactivating-users}

Gli utenti che sono stati disattivati non sono più autorizzati ad accedere all’account indicato all’inizio del menu Seleziona account per l’accesso.

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Nell’elenco degli utenti, seleziona o deseleziona la **[!UICONTROL Attivo]** accanto al nome dell&#39;utente.

### Modificare le informazioni utente {#editing-user-information}

Le informazioni utente che potete modificare dipendono dal vostro ruolo di amministratore e dal ruolo assegnato all’utente di cui desiderate modificare le informazioni. Le opzioni che appaiono attenuate (non disponibili) non possono essere modificate.

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Seleziona un utente dall’elenco, quindi seleziona **[!UICONTROL Modifica]**.
1. Seleziona la voce nella tabella che mostra la società per la quale stai tentando di modificare le autorizzazioni o l’accesso, quindi seleziona **[!UICONTROL Gestisci società]**.
1. Selezionate il ruolo utente.
1. Se desideri modificare l’iscrizione al gruppo dell’utente (se stai modificando o aggiungendo un utente o un collaboratore di Media Portal), seleziona **[!UICONTROL Successivo]** e modificare l&#39;iscrizione al gruppo.
1. Seleziona **[!UICONTROL Salva]**.

### Filtrare e ordinare l’elenco di utenti {#filtering-and-sorting-the-user-list}

Potete filtrare e ordinare l’elenco degli utenti per individuare un utente. Tutti gli utenti di tutti gli account da voi amministrati compaiono nell’elenco utenti, indipendentemente dall’account selezionato nel menu Seleziona account per l’accesso.

È possibile utilizzare le seguenti tecniche di filtro degli elenchi utente:

* **Filtra per gruppo** - Seleziona la **[!UICONTROL Per gruppo]** e scegli un’opzione per limitare l’elenco agli utenti di un gruppo.

* **Filtra per ruolo utente** - Seleziona la **[!UICONTROL Per ruolo utente]** e scegli un’opzione per limitare l’elenco a utenti o amministratori di tipi diversi.

* **Filtra per nome campo** - Seleziona **[!UICONTROL Abilita filtro per campo]**. Quindi seleziona la **[!UICONTROL Per nome campo]** scegliere una colonna per filtrare l’elenco, quindi selezionare il menu Filtra carattere e scegliere una lettera. L’elenco viene filtrato su una delle colonne in base alla lettera scelta. Per visualizzare l’elenco completo, deseleziona la **[!UICONTROL Abilita filtro per campo]** opzione .

* **Filtrare gli utenti non validi** - Deselezionare **[!UICONTROL Includi non valido]**. Nei risultati della ricerca vengono visualizzati solo gli utenti presenti nel sistema. Gli utenti non validi sono stati eliminati dal sistema e dagli account amministrati.

* **Ordina per intestazione di colonna** - Selezionare un’intestazione per ordinare tutti gli utenti in base al loro stato, in ordine alfabetico per nome, cognome o e-mail, per ruolo utente o per stato valido/non valido.

Se nel sistema è presente un numero elevato di utenti, potete limitare le dimensioni dell’elenco specificando un numero nel menu Dimensione massima elenco.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to an Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Larghezza di banda e storage {#bandwidth-storage}

Gli amministratori di Adobe Dynamic Media Classic possono generare larghezza di banda, storage e altri tipi di rapporti per le aziende che gestiscono. Questi report sono disponibili nella pagina Larghezza di banda e archiviazione.

Per aprire questa pagina, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**. Espandi **[!UICONTROL Impostazione amministrazione]**, quindi seleziona **[!UICONTROL Larghezza di banda e storage]**.

### Tipi di rapporti {#types-of-reports}

La tabella seguente descrive i rapporti che puoi generare dalla pagina Larghezza di banda e archiviazione:

| Rapporto | Informazioni | Utilizzo |
|:--- |:--- |:--- |
| Larghezza di banda | Larghezza di banda usata dalla società | Consente di tenere traccia dell’utilizzo di larghezza di banda da parte della società per specifici intervalli di date, al fine di determinare i pattern di traffico. |
| Archiviazione | Utilizzo dello spazio di archiviazione | Consente di tenere traccia della quantità di dati caricati dalla società. |
| Contenuti immagine | Quantità di richieste immagini per tipo | Consente di tenere traccia della quantità di richieste e volume per i diversi tipi di immagini. |
| Dominio | Quantità di richieste URL per dominio | Consente di tenere traccia dell’utilizzo di immagini in base al dominio delle richieste di immagini per una specifica società. (Adobe Dynamic Media Classic può fornire più di un dominio per account. Per ulteriori informazioni, rivolgetevi al supporto tecnico. |
| Streaming video | Utilizzo della larghezza di banda per lo streaming video | Consente di tenere traccia dell’utilizzo di streaming video da parte della società per specifici intervalli di date, al fine di determinare i pattern di traffico. |
| Contenuti video | Tempo di riproduzione di diversi video | Consente di individuare i video più visualizzati e quelli meno visualizzati. |

Il rapporto Contenuti immagine offre informazioni sulle richieste per i seguenti tipi di immagini:

* **Richiesta immagine** - Richieste di immagini.

* **Richiesta miniature** - Richieste di campioni o immagini alternative nei visualizzatori.

* **Richiesta maschera** - Richieste alle immagini che restituiscono maschere in scala di grigi.

* **Richiesta riquadro visualizzatore** - Richieste di immagini caricate da un visualizzatore.

* **Richiesta oggetto Vnt** - Richieste di rendering delle immagini che restituiscono un’immagine con oggetti specificati nelle vignette richieste.

* **Richiesta informazioni Vnt** - Richieste di rendering di immagini che restituiscono informazioni sulle vignette richieste.

>[!NOTE]
>
>il rapporto Streaming video è applicabile solo ai video in streaming. Non tiene traccia della visualizzazione di video progressivi.

### Generare un report {#generating-a-report}

Per generare un rapporto sulla larghezza di banda, l’archiviazione, i contenuti immagine, il dominio, lo streaming video o i contenuti video:

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**.
1. Espandi Impostazione amministrazione, quindi seleziona **[!UICONTROL Larghezza di banda e storage]**.
1. Seleziona una scheda: **[!UICONTROL Larghezza di banda]**, **[!UICONTROL Storage]**, **[!UICONTROL Contenuto immagine]**, **[!UICONTROL Dominio]**, **[!UICONTROL Streaming video]** oppure **[!UICONTROL Contenuto video]**.

   Consultate [Tipi di rapporti](administration-setup.md#types_of_reports).

### Visualizzare i dati in modi diversi {#viewing-data-in-different-ways}

Dopo la generazione di un rapporto dalla pagina Larghezza di banda e spazio di archiviazione, potete scegliere diverse opzioni per la visualizzazione delle informazioni. Potete scegliere come presentare le informazioni, se visualizzarle sotto forma di grafico o griglia, nonché specificare un periodo di tempo per i dati da acquisire. In visualizzazione Dati, potete inoltre ordinare le informazioni e riordinare le colonne.

* **Visualizzare i dati in un grafico o in una griglia dati** - Seleziona **[!UICONTROL Vista grafico]** visualizzare i dati in un grafico; select **[!UICONTROL Visualizzazione dati]** per visualizzare i dati in una griglia dati.

* **Scegliere un tipo di presentazione del rapporto** - Dal menu Tipo di rapporto, selezionare **[!UICONTROL Riepilogo]**, **[!UICONTROL Giornaliero]** oppure **[!UICONTROL Mensile]** per organizzare i dati in forma di riepilogo, per giorno o per mese. Questa opzione non è disponibile per tutti i rapporti.

* **Specificare un periodo di tempo** - Scegliere le opzioni per definire un periodo di tempo per il rapporto, quindi selezionare **[!UICONTROL Aggiorna]** dopo aver definito un periodo di tempo:

* **Periodo di tempo predefinito** - Scegliere un’opzione dal menu Rapporto predefinito. Ad esempio, scegliete Ultimo mese per acquisire i dati a partire dall’ultimo mese.

* **Periodo di tempo personalizzato** - Dal menu Rapporto predefinito, seleziona **[!UICONTROL Personalizzato]**. Quindi scegli una data sul **[!UICONTROL Mese iniziale]** o **[!UICONTROL Data di inizio]**) e una data nel menu # dei mesi (o # o giorni). Per i rapporti Dominio e Contenuti video, potete scegliere una data iniziale e finale specifica per l’acquisizione delle informazioni per il rapporto.

* **Ordinare i dati (solo visualizzazione dati)** - Per ordinare le informazioni in una colonna, selezionare l’intestazione della colonna. Seleziona di nuovo per ordinare in ordine decrescente.

* **Ridisporre le colonne (solo visualizzazione dati)** - Per spostare una colonna in una posizione diversa sulla griglia di dati, trascinarne l’intestazione.

### Esportazione e stampa dei rapporti {#exporting-and-printing-reports}

I rapporti generati possono essere esportati in modo da consentire l’utilizzo dei dati in fogli di calcolo e altre applicazioni. I rapporti possono inoltre essere stampati.

* **Esportare i dati del rapporto** - In visualizzazione Dati, ordinare e disporre i dati secondo necessità. Quindi apri la **[!UICONTROL Esporta]** e scegliere un formato: **[!UICONTROL Delimitato da tabulazione]**, **[!UICONTROL Separato da virgole]** oppure **[!UICONTROL Formattato da HTML]**. I dati vengono copiati negli Appunti nel formato scelto. e li potete quindi incollare in un foglio di calcolo o in un’altra applicazione.

* **Stampa di un rapporto** - Seleziona **[!UICONTROL Stampa]** scegliere le opzioni desiderate nella finestra di dialogo Stampa, quindi selezionare **[!UICONTROL OK]**.

## Errori immagini {#image-errors}

Gli amministratori di Adobe Dynamic Media Classic possono generare rapporti sugli errori immagine. Questi rapporti forniscono un elenco dei 20 errori più frequenti relativi alle immagini, per le ultime 24 ore, riferiti alla società a cui siete attualmente collegati. Per generare un rapporto di errore immagine, procedi come segue:

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**.
1. Espandi Impostazione amministrazione, quindi seleziona **[!UICONTROL Errori immagine]**.
1. (Facoltativo) Effettuate una o più delle operazioni seguenti:

   * Per ordinare gli errori in base alle informazioni sull’intestazione, selezionare un’intestazione. Per impostazione predefinita, gli errori vengono ordinati per numero di occorrenze, dalla più alta alla più bassa.
   * Portate il cursore sul campo Risposta di un errore per visualizzare il messaggio di errore specifico.
   * Per visualizzare il collegamento all’immagine o alla pagina Web del referente, sposta il cursore sul campo URL o sul campo Referrer.
   * Per copiare il collegamento all’immagine effettiva, seleziona **[!UICONTROL URL Copia URL]**. Potete quindi incollare il collegamento nel campo indirizzo della finestra di un browser per passare all’immagine ed esaminare l’errore.
   * Per copiare il collegamento alla pagina web del referente, seleziona **[!UICONTROL URL copia referente]**.

Gli errori visualizzati riguardano la società a cui hai effettuato l’accesso. Ciascun errore include le seguenti informazioni:

* **ID immagine** - ID per l&#39;immagine offensiva.

* **Time** - L&#39;intervallo di tempo della prima segnalazione dell&#39;errore all&#39;ultima segnalazione dell&#39;errore, nelle ultime 24 ore.

* **Conteggio** - Il numero di errori segnalati sull&#39;immagine.

* **Risposta** - Il messaggio di errore specifico. Gli errori possono essere di tipo 4xx o 5xx.

* **URL** - Elenca l&#39;URL dell&#39;immagine in Adobe Dynamic Media Classic.

* **Referrer** - Specifica l&#39;URL del sito Web da cui proviene la richiesta iniziale. Il referente può essere qualsiasi sito Web contenente un collegamento all’immagine.

Alle colonne URL e Referente è stata associata la relativa funzione Copia URL per facilitare la verifica.
