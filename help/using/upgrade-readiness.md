---
title: Preparazione all’aggiornamento
description: Elenco di controllo per la preparazione all'aggiornamento quando si desidera passare da [!DNL Adobe Dynamic Media Classic] a [!DNL Dynamic Media] il [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---

# Elenco di controllo preparazione all’aggiornamento

Utilizzare il seguente elenco di controllo per comprendere e preparare un aggiornamento da [!DNL Dynamic Media Classic] a [!DNL Dynamic Media].

|  | Attività | Descrizione |
| :--- | :--- | --- |
| **Fase 1: gestione licenze** | Esegui contratto | In base al traffico e all&#39;archiviazione, il team dell&#39;account Adobe collabora con l&#39;utente per passare dalla licenza [!DNL Dynamic Media Classic] al rinnovo della licenza [!DNL Dynamic Media]. |
| **Fase 2: Preparazione** | Convalidare l’utilizzo della funzione | Verificare che le funzionalità utilizzate in [!DNL Dynamic Media Classic] siano disponibili in [!DNL Dynamic Media]. Visita la pagina [Confronto delle funzionalità](/help/using/upgrade-feature-comparison.md). Le funzionalità chiave non ancora disponibili in [!DNL Dynamic Media] includono:<br>· Visual Configurator (Image Author, Image Render).<br>· Modelli immagine (modello 1:1).<br>· eCatalog.<br>Se vengono utilizzate le funzionalità precedenti, l&#39;aggiornamento può comunque verificarsi presupponendo che tali funzionalità siano accessibili tramite [!DNL Dynamic Media Classic]. |
|   | Identificare le risorse | Trova e prepara le risorse e i predefiniti da utilizzare per l’aggiornamento. |
| **Fase 3: ambiente** | Aggiorna [!DNL Adobe Experience Manager] | Tutte le istanze di [!DNL Adobe Experience Manager] devono essere aggiornate alla versione più recente. |
|   | Configura [!DNL Dynamic Media] | Adobe Consulting o il partner configura [!DNL Dynamic Media] con le tue credenziali. |
| **Fase 4: aggiornamento** | Replicare le risorse | Durante il processo di aggiornamento, [!DNL Dynamic Media Classic] risorse designate vengono replicate in Dynamic Medie. |
| **Fase 5: installazione amministrativa** | Configurare utenti e autorizzazioni | Creare utenti e concedere le autorizzazioni appropriate. |
|   | Configurare i profili di codifica video | Creare profili di codifica video. |
|   | Impostazioni predefinite visualizzatore | Creare predefiniti visualizzatore. |
|   | Imposta predefiniti immagine | Imposta predefiniti immagine. |
| **Fase 6: convalida** | Convalida | Verifica casi d’uso, risorse, collegamenti e API. |
