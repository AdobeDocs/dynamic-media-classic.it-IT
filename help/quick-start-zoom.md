---
title: '"Avvio rapido: zoom"'
description: Introduzione e Avvio rapido per lo zoom per aiutarti a iniziare e a usare rapidamente.
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
feature: Dynamic Media Classic,Visualizzatori,Zoom
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 41%

---

# Avvio rapido: zoom{#quick-start-zoom}

Lo zoom consente di visualizzare in modo interattivo i dettagli ad alta risoluzione nelle immagini. Potete ad esempio visualizzare i colori, le opzioni, le angolazioni e i dettagli di un’immagine in un visualizzatore integrato dinamico e completamente configurabile. Questo visualizzatore può essere incorporato in una pagina Web o visualizzato in una finestra a comparsa. È possibile controllare le immagini a una vasta gamma di livelli e le immagini panoramiche ad alta risoluzione per esaminarle attentamente. Lo zoom offre ai clienti un’esperienza interattiva, accattivante e informativa.

Dynamic Media Classic offre anche lo zoom guidato, un modo per evidenziare le funzioni importanti di un’immagine. Ad esempio, per richiamare l’attenzione degli utenti su un logo, potete creare una destinazione di zoom per il logo. Quando gli utenti fanno clic su questa destinazione di zoom, applicano lo zoom al logo. 

Tutte le immagini di zoom vengono create e servite da singoli elementi grafici, immagini e attributi basati su database principali. Lo zoom di Dynamic Media Classic riduce notevolmente i tempi e i costi di produzione e distribuzione delle immagini. È possibile utilizzare i visualizzatori zoom per ingrandire e ridurre le immagini. Il visualizzatore zoom include pulsanti su cui potete fare clic per applicare lo zoom e scorrere l’immagine (panning). Per scorrere l’immagine potete anche trascinare sullo schermo. Usando i predefiniti del visualizzatore zoom, potete configurare il visualizzatore zoom usato per applicare lo zoom alle immagini.

Questa Avvio rapido dello zoom è progettata per iniziare a usare le tecniche di zoom in Dynamic Media Classic. Seguite i passaggi da 1 a 6. Alla fine di ciascun passaggio è riportato un riferimento a un argomento correlato con ulteriori informazioni.

## 1. Caricamento delle immagini di zoom

Per iniziare, carica le immagini di zoom in Dynamic Media Classic. Per uno zoom ottimale, Dynamic Media Classic consiglia di utilizzare immagini di dimensioni almeno 2000 pixel.

Nella barra di navigazione globale, fai clic su **[!UICONTROL Carica]** per caricare immagini dal computer o dalla rete in una cartella di Dynamic Media Classic. Consultate [Caricamento delle immagini zoom](uploading-zoom-images.md#uploading_zoom_images).

## 2. Creazione di destinazioni di zoom per lo zoom guidato

Le destinazioni di zoom consentono di evidenziare porzioni specifiche di un’immagine. Potete ad esempio indirizzare l’attenzione alle parti di un’immagine che la rendono univoca o particolare. Nella finestra Visualizzatore zoom, le destinazioni di zoom vengono visualizzate come miniature a fianco dell’immagine. Se selezionate una di queste miniature di destinazione di zoom, viene applicato automaticamente lo zoom a una porzione specifica dell’immagine.

Per creare una destinazione di zoom, fai clic su **[!UICONTROL Modifica]** e scegli Destinazioni di zoom, oppure apri un&#39;immagine nel pannello Sfoglia in visualizzazione Dettagli e fai clic su **[!UICONTROL Destinazioni di zoom]**. Quindi utilizzate gli strumenti Zoom nella pagina Editor di destinazione zoom per isolare parte dell’immagine come destinazione. Consultate [Creazione di destinazioni di zoom per lo zoom guidato](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).

## 3. Impostazione dei predefiniti per visualizzatori zoom

I predefiniti per visualizzatori zoom determinano lo stile e il comportamento dei visualizzatori zoom usati. Gli amministratori possono impostare i predefiniti per visualizzatori zoom; Dynamic Media Classic viene fornito con i predefiniti per visualizzatori zoom &quot;best practice&quot;.

Per creare un predefinito per visualizzatori zoom, nella barra di navigazione globale fai clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**. Nella pagina Predefiniti visualizzatore fare clic su **[!UICONTROL Aggiungi]**, scegliere una piattaforma e un visualizzatore zoom, quindi fare clic su **[!UICONTROL Aggiungi]**. Quindi scegli le opzioni nella pagina Configura visualizzatore .

In Dynamic Media Classic sono disponibili le opzioni **[!UICONTROL Predefinito visualizzatore zoom]** che consentono di selezionare lo stile del pulsante e l’aspetto generale del visualizzatore. Potete inoltre personalizzare le impostazioni di zoom del sito Web. Consultate [Impostazione dei predefiniti per il visualizzatore zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## 4. Anteprima delle immagini con il visualizzatore zoom

Potete visualizzare in anteprima le immagini in un visualizzatore zoom per verificare l’esperienza di zoom quando questo viene applicato alle immagini.

Per esplorare diversi predefiniti per visualizzatori zoom e presentare l’esperienza di zoom, seleziona un’immagine nel pannello Sfoglia e fai clic su **[!UICONTROL Anteprima]**. Fai clic su **[!UICONTROL Predefiniti]** > **[!UICONTROL Zoom]**, quindi seleziona un predefinito con i menu Zoom.

Vengono visualizzati i pulsanti Zoom. Potete visualizzare l’aspetto delle immagini di zoom sul sito Web. Fare clic sui pulsanti Zoom (e sulle destinazioni di zoom) per verificare le impostazioni del predefinito visualizzatore zoom scelto. Consultate [Anteprima delle immagini con diversi visualizzatori zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)

## 5. Pubblicazione delle immagini zoom

La pubblicazione delle immagini zoom le inserisce sui server di immagini Dynamic Media in modo che possano essere distribuite al sito Web e all’applicazione. Come parte del processo di pubblicazione, Dynamic Media Classic attiva le stringhe URL. Queste stringhe URL richiamano le immagini di zoom dai server immagini Dynamic Media al sito Web o all&#39;applicazione.

Nella barra di navigazione globale, fate clic su **[!UICONTROL Pubblica]**. Nella finestra di dialogo Pubblica , fai clic su **[!UICONTROL Invia pubblicazione]**. Consultate [Pubblicazione delle immagini di zoom](publishing-zoom-images.md#publishing_zoom_images).

## 6. Collegamento dei visualizzatori zoom alla pagina web

Dynamic Media Classic crea le stringhe di callout URL necessarie per lo zoom delle immagini e le attiva quando le immagini vengono pubblicate sui server di immagini Dynamic Media. Puoi copiare queste stringhe URL dalla pagina **[!UICONTROL Anteprima]**. Dopo essere state copiate, le stringhe URL sono disponibili sui siti Web e le applicazioni. Consultate [Collegamento di visualizzatori zoom alla pagina Web](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages)
