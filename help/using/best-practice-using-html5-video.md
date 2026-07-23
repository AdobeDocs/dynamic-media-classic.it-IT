---
title: Procedure consigliate per l'utilizzo del visualizzatore video di HTML5
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
autotag-review: '2026-05-13T17:39:23.475Z'
TQID: 'https://experienceleague.adobe.com/wGnoHGEOQLVV-rnoKBOE8wzphK3VaM-vr9YB1Y-gT8c'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 5fdabd28c4d0defdf9f145b581c89640cc1f6118
workflow-type: tm+mt
source-wordcount: 482
ht-degree: 1%

---

# Best practice per l’utilizzo del visualizzatore video HTML5{#best-practice-using-the-html-video-viewer}

I predefiniti per visualizzatori video Adobe Dynamic Media Classic HTML5 sono lettori video ad alte prestazioni. Per la progettazione del lettore, puoi creare l’intera funzionalità del lettore video utilizzando gli strumenti di sviluppo web standard. Per personalizzare l&#39;aspetto, è possibile progettare pulsanti, controlli e un&#39;immagine poster personalizzata utilizzando HTML5 e CSS.

Per la riproduzione del visualizzatore, rileva automaticamente la funzionalità video del browser. Distribuisce quindi il video utilizzando HLS (HTTP Live Streaming), noto anche come streaming video adattivo. Oppure, se tale metodo di distribuzione non è presente, viene utilizzato HTML5 progressive.

Combinando le seguenti funzionalità in un singolo lettore:

* Componenti di riproduzione progettati con HTML5 e CSS.
* Riproduzione incorporata.
* Utilizzo di streaming adattivo e progressivo in base alle funzionalità del browser.

Aumentate la disponibilità dei contenuti rich media per gli utenti desktop e mobili. Puoi anche garantire un’esperienza video semplificata.

Vedi anche [Informazioni sui visualizzatori HTML5](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) nella Guida di riferimento dei visualizzatori Adobe.

Vedere anche [Predefiniti visualizzatore](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) video di formazione.

## Riproduzione di video su computer desktop e dispositivi mobili tramite il Visualizzatore video di Adobe Dynamic Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Per lo streaming video adattivo per desktop e dispositivi mobili, i video utilizzati per il passaggio a bit rate si basano su tutti i video MP4 nel set di video adattivi.

La riproduzione video viene eseguita mediante HLS o video progressivo. HLS (HTTP Live Streaming) è uno standard Apple per lo streaming video adattivo che regola automaticamente la riproduzione in base alla capacità della larghezza di banda della rete. Consente inoltre agli utenti di spostarsi in qualsiasi punto del video senza dover attendere il download del resto del video. Vedi anche [HTTP Live Streaming](https://developer.apple.com/streaming/). Il sistema offre video progressivo scaricandolo e memorizzandolo localmente sullo schermo del desktop o sul dispositivo mobile di un utente.

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
