---
title: Abilitazione di Adobe Analytics Video Report.
description: Scoprite come abilitare  rapporti video Adobe Analytics.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 20%

---


# Abilitazione di Adobe Analytics Video Report.{#enabling-adobe-analytics-video-reports}

Utilizzando  reportistica video basata su heartbeat Adobe Analytics, non è più necessario abilitare i quattro eventi del visualizzatore video (Riproduci, Pausa, Interrompi, Pietra miliare) quando si configura  Adobe Analytics in Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video HTML5 e per file multimediali diversi forniti con Dynamic Media Classic. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports.

* Per un&#39;introduzione allo streaming multimediale e alla &quot;misurazione heartbeat&quot;, vedere [Informazioni  Adobe Analytics per lo streaming di file multimediali](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* L&#39;integrazione di  rapporti video Adobe Analytics con Dynamic Media Classic supporta le variabili di soluzione, ma non le variabili personalizzate.

   Per ulteriori informazioni sulle variabili della soluzione e personalizzate, consultate [Parametri audio e video](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata).

* Sono supportati i segmenti forniti di incrementi di un minuto. Non è invece supportata la generazione di rapporti per segmenti personalizzati, ad esempio pietre miliari definite dall’utente basate su incrementi temporali, percentuali o scostamento.

   Per ulteriori informazioni sui requisiti e sulla configurazione dei supporti di streaming, vedere [Misurazione dei supporti di streaming in  Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Per informazioni sulle variabili personalizzate e della soluzione, consultate [Abilitazione dei report multimediali](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Se la soluzione con licenza di  Adobe Analytics non include Video Heartbeat, dovrete continuare a utilizzare i passaggi descritti in questo capitolo per assegnare  variabili Adobe Analytics agli eventi e alle variabili del visualizzatore Dynamic Media Classic.

