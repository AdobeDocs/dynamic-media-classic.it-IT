---
title: Procedure consigliate per l’utilizzo del visualizzatore video HTML5
description: Scopri le best practice per l’utilizzo del visualizzatore video HTML5.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 11%

---

# Best practice per l’utilizzo del visualizzatore video HTML5{#best-practice-using-the-html-video-viewer}

I predefiniti per visualizzatori video Adobe Dynamic Media Classic HTML5 sono lettori video affidabili. Dal lato del design del lettore, puoi creare l’intera funzionalità del lettore video utilizzando gli strumenti di sviluppo web standard. Ad esempio, potete offrire ai vostri clienti un’esperienza personalizzata creando pulsanti, controlli e sfondo personalizzato con immagine poster tramite HTML5 e CSS.

Dal punto di vista della riproduzione, il visualizzatore rileva automaticamente le capacità video del browser in uso. Il video viene quindi trasmesso tramite HLS (HTTP Live Streaming), noto anche come streaming video adattivo. Oppure, se tale metodo di consegna non è presente, viene invece utilizzato HTML5 progressive.

Combinando in un unico lettore le seguenti capacità:

* Componenti di riproduzione progettati con HTML5 e CSS
* Riproduzione incorporata
* Utilizzo dello streaming adattivo e progressivo in base alla capacità del browser

Estendi la portata dei contenuti rich media agli utenti desktop e mobili. Assicurati anche un’esperienza video semplificata.

Consulta anche [Informazioni sui visualizzatori HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) nella Guida di riferimento visualizzatori di Adobi.

Vedere anche video di formazione [Predefiniti visualizzatore](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

## Riproduzione di video su computer desktop e dispositivi mobili utilizzando il visualizzatore video Adobe Dynamic Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Per lo streaming video adattivo per desktop e dispositivi mobili, i video utilizzati per la commutazione del bit rate si basano su tutti i video MP4 nel set video adattivo.

La riproduzione video avviene tramite HLS o video progressivo. HLS (HTTP Live Streaming) è uno standard Apple per lo streaming video adattivo che regola automaticamente la riproduzione in base alla capacità della larghezza di banda della rete. Permette inoltre al cliente di &quot;cercare&quot; in qualsiasi punto del video senza dover attendere che il resto del video venga scaricato. Vedere anche [Streaming live HTTP](https://developer.apple.com/streaming/). Il video progressivo viene distribuito scaricando e memorizzando localmente il video sullo schermo desktop o sul dispositivo mobile di un utente.

La tabella seguente descrive il dispositivo, il browser e il metodo di riproduzione dei video su computer desktop e dispositivi mobili che utilizzano il visualizzatore video Adobe Dynamic Media Classic.

| Dispositivo | Browser | Modalità di riproduzione video |
|--- |--- |--- |
| Desktop | Internet Explorer 9 e 10 | Download progressivo. |
| Desktop | Internet Explorer 11+ | Streaming video HLS. |
| Desktop | Firefox 23-44 | Download progressivo. |
| Desktop | Firefox 45 o versione successiva | Streaming video HLS. |
| Desktop | Chrome | Streaming video HLS. |
| Desktop | Safari (Mac) | Streaming video HLS. |
| Cellulare | Chrome (Android™ 6 o precedente) | Download progressivo. |
| Cellulare | Chrome (Android™ 7 o successivo) | Streaming video HLS. |
| Cellulare | Android™ (browser predefinito) | Download progressivo. |
| Cellulare | Safari (iOS) | Streaming video HLS. |
| Cellulare | Chrome (iOS) | Streaming video HLS. |
| Cellulare | BlackBerry® | Streaming video HLS. |
