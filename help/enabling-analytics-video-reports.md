---
title: Abilitare i rapporti video su Adobe Analytics
description: Scopri come abilitare i rapporti video di Adobe Analytics in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 12%

---

# Abilitare i rapporti video su Adobe Analytics{#enabling-adobe-analytics-video-reports}

Utilizzando il reporting video basato su heartbeat di Adobe Analytics, non è più necessario abilitare i quattro eventi del visualizzatore video (Play, Pause, Stop, Milestone) durante la configurazione di Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video e file multimediali diversi Adobe Dynamic Media Classic HTML5 integrati. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports.

* Per un&#39;introduzione allo streaming media e alla &quot;misurazione heartbeat&quot;, vedi [Informazioni su Adobe Analytics per i file multimediali in streaming](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* L’integrazione dei rapporti video di Adobe Analytics con Adobe Dynamic Media Classic supporta le variabili della soluzione, ma non le variabili personalizzate.

   Vedi [Parametri audio e video](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) per ulteriori informazioni sulle variabili della soluzione e sulle variabili personalizzate.

* Sono supportati i segmenti preconfigurati di incrementi di un minuto. Non è invece supportata la generazione di rapporti per segmenti personalizzati, ad esempio pietre miliari definite dall’utente basate su incrementi temporali, percentuali o scostamento.

   Per ulteriori informazioni sui requisiti e sulla configurazione dei contenuti multimediali in streaming, consulta [Misurare i file multimediali in streaming in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Per informazioni sulle variabili personalizzate e della soluzione consulta [Abilitazione dei report multimediali](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Se la soluzione con licenza di Adobe Analytics non include Video Heartbeat, devi continuare a utilizzare i passaggi descritti in questo capitolo per assegnare le variabili Adobe Analytics agli eventi e alle variabili del visualizzatore Adobe Dynamic Media Classic.
