---
title: Personalizzazione di un visualizzatore con Adobe Analytics Instrumentation Kit
seo-title: Personalizzazione di un visualizzatore con Adobe Analytics Instrumentation Kit
description: 'null'
seo-description: Scoprite come misurare un visualizzatore con il kit di strumenti Adobe Analytics .
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 41%

---


# Personalizzazione di un visualizzatore con Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Potete usare  Adobe Analytics Instrumentation Kit per integrare un visualizzatore HTML5 con  Adobe Analytics.

Se usate uno dei predefiniti per visualizzatori HTML5 per Dynamic Media Classic, tenete presente che contengono già tutto il codice di implementazione necessario per inviare i dati ad  Adobe Analytics e che non è necessario alcun altro intervento.

## Impostazione  tracciamento Adobe Analytics da Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Per tutti i visualizzatori HTML5, aggiungete il seguente codice JavaScript al contenitore HTML, in genere nell’elemento &lt;head>:

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Company` è impostato sul nome della società Dynamic Media Classic. `&preset` è facoltativo, a meno che il nome del predefinito della società non sia `companypreset`. In such cases, it could be `companypreset-1, companypreset-2`, and so on. Le istanze più recenti del predefinito hanno un numero maggiore. To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

Quindi potrete aggiungere una funzione che trasmette l’evento visualizzatore al codice di tracciamento di Adobe Analytics.

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Nel nome della funzione viene fatta distinzione tra maiuscole e minuscole. The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` è definito in s_code.jsp incluso in precedenza. `s7track` gestisce tutto il tracciamento per ogni evento. Per personalizzare ulteriormente i dati trasmessi ad Adobe Analytics, occorre farlo qui.

## Attivazione di eventi HREF e ITEM {#enabling-href-and-item-events}

È possibile attivare gli eventi HREF (rollover) e ITEM (clic del mouse/tocco) nei visualizzatori attraverso la modifica delle mappe immagini. Definite gli identificatori per HREF e ITEM nella mappa immagine associata al contenuto del visualizzatore. Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
