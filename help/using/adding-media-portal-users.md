---
title: Aggiungere e gestire gli utenti di Media Portal
description: Scopri come aggiungere e gestire utenti Media Portal in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
topic: Administration
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 54%

---

# Aggiungere e gestire gli utenti di Media Portal{#adding-and-managing-media-portal-users}

In qualità di amministratore, potete aggiungere e gestire gli utenti, scegliere se consentire loro di cambiare la propria password, modificare le informazioni utente e caricare elenchi di utenti. Tali attività vengono svolte nella schermata Amministrazione utente. Per accedere a questa schermata, passa a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Configurazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.

>[!NOTE]
>
>prima di aggiungere degli utenti, impostate i gruppi con cui potrete amministrarli. In Media Portal non è possibile aggiungere un utente senza assegnarlo ad almeno un gruppo. Per ulteriori informazioni, consulta [Creare e gestire gruppi Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Amministrazione delle password di Media Portal {#handling-media-portal-passwords}

Quando vengono registrati per l’accesso, gli utenti, i collaboratori e i collaboratori-utenti di Media Portal ricevono un messaggio di benvenuto contenente una password. Gli amministratori possono scegliere se consentire agli utenti di Media Portal di modificare tale password.

1. Accedi a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione Media Portal]** > **[!UICONTROL Impostazioni generali]**.
1. Nella pagina Impostazioni generali, selezionate o deselezionate **[!UICONTROL Consenti a utente Media Portal di modificare la password]**.
1. Seleziona **[!UICONTROL Salva]**.

>[!NOTE]
>
>Gli utenti di Media Portal autorizzati a modificare le password possono farlo selezionando **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]** e la modifica delle password nella schermata Impostazione personale.

## Aggiungere un utente Media Portal {#adding-a-media-portal-user}

