---
title: Procedura ottimale per l’utilizzo del visualizzatore video HTML5
description: Scoprite le procedure ottimali per l’utilizzo del visualizzatore video HTML5.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 24%

---


# Procedure ottimali per l’utilizzo del visualizzatore video HTML5{#best-practice-using-the-html-video-viewer}

I predefiniti per visualizzatori video HTML5 di Dynamic Media Classic sono lettori video affidabili. Dal punto di vista della progettazione del lettore, potete creare tutte le funzionalità del lettore video utilizzando gli strumenti di sviluppo Web standard. Ad esempio, potete offrire ai vostri clienti un’esperienza personalizzata creando pulsanti, controlli e sfondo personalizzato con immagine poster tramite HTML5 e CSS.

Dal punto di vista della riproduzione, il visualizzatore rileva automaticamente le capacità video del browser in uso. Quindi trasmette il video usando HLS (streaming video adattivo). Oppure, se tale metodo di consegna non è presente, viene utilizzato lo progressivo HTML5.

Combinando in un singolo lettore la possibilità di progettare i componenti di riproduzione in HTML5 e CSS, di usufruire di riproduzione incorporata e di utilizzare lo streaming adattativo e progressivo a seconda delle caratteristiche del browser, i vostri contenuti multimediali potranno essere visti sia dagli utenti con computer desktop che da quelli con dispositivi mobili. Potrete così offrire ai visitatori un’esperienza di streaming video ottimizzata.

Consultate anche [I visualizzatori HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) nella guida di riferimento dei visualizzatori di Adobi .

## Riproduzione di video su computer desktop e dispositivi mobili mediante Dynamic Media Classic Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Per lo streaming di video adattivi per desktop e dispositivi mobili, i video utilizzati per il cambio di bitrate si basano su tutti i video MP4 presenti nel set video adattivo.

La riproduzione video si verifica utilizzando HLS o video progressivo. HLS (HTTP Live Streaming) è uno standard Apple per lo streaming di video adattivi che regola automaticamente la riproduzione in base alla capacità di larghezza di banda della rete. Consente inoltre al cliente di &quot;cercare&quot; in qualsiasi punto del video senza dover attendere il resto del video per scaricarlo. Vedere anche [HTTP Live Streaming](https://developer.apple.com/streaming/). Il video progressivo viene distribuito scaricando e memorizzando localmente il video sullo schermo desktop o sul dispositivo mobile di un utente.

La tabella seguente riassume il dispositivo, il browser e il metodo di riproduzione dei video su computer desktop e dispositivi mobili che utilizzano Dynamic Media Classic Video Viewer.

| Dispositivo | Browser | Modalità di riproduzione video |
|--- |--- |--- |
| Desktop | Internet Explorer 9 e 10 | Download progressivo. |
| Desktop | Internet Explorer 11+ | Streaming video HLS. |
| Desktop | Firefox 23-44 | Download progressivo. |
| Desktop | Firefox 45 o versione successiva | Streaming video HLS. |
| Desktop | Effetto cromatura | Streaming video HLS. |
| Desktop | Safari (Mac) | Streaming video HLS. |
| Cellulare | Chrome (Android 6 o versione precedente) | Download progressivo. |
| Cellulare | Chrome (Android 7 o successivo) | Streaming video HLS. |
| Cellulare | Android (browser predefinito) | Download progressivo. |
| Cellulare | Safari (iOS) | Streaming video HLS. |
| Cellulare | Chrome (iOS) | Streaming video HLS. |
| Cellulare | Blackberry | Streaming video HLS. |
