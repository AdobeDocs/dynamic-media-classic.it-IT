---
title: Personalizzazione di un visualizzatore con Adobe Analytics Instrumentation Kit
seo-title: Personalizzazione di un visualizzatore con Adobe Analytics Instrumentation Kit
description: 'null'
seo-description: Scoprite come personalizzare un visualizzatore utilizzando Adobe Analytics Instrumentation Kit.
uuid: cf 9 a 4002-966 d -4641-9 cd 0-2 ee 8 b 5454 f 60
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: a 2824244-1755-42 de-a 167-42 af 117 cf 038
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Personalizzazione di un visualizzatore con Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Potete utilizzare il kit Adobe Analytics Instrumentation Kit per integrare un visualizzatore HTML 5 con Adobe Analytics.

Se utilizzate uno dei predefiniti per visualizzatori HTML 5 di Dynamic Media Classic, tenete presente che contengono già tutto il codice di implementazione necessario per inviare dati ad Adobe Analytics—non è necessario alcun altro intervento.

## Impostazione del tracciamento Adobe Analytics da Scene7 Publishing System {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Per tutti i visualizzatori HTML 5, aggiungete il seguente codice javascript al contenitore HTML, in genere nell'elemento &lt; head &gt;:

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<SPS Company ID>&preset=companypreset-1"></script>
```

`Company` è impostato sul nome della società SPS. `&preset` è facoltativo, a meno che il nome del predefinito della società non sia `companypreset`. In such cases, it could be `companypreset-1, companypreset-2`, and so on. Le istanze più recenti del predefinito hanno un numero maggiore. To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

Quindi potrete aggiungere una funzione che trasmette l’evento visualizzatore al codice di tracciamento di Adobe Analytics.

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Nel nome della funzione viene fatta distinzione tra maiuscole e minuscole. The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` è definito in s_ code. jsp incluso sopra. `s7track` gestisce tutti i tracciamenti per ogni evento. Per personalizzare ulteriormente i dati trasmessi ad Adobe Analytics, occorre farlo qui.

## Attivazione di eventi HREF e ITEM {#enabling-href-and-item-events}

È possibile attivare gli eventi HREF (rollover) e ITEM (clic del mouse/tocco) nei visualizzatori attraverso la modifica delle mappe immagini. Definite gli identificatori per HREF e ITEM nella mappa immagine associata al contenuto del visualizzatore. Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
