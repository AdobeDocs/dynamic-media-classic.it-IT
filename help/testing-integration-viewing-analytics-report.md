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
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 15%

---

# Verificare l’integrazione visualizzando un rapporto di Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Dopo aver creato le variabili necessarie in Adobe Analytics, averle collegate agli eventi Adobe Dynamic Media Classic e aver completato i passaggi di implementazione necessari, puoi testare la configurazione. Potete verificare che i dati vengano acquisiti in Adobe Analytics stesso. Se la configurazione funziona, non sono necessari ulteriori interventi. Supponendo di aver seguito i passaggi precedenti e collegato i dati dell’evento Adobe Dynamic Media Classic a una o più variabili di traffico personalizzate, segui questo flusso di lavoro per testare i dati all’interno di Adobe Analytics.

**Per verificare l’integrazione visualizzando un rapporto di Adobe Analytics:**

1. Avvia un visualizzatore Dynamic Media Classic di Adobe dal tuo account, in particolare quello che trasmette la metrica che desideri ottenere, e interagisce con esso per creare alcuni dati dell’evento.

   Ad esempio, se desideri misurare le viste alternative più diffuse in un set di immagini, visualizza in anteprima un set di immagini e fai clic sulle diverse immagini delle miniature.

1. All&#39;interno di Adobe Analytics, vai a **[!UICONTROL Traffico personalizzato]** > **[!UICONTROL Traffico personalizzato 1-10]** > [Nome della proprietà], selezionando il nome della proprietà di traffico dalle scelte del menu.

   Ad esempio, per accedere alla proprietà **[!UICONTROL LoadAsset]** nell’account di esempio, la scelta corretta del menu sarà **[!UICONTROL Traffico personalizzato]** > **[!UICONTROL Traffico personalizzato 1-10]** > **[!UICONTROL LoadAsset]**. Se disponi di più di dieci proprietà personalizzate, vengono visualizzate anche altre opzioni di menu.

1. Visualizzate il grafico generato da Adobe Analytics. Questo grafico è in genere solo il dato di una singola metrica. Se desideri anche sapere con quale risorsa sono associati questi dati, ottieni i dati della risorsa di questo evento. Ad esempio, spesso è utile sapere quale video viene guardato solo al 50% o quale immagine in un set è popolare.

>[!NOTE]
>
>Tutti i dati del visualizzatore Dynamic Media Classic di Adobe vengono visualizzati e segnalati nei rapporti Traffico personalizzato o Conversione personalizzata di Adobe Analytics.

Per ulteriori informazioni, consulta [Tutorials di Analytics](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html).