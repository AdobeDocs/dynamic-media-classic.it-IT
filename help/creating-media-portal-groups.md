---
title: 'Creazione e gestione di gruppi in Media Portal '
seo-title: 'Creazione e gestione di gruppi in Media Portal '
description: 'null'
seo-description: Scoprite come creare e gestire i gruppi in Media Portal.
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 96%

---


# Creazione e gestione di gruppi in Media Portal {#creating-and-managing-media-portal-groups}

I *gruppi* facilitano l’amministrazione degli utenti di Media Portal. Per accedere a una risorsa, un utente deve appartenere ad almeno un gruppo autorizzato ad accedere a tale risorsa. Quando aggiungete un utente, lo potete assegnare a uno o più gruppi. Così facendo gli assegnate le autorizzazioni di accesso alle cartelle a cui è stato assegnato un dato gruppo. Potete inoltre scegliere i predefiniti per immagini disponibili per un dato gruppo.

## Utilizzo dei gruppi per limitare l’accesso a cartelle, risorse e predefiniti per immagini {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

La creazione di gruppi consente di assegnare diversi livelli di autorizzazione di accesso. Per ogni gruppo, potete assegnare le autorizzazioni di lettura, scrittura ed eliminazione per diverse cartelle e risorse nelle cartelle. Potete inoltre decidere quali predefiniti per immagini rendere disponibili per il gruppo. Successivamente, potete assegnare utenti ai relativi gruppi. Un utente può appartenere a più di un gruppo. Grazie all’uso dei gruppi potete limitare il diritto di accesso a soli alcuni set di risorse.

Se non assegnate espressamente a un gruppo l’autorizzazione per una risorsa o una cartella, questa eredita le autorizzazioni assegnate alla cartella principale (la cartella che si trova al livello superiore nella gerarchia di cartelle). Assegnando le autorizzazioni a una cartella principale potrete avere la certezza che tutte le relative sottocartelle ereditino le stesse autorizzazioni.

>[!NOTE]
>
>gli utenti possono appartenere a più di un gruppo. Se un utente appartiene a due gruppi con diverse autorizzazioni di accesso a una cartella, gli viene assegnato il livello di accesso più alto.

## Aggiunta di un gruppo {#adding-a-group}

1. Fate clic su **Configurazione** >**Configurazione Media Portal** > **Gruppi**.
1. Fate clic su **Aggiungi**.
1. Nella finestra di dialogo Aggiungi gruppo, inserite un nome per il gruppo nella casella Nome gruppo e fate clic su **Aggiungi gruppo**.
1. Se lo desiderate, potete selezionare le caselle di controllo accanto ai nomi di utenti per aggiungere degli utenti a un nuovo gruppo.
1. Se desiderate specificare autorizzazioni di accesso in questa fase, fate clic sulla scheda **Autorizzazioni di accesso alle risorse** e specificate le opzioni desiderate.

   Consultate [Definire le autorizzazioni di accesso alle risorse per un gruppo](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Per scegliere quali predefiniti per immagini rendere disponibili per il gruppo, fate clic sulla scheda **Autorizzazioni di accesso ImagePreset** e selezionate i predefiniti per immagini che potranno essere usati dal gruppo.

   Consultate [Scegliere le autorizzazioni di accesso ai predefiniti per immagini per un gruppo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Fate clic su **Chiudi**.

## Definizione delle autorizzazioni di accesso alle risorse per un gruppo {#establishing-asset-access-permissions-for-a-group}

1. Fate clic su **Configurazione** >**Configurazione Media Portal** > **Gruppi**.
1. Nella pagina dell’elenco Gruppi, effettuate una delle seguenti operazioni:

   * Per aggiungere un gruppo e specificare le autorizzazioni, fate clic su **Aggiungi**. Nella finestra di dialogo Aggiungi gruppo, inserite un nome per il gruppo, fate clic su **Aggiungi gruppo** e aggiungete utenti al gruppo.
   * Per modificare le autorizzazioni assegnate a un gruppo, selezionate il gruppo e fate clic su **Modifica**.

1. Nella finestra di dialogo Aggiungi gruppo o Modifica gruppo, fate clic sulla scheda **Autorizzazioni di accesso alle risorse**. Nella parte destra della scheda sono disponibili le caselle per specificare le autorizzazioni di lettura, scrittura ed eliminazione per cartelle e risorse. Potete espandere e comprimere cartelle e sottocartelle nel riquadro a sinistra.
1. Per assegnare le autorizzazioni necessarie a cartelle o singole risorse, selezionate la cartella nel riquadro a sinistra. Il contenuto della cartella viene visualizzato nel riquadro a destra. Per assegnare le autorizzazioni al gruppo, selezionate le caselle per i corrispondenti file e cartelle nel riquadro a destra.

   La tabella di seguito presenta le associazioni tra diverse attività e le autorizzazioni di lettura, scrittura ed eliminazione.

   | Attività | Lettura (r) | Scrittura (w) | Eliminazione (d) |
   |--- |--- |--- |--- |
   | Sfogliare cartelle e file | X |  |  |
   | Modificare i file (ritaglio, nitidezza, regolazione) |  | X |  |
   | Cambiare i nomi di file |  | X |  |
   | Spostare i file in altre cartelle |  | X |  |
   | Rinominare i file |  | X |  |
   | Eliminare i file |  |  | X |

1. Fai clic su **Chiudi**.

>[!NOTE]
>
>le autorizzazioni di accesso entrano in vigore non appena selezionate una casella. Quando assegnate le autorizzazioni a una cartella, queste vengono applicate anche alle relative sottocartelle e a tutti i file al loro interno. Tuttavia, potete specificare autorizzazioni diverse per singole sottocartelle e file di risorse.

## Scelta delle autorizzazioni di accesso ai predefiniti per immagini per un gruppo {#choosing-image-preset-access-permissions-for-a-group}

Le autorizzazioni di accesso ai predefiniti per immagini per un gruppo vi permettono di specificare quali predefiniti per immagini sono disponibili per gli utenti del gruppo al momento dell’esportazione di risorse in Media Portal.

Consultate anche [Specifica delle opzioni di esportazione disponibili per gli utenti di Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

1. Fate clic su **Configurazione** >**Configurazione Media Portal** > **Gruppi**.
1. Nella pagina dell’elenco Gruppi, effettuate una delle seguenti operazioni:

   * Per aggiungere un gruppo e specificare quali predefiniti per immagini sono disponibili per tale gruppo, fate clic su **Aggiungi**. Nella finestra di dialogo Aggiungi gruppo, inserite un nome per il gruppo, fate clic su **Aggiungi gruppo** e aggiungete utenti al gruppo.
   * Per modificare le opzioni di predefiniti per immagini di un gruppo, selezionate il gruppo e fate clic su **Modifica**.

1. Nella finestra di dialogo Aggiungi gruppo o Modifica gruppo, fate clic sulla scheda **Autorizzazioni di accesso ImagePreset**.
1. Selezionate o deselezionate i predefiniti per immagini per specificare quelli che devono essere disponibili per gli utenti di Media Portal in fase di esportazione delle risorse.
1. Fate clic su **Chiudi**.

## Modificare ed eliminare i gruppi {#edit-and-delete-groups}

1. Fate clic su **Configurazione** >**Configurazione Media Portal** > **Gruppi**.
1. Nella pagina dell’elenco Gruppi, selezionate un gruppo e modificatelo o eliminatelo.

   **Modifica di un gruppo** Fate clic su Modifica, quindi scegliete le opzioni desiderate nella finestra di dialogo Modifica gruppo.

   **Eliminazione di un gruppo** Fate clic su Elimina.

