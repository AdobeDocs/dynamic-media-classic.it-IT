---
title: Preparazione all’aggiornamento
description: Elenco di controllo per la preparazione all'aggiornamento quando si desidera passare da [!DNL Adobe Dynamic Media Classic] a [!DNL Dynamic Media] il [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
autotag-review: '2026-05-13T20:16:07.073Z'
TQID: 'https://experienceleague.adobe.com/3Kcp3UwvJV8Mkzk6RBRgOJQ7JKF3Ldek-SiOeqS5EKE'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 221
ht-degree: 0%

---

# Elenco di controllo preparazione all’aggiornamento

Utilizzare il seguente elenco di controllo per comprendere e preparare un aggiornamento da [!DNL Dynamic Media Classic] a [!DNL Dynamic Media].

|  | Attività | Descrizione |
| :--- | :--- | --- |
| **Fase 1: gestione licenze** | Esegui contratto | In base al traffico e all&#39;archiviazione, il team dell&#39;account Adobe collabora con te per passare dalla licenza [!DNL Dynamic Media Classic] al rinnovo della licenza [!DNL Dynamic Media]. |
| **Fase 2: Preparazione** | Convalidare l’utilizzo della funzione | Verificare che le funzionalità utilizzate in [!DNL Dynamic Media Classic] siano disponibili in [!DNL Dynamic Media]. Visita la pagina [Confronto delle funzionalità](/help/using/upgrade-feature-comparison.md). Le funzionalità chiave non ancora disponibili in [!DNL Dynamic Media] includono:<br>· Visual Configurator (Image Author, Image Render).<br>· Image Templates (1:1 Templating).<br>· eCatalog.<br>Se vengono utilizzate le funzionalità precedenti, l&#39;aggiornamento può comunque essere eseguito presupponendo che tali funzionalità siano accessibili tramite [!DNL Dynamic Media Classic]. |
|   | Identificare le risorse | Trova e prepara le risorse e i predefiniti da utilizzare per l’aggiornamento. |
| **Fase 3: ambiente** | Aggiorna [!DNL Adobe Experience Manager] | Tutte le istanze di [!DNL Adobe Experience Manager] devono essere aggiornate alla versione più recente. |
|   | Configura [!DNL Dynamic Media] | Adobe Consulting o il partner configura [!DNL Dynamic Media] con le tue credenziali. |
| **Fase 4: aggiornamento** | Replicare le risorse | Durante il processo di aggiornamento, [!DNL Dynamic Media Classic] risorse designate vengono replicate in Dynamic Media. |
| **Fase 5: installazione amministrativa** | Configurare utenti e autorizzazioni | Creare utenti e concedere le autorizzazioni appropriate. |
|   | Configurare i profili di codifica video | Creare profili di codifica video. |
|   | Impostazioni predefinite visualizzatore | Creare predefiniti visualizzatore. |
|   | Imposta predefiniti immagine | Imposta predefiniti immagine. |
| **Fase 6: convalida** | Convalida | Verifica casi d’uso, risorse, collegamenti e API. |
