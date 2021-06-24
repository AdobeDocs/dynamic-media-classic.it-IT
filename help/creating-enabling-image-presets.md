---
title: Creazione e attivazione dei predefiniti per immagini
description: Scopri come creare e abilitare i predefiniti per immagini.
uuid: 62cfc6fa-da91-4c42-a3ed-10956384d633
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84257b2a-681c-4fe9-a6e5-3633c1d61d8c
feature: Dynamic Media Classic, Collaborazione, Predefiniti immagine, Gestione risorse
role: Administrator,Business Practitioner
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 81%

---

# Creazione e attivazione dei predefiniti per immagini{#creating-and-enabling-image-presets}

Quando gli utenti esportano delle risorse immagini mediante Media Portal, possono scegliere un predefinito per immagini nella finestra di dialogo Esporta risorse selezionate. Un predefinito per immagini è una raccolta di impostazioni preconfigurate che agiscono sulla dimensione, la qualità immagine, il formato, la risoluzione e altri aspetti di un’immagine quando questa viene esportata. 

Gli amministratori di Media Portal possono creare i predefiniti per immagini per determinare il modo in cui le immagini vengono riformattate al momento dell’esportazione. I predefiniti per immagini riformattano le immagini in base alle specifiche della tua azienda quando gli utenti esportano le immagini da Dynamic Media Classic. Anziché riformattare le immagini singolarmente impostandone le varie opzioni, gli utenti possono così esportarle secondo le esatte specifiche determinate da un particolare predefinito per immagini.

Per l’esportazione delle risorse di immagine sono applicabili le restrizioni seguenti:

* Le dimensioni larghezza x altezza devono essere inferiori o uguali a 100 MB per immagine. Ad esempio, l’immagine non può essere più grande di 10.000x10.000 o di variazioni di proporzioni inferiori come ad esempio 8.000x12.000.
* È disponibile un massimo di 1 GB di dimensione totale del file per processo di esportazione.
* Il limite massimo per il numero di risorse totali per singolo processo di esportazione è di 500 risorse.

>[!NOTE]
>
>queste restrizioni riguardano solo l’esportazione di risorse di immagine derivate, non l’esportazione dei file principali.

Per creare i predefiniti per immagini, consultate [Predefiniti per immagini](application-setup.md#image_presets).

Per consentire agli utenti di scegliere Predefiniti immagine al momento dell’esportazione dei file, consultate [Specifica delle opzioni di esportazione disponibili per gli utenti di Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

Per scegliere i predefiniti per immagini disponibili per i membri di un gruppo, consultate [Scegliere le autorizzazioni di accesso ai predefiniti per immagini per un gruppo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
