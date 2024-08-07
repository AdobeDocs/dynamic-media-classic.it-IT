---
title: Creare e gestire gruppi Media Portal
description: Scopri come creare e gestire i gruppi Media Portal in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 49%

---

# Creare e gestire gruppi Media Portal{#creating-and-managing-media-portal-groups}

I *gruppi* facilitano l’amministrazione degli utenti di Media Portal. Per accedere a una risorsa, un utente deve appartenere ad almeno un gruppo autorizzato ad accedere a tale risorsa. Quando aggiungete un utente, lo potete assegnare a uno o più gruppi. In questo modo, si concede all&#39;utente l&#39;accesso alle cartelle a cui è stato assegnato il gruppo. Potete inoltre scegliere i predefiniti per immagini disponibili per un dato gruppo.

## Utilizzare i gruppi per limitare l’accesso a cartelle, risorse e predefiniti immagine {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

La creazione di gruppi consente di assegnare diversi livelli di autorizzazione di accesso. Per ogni gruppo, potete assegnare le autorizzazioni di lettura, scrittura ed eliminazione per diverse cartelle e risorse nelle cartelle. Potete inoltre decidere quali predefiniti per immagini rendere disponibili per il gruppo. Successivamente, potete assegnare utenti ai relativi gruppi. Un utente può appartenere a più di un gruppo. Grazie all’uso dei gruppi potete limitare il diritto di accesso a soli alcuni set di risorse.

Se specificatamente non concedi un’autorizzazione di gruppo a una risorsa o cartella, questa eredita le autorizzazioni assegnate alla relativa cartella principale, ovvero la cartella al di sopra di essa nella gerarchia delle cartelle. Assegnando le autorizzazioni a una cartella principale potrete avere la certezza che tutte le relative sottocartelle ereditino le stesse autorizzazioni.

>[!NOTE]
>
>gli utenti possono appartenere a più di un gruppo. Se un utente appartiene a due gruppi con diverse autorizzazioni di accesso a una cartella, gli viene assegnato il livello di accesso più alto.

