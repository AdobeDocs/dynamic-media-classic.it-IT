---
title: Verificare l’integrazione visualizzando un rapporto di Adobe Analytics
seo-title: Verificare l’integrazione visualizzando un rapporto di Adobe Analytics
description: 'null'
seo-description: Come verificare l'integrazione visualizzando un rapporto di Adobe Analytics.
uuid: 937375 e 0-6 dea -4 baa-a 2 b 0-4 f 3 e 461 c 9 ee 2
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: 1 ddc 89 ff-d 2 e 9-42 eb-a 442-aa 6 b 9871 c 991
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Verificare l’integrazione visualizzando un rapporto di Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Dopo aver creato le variabili necessarie in Adobe Analytics, averle collegate agli eventi Dynamic Media Classic e aver completato i passaggi di implementazione necessari, è necessario verificare l'impostazione. Potete verificare che i dati vengano acquisiti in Adobe Analytics stesso. Se la configurazione funziona, non sono necessari ulteriori interventi. Se hai seguito i passaggi descritti qui sopra e collegato i dati dell'evento Dynamic Media Classic a una o più variabili di traffico personalizzate, segui questo flusso di lavoro per testare i dati in Adobe Analytics.

**Per verificare l’integrazione con visualizzando un rapporto di Adobe Analytics**

1. Avviate un visualizzatore Dynamic Media Classic dal vostro account, in particolare uno che trasmette la metrica che desiderate acquisire e interagite con esso per creare alcuni dati evento.

   Ad esempio, se desiderate misurare le visualizzazioni alternative di maggior successo in un set di immagini, visualizzate un’anteprima del set di immagini e fate clic sulle varie miniature.

1. Inside Adobe Analytics, go to Custom Traffic &gt; Custom Traffic 1-10 &gt; [Name of prop], selecting your traffic prop name from the menu choices.

   Ad esempio, per accedere a LoadAsset nell’account di esempio, scegliete Custom Traffic &gt; Custom Traffic 1-10 &gt; LoadAsset. Se sono presenti più di 10 proprietà personalizzate, saranno visualizzate ulteriori voci di menu.

1. Visualizzate il grafico generato da Adobe Analytics. Tenete presente che si tratterà in genere dei dati di una sola metrica. Se desiderate anche sapere con quale risorsa sono associati questi dati (ad esempio, quale video viene guardato solo a 50% o quale immagine è più popolare), assicuratevi di acquisire anche i dati delle risorse di questo evento.

>[!NOTE]
>
>Tutti i dati del visualizzatore Dynamic Media Classic vengono visualizzati e riportati nei report Traffico personalizzato o nei rapporti Conversione personalizzata di Adobe Analytics.

Per ulteriori informazioni, consultate [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