1. Accedi a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Configurazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Nella pagina User Administration (Amministrazione utenti), seleziona **Aggiungi**.
1. In **[!UICONTROL `Add User`]** nel pannello Informazioni utente, immettete Nome, Cognome e Indirizzo e-mail dell&#39;utente, quindi selezionate **[!UICONTROL Successivo]**.
1. Nel pannello Società/Ruolo, nell’elenco a discesa Società, selezionate una o più società per l’utente.
1. Nell&#39;elenco Ruolo selezionare un ruolo Media Portal e quindi selezionare **[!UICONTROL Successivo]**.

   Consultate [Ruoli utenti di Media Portal](media-portal-user-roles.md#media_portal_user_roles).

1. Nel pannello Gruppi di accesso, selezionate uno o più gruppi.

   Consulta [Creare e gestire gruppi Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Facoltativo) Seleziona **[!UICONTROL Impostazioni e-mail]** per scegliere impostazioni di posta elettronica diverse dalle impostazioni predefinite.

   Consultate [Impostare il messaggio di benvenuto per gli utenti di Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Seleziona **[!UICONTROL Aggiungi utente]**.

Dopo avere aggiunto un utente, Media Portal invia all’utente un messaggio e-mail di benvenuto. Il messaggio contiene una password temporanea e l’URL di Media Portal.

## Caricare un elenco di utenti in Media Portal {#uploading-a-media-portal-user-list}

Se dovete aggiungere numerosi utenti, potete caricare un elenco di utenti. Gli utenti vengono aggiunti automaticamente all’account attualmente selezionato.

Create l’elenco di utenti in un file in formato CSV (con valori separati da virgole) contenente le informazioni sugli utenti. Una volta caricato il file, gli utenti inclusi nell’elenco vengono automaticamente aggiunti all’account e assegnati ai gruppi specificati. A ogni nuovo utente viene inviato un messaggio e-mail di benvenuto contenente un collegamento a Media Portal e una password temporanea.

### Creare il file CSV {#create-the-csv-file}

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
| Prato | Kat | `prairiek@company.com` | benvenuto | MediaPortalAdmin | PortalCo/IT, PortalCo/Admin |
| Rick | Rugosità | `rickb@myco.com` | benvenuto | MediaPortalUser | PortalCo/MktgGroup,PortalCo/test |

### Caricare il file CSV {#uploading-the-csv-file}

1. Aprite la schermata di configurazione Amministrazione utente.
1. Seleziona **[!UICONTROL Carica elenco utenti]**.
1. Nella finestra di dialogo Seleziona file da caricare, seleziona il file CSV, quindi fai clic su **[!UICONTROL Apri]**.

Ogni utente dell&#39;elenco viene aggiunto automaticamente ai gruppi specificati. Inoltre, a ognuno viene inviato un messaggio e-mail di benvenuto.

>[!NOTE]
>
>Se il file CSV non è stato formattato correttamente, viene visualizzato il seguente messaggio di errore: &quot;Si è verificato un errore durante l’elaborazione del file CSV caricato. Verificare che il contenuto del file contenga dati validi.&quot; Inoltre, se il file CSV contiene un utente IP o IPS esistente, quest’ultimo non viene aggiunto all’elenco di utenti.

## Generare un elenco selezionabile di utenti Media Portal {#generating-a-selectable-list-of-media-portal-users}

Potete visualizzare i nomi e gli indirizzi e-mail degli utenti Media Portal in una finestra a comparsa. Questo elenco è utile per tagliare e incollare nomi utente e indirizzi da usare all’esterno di Media Portal.

1. Accedi a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Configurazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. In **[!UICONTROL Per ruolo utente]** , scegliere il nome di un ruolo utente di Media Portal e selezionare **[!UICONTROL Aggiorna]** per visualizzare i nomi di una classe di utenti di Media Portal.
1. Seleziona **[!UICONTROL Elenco a comparsa]**. Copia e incolla questo elenco.

## Impostare il messaggio di benvenuto per gli utenti di Media Portal {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Quando aggiungete nuovi utenti, collaboratori e collaboratori-utenti di Media Portal, potete inviare loro un messaggio di benvenuto. È possibile configurare questo messaggio di posta elettronica o comunicare a Adobe Dynamic Media Classic di non inviarlo.

1. Accedi a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Configurazione amministrazione]** > **[!UICONTROL Amministrazione utente]**.
1. Nella schermata User Administration Setup (Impostazione amministrazione utente), seleziona **[!UICONTROL Impostazioni e-mail]**.
1. Nella finestra di dialogo Impostazioni e-mail, specificate una delle seguenti impostazioni:

   * **[!UICONTROL Invia e-mail]**: deseleziona questa opzione per informare i nuovi utenti tramite e-mail che li hai iscritti.

   * **[!UICONTROL Password predefinita]**: immetti una password temporanea per i nuovi utenti o lascia vuoto il campo affinché Adobe Dynamic Media Classic generi password casuali. Gli utenti devono cambiare la password al primo accesso.

   * **[!UICONTROL URL sostitutivo]**: immetti un URL diverso da quello predefinito se gli utenti accedono a Adobe Dynamic Media Classic tramite un URL diverso.

## Altre attività di gestione degli utenti {#other-user-management-tasks}

A partire dalla schermata di configurazione Amministrazione utenti potete effettuare le seguenti attività:

* **[!UICONTROL Filtrare e ordinare l’elenco degli utenti]**: filtra l’elenco degli utenti di Media Portal per individuare gli utenti.

* **[!UICONTROL Elimina utenti]**: rimuove un utente dall’elenco.

* **[!UICONTROL Attivare e disattivare gli utenti]**: sospende l’accesso di un utente alle cartelle.

* **[!UICONTROL Modifica informazioni utente]**: immetti informazioni aggiornate su un utente.

* **[!UICONTROL Creare campi definiti dall&#39;utente]**: crea campi di metadati personalizzati e definiti dall’utente, che consentono di organizzare le risorse in Adobe Dynamic Media Classic. I campi possono essere attivati o disattivati, in base alle esigenze.

Consultate [Campi definiti dall’utente](application-setup.md#user_defined_fields).
