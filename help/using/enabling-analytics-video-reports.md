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
source-git-commit: 1b90beb99b161b76da81403f5aed9755b3a92c8b
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 5%

---

# Abilita rapporti video di Adobe Analytics{#enabling-adobe-analytics-video-reports}

Utilizzando il reporting video basato su heartbeat in Adobe Analytics, non è più necessario abilitare i quattro eventi visualizzatore video (Riproduci, Pausa, Interrompi, Milestone) quando si configura Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con visualizzatori Adobe Dynamic Media Classic HTML5 Video e Multimediali misti pronti all’uso. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports.

* Per un’introduzione allo streaming multimediale e alla &quot;misurazione heartbeat&quot;, consulta [Informazioni su 适用于流媒体的 Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* L’integrazione dei rapporti video di Adobe Analytics con Adobe Dynamic Media Classic supporta le variabili della soluzione, ma non le variabili personalizzate.

  Consulta [Parametri audio e video](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/variables/audio-video-parameters.html) per ulteriori informazioni sulle variabili di soluzione e le variabili personalizzate.

* Sono supportati segmenti predefiniti di incrementi di un minuto. Tuttavia, non è supportato il reporting dei segmenti personalizzato, ad esempio i milestone definiti dal cliente in base a incrementi di tempo, milestone di percentuale o milestone di offset.

  Per ulteriori informazioni sui requisiti e la configurazione dei contenuti multimediali in streaming, consulta [Misurare i contenuti multimediali in streaming in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Per informazioni sulle variabili personalizzate e di soluzione consulta [Abilitazione di rapporti sui contenuti multimediali](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Se la soluzione con licenza di Adobe Analytics non include Video Heartbeat, devi continuare a utilizzare i passaggi descritti in questo capitolo per assegnare variabili Adobe Analytics a eventi e variabili visualizzatore Adobe Dynamic Media Classic.
