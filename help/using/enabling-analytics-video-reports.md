---
title: Abilita rapporti video di Adobe Analytics
description: Scopri come abilitare i rapporti video di Adobe Analytics in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
autotag-review: '2026-05-13T19:47:00.853Z'
TQID: 'https://experienceleague.adobe.com/bXlrGU0zMEyfa-E-x-29-biChC17GJTEViBP8GoouTU'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 0%

---

# Abilita rapporti video di Adobe Analytics{#enabling-adobe-analytics-video-reports}

Utilizzando il reporting video basato su heartbeat in Adobe Analytics, non è più necessario abilitare i quattro eventi visualizzatore video (Riproduci, Pausa, Interrompi, Milestone) quando si configura Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con visualizzatori Adobe Dynamic Media Classic HTML5 Video e Multimediali misti pronti all’uso. Il lettore video genera i dati di tracciamento per la visualizzazione nei rapporti video di Adobe Analytics.

* Per un&#39;introduzione allo streaming di file multimediali e alla misurazione heartbeat, vedere [Informazioni su Adobe Analytics for Streaming Media](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* L’integrazione dei rapporti video di Adobe Analytics con Adobe Dynamic Media Classic supporta le variabili della soluzione, ma non le variabili personalizzate.

  Per ulteriori informazioni sulle variabili di soluzione e le variabili personalizzate, vedere [Parametri audio e video](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters).

* Sono supportati segmenti predefiniti di incrementi di un minuto. Tuttavia, non è supportato il reporting dei segmenti personalizzato, ad esempio i milestone definiti dal cliente in base a incrementi di tempo, milestone di percentuale o milestone di offset.

  Per ulteriori informazioni sui requisiti e la configurazione dei contenuti multimediali in streaming, consulta [Misurare i contenuti multimediali in streaming in Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Per informazioni sulle variabili personalizzate e di soluzione, vedere [Abilitazione di report multimediali](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Se la soluzione con licenza di Adobe Analytics non include Video Heartbeat, continua a utilizzare i passaggi descritti in questo capitolo per assegnare le variabili di Adobe Analytics agli eventi e alle variabili del visualizzatore Adobe Dynamic Media Classic.
