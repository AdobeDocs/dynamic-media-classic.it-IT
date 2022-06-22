---
title: '"Avvio rapido: set di immagini"'
description: Introduzione e avvio rapido ai set di immagini per consentirti di iniziare a utilizzare rapidamente le tecniche per i set di immagini in Adobe Dynamic Media Classic.
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
source-git-commit: d5293a2983e1105c65005634e7eb4147e17e8328
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 21%

---

# Avvio rapido: set di immagini{#quick-start-image-sets}

I set di immagini di Adobe Dynamic Media Classic offrono agli utenti un’esperienza di visualizzazione integrata. Nel visualizzatore di set di immagini dinamico, gli utenti possono fare clic su una miniatura per vedere diverse vedute dello stesso oggetto. I set di immagini consentono di presentare viste alternative ad alta risoluzione di un elemento.

Per esaminare le immagini da vicino, questo visualizzatore offre inoltre degli strumenti di zoom. Se lo desiderate, potete includere nel set di immagini anche destinazioni di zoom e mappe immagine. I set di immagini offrono agli utenti un’esperienza di visualizzazione più organizzata e personale.

Vedi [Set di immagini e set 360 gradi: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) video di formazione.

Quando crei un set di immagini, Adobe consiglia le seguenti best practice e applica i seguenti limiti:

| Tipo limite set di immagini | Best practice | Limite implementato | Modifiche al limite del 31 dicembre 2022 |
| --- | --- | --- | --- |
| Numero di risorse duplicate per set | Nessun duplicato | 100 | 20 |
| Numero massimo di immagini per set | 5-10 immagini per set | 1000 |

La seguente procedura rapida per i set di immagini è stata progettata per aiutarti a iniziare rapidamente a usare le tecniche per i set di immagini in Adobe Dynamic Media Classic.

## 1. Carica le immagini principali per più viste e campioni

Per iniziare, caricate le immagini per il set di immagini. Poiché gli utenti possono eseguire lo zoom sulle immagini nel Visualizzatore set di immagini, assicurati di tenere conto di questa funzionalità durante la scelta delle immagini. Assicurati che le immagini siano di almeno 2000 pixel nelle dimensioni più grandi. Adobe Dynamic Media Classic supporta molti formati di file immagine, ma si consiglia di utilizzare immagini TIFF, PNG e EPS senza perdita di dati.

Nella barra di navigazione globale, seleziona **[!UICONTROL Carica]** per caricare i file dal computer in una cartella su Adobe Dynamic Media Classic.

Vedi [Preparare le risorse del set di immagini per il caricamento](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) e [Caricare i file](uploading-files.md#uploading-your-files).

## 2. Creare un set di immagini

In Set immagini, gli utenti selezionano le miniature nel visualizzatore di set di immagini per vedere un’immagine da un lato o da un’angolazione diversi.

Per creare un set di immagini, nella barra di navigazione globale seleziona **[!UICONTROL Crea]**, quindi scegli **[!UICONTROL Set di immagini]**. Nella finestra Set immagini, trascina le immagini sulla pagina per comporre il set di immagini. Organizzate, aggiungete ed eliminate le immagini in base alle vostre esigenze.

Vedi [Creare un set di immagini](creating-image-set.md#creating-an-image-set).

Vedi anche [Includere destinazioni di zoom e mappe immagine nei set di immagini](/help/including-zoom-targets-image-maps-image-sets.md)

## 3. Preparare i predefiniti visualizzatore dei set di immagini, in base alle esigenze

Gli amministratori possono creare e modificare i predefiniti per i visualizzatori di set di immagini. Adobe Dynamic Media Classic viene fornito con predefiniti per visualizzatori per ogni tipo di rich media. Utilizza il visualizzatore zoom: **[!UICONTROL Personalizzato]** > **[!UICONTROL Immagini]** o **[!UICONTROL Set di immagini]**/**[!UICONTROL Viste multiple]** per visualizzare i set di immagini.

Potete aggiungere o modificare i predefiniti per visualizzatori dalla schermata Impostazione applicazione.

Vedi [Creare e modificare i predefiniti per visualizzatori](application-setup.md#adding-and-editing-viewer-presets).

## 4. Anteprima di un set di immagini

Seleziona il set di immagini nel pannello Sfoglia, quindi seleziona **[!UICONTROL Anteprima]**. Nella pagina Anteprima, seleziona le icone delle miniature per esaminare il set di immagini nel visualizzatore selezionato. Nel menu Predefiniti, potete scegliere diversi visualizzatori.

Vedi [Visualizzare un&#39;anteprima di una risorsa](previewing-asset.md#previewing-an-asset).

## 5. Pubblicare un set di immagini

La pubblicazione di un set di immagini lo inserisce sui server Adobe Dynamic Media Classic e attiva la stringa URL.

>[!NOTE]
>
>Questo passaggio è facoltativo se avete selezionato **[!UICONTROL Pubblica dopo il salvataggio]** (impostazione predefinita) al momento della creazione e del salvataggio del set di immagini.

Seleziona **[!UICONTROL Contrassegna per pubblicazione]** a sinistra del nome nel pannello Sfoglia. Quindi, seleziona **[!UICONTROL Pubblica]**. Nella pagina Pubblica , seleziona **[!UICONTROL Invia pubblicazione]**.

Vedi [Pubblicare i file](publishing-files.md#publishing-files).

## 6. Collega un set di immagini al tuo sito web

Adobe Dynamic Media Classic crea chiamate URL per i set di immagini e li attiva dopo la pubblicazione. Potete copiare tali URL dalla schermata Anteprima.

Seleziona il set di immagini, quindi seleziona **[!UICONTROL Anteprima]**. Ora seleziona un predefinito per visualizzatori di set di immagini, quindi seleziona **[!UICONTROL Copia URL]**.

Vedi [Collegamento di un set di immagini a una pagina web](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
