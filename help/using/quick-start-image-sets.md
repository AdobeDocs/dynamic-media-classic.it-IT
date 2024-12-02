---
title: 'Avvio rapido: set di immagini'
description: Introduzione e Guida rapida ai set di immagini per aiutarti a iniziare rapidamente a utilizzare le tecniche per i set di immagini in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 11%

---

# Avvio rapido: set di immagini{#quick-start-image-sets}

I set di immagini Adobe Dynamic Media Classic offrono agli utenti un&#39;esperienza di visualizzazione integrata. In Visualizzatore set di immagini dinamico, gli utenti possono visualizzare diverse visualizzazioni di un elemento selezionando una miniatura. I set di immagini consentono di presentare visualizzazioni alternative ad alta risoluzione di un elemento.

Per esaminare le immagini da vicino, questo visualizzatore offre inoltre degli strumenti di zoom. Se lo desideri, puoi rendere le destinazioni di zoom guidate e le mappe immagine parte del set di immagini. I set di immagini offrono agli utenti un’esperienza di visualizzazione più organizzata e personale.

Guarda il video di formazione su [Set di immagini e 360 gradi: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS).

Quando crei un set di immagini, Adobe consiglia le seguenti best practice e applica i seguenti limiti:

| Tipo di limite | Best practice | Limite imposto |
| --- | --- | --- |
| Numero di risorse duplicate per set | Nessun duplicato | 20‡ |
| Numero massimo di immagini per set | 5-10 immagini per set | 1000 |

‡ Si consiglia di non avere risorse duplicate in un set. Il limite è di 20 duplicati per una singola risorsa. Se aggiungi un altro duplicato per quella risorsa, all’interno di quel set, la richiesta restituisce un errore o ignora il duplicato.

Vedi anche [Limitazioni di Dynamic Media](/help/using/limitations.md).

La Guida introduttiva per set di immagini riportata di seguito è stata progettata per consentirti di iniziare rapidamente a lavorare con le tecniche per set di immagini in Adobe Dynamic Media Classic.

## 1. Carica le immagini primarie per più viste e campioni

Per iniziare, caricate le immagini per il set di immagini. Poiché gli utenti possono eseguire lo zoom sulle immagini nel Visualizzatore set di immagini, assicurati di tenere presente questa possibilità quando scegli le immagini. Assicurati che le dimensioni delle immagini siano di almeno 2000 pixel. Adobe Dynamic Media Classic supporta molti formati di file immagine, ma si consiglia di utilizzare immagini TIFF, PNG e EPS senza perdita di dati.

Sulla barra di navigazione globale, seleziona **[!UICONTROL Carica]** per caricare i file dal computer in una cartella su Adobe Dynamic Media Classic.

Consulta [Preparare le risorse del set di immagini per il caricamento](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) e [Caricare i file](uploading-files.md#uploading-your-files).

## 2. Creare un set di immagini

In Set di immagini, gli utenti selezionano le miniature nel Visualizzatore set di immagini per visualizzare un&#39;immagine da un lato o da un angolo diverso.

Per creare un set di immagini, sulla barra di navigazione globale, seleziona **[!UICONTROL Build]**, quindi scegli **[!UICONTROL Set di immagini]**. Nella finestra Set di immagini trascinare le immagini nella pagina per comporre il set di immagini. Organizzate, aggiungete ed eliminate le immagini in base alle vostre esigenze.

Vedi [Creare un set di immagini](creating-image-set.md#creating-an-image-set).

Vedi anche [Includere destinazioni di zoom e mappe immagine nei set di immagini](/help/using/including-zoom-targets-image-maps-image-sets.md)

## 3. Prepara i predefiniti visualizzatore per set di immagini, in base alle esigenze

Gli amministratori possono creare e modificare i predefiniti per i visualizzatori di set di immagini. Adobe Dynamic Media Classic viene fornito con predefiniti visualizzatore per ogni tipo di file rich media. Utilizza il Visualizzatore zoom: **[!UICONTROL Personalizzato]** > **[!UICONTROL Immagini]** o **[!UICONTROL Set di immagini]**/**[!UICONTROL Visualizzazioni multiple]** predefiniti per visualizzare i set di immagini.

È possibile aggiungere o modificare i predefiniti visualizzatore dalla schermata Impostazione applicazione.

Consulta [Creare e modificare i predefiniti visualizzatore](application-setup.md#adding-and-editing-viewer-presets).

## 4. Anteprima di un set di immagini

Selezionare il set di immagini nel pannello Sfoglia, quindi selezionare **[!UICONTROL Anteprima]**. Nella pagina Anteprima, seleziona le icone delle miniature per esaminare il set di immagini nel visualizzatore selezionato. Nel menu Predefiniti, potete scegliere diversi visualizzatori.

Vedi [Visualizzare l&#39;anteprima di una risorsa](previewing-asset.md#previewing-an-asset).

## 5. Publish e set di immagini

Quando si pubblica un set di immagini, questo viene posizionato sui server Adobe Dynamic Media Classic e viene attivata la stringa dell&#39;URL.

>[!NOTE]
>
>Questo passaggio non è necessario se al momento della creazione e del salvataggio del set di immagini è stato selezionato **[!UICONTROL Publish dopo un salvataggio]** (impostazione predefinita).

Selezionare l&#39;icona **[!UICONTROL Contrassegna per Publish]** a sinistra del nome nel pannello Sfoglia. Quindi selezionare **[!UICONTROL Publish]**. Nella pagina Pubblicazione, seleziona **[!UICONTROL Invia Publish]**.

Vedi [file Publish](publishing-files.md#publishing-files).

## 6. Collegare un set di immagini al sito Web

Adobe Dynamic Media Classic crea chiamate URL per i set di immagini e li attiva dopo la pubblicazione. Potete copiare tali URL dalla schermata Anteprima.

Selezionare il set di immagini, quindi selezionare **[!UICONTROL Anteprima]**. Selezionare un predefinito visualizzatore set di immagini, quindi fare clic sul pulsante **[!UICONTROL Copia URL]**.

Consulta [Collegare il set di immagini a una pagina Web](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
