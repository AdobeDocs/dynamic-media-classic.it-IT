---
title: "Avvio rapido: ridimensionamento delle immagini"
description: Introduzione e rapida alle dimensioni dell’immagine per aiutarti a iniziare rapidamente a usare le tecniche di dimensionamento dell’immagine in Adobe Dynamic Media Classic.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 23%

---

# Avvio rapido: ridimensionamento delle immagini{#quick-start-image-sizing}

Il dimensionamento dell&#39;immagine si riferisce alla capacità di Adobe Dynamic Media Classic di creare più immagini derivate basate su un&#39;unica immagine ad alta risoluzione. Invece di creare manualmente diverse immagini (ad esempio una miniatura e un’immagine ingrandita) per il sito Web o l’applicazione, fornisci un’unica immagine primaria. Adobe Dynamic Media Classic genera tutte le immagini modificate come richiesto. La capacità di fornire immagini in modo dinamico da una singola immagine primaria presenta molti vantaggi:

* Non è necessario creare manualmente più copie dell’immagine in diversi formati. Fornisci un’immagine primaria a Adobe Dynamic Media Classic e Adobe Dynamic Media Classic genera derivati di dimensioni diverse dall’immagine primaria.
* Potete rapidamente modificare le dimensioni di un tipo di immagine usato nell’intero sito Web o nell’applicazione. Ad esempio, per modificare tutte le miniature, è sufficiente modificare il relativo predefinito. Un predefinito per immagini, paragonabile a una macro, consiste in un insieme di attributi di dimensione e formattazione. Per modificare la dimensione di tutte le miniature nel sito Web o nell’applicazione, potete modificare il predefinito per immagini “Miniatura”.
* Non è necessario gestire i file principali e tutti i vari derivati in nessuno dei sistemi di gestione dei contenuti o delle risorse internamente o esternamente.

![È possibile creare più immagini derivate di dimensioni diverse dallo stesso file primario ad alta risoluzione.](/help/assets/is_derivative_sizes_popup.png)

Vedi [Dimensionamento dell&#39;immagine: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) video di formazione.

La seguente Guida rapida alle dimensioni delle immagini è stata progettata per aiutarti a iniziare rapidamente a usare le tecniche di dimensionamento delle immagini in Adobe Dynamic Media Classic. Segui i punti da 1 a 5. Dopo ogni passaggio, è disponibile un riferimento incrociato dove è possibile trovare ulteriori informazioni, se necessario.

## 1. Caricare immagini primarie

Inizia caricando le immagini principali su Adobe Dynamic Media Classic. Per quanto riguarda le dimensioni, Adobe Dynamic Media Classic consiglia di utilizzare immagini delle dimensioni più grandi che si prevede di utilizzare sul sito Web o sull&#39;applicazione. Ad esempio, se desideri che gli utenti visualizzino le immagini con zoom, carica le immagini di dimensioni massime pari ad almeno 2000 pixel. Adobe Dynamic Media Classic supporta molti formati di file immagine, ma si consiglia di utilizzare immagini TIFF e PNG senza perdita di dati.

Nella barra di navigazione globale, seleziona **[!UICONTROL Carica]** per caricare i file dal computer in una cartella su Adobe Dynamic Media Classic. Vedi [Caricare immagini primarie](uploading-master-images.md#uploading_master_images).

## 2. Impostare i predefiniti per le immagini

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Un predefinito per immagini regola le dimensioni e la formattazione con cui le immagini vengono distribuite dai server di immagini Dynamic Media. Se siete amministratori della società, potete configurare i predefiniti per immagini voi stessi. Adobe Dynamic Media Classic viene fornito anche con predefiniti per immagini predefiniti, che possono essere utilizzati per distribuire dinamicamente le immagini.

Per creare un predefinito per immagini (se sei un amministratore), nella barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti immagine]**. Quindi seleziona **[!UICONTROL Aggiungi]** per creare un predefinito immagine o seleziona **[!UICONTROL Modifica]** per modificare un predefinito per immagini esistente.

Il predefinito immagine creato viene aggiunto al menu Predefinito immagine nella pagina Anteprima. Potete usare il nuovo predefinito per immagini per visualizzare le immagini sui siti Web e sulle applicazioni in modo dinamico. Vedi [Impostazione dei predefiniti per immagini](setting-image-presets.md#setting_up_image_presets).

## 3. Anteprima predefiniti immagine

La fase successiva consiste nel visualizzare l’anteprima dei predefiniti per immagini configurati dall’amministratore nelle varie dimensioni.

Per esplorare i predefiniti immagine, nella barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**, quindi cerca un predefinito per immagini.

Provate i vari predefiniti per immagini Scopri come viene visualizzata l’immagine quando viene consegnata dinamicamente al sito Web o all’applicazione con dimensioni diverse.

Vedi [Visualizzare in anteprima una risorsa immagine in base al relativo predefinito per immagini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Pubblicare le immagini primarie

La pubblicazione dei file immagine principali ha due scopi essenziali:

* Pubblicazione delle immagini primarie sui server di immagini Dynamic Media in modo che le immagini possano essere distribuite in modo dinamico al sito Web e all&#39;applicazione.
* La pubblicazione attiva le stringhe URL per richiamare le immagini dai server immagini Dynamic Media al sito Web o all&#39;applicazione. Dopo la pubblicazione, puoi copiare e inserire gli URL generati da Adobe Dynamic Media Classic, se necessario, nel sito web o nell’applicazione.

Nella barra di navigazione globale, seleziona **[!UICONTROL Pubblica]** per avviare un processo di pubblicazione. Nella finestra di dialogo Pubblica, seleziona **[!UICONTROL Invia pubblicazione]**. Vedi [Pubblicare immagini primarie](publishing-master-images.md#publishing_master_images).

## 5. Collegare gli URL all&#39;applicazione web

Adobe Dynamic Media Classic crea stringhe di callout URL per le immagini. Quando pubblichi le immagini sui server di immagini Dynamic Media, gli URL diventano attivi. Puoi copiare queste stringhe URL dal pannello Sfoglia (in Vista dettaglio) o dalla schermata Anteprima. Dopo aver copiato le stringhe URL, potete usarle nel sito Web o nelle applicazioni. Nel codice della pagina Web, l’URL per il ridimensionamento delle immagini sostituisce il riferimento al nome di un’immagine statica. L’URL fa riferimento a un nome immagine principale, che viene sostituito dal database per ogni nuova immagine da visualizzare.

Le stringhe URL generate tramite Predefiniti immagine contengono il nome di un predefinito per immagini. Il nome è racchiuso tra simboli di dollaro (`$`). Ad esempio: `$thumbnail$` può essere il predefinito per immagini progettato per mostrare le immagini primarie alle dimensioni delle miniature. Vedi [Collegare gli URL all’applicazione web](linking-urls-web-application.md#linking_urls_to_your_web_application).
