---
title: Aggiunta e gestione di utenti in Media Portal
description: Scopri come aggiungere e gestire gli utenti di Media Portal
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic,Collaborazione,Gestione risorse
role: Administrator,Business Practitioner
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
source-git-commit: 31ac96e6fd11c47284d58540f5ec0135f0e6223b
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 81%

---

# Aggiunta e gestione di utenti in Media Portal{#adding-and-managing-media-portal-users}

In qualità di amministratore, potete aggiungere e gestire gli utenti, scegliere se consentire loro di cambiare la propria password, modificare le informazioni utente e caricare elenchi di utenti. Tali attività vengono svolte nella schermata Amministrazione utente. Per accedere a questa schermata, scegliete **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]**, quindi in **[!UICONTROL Impostazione amministrazione]** fate clic su **[!UICONTROL Amministrazione utente]**.

>[!NOTE]
>
>prima di aggiungere degli utenti, impostate i gruppi con cui potrete amministrarli. In Media Portal non è possibile aggiungere un utente senza assegnarlo ad almeno un gruppo. Per ulteriori informazioni, consultate [Creazione e gestione di gruppi in Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Gestione delle password per Media Portal {#handling-media-portal-passwords}

Quando vengono registrati per l’accesso, gli utenti, i collaboratori e i collaboratori-utenti di Media Portal ricevono un messaggio di benvenuto contenente una password. Gli amministratori possono scegliere se consentire agli utenti di Media Portal di modificare tale password.

1. Fate clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione Media Portal]** > **[!UICONTROL Impostazioni generali]**.
1. Nella pagina Impostazioni generali, selezionate o deselezionate **[!UICONTROL Consenti a utente Media Portal di modificare la password]**.
1. Fate clic su **[!UICONTROL Salva]**.

>[!NOTE]
>
>gli utenti Media Portal cui tale modifica è consentita possono scegliere **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]** e modificare la propria password nella schermata risultante.

## Aggiunta di utente di Media Portal {#adding-a-media-portal-user}

