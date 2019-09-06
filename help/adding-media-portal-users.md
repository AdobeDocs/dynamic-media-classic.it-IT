---
title: Aggiunta e gestione di utenti in Media Portal
seo-title: Aggiunta e gestione di utenti in Media Portal
description: 'null'
seo-description: Informazioni su come aggiungere e gestire utenti di Media Portal
uuid: 96 d 4103 c -6428-4 ce 1-b 9 e 4-231599304 f 27
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/media_ portal
discoiquuid: 5 e 933045-ce 1 a -41 b 9-ba 8 b -2151 c 396 b 7 a 2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Aggiunta e gestione di utenti in Media Portal{#adding-and-managing-media-portal-users}

In qualità di amministratore, potete aggiungere e gestire gli utenti, scegliere se consentire loro di cambiare la propria password, modificare le informazioni utente e caricare elenchi di utenti. Tali attività vengono svolte nella schermata Amministrazione utente. Per accedere a questa schermata, scegliete **Configurazione** &gt; **Impostazione applicazione**, quindi in **Impostazione amministrazione** fate clic su **Amministrazione utente**.

>[!NOTE]
>
>prima di aggiungere degli utenti, impostate i gruppi con cui potrete amministrarli. In Media Portal non è possibile aggiungere un utente senza assegnarlo ad almeno un gruppo. Per ulteriori informazioni, consultate [Creazione e gestione di gruppi in Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Gestione delle password per Media Portal {#handling-media-portal-passwords}

Quando vengono registrati per l’accesso, gli utenti, i collaboratori e i collaboratori-utenti di Media Portal ricevono un messaggio di benvenuto contenente una password. Gli amministratori possono scegliere se consentire agli utenti di Media Portal di modificare tale password.

1. Fate clic su **Configurazione** &gt; **Configurazione Media Portal** &gt; **Impostazioni generali**.
1. Nella pagina Impostazioni generali, selezionate o deselezionate **Consenti a utente Media Portal di modificare la password**.
1. Fate clic su **Salva**.

>[!NOTE]
>
>gli utenti Media Portal cui tale modifica è consentita possono scegliere **Configurazione** &gt; **Configurazione personale** e modificare la propria password nella schermata risultante.

## Aggiunta di utente di Media Portal {#adding-a-media-portal-user}

1. Fate clic su **Configurazione** &gt; **Impostazione applicazione** &gt; **Impostazione amministrazione** &gt; **Amministrazione utente**.
1. Nella pagina Amministrazione utente, fate clic su **Aggiungi**.
1. Nella finestra di dialogo Aggiungi utente, nel pannello Informazioni utente, immettete il nome, il cognome e l’indirizzo e-mail dell’utente e fate clic su **Avanti**.
1. Nel pannello Società/Ruolo, nell’elenco a discesa Società, selezionate una o più società per l’utente.
1. Nell’elenco Ruolo, selezionate un ruolo Media Portal e fate clic su **Avanti**.

   Consultate [Ruoli utenti di Media Portal](media-portal-user-roles.md#media_portal_user_roles).

1. Nel pannello Gruppi di accesso, selezionate uno o più gruppi.

   Consultate [Creazione e gestione di gruppi in Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Facoltativo) Fate clic su **Impostazioni e-mail** per scegliere impostazioni e-mail diverse da quelle predefinite.

   Consultate [Impostare il messaggio di benvenuto per gli utenti di Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Fate clic su **Aggiungi utente**.

Dopo avere aggiunto un utente, Media Portal invia all’utente un messaggio e-mail di benvenuto. Il messaggio contiene una password temporanea e l’URL di Media Portal.

## Caricamento di un elenco di utenti in Media Portal {#uploading-a-media-portal-user-list}

Se dovete aggiungere numerosi utenti, potete caricare un elenco di utenti. Gli utenti vengono aggiunti automaticamente all’account attualmente selezionato.

Create l’elenco di utenti in un file in formato CSV (con valori separati da virgole) contenente le informazioni sugli utenti. Una volta caricato il file, gli utenti inclusi nell’elenco vengono automaticamente aggiunti all’account e assegnati ai gruppi specificati. A ogni nuovo utente viene inviato un messaggio e-mail di benvenuto contenente un collegamento a Media Portal e una password temporanea.

### Creazione del file CSV {#creating-the-csv-file}

Create un file CSV (nomefile.csv) rispettando il formato e i campi indicati di seguito. La prima riga del file deve contenere le intestazioni di colonna riportate in questa tabella; potete ordinare le colonne in base alle vostre esigenze. Tutte le colonne sono obbligatorie.

| Nome colonna | Descrizione |
|--- |--- |
| Nome | Il nome dell’utente. |
| Cognome | Il cognome dell’utente. |
| E-mail | Un indirizzo e-mail valido. |
| Password | Una stringa di testo sensibile alle maiuscole. |
| Ruolo utente | Mediaportaladminmediaportalusermediaportalcontributormediaportalcontributoruser |
| Gruppi | Elenco di uno o più gruppi a cui assegnare ciascun utente, separati da virgole. Specificate il gruppo anteponendo come prefisso il nome account, separato da una barra (/). Ad esempio, PortalCo/IT, dove PortalCo è l’account e IT è il gruppo all’interno dell’account PortalCo. |

Il seguente foglio di calcolo di esempio illustra come deve essere preparato il file CSV:

| Nome | Cognome | E-mail | Password | Ruolo utente | Gruppi |
|--- |--- |--- |--- |--- |--- |
| Giovanni | Bianchi | `petep@company.com` | benvenuto | MediaPortalAdmin | PortalCo/IT,PortalCo/Admin |
| Andrea | Rossi | `kevinm@myco.com` | benvenuto | MediaPortalUser | PortalCo/MktgGroup,PortalCo/test |


### Caricamento del file CSV {#uploading-the-csv-file}

1. Aprite la schermata di configurazione Amministrazione utente.
1. Fate clic su **Carica elenco utenti**.
1. Nella finestra di dialogo Seleziona file da caricare, selezionate il file CSV e fate clic su **Apri**.

Ogni utente dell’elenco viene automaticamente aggiunto al gruppo specificato. Inoltre, a ognuno viene inviato un messaggio e-mail di benvenuto.

>[!NOTE]
se il file CSV non è stato formattato correttamente, viene visualizzato il seguente messaggio di errore: “Si è verificato un errore durante l’elaborazione del file CSV caricato. Verificate che il file contenga dati validi.” Inoltre, se il file CSV contiene un utente IP o IPS esistente, quest’ultimo non viene aggiunto all’elenco di utenti.

## Generazione di un elenco selezionabile di utenti Media Portal {#generating-a-selectable-list-of-media-portal-users}

Potete visualizzare i nomi e gli indirizzi e-mail degli utenti Media Portal in una finestra a comparsa. Questo elenco è utile per tagliare e incollare nomi utente e indirizzi da usare all’esterno di Media Portal.

1. Fate clic su **Configurazione** &gt; **Impostazione applicazione** &gt; **Impostazione amministrazione** &gt; **Amministrazione utente**.
1. Per ottenere solo i nomi di uno specifico tipo di utenti di Media Portal, dall’elenco a discesa **Per ruolo utente** scegliete il nome di un ruolo utente di Media Portal e fate clic su **Aggiorna**.
1. Per aprire la finestra a comparsa fate clic su **Elenco a comparsa**. Potete quindi copiare e incollare l’elenco risultante.

## Impostazione de l messaggio di benvenuto per gli utenti di Media Portal {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Quando aggiungete nuovi utenti, collaboratori e collaboratori-utenti di Media Portal, potete inviare loro un messaggio di benvenuto. Potete configurare questo messaggio e-mail o indicare a Dynamic Media Classic di non inviarlo.

1. Scegliete **Configurazione** &gt; **Impostazione applicazione** &gt; **Impostazione amministrazione** &gt; **Amministrazione utente**.
1. In the User Administration Setup screen, click **Email Settings**.
1. Nella finestra di dialogo Impostazioni e-mail, specificate una delle seguenti impostazioni:

   **Invia e-mail** Deselezionate questa opzione se non desiderate inviare per e-mail i nuovi utenti che sono stati registrati.

   **Password predefinita** Consente di immettere una password temporanea per i nuovi utenti oppure di lasciare il campo vuoto per generare password casuali generate da Dynamic Media Classic. Agli utenti verrà chiesto di cambiare questa password al loro primo accesso.

   **URL sostituzione** Consente di immettere un URL diverso da quello predefinito se gli utenti accedono a Dynamic Media Classic tramite un URL diverso.

## Altre attività di gestione degli utenti {#other-user-management-tasks}

A partire dalla schermata di configurazione Amministrazione utenti potete effettuare le seguenti attività:

**Filtrare e ordinare l'elenco di utenti** Filtrare l'elenco degli utenti di Media Portal per individuare gli utenti. Consultate Filtrare e ordinare l’elenco di utenti.

**Elimina utenti** Consente di eliminare un utente dall'elenco. Consultate Eliminare un utente.

**Attivazione e disattivazione degli utenti** Sospendi un utente dalle cartelle. Consultate Attivare e disattivare gli utenti.

**Modifica delle informazioni utente** Consente di immettere informazioni aggiornate su un utente. Consultate Modificare le informazioni utente.

**Creazione di campi definiti dall'utente** Create campi di metadati definiti dall'utente per organizzare le risorse in Scene 7 Publishing System. I campi possono essere attivati o disattivati, in base alle esigenze.

Consultate [Campi definiti dall’utente](application-setup.md#user_defined_fields).
