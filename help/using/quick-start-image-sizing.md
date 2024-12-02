---
title: 'Avvio rapido: ridimensionamento delle immagini'
description: Introduzione e Guida rapida al dimensionamento delle immagini per aiutarti a iniziare rapidamente a utilizzare le tecniche di dimensionamento delle immagini in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 7%

---

# Avvio rapido: ridimensionamento delle immagini{#quick-start-image-sizing}

Il dimensionamento dell&#39;immagine si riferisce alla capacità di Adobe Dynamic Media Classic di creare più immagini derivate basate su un&#39;unica immagine ad alta risoluzione. Anziché creare manualmente più immagini, ad esempio una miniatura e un&#39;immagine ingrandita, per il sito Web o l&#39;applicazione in uso, è possibile fornire un&#39;unica immagine principale. Adobe Dynamic Media Classic genera tutte le immagini modificate come richiesto dall&#39;utente. La possibilità di distribuire le immagini in modo dinamico da una singola immagine primaria presenta molti vantaggi:

* Non è necessario creare manualmente diverse copie dell’immagine a dimensioni diverse. Fornite un&#39;immagine principale a Adobe Dynamic Media Classic, e Adobe Dynamic Media Classic genera derivati di dimensioni diverse dall&#39;immagine principale.
* È possibile modificare rapidamente le dimensioni di un tipo di immagine in tutto il sito Web o l&#39;applicazione. Ad esempio, per modificare tutte le miniature, puoi modificare il predefinito immagine &quot;miniatura&quot;. Un predefinito immagine, simile a una macro, è una raccolta di attributi di dimensione e formattazione. È possibile modificare il predefinito immagine &quot;miniatura&quot; per modificare le dimensioni di tutte le miniature presenti nel sito Web o nell&#39;applicazione.
* Non è necessario gestire i file primari e tutti i vari derivati in nessuno dei sistemi di gestione dei contenuti o delle risorse, né internamente né esternamente.

![È possibile creare più immagini derivate con dimensioni diverse dallo stesso file primario ad alta risoluzione.](/help/using/assets/is_derivative_sizes_popup.png)

Guarda il video di formazione su [Dimensioni immagine: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS).

La seguente Guida introduttiva al dimensionamento delle immagini è stata progettata per aiutarti a iniziare rapidamente a usare le tecniche di dimensionamento delle immagini in Adobe Dynamic Media Classic. Seguire i punti da 1 a 5. Dopo ogni passaggio, esiste un riferimento incrociato in cui è possibile trovare ulteriori informazioni, se necessario.

## 1. Caricare immagini primarie

Per iniziare, carica le immagini principali su Adobe Dynamic Media Classic. Per quanto riguarda le dimensioni, Adobe Dynamic Media Classic consiglia di utilizzare immagini delle dimensioni massime previste per il sito Web o l&#39;applicazione. Ad esempio, se desideri che i visualizzatori ingrandiscano le immagini, carica quelle di dimensioni pari ad almeno 2000 pixel. Adobe Dynamic Media Classic supporta molti formati di file immagine, ma si consiglia di utilizzare immagini TIFF e PNG senza perdita di dati.

Sulla barra di navigazione globale, seleziona **[!UICONTROL Carica]** per caricare i file dal computer in una cartella su Adobe Dynamic Media Classic. Consulta [Caricare immagini primarie](uploading-master-images.md#uploading_master_images).

## 2. Impostare i predefiniti per le immagini

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Un predefinito per immagini definisce le dimensioni e la formattazione delle immagini distribuite dai server immagini Dynamic Media. Se hai lo stato di Amministratore della società, puoi impostare autonomamente i predefiniti immagine. Puoi distribuire le immagini in modo dinamico utilizzando i predefiniti immagine già disponibili in Adobe Dynamic Media Classic.

Per creare un predefinito immagine (se sei un amministratore), vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Predefiniti immagine]** nella barra di navigazione globale. Quindi seleziona **[!UICONTROL Aggiungi]** per creare un predefinito immagine, oppure seleziona **[!UICONTROL Modifica]** per modificare un predefinito immagine esistente.

Il predefinito immagine creato viene aggiunto al menu Predefinito immagine nella pagina Anteprima. È possibile utilizzare il nuovo predefinito immagine per visualizzare le immagini in modo dinamico sui siti Web e sulle applicazioni. Consulta [Configurazione predefiniti immagine](setting-image-presets.md#setting_up_image_presets).

## 3. Anteprima predefiniti immagine

La fase successiva consiste nel visualizzare l’anteprima dei predefiniti per immagini configurati dall’amministratore nelle varie dimensioni.

Per esplorare i predefiniti immagine, sulla barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**, quindi passa a un predefinito immagine.

Provate i vari predefiniti per immagini Scopri come viene visualizzata l’immagine quando viene distribuita dinamicamente al sito Web o all’applicazione in diverse dimensioni.

Consulta [Visualizzare in anteprima una risorsa immagine in base al suo predefinito immagine](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Publish le immagini principali

La pubblicazione dei file di immagine principali ha due scopi essenziali:

* Pubblicazione delle immagini principali sui server immagini Dynamic Media per l&#39;invio dinamico delle immagini al sito Web e all&#39;applicazione.
* La pubblicazione attiva le stringhe URL per la chiamata di immagini dai server immagini Dynamic Media al sito Web o all&#39;applicazione. Dopo la pubblicazione, è possibile copiare e inserire gli URL generati da Adobe Dynamic Media Classic, se necessario, nel sito Web o nell&#39;applicazione.

Sulla barra di navigazione globale, seleziona **[!UICONTROL Publish]** per avviare un processo di pubblicazione. Nella finestra di dialogo Pubblicazione selezionare **[!UICONTROL Invia Publish]**. Vedi [Immagini primarie di Publish](publishing-master-images.md#publishing_master_images).

## 5. Collegare gli URL all’applicazione web

Adobe Dynamic Media Classic crea stringhe di callout URL per le immagini. Quando si pubblicano immagini su Dynamic Media Image Server, gli URL diventano attivi. Puoi copiare queste stringhe URL dal pannello Sfoglia (in Vista dettagli) o dalla schermata Anteprima. Dopo aver copiato le stringhe URL, è possibile utilizzarle nel sito Web e nelle applicazioni. L’URL per Image Sizing sostituisce il riferimento a un nome di immagine statico nel codice della pagina web. L’URL fa riferimento a un nome di immagine principale che il database sostituisce per ogni nuova immagine da visualizzare.

Le stringhe URL generate tramite Predefiniti immagine contengono il nome di un predefinito per immagini. Questo nome è racchiuso tra simboli di dollaro (`$`). Ad esempio, `$thumbnail$` può essere il predefinito immagine progettato per mostrare le immagini primarie alle dimensioni delle miniature. Consulta [Collegare gli URL all&#39;applicazione Web](linking-urls-web-application.md#linking_urls_to_your_web_application).