1. Fate clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Nella pagina Amministrazione utente, fate clic su **Aggiungi**.
1. Nella finestra di dialogo Aggiungi utente, nel pannello Informazioni utente, immettete il nome, il cognome e l’indirizzo e-mail dell’utente e fate clic su **[!UICONTROL Avanti]**.
1. Nel pannello Società/Ruolo, nell’elenco a discesa Società, selezionate una o più società per l’utente.
1. Nell’elenco Ruolo, selezionate un ruolo Media Portal e fate clic su **[!UICONTROL Avanti]**.

   Consultate [Ruoli utenti di Media Portal](media-portal-user-roles.md#media_portal_user_roles).

1. Nel pannello Gruppi di accesso, selezionate uno o più gruppi.

   Consultate [Creazione e gestione di gruppi in Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Facoltativo) Fate clic su **[!UICONTROL Impostazioni e-mail]** per scegliere impostazioni e-mail diverse da quelle predefinite.

   Consultate [Impostare il messaggio di benvenuto per gli utenti di Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Fate clic su **[!UICONTROL Aggiungi utente]**.

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
| Ruolo utente | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUser |
| Gruppi | Elenco di uno o più gruppi a cui assegnare ciascun utente, separati da virgole. Specificate il gruppo anteponendo come prefisso il nome account, separato da una barra (/). Ad esempio, PortalCo/IT, dove PortalCo è l’account e IT è il gruppo all’interno dell’account PortalCo. |

Il seguente foglio di calcolo di esempio illustra come deve essere preparato il file CSV:

| Nome | Cognome | E-mail | Password | Ruolo utente | Gruppi |
|--- |--- |--- |--- |--- |--- |
| Prato | Kat | `prairiek@company.com` | benvenuto | MediaPortalAdmin | PortalCo/IT,PortalCo/Admin |
| Rick | Brodo | `rickb@myco.com` | benvenuto | MediaPortalUser | PortalCo/MktgGroup,PortalCo/test |


### Caricamento del file CSV {#uploading-the-csv-file}

1. Aprite la schermata di configurazione Amministrazione utente.
1. Fate clic su **[!UICONTROL Carica elenco utenti]**.
1. Nella finestra di dialogo Seleziona file da caricare, selezionate il file CSV e fate clic su **[!UICONTROL Apri]**.

Ogni utente dell’elenco viene automaticamente aggiunto al gruppo specificato. Inoltre, a ognuno viene inviato un messaggio e-mail di benvenuto.

>[!NOTE]
>
>se il file CSV non è stato formattato correttamente, viene visualizzato il seguente messaggio di errore: “Si è verificato un errore durante l’elaborazione del file CSV caricato. Verificate che il file contenga dati validi.” Inoltre, se il file CSV contiene un utente IP o IPS esistente, quest’ultimo non viene aggiunto all’elenco di utenti.

## Generazione di un elenco selezionabile di utenti Media Portal {#generating-a-selectable-list-of-media-portal-users}

Potete visualizzare i nomi e gli indirizzi e-mail degli utenti Media Portal in una finestra a comparsa. Questo elenco è utile per tagliare e incollare nomi utente e indirizzi da usare all’esterno di Media Portal.

1. Fate clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Per ottenere solo i nomi di uno specifico tipo di utenti di Media Portal, dall’elenco a discesa **[!UICONTROL Per ruolo utente]** scegliete il nome di un ruolo utente di Media Portal e fate clic su **[!UICONTROL Aggiorna]**.
1. Per aprire la finestra a comparsa fate clic su **[!UICONTROL Elenco a comparsa]**. Copia e incolla questo elenco.

## Impostazione de l messaggio di benvenuto per gli utenti di Media Portal {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Quando aggiungete nuovi utenti, collaboratori e collaboratori-utenti di Media Portal, potete inviare loro un messaggio di benvenuto. È possibile configurare questo messaggio di posta elettronica o comunicare a Dynamic Media Classic di non inviarlo.

1. Scegliete **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Nella schermata Configurazione amministrazione utente, fai clic su **[!UICONTROL Impostazioni e-mail]**.
1. Nella finestra di dialogo Impostazioni e-mail, specificate una delle seguenti impostazioni:

   * **[!UICONTROL Invia e-mail]** : deseleziona questa opzione se non desideri informare i nuovi utenti via e-mail che li hai registrati.

   * **[!UICONTROL Password predefinita]** : immetti una password temporanea per i nuovi utenti o lascia vuoto il campo per consentire a Dynamic Media Classic di generare password casuali. Agli utenti viene richiesto di cambiare la password al primo accesso.

   * **[!UICONTROL URL di sostituzione]** : immetti un URL diverso da quello predefinito se i tuoi utenti accedono a Dynamic Media Classic tramite un URL diverso.

## Altre attività di gestione degli utenti {#other-user-management-tasks}

A partire dalla schermata di configurazione Amministrazione utenti potete effettuare le seguenti attività:

* **[!UICONTROL Filtrare e ordinare l’elenco degli utenti]**  - Filtrare l’elenco degli utenti di Media Portal per individuare gli utenti.

* **[!UICONTROL Elimina utenti]**  - Rimuovi un utente dall&#39;elenco.

* **[!UICONTROL Attivare e disattivare gli utenti]**  - Sospendi l&#39;accesso alle cartelle da parte di un utente.

* **[!UICONTROL Modifica informazioni utente]**  - Inserisci informazioni aggiornate su un utente.

* **[!UICONTROL Creazione di campi definiti dall’utente]** : consente di creare campi di metadati personalizzati definiti dall’utente per organizzare le risorse in Dynamic Media Classic. I campi possono essere attivati o disattivati, in base alle esigenze.

Consultate [Campi definiti dall’utente](application-setup.md#user_defined_fields).