## Aggiungere un gruppo {#adding-a-group}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione Media Portal]** > **[!UICONTROL Gruppi]**.
1. Seleziona **[!UICONTROL Aggiungi]**.
1. Nella finestra di dialogo Aggiungi gruppo immettere un nome per il gruppo nella casella Nome gruppo, quindi selezionare **[!UICONTROL Aggiungi gruppo]**.
1. Se lo desiderate, potete selezionare le caselle di controllo accanto ai nomi di utenti per aggiungere degli utenti a un nuovo gruppo.
1. Se desideri specificare ora le autorizzazioni di accesso, seleziona la scheda **[!UICONTROL Autorizzazioni di accesso alle risorse]**, quindi specifica le opzioni desiderate.

   Consultate [Definire le autorizzazioni di accesso alle risorse per un gruppo](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Potete scegliere quali predefiniti immagine sono disponibili per il gruppo. Fai clic sulla scheda **[!UICONTROL Autorizzazioni di accesso al predefinito immagine]** e seleziona Predefiniti immagine utilizzabili dal gruppo.

   Consultate [Scegliere le autorizzazioni di accesso ai predefiniti per immagini per un gruppo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Seleziona **[!UICONTROL Chiudi]**.

## Definire le autorizzazioni di accesso alle risorse per un gruppo {#establishing-asset-access-permissions-for-a-group}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione Media Portal]** > **[!UICONTROL Gruppi]**.
1. Nella pagina dell’elenco Gruppi, effettuate una delle seguenti operazioni:

   * Per aggiungere un gruppo e specificare le autorizzazioni, selezionare **[!UICONTROL Aggiungi]**. Nella finestra di dialogo Aggiungi gruppo immettere un nome per il gruppo, selezionare **[!UICONTROL Aggiungi gruppo]** e aggiungere utenti al gruppo.
   * Per modificare le autorizzazioni di un gruppo, selezionare il gruppo, quindi selezionare **[!UICONTROL Modifica]**.

1. Nella finestra di dialogo Aggiungi gruppo o Modifica gruppo, seleziona la scheda **[!UICONTROL Autorizzazioni di accesso alle risorse]**. Nella parte destra della scheda sono disponibili le caselle per specificare le autorizzazioni di lettura, scrittura ed eliminazione per cartelle e risorse. Potete espandere e comprimere cartelle e sottocartelle nel riquadro a sinistra.
1. Per assegnare le autorizzazioni necessarie a cartelle o singole risorse, selezionate la cartella nel riquadro a sinistra. Il contenuto della cartella viene visualizzato nel riquadro a destra. Quindi assegnare i diritti per il gruppo selezionando le caselle per i file corrispondenti. Oppure, selezionando le cartelle nel riquadro di destra.

   La tabella di seguito presenta le associazioni tra diverse attività e le autorizzazioni di lettura, scrittura ed eliminazione.

   | Attività | Lettura (r) | Scrittura (w) | Eliminazione (d) |
   | --- | --- | --- | --- |
   | Sfogliare cartelle e file | X | | |
   | Modificare i file (ritaglio, nitidezza, regolazione) | | X | |
   | Cambiare i nomi di file | | X | |
   | Spostare i file in altre cartelle | | X | |
   | Rinominare i file | | X | |
   | Eliminare i file | | | X |

1. Seleziona **[!UICONTROL Chiudi]**.

>[!NOTE]
>
>le autorizzazioni di accesso entrano in vigore non appena selezionate una casella. Quando hai assegnato i diritti a una cartella, alle sue sottocartelle e a tutti i file al suo interno vengono assegnati gli stessi diritti della cartella principale. Tuttavia, potete specificare autorizzazioni diverse per singole sottocartelle e file di risorse.

## Scegliere le autorizzazioni di accesso ai predefiniti per immagini per un gruppo

Le autorizzazioni di accesso ai predefiniti per immagini per un gruppo vi permettono di specificare quali predefiniti per immagini sono disponibili per gli utenti del gruppo al momento dell’esportazione di risorse in Media Portal.

Vedere anche [Specificare le opzioni di esportazione disponibili per gli utenti di Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**Per scegliere le autorizzazioni di accesso al predefinito immagine per un gruppo:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione Media Portal]** > **[!UICONTROL Gruppi]**.
1. Nella pagina dell’elenco Gruppi, effettuate una delle seguenti operazioni:

   * Per aggiungere un gruppo e specificare i predefiniti immagine disponibili, selezionare **[!UICONTROL Aggiungi]**. Nella finestra di dialogo Aggiungi gruppo immettere un nome per il gruppo, selezionare **[!UICONTROL Aggiungi gruppo]** e aggiungere utenti al gruppo.
   * Per modificare le opzioni del predefinito immagine di un gruppo, selezionare il gruppo, quindi selezionare **[!UICONTROL Modifica]**.

1. Nella finestra di dialogo Aggiungi gruppo o Modifica gruppo, seleziona la scheda **[!UICONTROL Autorizzazioni di accesso per il predefinito immagine]**.
1. Per specificare quali predefiniti sono disponibili per gli utenti di Media Portal quando esportano le risorse, seleziona o deseleziona Predefiniti immagine.
1. Seleziona **[!UICONTROL Chiudi]**.

## Modificare ed eliminare i gruppi {#edit-and-delete-groups}

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione Media Portal]** > **[!UICONTROL Gruppi]**.
1. Nella pagina dell’elenco Gruppi, selezionate un gruppo e modificatelo o eliminatelo.

   **Modifica un gruppo**: selezionare **[!UICONTROL Modifica]**, quindi scegliere le opzioni nella finestra di dialogo Modifica gruppo.

   **Elimina un gruppo**: selezionare **[!UICONTROL Elimina]**.
