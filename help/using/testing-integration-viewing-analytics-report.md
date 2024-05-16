---
title: Testare l’integrazione visualizzando un rapporto di Adobe Analytics
description: Scopri come testare l’integrazione in Adobe Dynamic Media Classic visualizzando un rapporto di Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 5%

---

# Testare l’integrazione visualizzando un rapporto di Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Dopo aver creato le variabili necessarie in Adobe Analytics, averle collegate agli eventi Adobe Dynamic Media Classic e completato i passaggi di implementazione necessari, puoi testare la configurazione. Puoi testare e verificare che i dati vengano acquisiti all’interno di Adobe Analytics stessa. Se la configurazione funziona, non sono necessari ulteriori interventi. Supponendo di aver seguito i passaggi precedenti e collegato i dati dell’evento Adobe Dynamic Media Classic a una o più variabili di traffico personalizzate, segui questo flusso di lavoro per verificare i dati in Adobe Analytics.

**Per testare l’integrazione visualizzando un rapporto di Adobe Analytics:**

1. Avvia un visualizzatore Adobe Dynamic Media Classic dal tuo account, in particolare quello che trasmette la metrica che desideri ottenere, e interagisci con esso per creare alcuni dati dell’evento.

   Ad esempio, se desideri misurare le visualizzazioni alternative più comuni in un set di immagini, visualizza l’anteprima di un set di immagini e fai clic sulle diverse immagini delle miniature.

1. All’interno di Adobe Analytics, vai a **[!UICONTROL Traffico personalizzato]** > **[!UICONTROL Traffico personalizzato 1-10]** > [Nome del prop], selezionando il nome della proprietà traffico dalle opzioni di menu.

   Ad esempio, per accedere a **[!UICONTROL LoadAsset]** prop nell’account di esempio, la scelta di menu corretta è **[!UICONTROL Traffico personalizzato]** > **[!UICONTROL Traffico personalizzato 1-10]** > **[!UICONTROL LoadAsset]**. Se disponi di più di dieci proprietà personalizzate, puoi visualizzare anche altre opzioni di menu.

1. Visualizzate il grafico generato da Adobe Analytics. In genere, questo grafico contiene solo i dati di una singola metrica. Se desideri anche sapere a quale risorsa sono associati questi dati, ottieni i dati della risorsa di questo evento. Ad esempio, spesso è utile sapere quale video viene guardato solo al 50% o quale immagine in un set è più popolare.

>[!NOTE]
>
>Tutti i dati dei visualizzatori Adobe Dynamic Media Classic vengono visualizzati e segnalati nei rapporti Traffico personalizzato o Conversione personalizzata di Adobe Analytics.

Per ulteriori informazioni, consulta [Tutorials di Analytics](https://experienceleague.adobe.com/en/docs/analytics-learn/tutorials/overview).