---
title: Strumento per un visualizzatore che utilizza Adobe Analytics Instrumentation Kit
description: Scopri come dotare un visualizzatore di strumenti utilizzando Adobe Analytics Instrumentation Kit in Adobe Dynamic Media Classic.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 20%

---

# Strumento per un visualizzatore che utilizza Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Puoi usare Adobe Analytics Instrumentation Kit per integrare un visualizzatore HTML5 con Adobe Analytics.

Se utilizzi uno dei predefiniti visualizzatore HTML5 per Adobe Classic, questi contengono già tutto il codice di implementazione per inviare dati ad Adobe Analytics; non è richiesta alcuna ulteriore strumentazione da parte dell&#39;utente.

## Configurare il tracciamento di Adobe Analytics da Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Per tutti i visualizzatori HTML5, aggiungi il seguente JavaScript al contenitore HTML, in genere nell&#39;elemento &lt;head> :

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Dove `Adobe Dynamic Media Classic Company ID` è impostato sul nome della società Dynamic Media Classic di Adobe. E `&preset` è facoltativo a meno che il nome del predefinito aziendale non sia `companypreset`. In questi casi, potrebbe essere `companypreset-1, companypreset-2` e così via. Le istanze più recenti del predefinito hanno un numero maggiore. Per determinare il nome corretto del valore predefinito della società, seleziona **[!UICONTROL Copia URL]** , quindi osserva il parametro `preset=`per trovare il nome predefinito della società.

Continua, aggiungi ora una funzione che trasmette l’evento del visualizzatore al codice di tracciamento di Adobe Analytics.

Aggiungi la funzione `s7ComponentEvent()` al contenitore HTML (o JSP, o ASPX o altro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Il nome della funzione distingue tra maiuscole e minuscole. L&#39;unico parametro passato a `s7componentEvent`richiesto è l&#39;ultimo: `eventData`. Dove `s7track()` è definito in s_code.jsp incluso in precedenza. E `s7track` gestisce tutto il tracciamento per ogni evento. Per personalizzare ulteriormente i dati trasmessi ad Adobe Analytics, occorre farlo qui.

## Attiva eventi HREF e ITEM {#enabling-href-and-item-events}

È possibile attivare gli eventi HREF (rollover) e ITEM (clic del mouse/tocco) nei visualizzatori attraverso la modifica delle mappe immagini. Definite gli identificatori per HREF e ITEM nella mappa immagine associata al contenuto del visualizzatore. Aggiungere un parametro `&rolloverKey=` al valore HREF nella mappa immagine.
