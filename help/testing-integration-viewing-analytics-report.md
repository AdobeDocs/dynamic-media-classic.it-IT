---
title: Verificare l’integrazione visualizzando un rapporto di Adobe Analytics
description: Scopri come verificare l’integrazione visualizzando un rapporto di Adobe Analytics.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 39%

---


# Verificare l’integrazione visualizzando un rapporto di Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Dopo aver creato le variabili necessarie in Adobe Analytics, averle collegate agli eventi di Dynamic Media Classic e aver completato i passaggi di implementazione necessari, verifica la configurazione. Potete verificare che i dati vengano acquisiti in Adobe Analytics stesso. Se la configurazione funziona, non sono necessari ulteriori interventi. Supponendo di aver seguito i passaggi precedenti e collegato i dati dell’evento Dynamic Media Classic a una o più variabili di traffico personalizzate, segui questo flusso di lavoro per testare i dati all’interno di Adobe Analytics.

**Per verificare l’integrazione con visualizzando un rapporto di Adobe Analytics**

1. Avvia un visualizzatore Dynamic Media Classic dal tuo account, in particolare quello che trasmette la metrica che desideri acquisire e interagisce con esso per creare alcuni dati dell’evento.

   Ad esempio, se desiderate misurare le visualizzazioni alternative di maggior successo in un set di immagini, visualizzate un’anteprima del set di immagini e fate clic sulle varie miniature.

1. All&#39;interno di Adobe Analytics, passa a Traffico personalizzato > Traffico personalizzato 1-10 > [Nome della proprietà], selezionando il nome della proprietà del traffico dalle scelte del menu.

   Ad esempio, per accedere a LoadAsset nell’account di esempio, scegliete Custom Traffic > Custom Traffic 1-10 > LoadAsset. Se sono presenti più di 10 proprietà personalizzate, saranno visualizzate ulteriori voci di menu.

1. Visualizzate il grafico generato da Adobe Analytics. Tenete presente che si tratterà in genere dei dati di una sola metrica. Se desideri anche sapere con quale risorsa sono associati questi dati (ad esempio, quale video viene guardato solo al 50% o quale immagine in un set è più popolare), assicurati di acquisire anche i dati della risorsa di questo evento.

>[!NOTE]
>
>Tutti i dati del visualizzatore Dynamic Media Classic vengono visualizzati e segnalati nei rapporti Traffico personalizzato o Conversione personalizzata di Adobe Analytics.

Per ulteriori informazioni, consulta [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
