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
autotag-review: '2026-05-13T20:09:40.553Z'
TQID: 'https://experienceleague.adobe.com/s3cXJgoACODCKQ8oMlykXjLAVmx6yWw9F2EC-3EbR0k'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: c1f9ca034a6cc7545f18a41876f737eb9144e157
workflow-type: tm+mt
source-wordcount: 707
ht-degree: 10%

---

# Avvio rapido: set di immagini{#quick-start-image-sets}

I set di immagini Adobe Dynamic Media Classic offrono agli utenti un&#39;esperienza di visualizzazione integrata. In Visualizzatore set di immagini dinamico, gli utenti possono visualizzare diverse visualizzazioni di un elemento selezionando una miniatura. I set di immagini consentono di presentare visualizzazioni alternative ad alta risoluzione di un elemento.

Per esaminare le immagini da vicino, questo visualizzatore offre inoltre degli strumenti di zoom. Potete rendere le destinazioni di zoom guidate e le mappe immagine parte del set di immagini. I set di immagini forniscono un’esperienza di visualizzazione più coerente e mirata.

Vedi [Set di immagini e 360 gradi: video di formazione su Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS).

Quando crei un set di immagini, Adobe consiglia le seguenti best practice e applica i seguenti limiti:

| Tipo di limite | Best practice | Limite imposto |
| --- | --- | --- |
| Numero di risorse duplicate per set | Nessun duplicato | 20‡ |
| Numero massimo di immagini per set | 5-10 immagini per set | 1000 |

‡ Si consiglia di non avere risorse duplicate in un set. Il limite è di 20 duplicati per una singola risorsa. Se aggiungi un altro duplicato per quella risorsa, all’interno di quel set, la richiesta restituisce un errore o ignora il duplicato.

Vedi anche [Limitazioni di Dynamic Media](/help/using/limitations.md).

La Guida introduttiva per i set di immagini seguente è stata progettata per consentire l&#39;utilizzo delle tecniche per i set di immagini in [!DNL Adobe Dynamic Media Classic].

## &#x200B;1. Carica le immagini primarie per più visualizzazioni e campioni

Per iniziare, caricate le immagini per il set di immagini. Poiché gli utenti possono eseguire lo zoom avanti sulle immagini nel Visualizzatore set di immagini, assicurati di valutare questa funzione quando scegli le immagini. Assicurati che le immagini siano almeno 2000 pixel nella dimensione più grande. Adobe Dynamic Media Classic supporta molti formati di file immagine, ma si consiglia di utilizzare immagini TIFF, PNG e EPS senza perdita di dati.

Sulla barra di navigazione globale, seleziona **[!UICONTROL Carica]** per caricare i file dal computer in una cartella in Adobe Dynamic Media Classic.

Consulta [Preparare le risorse del set di immagini per il caricamento](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) e [Caricare i file](uploading-files.md#uploading-your-files).

## &#x200B;2. Creare un set di immagini

In Set di immagini, gli utenti selezionano le miniature nel Visualizzatore set di immagini per visualizzare un&#39;immagine da un lato o da un angolo diverso.

Per creare un set di immagini, sulla barra di navigazione globale, seleziona **[!UICONTROL Build]**, quindi scegli **[!UICONTROL Set di immagini]**. Per comporre il set di immagini, trascinate le immagini nella pagina della finestra Set di immagini. Organizzate, aggiungete ed eliminate le immagini in base alle vostre esigenze.

Vedi [Creare un set di immagini](creating-image-set.md#creating-an-image-set).

Vedi anche [Includere destinazioni di zoom e mappe immagine nei set di immagini](/help/using/including-zoom-targets-image-maps-image-sets.md)

## &#x200B;3. Prepara i predefiniti visualizzatore set immagini, se necessario

Gli amministratori possono creare e modificare i predefiniti per i visualizzatori di set di immagini. Adobe Dynamic Media Classic viene fornito con predefiniti visualizzatore per ogni tipo di file rich media. Utilizza il Visualizzatore zoom: **[!UICONTROL Personalizzato]** > **[!UICONTROL Immagini]** o **[!UICONTROL Set di immagini]**/**[!UICONTROL Visualizzazioni multiple]** predefiniti per visualizzare i set di immagini.

È possibile aggiungere o modificare i predefiniti visualizzatore dalla schermata Impostazione applicazione.

Consulta [Creare e modificare i predefiniti visualizzatore](application-setup.md#adding-and-editing-viewer-presets).

## &#x200B;4. Anteprima di un set di immagini

Selezionare il set di immagini nel pannello Sfoglia, quindi selezionare **[!UICONTROL Anteprima]**. Nella pagina Anteprima, seleziona le icone delle miniature per esaminare il set di immagini nel visualizzatore selezionato. Nel menu Predefiniti, potete scegliere diversi visualizzatori.

Vedi [Visualizzare l&#39;anteprima di una risorsa](previewing-asset.md#previewing-an-asset).

## &#x200B;5. Pubblicare un set di immagini

Quando si pubblica un set di immagini, questo viene posizionato sui server Adobe Dynamic Media Classic e viene attivata la stringa dell&#39;URL.

>[!NOTE]
>
>Questo passaggio non è necessario se hai selezionato **[!UICONTROL Pubblica dopo un salvataggio]** (impostazione predefinita) al momento della creazione e del salvataggio del set di immagini.

Selezionare l&#39;icona **[!UICONTROL Contrassegna per pubblicazione]** a sinistra del nome nel pannello Sfoglia. Quindi seleziona **[!UICONTROL Pubblica]**. Nella pagina Pubblicazione, seleziona **[!UICONTROL Invia pubblicazione]**.

Vedi [File di pubblicazione](publishing-files.md#publishing-files).

## &#x200B;6. Collegare un set di immagini al sito Web

Adobe Dynamic Media Classic crea chiamate URL per i set di immagini e li attiva dopo la pubblicazione. Potete copiare tali URL dalla schermata Anteprima.

Selezionare il set di immagini, quindi selezionare **[!UICONTROL Anteprima]**. Selezionare un predefinito visualizzatore set di immagini, quindi fare clic sul pulsante **[!UICONTROL Copia URL]**.

Consulta [Collegare il set di immagini a una pagina Web](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
