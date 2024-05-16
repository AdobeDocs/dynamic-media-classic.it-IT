---
title: Creare e abilitare i predefiniti immagine
description: Scopri come creare e abilitare i predefiniti immagine in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 49%

---

# Creare e abilitare i predefiniti immagine{#creating-and-enabling-image-presets}

Quando gli utenti esportano delle risorse immagini mediante Media Portal, possono scegliere un predefinito per immagini nella finestra di dialogo Esporta risorse selezionate. Un predefinito immagine è una raccolta di impostazioni predefinite che modificano le dimensioni, la qualità, il formato, la risoluzione e altri aspetti dell&#39;aspetto di un&#39;immagine esportata.

Gli amministratori di Media Portal possono creare i predefiniti per immagini per determinare il modo in cui le immagini vengono riformattate al momento dell’esportazione. I predefiniti per immagini riformattano le immagini secondo le specifiche della società quando gli utenti esportano immagini da Adobe Dynamic Media Classic. Anziché riformattare le immagini singolarmente impostandone le varie opzioni, gli utenti possono così esportarle secondo le esatte specifiche determinate da un particolare predefinito per immagini.

Per l’esportazione delle risorse di immagine sono applicabili le restrizioni seguenti:

* La larghezza × l&#39;altezza devono essere inferiori o uguali a 100 MB per immagine. Ad esempio, l&#39;immagine non può superare i 10 K × 10 K o qualsiasi variante di aspetto inferiore, ad esempio 8 K × 12 K.
* Per ogni processo di esportazione è disponibile un massimo di 1 GB di dimensione totale del file.
* Il limite massimo per il numero di risorse totali per singolo processo di esportazione è di 500 risorse.

>[!NOTE]
>
>Queste restrizioni si applicano solo all’esportazione di risorse immagine derivate, non all’esportazione di file primari.

Per creare i predefiniti per immagini, consultate [Predefiniti per immagini](application-setup.md#image_presets).

Per consentire agli utenti di scegliere Predefiniti immagine al momento dell’esportazione dei file, consultate [Specifica delle opzioni di esportazione disponibili per gli utenti di Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

Per scegliere i predefiniti per immagini disponibili per i membri di un gruppo, consultate [Scegliere le autorizzazioni di accesso ai predefiniti per immagini per un gruppo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
