---
title: Verificare l’integrazione visualizzando un rapporto di Adobe Analytics
seo-title: Verificare l’integrazione visualizzando un rapporto di Adobe Analytics
description: 'null'
seo-description: Scoprite come verificare l'integrazione visualizzando un rapporto Adobe Analytics .
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 42%

---


# Verificare l’integrazione visualizzando un rapporto di Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Dopo aver creato le variabili necessarie in  Adobe Analytics, averle collegate agli eventi di Dynamic Media Classic e aver completato i passaggi di implementazione necessari, è necessario verificare la configurazione. Potete verificare che i dati vengano acquisiti in Adobe Analytics stesso. Se la configurazione funziona, non sono necessari ulteriori interventi. Se avete seguito i passaggi descritti qui sopra e collegato i dati dell&#39;evento Dynamic Media Classic a una o più variabili di traffico personalizzate, seguite questo flusso di lavoro per verificare i dati all&#39;interno  Adobe Analytics.

**Per verificare l’integrazione con visualizzando un rapporto di Adobe Analytics**

1. Avviate un visualizzatore Dynamic Media Classic dal vostro account, in particolare uno che trasmette la metrica da acquisire, e interagite con esso per creare alcuni dati dell&#39;evento.

   Ad esempio, se desiderate misurare le visualizzazioni alternative di maggior successo in un set di immagini, visualizzate un’anteprima del set di immagini e fate clic sulle varie miniature.

1. All&#39;interno  Adobe Analytics, passare a Custom Traffic (Traffico personalizzato) > Custom Traffic 1-10 > [Name of prop] (Traffico personalizzato), selezionando il nome proprietà traffico dalle opzioni di menu.

   Ad esempio, per accedere a LoadAsset nell’account di esempio, scegliete Custom Traffic > Custom Traffic 1-10 > LoadAsset. Se sono presenti più di 10 proprietà personalizzate, saranno visualizzate ulteriori voci di menu.

1. Visualizzate il grafico generato da Adobe Analytics. Tenete presente che si tratterà in genere dei dati di una sola metrica. Se desiderate anche sapere con quale risorsa sono associati questi dati (ad esempio, quale video viene guardato solo per il 50% o quale immagine di un set è più popolare), accertatevi di acquisire anche i dati delle risorse di questo evento.

>[!NOTE]
>
>Tutti i dati del visualizzatore Dynamic Media Classic vengono visualizzati e riportati nei rapporti Traffico personalizzato o Conversione personalizzata di  Adobe Analytics.

Per ulteriori informazioni, vedere [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
