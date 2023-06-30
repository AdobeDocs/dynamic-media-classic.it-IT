---
title: "Avvio rapido: ridimensionamento delle immagini"
description: Introduzione e Guida rapida al dimensionamento delle immagini per aiutarti a iniziare rapidamente a utilizzare le tecniche di dimensionamento delle immagini in Adobe Dynamic Media Classic.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
topic: Content Management
level: Beginner
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 23%

---

# Avvio rapido: ridimensionamento delle immagini{#quick-start-image-sizing}

Il dimensionamento dell&#39;immagine si riferisce alla capacità di Adobe Dynamic Media Classic di creare più immagini derivate basate su un&#39;unica immagine ad alta risoluzione. Anziché creare manualmente più immagini per il sito Web o l&#39;applicazione, ad esempio una miniatura e un&#39;immagine ingrandita, è possibile fornire una singola immagine principale. Adobe Dynamic Media Classic genera tutte le immagini modificate come richiesto dall&#39;utente. La possibilità di distribuire le immagini in modo dinamico da una singola immagine primaria presenta molti vantaggi:

* Non è necessario creare manualmente più copie dell’immagine in diversi formati. Fornite un&#39;immagine principale a Adobe Dynamic Media Classic, e Adobe Dynamic Media Classic genera derivati di dimensioni diverse dall&#39;immagine principale.
* Potete rapidamente modificare le dimensioni di un tipo di immagine usato nell’intero sito Web o nell’applicazione. Ad esempio, per modificare tutte le miniature, è sufficiente modificare il relativo predefinito. Un predefinito per immagini, paragonabile a una macro, consiste in un insieme di attributi di dimensione e formattazione. Per modificare la dimensione di tutte le miniature nel sito Web o nell’applicazione, potete modificare il predefinito per immagini “Miniatura”.
* Non è necessario gestire i file primari e tutti i vari derivati in nessuno dei sistemi di gestione dei contenuti o delle risorse, né internamente né esternamente.

![È possibile creare più immagini derivate di dimensioni diverse dallo stesso file principale ad alta risoluzione.](/help/using/assets/is_derivative_sizes_popup.png)

Consulta [Dimensioni immagine: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) video di formazione.

La seguente Guida introduttiva al dimensionamento delle immagini è stata progettata per aiutarti a iniziare rapidamente a usare le tecniche di dimensionamento delle immagini in Adobe Dynamic Media Classic. Seguire i punti da 1 a 5. Dopo ogni passaggio, esiste un riferimento incrociato in cui è possibile trovare ulteriori informazioni, se necessario.

## 1. Caricare immagini primarie

Per iniziare, carica le immagini principali su Adobe Dynamic Media Classic. Per quanto riguarda le dimensioni, Adobe Dynamic Media Classic consiglia di utilizzare immagini delle dimensioni più grandi previste per il sito web o l’applicazione. Ad esempio, se desideri che i visualizzatori ingrandiscano le immagini, carica quelle di dimensioni pari ad almeno 2000 pixel. Adobe Dynamic Media Classic supporta molti formati di file immagine, ma si consiglia di utilizzare immagini TIFF e PNG senza perdita di dati.

Sulla barra di navigazione globale, seleziona **[!UICONTROL Carica]** per caricare file dal computer in una cartella su Adobe Dynamic Media Classic. Consulta [Carica immagini primarie](uploading-master-images.md#uploading_master_images).

## 2. Impostare i predefiniti per le immagini

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Un predefinito per immagini definisce le dimensioni e la formattazione delle immagini distribuite dai server immagini Dynamic Media. Se siete amministratori della società, potete configurare i predefiniti per immagini voi stessi. Adobe Dynamic Media Classic viene inoltre fornito con predefiniti immagine predefiniti che è possibile utilizzare per distribuire le immagini in modo dinamico.

Per creare un predefinito immagine (se sei un amministratore), nella barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti immagine]**. Quindi seleziona **[!UICONTROL Aggiungi]** per creare un predefinito immagine, oppure seleziona **[!UICONTROL Modifica]** per modificare un predefinito immagine esistente.

Il predefinito immagine creato viene aggiunto al menu Predefinito immagine nella pagina Anteprima. Potete usare il nuovo predefinito per immagini per visualizzare le immagini sui siti Web e sulle applicazioni in modo dinamico. Consulta [Configurazione predefiniti immagine](setting-image-presets.md#setting_up_image_presets).

## 3. Anteprima predefiniti immagine

La fase successiva consiste nel visualizzare l’anteprima dei predefiniti per immagini configurati dall’amministratore nelle varie dimensioni.

Per esplorare i predefiniti immagine, sulla barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**, quindi individuare un predefinito immagine.

Provate i vari predefiniti per immagini Scopri come appare l’immagine quando viene distribuita dinamicamente al sito web o all’applicazione in diverse dimensioni.

Consulta [Visualizzare in anteprima una risorsa immagine in base al suo predefinito immagine](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Pubblicare le immagini principali

La pubblicazione dei file di immagine principali ha due scopi essenziali:

* Pubblicazione delle immagini principali sui server immagini Dynamic Media per l&#39;invio dinamico delle immagini al sito Web e all&#39;applicazione.
* La pubblicazione attiva le stringhe URL per la chiamata di immagini dai server immagini Dynamic Media al sito Web o all&#39;applicazione. Dopo la pubblicazione, puoi copiare e inserire gli URL generati da Adobe Dynamic Media Classic, se necessario, nel sito web o nell’applicazione.

Sulla barra di navigazione globale, seleziona **[!UICONTROL Pubblica]** per avviare un processo di pubblicazione. Nella finestra di dialogo Pubblica, seleziona **[!UICONTROL Invia pubblicazione]**. Consulta [Pubblicare immagini primarie](publishing-master-images.md#publishing_master_images).

## 5. Collegare gli URL all’applicazione web

Adobe Dynamic Media Classic crea stringhe di callout URL per le immagini. Quando si pubblicano immagini su Dynamic Media Image Server, gli URL diventano attivi. Puoi copiare queste stringhe URL dal pannello Sfoglia (in Vista dettagli) o dalla schermata Anteprima. Dopo aver copiato le stringhe URL, potete usarle nel sito Web o nelle applicazioni. Nel codice della pagina Web, l’URL per il ridimensionamento delle immagini sostituisce il riferimento al nome di un’immagine statica. L’URL fa riferimento a un nome di immagine principale, che viene sostituito dal database per ogni nuova immagine da visualizzare.

Le stringhe URL generate tramite Predefiniti immagine contengono il nome di un predefinito per immagini. Il nome è racchiuso tra simboli di dollaro (`$`). Ad esempio: `$thumbnail$` può essere il predefinito per immagini progettato per mostrare le immagini primarie alle dimensioni delle miniature. Consulta [Collegare gli URL all’applicazione web](linking-urls-web-application.md#linking_urls_to_your_web_application).
