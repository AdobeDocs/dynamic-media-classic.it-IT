---
title: Personalizzazione di un visualizzatore con Adobe Analytics Instrumentation Kit
description: Scopri come dotare un visualizzatore utilizzando Adobe Analytics Instrumentation Kit.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 28%

---

# Personalizzazione di un visualizzatore con Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Puoi usare Adobe Analytics Instrumentation Kit per integrare un visualizzatore HTML5 con Adobe Analytics.

Se utilizzi uno dei predefiniti visualizzatore HTML5 di Dynamic Media Classic, questi contengono già tutto il codice di implementazione per inviare dati ad Adobe Analytics; non è richiesta alcuna ulteriore strumentazione da parte dell&#39;utente.

## Configurare il tracciamento Adobe Analytics da Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Per tutti i visualizzatori HTML5, aggiungi il seguente JavaScript™ al contenitore HTML, in genere nell&#39;elemento &lt;head> :

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Dove `Dynamic Media Classic Company ID` è impostato sul nome della società Dynamic Media Classic. E `&preset` è facoltativo a meno che il nome del predefinito aziendale non sia `companypreset`. In questi casi, potrebbe essere `companypreset-1, companypreset-2` e così via. Le istanze più recenti del predefinito hanno un numero maggiore. Per determinare il nome corretto del valore predefinito della società, fai clic su **[!UICONTROL Copia URL]** , quindi osserva il parametro `preset=`per trovare il nome del predefinito della società.

Continua, aggiungi ora una funzione che trasmette l’evento del visualizzatore al codice di tracciamento di Adobe Analytics.

Aggiungi la funzione `s7ComponentEvent()` al contenitore HTML (o JSP, o ASPX o altro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Il nome della funzione distingue tra maiuscole e minuscole. L&#39;unico parametro passato a `s7componentEvent`richiesto è l&#39;ultimo: `eventData`. Dove `s7track()` è definito in s_code.jsp incluso in precedenza. E `s7track` gestisce tutto il tracciamento per ogni evento. Per personalizzare ulteriormente i dati trasmessi ad Adobe Analytics, occorre farlo qui.

## Attivazione di eventi HREF e ITEM {#enabling-href-and-item-events}

È possibile attivare gli eventi HREF (rollover) e ITEM (clic del mouse/tocco) nei visualizzatori attraverso la modifica delle mappe immagini. Definite gli identificatori per HREF e ITEM nella mappa immagine associata al contenuto del visualizzatore. Aggiungere un parametro `&rolloverKey=` al valore HREF nella mappa immagine.
