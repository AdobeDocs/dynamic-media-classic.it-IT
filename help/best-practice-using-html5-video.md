---
title: '"Procedura ottimale: utilizzo del visualizzatore per video HTML5"'
seo-title: '"Procedura ottimale: utilizzo del visualizzatore per video HTML5"'
description: 'null'
seo-description: Scoprite le best practice per l'utilizzo del visualizzatore video HTML 5.
uuid: 3 c 8924 dc -7 bea -4 c 25-b 77 b -005 f 57 b 71 b 64
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/video
discoiquuid: 4 b 11 cab 7-88 cf -42 dd -8554-2 eea 530753 bb
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Procedura ottimale: utilizzo del visualizzatore per video HTML5{#best-practice-using-the-html-video-viewer}

I predefiniti per visualizzatori video HTML 5 dinamici sono lettori video affidabili. Dal punto di vista della progettazione del lettore, è possibile creare tutte le funzionalità del lettore video utilizzando strumenti standard di sviluppo Web. Ad esempio, potete offrire ai vostri clienti un’esperienza personalizzata creando pulsanti, controlli e sfondo personalizzato con immagine poster tramite HTML5 e CSS.

Dal punto di vista della riproduzione, il visualizzatore rileva automaticamente le capacità video del browser in uso. Quindi trasmette il video tramite HLS (streaming video adattativo). Oppure, se il metodo di consegna non è presente, viene utilizzato lo progressivo HTML 5.

Combinando in un singolo lettore la possibilità di progettare i componenti di riproduzione in HTML5 e CSS, di usufruire di riproduzione incorporata e di utilizzare lo streaming adattativo e progressivo a seconda delle caratteristiche del browser, i vostri contenuti multimediali potranno essere visti sia dagli utenti con computer desktop che da quelli con dispositivi mobili. Potrete così offrire ai visitatori un’esperienza di streaming video ottimizzata.

Consultate anche [I visualizzatori HTML 5](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) nella Guida di riferimento dei visualizzatori Adobe.

## Riproduzione di video su computer desktop e dispositivi mobili mediante il visualizzatore video Dynamic Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Per lo streaming di video adattivi per desktop e dispositivi mobili, i video utilizzati per il cambio di bitrate sono basati su tutti i video MP 4 presenti nel set video adattivo.

La riproduzione video avviene con HLS o video progressivo. HLS (HTTP Live Streaming) è uno standard Apple per lo streaming di video adattivi che regola automaticamente la riproduzione in base alla capacità di larghezza di banda della rete. Inoltre, consente al cliente di effettuare ricerche in qualsiasi punto del video senza dover attendere il download del resto del video (consultate anche [Streaming dinamico HTTP](#UnresolvedLink-https://developer.apple.com/streaming/)). Il video progressivo viene distribuito scaricando e memorizzando il video localmente sullo schermo desktop o sul dispositivo mobile di un utente.

La tabella seguente descrive il dispositivo, il browser e il metodo di riproduzione dei video su computer desktop e dispositivi mobili mediante il visualizzatore video Dynamic Media Classic.

| Dispositivo | Browser | Modalità di riproduzione video |
|--- |--- |--- |
| Desktop | Internet Explorer 9 e 10 | Download progressivo. |
| Desktop | Internet Explorer 11 + | Streaming di video HLS. |
| Desktop | Firefox 23-44 | Download progressivo. |
| Desktop | Firefox 45 o versione successiva | Streaming di video HLS. |
| Desktop | Chrome | Streaming di video HLS. |
| Desktop | Safari (Mac) | Streaming di video HLS. |
| Cellulare | Chrome (Android 6 o versioni precedenti) | Download progressivo. |
| Cellulare | Chrome (Android 7 o versione successiva) | Streaming di video HLS. |
| Cellulare | Android (browser predefinito) | Download progressivo. |
| Cellulare | Safari (iOS) | Streaming di video HLS. |
| Cellulare | Chrome (iOS) | Streaming di video HLS. |
| Cellulare | Blackberry | Streaming di video HLS. |
