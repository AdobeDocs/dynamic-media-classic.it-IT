---
title: Abilitazione di Adobe Analytics Video Report.
seo-title: Abilitazione di Adobe Analytics Video Report.
description: 'null'
seo-description: Scoprite come abilitare i rapporti video di Adobe  Analytics.
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 25%

---


# Abilitazione di Adobe Analytics Video Report.{#enabling-adobe-analytics-video-reports}

Utilizzando la generazione di rapporti sui video basati su heartbeat di Adobe  Analytics, non è più necessario abilitare i quattro eventi dei visualizzatori video (Riproduci, Pausa, Interrompi, Pietra miliare) quando si configura Adobe  Analytics in Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video HTML5 e per file multimediali diversi forniti con Dynamic Media Classic. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports.

* L&#39;integrazione di Adobe  Analytics Video Report con Dynamic Media Classic supporta le variabili di soluzione, ma non le variabili personalizzate.

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* Sono supportati i segmenti forniti di incrementi di un minuto. Non è invece supportata la generazione di rapporti per segmenti personalizzati, ad esempio pietre miliari definite dall’utente basate su incrementi temporali, percentuali o scostamento.

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Se la soluzione con licenza di Adobe  Analytics non include Video Heartbeat, dovrete continuare a utilizzare i passaggi descritti in questo capitolo per assegnare le variabili Adobe  Analytics agli eventi e alle variabili del visualizzatore Dynamic Media Classic.

