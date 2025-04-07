---
title: Impostazione amministrazione
description: Scopri come impostare l’area di amministrazione di Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
topic: Administration
level: Intermediate
source-git-commit: fc2138cc9fd08cb4ce7466724af03f0901edebf3
workflow-type: tm+mt
source-wordcount: '1995'
ht-degree: 29%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Configurazione dell’amministrazione{#administration-setup}

Le schermate di configurazione dell’amministrazione sono per l’amministrazione degli utenti di Adobe Dynamic Media Classic. Utilizzare queste schermate per consentire agli utenti di lavorare in Adobe Dynamic Media Classic e comunicare tramite posta elettronica con altri utenti.

1. Per accedere alle opzioni di installazione dell&#39;amministrazione, passare a **Configurazione** > **Configurazione personale** > **Configurazione dell&#39;amministrazione**.

## Amministrazione utenti {#user-administration}

A tutti gli utenti di Adobe Dynamic Media Classic viene assegnato un ruolo che determina i loro privilegi e i diritti di accesso alle funzioni di Adobe Dynamic Media Classic. Gli amministratori specificano i diversi ruoli e responsabilità per le società a cui sono assegnati.

In genere, Adobe Dynamic Media Classic configura il primo gruppo di società e assegna un amministratore della società. L’amministratore aziendale imposta e amministra quindi gli utenti di Adobe Dynamic Media Classic.

Adobe Dynamic Media Classic supporta diversi ruoli utente. Questi ruoli possono accedere alle aziende configurate per Adobe Dynamic Media Classic:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Utente Adobe Dynamic Media Classic** può accedere alle società a cui è stato assegnato; non può eseguire attività amministrative.

**L&#39;amministratore della società Adobe Dynamic Media Classic** può visualizzare e amministrare solo le proprie società. Un amministratore di società può inoltre eseguire tutte le funzioni amministrative, inclusa l’aggiunta di amministratori e utenti. Un amministratore della società può aggiungere un utente agli account di amministratore della società DMC. Questo ruolo è il ruolo utente predefinito.

Dopo aver aggiunto un utente, Adobe Dynamic Media Classic invia all&#39;utente un messaggio di posta elettronica di benvenuto. Il messaggio include una password e l’URL di Adobe Dynamic Media Classic.

### Aggiungere un utente o un amministratore {#adding-a-user-or-administrator}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Configurazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Seleziona **[!UICONTROL Aggiungi]**.
1. Immettere il nome e l&#39;indirizzo di posta elettronica dell&#39;utente o dell&#39;amministratore che si desidera aggiungere, quindi selezionare **[!UICONTROL Avanti]**.

   >[!NOTE]
   >
   >Il carattere apostrofo (`'`) non è consentito negli indirizzi e-mail.

1. Per assegnare un ruolo all&#39;utente, scegliere un&#39;opzione Ruolo.

   Consulta [Ruoli utente e privilegi di Adobe Dynamic Media Classic](administration-setup.md#user_administration).

1. Per aggiungere un utente a una società, selezionare il nome della società.
1. Se si desidera aggiungere l&#39;utente a un gruppo (se si sta aggiungendo un utente Media Portal o un collaboratore), selezionare **[!UICONTROL Avanti]** e aggiungere l&#39;utente.
1. Seleziona **[!UICONTROL Salva]** per completare la configurazione utente.

   Dopo il salvataggio, un messaggio chiede se desiderate aggiungere l’utente a un’altra società. Seleziona **[!UICONTROL Aggiungi]** se desideri aggiungere l&#39;utente a una società.

   A tutti i nuovi utenti viene assegnata una password generata in modo casuale; gli utenti devono modificare le password al primo accesso all’applicazione desktop Adobe Dynamic Media Classic.

   Dopo essere stati aggiunti da un amministratore, i nuovi utenti ricevono un messaggio e-mail di benvenuto. Il messaggio di posta elettronica fornisce una password temporanea e spiega come accedere a Adobe Dynamic Media Classic.

   Se l&#39;utente non riceve l&#39;e-mail di benvenuto, chiedere di accedere alla pagina di accesso di Adobe Dynamic Media Classic (https://s7sps1.scene7.com) e selezionare **[!UICONTROL Password dimenticata]**. La password viene reimpostata e viene inviato un nuovo messaggio e-mail. Se l’utente non riceve l’e-mail (e se il messaggio non è stato inserito nella cartella della posta indesiderata), contattate il Supporto tecnico.

   Quando si aggiungono nuovi utenti Media Portal, è inoltre possibile passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Amministrazione utente]**, quindi selezionare **[!UICONTROL Carica elenco utenti]** e selezionare un file .csv contenente non più di 500 utenti.

### Eliminare un utente {#delet-a-user}

Puoi eliminare gli utenti da Adobe Dynamic Media Classic rendendoli non validi. Gli utenti con stato Non valido vengono eliminati dal sistema e da tutti gli account.

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Configurazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Selezionare un utente dall&#39;elenco, quindi selezionare **[!UICONTROL Modifica]**.
1. Deselezionate Valido.
1. Seleziona **[!UICONTROL Salva]**.

### Attivare o disattivare gli utenti {#activating-or-deactivating-users}

Gli utenti che sono stati disattivati non sono più autorizzati ad accedere all’account indicato all’inizio del menu Seleziona account per l’accesso.

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Configurazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Nell&#39;elenco degli utenti selezionare o deselezionare l&#39;opzione **[!UICONTROL Attivo]** accanto al nome dell&#39;utente.

### Modificare le informazioni utente {#editing-user-information}

Le informazioni utente che potete modificare dipendono dal vostro ruolo di amministratore e dal ruolo assegnato all’utente di cui desiderate modificare le informazioni. Le opzioni che appaiono attenuate (non disponibili) non possono essere modificate.

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Configurazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Selezionare un utente dall&#39;elenco, quindi selezionare **[!UICONTROL Modifica]**.
1. Selezionare la voce nella tabella che mostra la società per la quale si sta tentando di modificare le autorizzazioni o l&#39;accesso, quindi selezionare **[!UICONTROL Gestisci società]**.
1. Selezionate il ruolo utente.
1. Se si desidera modificare l&#39;appartenenza al gruppo dell&#39;utente (se si sta modificando o aggiungendo un utente o un collaboratore di Media Portal), selezionare **[!UICONTROL Avanti]** e modificare l&#39;appartenenza al gruppo.
1. Seleziona **[!UICONTROL Salva]**.

### Filtrare e ordinare l’elenco di utenti {#filtering-and-sorting-the-user-list}

Potete filtrare e ordinare l’elenco degli utenti per individuare un utente. Tutti gli utenti di tutti gli account da voi amministrati compaiono nell’elenco utenti, indipendentemente dall’account selezionato nel menu Seleziona account per l’accesso.

Puoi utilizzare le seguenti tecniche di filtro degli elenchi utente:

* **Filtra per gruppo**: seleziona il menu **[!UICONTROL Per gruppo]** e scegli un&#39;opzione per limitare l&#39;elenco agli utenti di un gruppo.

* **Filtra per ruolo utente**: seleziona il menu **[!UICONTROL Per ruolo utente]** e scegli un&#39;opzione per limitare l&#39;elenco a utenti o amministratori di tipi diversi.

* **Filtra per nome campo**: selezionare **[!UICONTROL Abilita filtro per campo]**. Selezionare quindi il menu **[!UICONTROL Per nome campo]**, scegliere una colonna per filtrare l&#39;elenco, quindi scegliere Filtra carattere e scegliere una lettera. L’elenco viene filtrato su una delle colonne in base alla lettera scelta. Per visualizzare l&#39;elenco completo, deselezionare l&#39;opzione **[!UICONTROL Abilita filtro per campo]**.

* **Escludi utenti non validi**: deseleziona **[!UICONTROL Includi non validi]**. Nei risultati della ricerca vengono visualizzati solo gli utenti presenti nel sistema. Gli utenti non validi sono stati eliminati dal sistema e dagli account amministrati.

* **Ordina per intestazione colonna**: selezionare un&#39;intestazione per ordinare tutti gli utenti in base al loro stato, in ordine alfabetico in base al nome, al cognome o all&#39;indirizzo e-mail. Oppure, ordinare in base al ruolo utente o in base a uno stato valido/non valido.

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

      Replace "N" in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Larghezza di banda e spazio di archiviazione {#bandwidth-storage}

Gli amministratori di Adobe Dynamic Media Classic possono generare rapporti sulla larghezza di banda, sullo spazio di archiviazione e su altri tipi di rapporti per le aziende che amministrano. Questi rapporti sono disponibili nella pagina Larghezza di banda e spazio di archiviazione.

Per aprire questa pagina, passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**. Espandere **[!UICONTROL Configurazione amministrazione]**, quindi selezionare **[!UICONTROL Larghezza di banda e spazio di archiviazione]**.

### Tipi di rapporti {#types-of-reports}

Nella tabella seguente sono descritti i rapporti che è possibile generare dalla pagina Larghezza di banda e spazio di archiviazione:

| Rapporto | Informazioni | Utilizzo |
| --- | --- | --- |
| Larghezza di banda | | <!-- CQDOC-22504 --> **IMPORTANTE**: la scheda Larghezza di banda non è più supportata. Anche se viene ancora visualizzato nell&#39;interfaccia utente, i dati della larghezza di banda non sono disponibili e tutti i valori vengono visualizzati come `0`. |
| Archiviazione | Utilizzo dello spazio di archiviazione | Monitora la quantità di dati caricati dall’azienda. |
| Contenuti immagine | Visualizza il totale degli hit e del volume di consegna delle immagini suddivisi per tipo di richiesta e sottotipo. | Monitora il numero di richieste e il volume per diversi tipi di immagini, comprese le metriche provenienti da risorse non video. <!-- CQDOC-22504 --> |
| Dominio | Quantità di richieste URL per dominio | Consente di tenere traccia dell’utilizzo di immagini in base al dominio delle richieste di immagini per una specifica società. (Adobe Dynamic Media Classic può fornire più domini per account. Per ulteriori informazioni, rivolgetevi al supporto tecnico. |
| Streaming video | Utilizzo della larghezza di banda per lo streaming video | Consente di tenere traccia dell’utilizzo di streaming video da parte della società per specifici intervalli di date, al fine di determinare i pattern di traffico. |
| Contenuti video | Tempo di riproduzione di diversi video | Consente di individuare i video più visualizzati e quelli meno visualizzati. |

Il rapporto Contenuti immagine offre informazioni sulle richieste per i seguenti tipi di immagini:

* **Richiesta immagine**: richieste di immagini.

* **Richiesta miniature**: richieste di immagini campione o alternative nei visualizzatori.

* **Richiesta maschera**: richiede alle immagini di restituire maschere in scala di grigio.

* **Richiesta riquadro visualizzatore**: richieste di immagini caricate da un visualizzatore.

* **Richiesta oggetto VNT**: richieste di rendering immagini che restituiscono un&#39;immagine con gli oggetti specificati nelle vignettature richieste.

* **Richiesta informazioni VNT**: richieste di rendering immagini che restituiscono informazioni sulle vignettature richieste.

>[!NOTE]
>
>il rapporto Streaming video è applicabile solo ai video in streaming. Non tiene traccia della visualizzazione di video progressivi.

### Generare un rapporto {#generating-a-report}

Per generare un rapporto sulla larghezza di banda, l’archiviazione, i contenuti immagine, il dominio, lo streaming video o i contenuti video:

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**.
1. Espandere Setup amministrazione, quindi selezionare **[!UICONTROL Larghezza di banda e spazio di archiviazione]**.
1. Selezionare una scheda: **[!UICONTROL Larghezza di banda]**, **[!UICONTROL Archiviazione]**, **[!UICONTROL Contenuto immagine]**, **[!UICONTROL Dominio]**, **[!UICONTROL Streaming video]** o **[!UICONTROL Contenuto video]**.

   Consultate [Tipi di rapporti](administration-setup.md#types_of_reports).

### Visualizzare i dati in modi diversi {#viewing-data-in-different-ways}

Dopo la generazione di un rapporto dalla pagina Larghezza di banda e spazio di archiviazione, potete scegliere diverse opzioni per la visualizzazione delle informazioni. Potete scegliere come presentare le informazioni, se visualizzarle sotto forma di grafico o griglia, nonché specificare un periodo di tempo per i dati da acquisire. In visualizzazione Dati, potete inoltre ordinare le informazioni e riordinare le colonne.

* **Visualizza dati in un grafico o in una griglia dati**: selezionare **[!UICONTROL Visualizzazione grafico]** per visualizzare i dati in un grafico; selezionare **[!UICONTROL Visualizzazione dati]** per visualizzare i dati in una griglia dati.

* **Scegli un tipo di presentazione per report**: dal menu Tipo di report, seleziona **[!UICONTROL Riepilogo]**, **[!UICONTROL Giornaliero]** o **[!UICONTROL Mensile]** per organizzare i dati in forma di riepilogo, per giorno o per mese. Questa opzione non è disponibile per tutti i rapporti.

* **Specifica un periodo di tempo**: scegliere le opzioni per definire un periodo di tempo per il report, quindi selezionare **[!UICONTROL Aggiorna]** dopo aver definito un periodo di tempo:

* **Periodo di tempo predefinito**: scegliere un&#39;opzione dal menu Report predefinito. Ad esempio, scegliete Ultimo mese per acquisire i dati a partire dall’ultimo mese.

* **Periodo di tempo personalizzato**: dal menu Report predefinito, seleziona **[!UICONTROL Personalizzato]**. Quindi scegli una data nel menu **[!UICONTROL Mese iniziale]** (o **[!UICONTROL Data inizio]**) e una data nel menu # di mesi (o # o giorni). Per i rapporti Dominio e Contenuti video, potete scegliere una data iniziale e finale specifica per l’acquisizione delle informazioni per il rapporto.

* **Ordinare i dati (solo visualizzazione dati)**: ordinare le informazioni in una colonna. Seleziona l’intestazione della colonna. Seleziona nuovamente per ordinare in ordine decrescente.

* **Ridisponi colonne (solo visualizzazione dati)**: per spostare una colonna in una posizione diversa nella griglia dati, trascinarne l&#39;intestazione.

### Esportare e stampare i rapporti {#exporting-and-printing-reports}

I rapporti generati possono essere esportati in modo da consentire l’utilizzo dei dati in fogli di calcolo e altre applicazioni. I rapporti possono inoltre essere stampati.

* **Esporta dati report**: nella visualizzazione dati, ordinare e disporre i dati in base alle esigenze. Apri il menu **[!UICONTROL Esporta]** e scegli un formato: **[!UICONTROL Delimitato da tabulazioni]**, **[!UICONTROL Separato da virgole]** o **[!UICONTROL Formattato da HTML]**. I dati vengono copiati negli Appunti nel formato scelto. e li potete quindi incollare in un foglio di calcolo o in un’altra applicazione.

* **Stampa un report**: selezionare **[!UICONTROL Stampa]**, scegliere le opzioni desiderate nella finestra di dialogo Stampa, quindi selezionare **[!UICONTROL OK]**.

## Errori immagini {#image-errors}

Gli amministratori di Adobe Dynamic Media Classic possono generare rapporti di errore immagine. Questi rapporti forniscono un elenco dei 20 errori più frequenti relativi alle immagini, per le ultime 24 ore, riferiti alla società a cui siete attualmente collegati. Per generare un report di errori immagine, effettuare le seguenti operazioni:

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**.
1. Espandere Amministrazione, quindi selezionare **[!UICONTROL Errori immagine]**.
1. (Facoltativo) Effettuate una o più delle operazioni seguenti:

   * Per ordinare gli errori in base alle informazioni sull&#39;intestazione, selezionare un&#39;intestazione. Per impostazione predefinita, gli errori vengono ordinati per numero di occorrenze, dalla più alta alla più bassa.
   * Portate il cursore sul campo Risposta di un errore per visualizzare il messaggio di errore specifico.
   * Per visualizzare il collegamento all&#39;immagine o alla pagina Web del referente, spostare il cursore sul campo URL o sul campo Referrer.
   * Per copiare il collegamento all&#39;immagine effettiva, selezionare **[!UICONTROL URL copia URL]**. Potete quindi incollare il collegamento nel campo indirizzo della finestra di un browser per passare all’immagine ed esaminare l’errore.
   * Per copiare il collegamento alla pagina Web del referente, selezionare **[!UICONTROL URL copia referente]**.

Gli errori visualizzati si riferiscono alla società a cui hai effettuato l’accesso. Ciascun errore include le seguenti informazioni:

* **ID immagine**: ID dell&#39;immagine offesa.

* **Ora**: l&#39;intervallo di tempo della prima segnalazione dell&#39;errore all&#39;ultima segnalazione dell&#39;errore, nelle ultime 24 ore.

* **Count**: numero di errori segnalati nell&#39;immagine.

* **Risposta**: messaggio di errore specifico. Gli errori possono essere di tipo 4xx o 5xx.

* **URL**: elenca l&#39;URL dell&#39;immagine in Adobe Dynamic Media Classic.

* **Referrer**: specifica l&#39;URL del sito Web da cui proviene la richiesta iniziale. Il referente può essere qualsiasi sito Web con un collegamento all&#39;immagine.

Alle colonne URL e Referente è stata associata la relativa funzione Copia URL per facilitare la verifica.
