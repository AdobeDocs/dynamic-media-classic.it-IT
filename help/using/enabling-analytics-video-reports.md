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
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 12%

---

# Abilita rapporti video di Adobe Analytics{#enabling-adobe-analytics-video-reports}

Utilizzando il reporting video basato su heartbeat in Adobe Analytics, non è più necessario abilitare i quattro eventi visualizzatore video (Riproduci, Pausa, Interrompi, Milestone) quando si configura Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con visualizzatori Adobe Dynamic Media Classic HTML5 Video e Multimediali misti pronti all’uso. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports.

* Per un’introduzione allo streaming multimediale e alla &quot;misurazione heartbeat&quot;, consulta [Informazioni su Adobe Analytics per contenuti in streaming](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* L’integrazione dei rapporti video di Adobe Analytics con Adobe Dynamic Media Classic supporta le variabili della soluzione, ma non le variabili personalizzate.

   Consulta [Parametri audio e video](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) per ulteriori informazioni sulle variabili di soluzione e le variabili personalizzate.

* Sono supportati segmenti predefiniti di incrementi di un minuto. Non è invece supportata la generazione di rapporti per segmenti personalizzati, ad esempio pietre miliari definite dall’utente basate su incrementi temporali, percentuali o scostamento.

   Per ulteriori informazioni sui requisiti e la configurazione dei contenuti multimediali in streaming, consulta [Misurare i contenuti multimediali in streaming in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Per informazioni sulle variabili personalizzate e di soluzione consulta [Abilitazione di rapporti sui contenuti multimediali](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Se la soluzione con licenza di Adobe Analytics non include Video Heartbeat, devi continuare a utilizzare i passaggi descritti in questo capitolo per assegnare variabili Adobe Analytics a eventi e variabili visualizzatore Adobe Dynamic Media Classic.
