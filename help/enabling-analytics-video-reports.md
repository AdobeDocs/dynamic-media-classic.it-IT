---
title: Abilitazione di Adobe Analytics Video Report.
description: Scopri come abilitare i rapporti video di Adobe Analytics.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 17%

---

# Abilitazione di Adobe Analytics Video Report.{#enabling-adobe-analytics-video-reports}

Utilizzando il reporting video basato su heartbeat di Adobe Analytics, non è più necessario abilitare i quattro eventi del visualizzatore video (Play, Pause, Stop, Milestone) durante la configurazione di Adobe Analytics in Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video HTML5 e file multimediali diversi di Dynamic Media Classic integrati. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports.

* Per un&#39;introduzione allo streaming media e alla &quot;misurazione heartbeat&quot;, consulta [Informazioni su Adobe Analytics per lo streaming multimediale](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* L’integrazione dei rapporti video di Adobe Analytics con Dynamic Media Classic supporta le variabili della soluzione, ma non le variabili personalizzate.

   Per ulteriori informazioni sulle variabili della soluzione e le variabili personalizzate, consulta [Parametri audio e video](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) .

* Sono supportati i segmenti preconfigurati di incrementi di un minuto. Non è invece supportata la generazione di rapporti per segmenti personalizzati, ad esempio pietre miliari definite dall’utente basate su incrementi temporali, percentuali o scostamento.

   Per ulteriori informazioni sui requisiti e sulla configurazione dei contenuti multimediali in streaming, consulta [Misurazione dei file multimediali in streaming in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Per informazioni sulle variabili personalizzate e della soluzione, consulta [Abilitazione dei report multimediali](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Se la soluzione con licenza di Adobe Analytics non include Video Heartbeat, devi continuare a utilizzare i passaggi descritti in questo capitolo per assegnare le variabili Adobe Analytics agli eventi e alle variabili del visualizzatore Dynamic Media Classic.
