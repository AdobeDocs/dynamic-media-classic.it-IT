---
title: Abilitazione di Adobe Analytics Video Report.
seo-title: Abilitazione di Adobe Analytics Video Report.
description: 'null'
seo-description: Scopri come abilitare i rapporti video di Adobe Analytics.
uuid: 078594 b 2-7 d 53-4714-8128-ff 3 b 5 c 3 a 5 e 36
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: 18644 a 53-92 da -40 ab-b 961-318 d 8332 c 54 d
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Abilitazione di Adobe Analytics Video Report.{#enabling-adobe-analytics-video-reports}

Utilizzando i rapporti sui video basati su heartbeat Adobe Analytics, non è più necessario abilitare i quattro eventi dei visualizzatori video (Riproduci, Pausa, Interrompi, Pietra miliare) quando si configura Adobe Analytics in Dynamic Media Classic. Heartbeat video funziona con i visualizzatori HTML 5 Video Classic Classic e mixedmedia integrati. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports.

* L'integrazione di Adobe Analytics Video Report con Dynamic Media Classic supporta le variabili della soluzione, ma non le variabili personalizzate.

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* Sono supportati i segmenti forniti di incrementi di un minuto. Non è invece supportata la generazione di rapporti per segmenti personalizzati, ad esempio pietre miliari definite dall’utente basate su incrementi temporali, percentuali o scostamento.

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Se la soluzione con licenza di Adobe Analytics non include Video Heartbeat, dovrete continuare a utilizzare i passaggi descritti in questo capitolo per assegnare variabili Adobe Analytics agli eventi e alle variabili di visualizzatore Dynamic Media Classic.

