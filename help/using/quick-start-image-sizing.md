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
autotag-review: '2026-05-13T20:09:57.533Z'
TQID: 'https://experienceleague.adobe.com/VGp4OQ03iRiobXKWuUERNtFwUMQ4z7a19wyOgHWuv3w'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: e66a98d5071f107477891c3769f1301fcc0d86db
workflow-type: tm+mt
source-wordcount: 870
ht-degree: 6%

---

# Avvio rapido: ridimensionamento delle immagini{#quick-start-image-sizing}

Il dimensionamento dell&#39;immagine si riferisce alla capacità di Adobe Dynamic Media Classic di creare più immagini derivate basate su un&#39;unica immagine ad alta risoluzione. Invece di creare manualmente più immagini per il sito web o l’applicazione, fornisci un’unica immagine principale. Adobe Dynamic Media Classic genera tutte le immagini modificate come richiesto. La distribuzione dinamica di immagini da una singola immagine primaria presenta numerosi vantaggi:

* Non è necessario creare manualmente diverse copie dell’immagine a dimensioni diverse. Fornite un&#39;immagine primaria a Adobe Dynamic Media Classic, e genera derivati di dimensioni diverse dall&#39;immagine primaria.
* Puoi modificare rapidamente le dimensioni di un’immagine in tutto il sito web o nell’applicazione. Ad esempio, per modificare tutte le miniature, puoi modificare il predefinito immagine &quot;miniatura&quot;. Un predefinito immagine è una raccolta di attributi di dimensione e formattazione. Per modificare le dimensioni di tutte le miniature in tutto il sito Web o l&#39;applicazione, potete modificare il predefinito immagine &quot;miniatura&quot;.
* Non è necessario gestire i file primari o tutti i vari derivati in nessuno dei sistemi di gestione dei contenuti o delle risorse.

![È possibile creare più immagini derivate con dimensioni diverse dallo stesso file primario ad alta risoluzione.](/help/using/assets/is_derivative_sizes_popup.png)

Vedere [Dimensioni immagine: video di formazione di Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS).

La seguente Guida introduttiva al ridimensionamento delle immagini è stata progettata per aiutarti a iniziare a utilizzare le tecniche di ridimensionamento delle immagini in Adobe Dynamic Media Classic. Completa i passaggi 1-5. Dopo ogni passaggio, esiste un riferimento incrociato in cui è possibile trovare ulteriori informazioni, se necessario.

## &#x200B;1. Carica immagini primarie

Carica le immagini principali in Adobe Dynamic Media Classic. Adobe Dynamic Media Classic consiglia di utilizzare immagini delle dimensioni massime previste per il sito web o l’applicazione. Ad esempio, se desideri che i visualizzatori ingrandiscano le immagini, carica quelle di dimensioni pari ad almeno 2000 pixel. Adobe Dynamic Media Classic supporta molti formati di file immagine, ma si consiglia di utilizzare immagini TIFF e PNG senza perdita di dati.

Sulla barra di navigazione globale, seleziona **[!UICONTROL Carica]** per caricare i file dal computer in una cartella su Adobe Dynamic Media Classic. Consulta [Caricare immagini primarie](uploading-master-images.md#uploading_master_images).

## &#x200B;2. Configura predefiniti immagine

Un predefinito immagine è una raccolta di comandi di formattazione e dimensione predefiniti salvati con un nome. Un predefinito per immagini governa le dimensioni e la formattazione con cui le immagini vengono distribuite dai server immagini Dynamic Media. Se disponi dello stato di Amministratore della società, puoi configurare i predefiniti immagine in modo indipendente. Puoi distribuire le immagini in modo dinamico utilizzando i predefiniti immagine predefiniti inclusi in Adobe Dynamic Media Classic.

Per creare un predefinito immagine (se sei un amministratore), vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Predefiniti immagine]** nella barra di navigazione globale. Quindi seleziona **[!UICONTROL Aggiungi]** per creare un predefinito immagine, oppure seleziona **[!UICONTROL Modifica]** per modificare un predefinito immagine esistente.

Il predefinito immagine creato viene aggiunto al menu Predefinito immagine nella pagina Anteprima. Potete usare il nuovo predefinito per immagini per visualizzare le immagini sui siti Web e sulle applicazioni in modo dinamico. Consulta [Configurazione predefiniti immagine](setting-image-presets.md#setting_up_image_presets).

## &#x200B;3. Anteprima predefiniti immagine

La fase successiva consiste nel visualizzare l’anteprima dei predefiniti per immagini configurati dall’amministratore nelle varie dimensioni.

Per esplorare i predefiniti immagine, sulla barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**, quindi passa a un predefinito immagine.

Verifica i diversi predefiniti immagine. Determina la modalità di visualizzazione dell’immagine quando viene distribuita dinamicamente al sito web o all’applicazione in diverse dimensioni.

Consulta [Visualizzare in anteprima una risorsa immagine in base al suo predefinito immagine](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## &#x200B;4. Pubblicare le immagini principali

La pubblicazione dei file di immagine principali ha due scopi essenziali:

* Pubblica le immagini primarie sui server di immagini Dynamic Media in modo che possano essere distribuite dinamicamente al sito web e all’applicazione.
* La pubblicazione attiva le stringhe URL per richiamare le immagini dai server immagini Dynamic Media al sito web o all’applicazione. Dopo la pubblicazione, puoi copiare e inserire gli URL generati da Adobe Dynamic Media Classic, se necessario, nel sito web o nell’applicazione.

Sulla barra di navigazione globale, seleziona **[!UICONTROL Pubblica]** per avviare un processo di pubblicazione. Nella finestra di dialogo Pubblicazione selezionare **[!UICONTROL Invia pubblicazione]**. Vedi [Pubblicare immagini primarie](publishing-master-images.md#publishing_master_images).

## &#x200B;5. Collegare gli URL all’applicazione web

Adobe Dynamic Media Classic crea stringhe di callout URL per le immagini. Quando pubblichi le immagini su Dynamic Media Image Server, gli URL diventano attivi. Puoi copiare queste stringhe URL dal pannello Sfoglia (in Vista dettagli) o dalla schermata Anteprima. Dopo aver copiato le stringhe URL, puoi utilizzarle nel sito web o nell’applicazione. L’URL per Image Sizing sostituisce il riferimento a un nome di immagine statico nel codice della pagina web. L&#39;URL fa riferimento a un nome di immagine principale che il database sostituisce per ogni nuova immagine visualizzata.

Le stringhe URL generate tramite Predefiniti immagine contengono il nome di un predefinito per immagini. Questo nome è racchiuso tra simboli di dollaro (`$`). Ad esempio, `$thumbnail$` può essere il predefinito immagine progettato per mostrare le immagini primarie alle dimensioni delle miniature. Consulta [Collegare gli URL all&#39;applicazione Web](linking-urls-web-application.md#linking_urls_to_your_web_application).
