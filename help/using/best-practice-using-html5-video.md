---
title: Procedure consigliate per l’utilizzo del visualizzatore video di HTML5
description: Scopri le best practice per l’utilizzo del visualizzatore video di HTML5.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 7%

---

# Best practice per l’utilizzo del visualizzatore video di HTML5{#best-practice-using-the-html-video-viewer}

I predefiniti per visualizzatore video di Adobe Dynamic Media Classic HTML5 sono lettori video affidabili. Dal lato della progettazione del lettore, puoi creare l’intera funzionalità del lettore video utilizzando gli strumenti di sviluppo web standard. Ad esempio, potete offrire ai vostri clienti un’esperienza personalizzata creando pulsanti, controlli e sfondo personalizzato con immagine poster tramite HTML5 e CSS.

Sul lato di riproduzione del visualizzatore, rileva automaticamente la funzionalità video del browser. Distribuisce quindi il video utilizzando HLS (HTTP Live Streaming), noto anche come streaming video adattivo. Oppure, se tale metodo di consegna non è presente, allora viene utilizzato HTML5 progressive.

Combinando in un singolo giocatore le seguenti abilità:

* Componenti di riproduzione progettati con HTML5 e CSS
* Riproduzione incorporata
* Uso dello streaming adattivo e progressivo in base alla funzionalità del browser

È possibile estendere la portata dei contenuti rich media agli utenti desktop e mobili. Puoi anche garantire un’esperienza video semplificata.

Vedi anche [Informazioni sui visualizzatori HTML5](https://experienceleague.adobe.com/it/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) nella Guida di riferimento dei visualizzatori Adobe.

Vedere anche [Predefiniti visualizzatore](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) video di formazione.

## Riproduzione di video su computer desktop e dispositivi mobili tramite il Visualizzatore video di Adobe Dynamic Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Per lo streaming video adattivo per desktop e dispositivi mobili, i video utilizzati per il passaggio a bit rate si basano su tutti i video MP4 nel set di video adattivi.

La riproduzione del video avviene tramite HLS o video progressivo. HLS (HTTP Live Streaming) è uno standard Apple per lo streaming video adattivo che regola automaticamente la riproduzione in base alla capacità della larghezza di banda della rete. Consente inoltre al cliente di &quot;cercare&quot; in qualsiasi punto del video senza dover attendere il download del resto del video. Vedi anche [HTTP Live Streaming](https://developer.apple.com/streaming/). Il video progressivo viene distribuito scaricando e memorizzando il video localmente sullo schermo del desktop o sul dispositivo mobile di un utente.

La tabella seguente descrive il dispositivo, il browser e il metodo di riproduzione dei video su computer desktop e dispositivi mobili che utilizzano il Visualizzatore video di Adobe Dynamic Media Classic.

| Dispositivo | Browser | Modalità di riproduzione video |
|--- |--- |--- |
| Desktop | Internet Explorer 9 e 10 | Download progressivo. |
| Desktop | Internet Explorer 11+ | Streaming video HLS. |
| Desktop | Firefox 23-44 | Download progressivo. |
| Desktop | Firefox 45 o versione successiva | Streaming video HLS. |
| Desktop | Chrome | Streaming video HLS. |
| Desktop | Safari (Mac) | Streaming video HLS. |
| Dispositivi mobili | Chrome (Android™ 6 o versioni precedenti) | Download progressivo. |
| Dispositivi mobili | Chrome (Android™ 7 o versione successiva) | Streaming video HLS. |
| Dispositivi mobili | Android™ (browser predefinito) | Download progressivo. |
| Dispositivi mobili | Safari (iOS) | Streaming video HLS. |
| Dispositivi mobili | Chrome (iOS) | Streaming video HLS. |
| Dispositivi mobili | Blackberry® | Streaming video HLS. |
