---
title: Abilita rapporti video di Adobe Analytics
description: Scopri come abilitare i rapporti video di Adobe Analytics in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Abilita rapporti video di Adobe Analytics{#enabling-adobe-analytics-video-reports}

Utilizzando il reporting video basato su heartbeat in Adobe Analytics, non è più necessario abilitare i quattro eventi visualizzatore video (Riproduci, Pausa, Interrompi, Milestone) quando si configura Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con visualizzatori Adobe Dynamic Media Classic HTML5 Video e Multimediali misti pronti all’uso. Il lettore video genera i dati di tracciamento per la visualizzazione nei rapporti video di Adobe Analytics.

* Per un&#39;introduzione allo streaming di file multimediali e alla misurazione heartbeat, vedere [Informazioni su 适用于流媒体的 Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* L’integrazione dei rapporti video di Adobe Analytics con Adobe Dynamic Media Classic supporta le variabili della soluzione, ma non le variabili personalizzate.

  Per ulteriori informazioni sulle variabili di soluzione e le variabili personalizzate, vedere [Parametri audio e video](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters).

* Sono supportati segmenti predefiniti di incrementi di un minuto. Tuttavia, non è supportato il reporting dei segmenti personalizzato, ad esempio i milestone definiti dal cliente in base a incrementi di tempo, milestone di percentuale o milestone di offset.

  Per ulteriori informazioni sui requisiti e la configurazione dei contenuti multimediali in streaming, consulta [Misurare i contenuti multimediali in streaming in Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Per informazioni sulle variabili personalizzate e di soluzione, vedere [Abilitazione di report multimediali](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Se la soluzione con licenza di Adobe Analytics non include Video Heartbeat, continua a utilizzare i passaggi descritti in questo capitolo per assegnare le variabili di Adobe Analytics agli eventi e alle variabili del visualizzatore Adobe Dynamic Media Classic.
