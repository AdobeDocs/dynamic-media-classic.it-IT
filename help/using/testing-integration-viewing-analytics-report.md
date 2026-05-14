---
title: Testare l’integrazione visualizzando un rapporto di Adobe Analytics
description: Scopri come testare l’integrazione in Adobe Dynamic Media Classic visualizzando un rapporto di Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T20:14:40.601Z'
TQID: 'https://experienceleague.adobe.com/BwQe9AuhBfi-bLCuO-j48kE-3gw9rgtz5GEI9nIBRjE'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 345
ht-degree: 5%

---

# Testare l’integrazione visualizzando un rapporto di Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Dopo aver creato le variabili necessarie in Adobe Analytics, averle collegate agli eventi Adobe Dynamic Media Classic e completato i passaggi di implementazione necessari, puoi testare la configurazione. Puoi testare e verificare che i dati vengano acquisiti all’interno di Adobe Analytics stessa. Se la configurazione funziona, non sono necessari ulteriori interventi. Supponendo di aver seguito i passaggi precedenti e collegato i dati dell’evento Adobe Dynamic Media Classic a una o più variabili di traffico personalizzate, segui questo flusso di lavoro per verificare i dati in Adobe Analytics.

**Per testare l&#39;integrazione visualizzando un report di Adobe Analytics:**

1. Avvia un visualizzatore Adobe Dynamic Media Classic dal tuo account, in particolare quello che trasmette la metrica che desideri ottenere, e interagisci con esso per creare alcuni dati dell’evento.

   Ad esempio, se desideri misurare le visualizzazioni alternative più comuni in un set di immagini, visualizza l’anteprima di un set di immagini e fai clic sulle diverse immagini delle miniature.

1. All&#39;interno di Adobe Analytics, vai a **[!UICONTROL Traffico personalizzato]** > **[!UICONTROL Traffico personalizzato 1-10]** > [Nome della proprietà], selezionando il nome della proprietà traffico dalle scelte di menu.

   Ad esempio, per accedere alla proprietà **[!UICONTROL LoadAsset]** nell&#39;account di esempio, la scelta di menu corretta è **[!UICONTROL Traffico personalizzato]** > **[!UICONTROL Traffico personalizzato 1-10]** > **[!UICONTROL LoadAsset]**. Se disponi di più di dieci proprietà personalizzate, puoi visualizzare anche altre opzioni di menu.

1. Visualizzate il grafico generato da Adobe Analytics. In genere, questo grafico contiene solo i dati di una singola metrica. Se desideri anche sapere a quale risorsa sono associati questi dati, ottieni i dati della risorsa di questo evento. Ad esempio, spesso è utile sapere quale video viene guardato solo al 50% o quale immagine in un set è più popolare.

>[!NOTE]
>
>Tutti i dati dei visualizzatori Adobe Dynamic Media Classic vengono visualizzati e segnalati nei rapporti Traffico personalizzato o Conversione personalizzata di Adobe Analytics.

Per ulteriori informazioni, consulta [Tutorial su Analytics](https://experienceleague.adobe.com/en/docs/analytics-learn/tutorials/overview).