---
title: Strumentazione di un visualizzatore mediante Adobe Analytics Instrumentation Kit
description: Scopri come dotare un visualizzatore di strumenti utilizzando Adobe Analytics Instrumentation Kit in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:51:34.654Z'
TQID: 'https://experienceleague.adobe.com/veMzN35J6flKfCAFvdPfZPgxJ9oGy0LYYGhjr-hZLcY'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 307
ht-degree: 14%

---

# Strumentazione di un visualizzatore mediante Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

È possibile utilizzare Adobe Analytics Instrumentation Kit per integrare un visualizzatore HTML5 con Adobe Analytics.

Se utilizzi uno dei predefiniti visualizzatore Adobe Dynamic Media Classic HTML5, questo contiene già tutto il codice di implementazione per inviare dati ad Adobe Analytics. Non è necessario aggiungere altri strumenti.

## Configurare il tracciamento di Adobe Analytics da Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Per tutti i visualizzatori HTML5, aggiungi il seguente JavaScript al contenitore HTML, in genere nell’elemento &lt;head>:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Dove `Adobe Dynamic Media Classic Company ID` è impostato sul nome della società Adobe Dynamic Media Classic. E `&preset` è facoltativo. Se il nome del predefinito della società non è `companypreset`, non è facoltativo. In questi casi, potrebbe essere `companypreset-1, companypreset-2` e così via. Le istanze più recenti del predefinito hanno un numero maggiore. Per determinare il nome del valore predefinito della società corretto, selezionare **[!UICONTROL Copia URL]**, quindi controllare il parametro `preset=`per trovare il nome del predefinito della società.

Continuando, ora aggiungi una funzione che trasmette l’evento visualizzatore al codice di tracciamento di Adobe Analytics.

Aggiungi la funzione `s7ComponentEvent()` al HTML contenitore (o JSP, o ASPX o altro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Il nome della funzione distingue tra maiuscole e minuscole. L&#39;unico parametro obbligatorio passato a `s7componentEvent` è l&#39;ultimo: `eventData`. Dove `s7track()` è definito in s_code.jsp incluso in precedenza. E `s7track` gestisce tutto il tracciamento per ogni evento. In quest’area puoi personalizzare ulteriormente i dati trasmessi ad Adobe Analytics.

## Attiva eventi HREF ed ITEM {#enabling-href-and-item-events}

È possibile attivare gli eventi HREF (rollover) e ITEM (clic del mouse/tocco) nei visualizzatori attraverso la modifica delle mappe immagini. Definite gli identificatori per HREF e ITEM nella mappa immagine associata al contenuto del visualizzatore. Aggiungi un parametro `&rolloverKey=` al valore HREF nella mappa immagine.
