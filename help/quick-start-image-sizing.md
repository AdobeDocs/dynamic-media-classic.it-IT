---
title: '"Avvio rapido: ridimensionamento delle immagini"'
description: Introduzione e rapida alle dimensioni dell’immagine per aiutarti a iniziare rapidamente a usare le tecniche di dimensionamento dell’immagine.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Gestione risorse
role: Business Practitioner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 38%

---

# Avvio rapido: ridimensionamento delle immagini{#quick-start-image-sizing}

Il dimensionamento dell&#39;immagine si riferisce alla capacità di Dynamic Media Classic di creare più immagini derivate basate su un&#39;unica immagine ad alta risoluzione. Invece di creare manualmente diverse immagini (ad esempio, una miniatura e un’immagine ingrandita) per il sito Web o l’applicazione, fornisci un’unica immagine principale. Dynamic Media Classic genera tutte le immagini modificate come richiesto. I vantaggi di poter offrire immagini in modo dinamico da una singola immagine originale sono notevoli:

* Non è necessario creare manualmente più copie dell’immagine in diversi formati. Fornisci un’immagine principale a Dynamic Media Classic e Dynamic Media Classic genera derivati di dimensioni diverse dall’immagine principale.
* Potete rapidamente modificare le dimensioni di un tipo di immagine usato nell’intero sito Web o nell’applicazione. Ad esempio, per modificare tutte le miniature, è sufficiente modificare il relativo predefinito. Un predefinito per immagini, paragonabile a una macro, consiste in un insieme di attributi di dimensione e formattazione. Per modificare la dimensione di tutte le miniature nel sito Web o nell’applicazione, potete modificare il predefinito per immagini “Miniatura”.
* Non è necessario gestire i master e tutti i vari derivati in nessuno dei sistemi di gestione dei contenuti o delle risorse internamente o esternamente.

![È possibile creare più immagini derivate di dimensioni diverse dallo stesso file master ad alta risoluzione.](/help/assets/is_derivative_sizes_popup.png)

Questa guida rapida alle dimensioni delle immagini è stata progettata per aiutarti a iniziare rapidamente a usare le tecniche di dimensionamento delle immagini in Dynamic Media Classic. Segui i punti da 1 a 5. Inoltre, per ogni passaggio è riportato un riferimento incrociato in cui potete trovare ulteriori informazioni.

## 1. Caricamento delle immagini master

Per iniziare, carica le immagini principali in Dynamic Media Classic. Per quanto riguarda le dimensioni, Dynamic Media Classic consiglia di utilizzare immagini di dimensioni maggiori che si prevede di utilizzare sul sito Web o sull&#39;applicazione. Ad esempio, se desideri che gli utenti visualizzino le immagini con zoom, carica le immagini di dimensioni massime pari ad almeno 2000 pixel. Dynamic Media Classic supporta molti formati di file immagine, ma si consiglia di utilizzare immagini TIFF e PNG senza perdita di dati.

Nella barra di navigazione globale, fai clic su **[!UICONTROL Carica]** per caricare i file dal computer in una cartella di Dynamic Media Classic. Consultate [Caricamento delle immagini originali](uploading-master-images.md#uploading_master_images).

## 2. Impostazione dei predefiniti per le immagini

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Un predefinito per immagini regola le dimensioni e la formattazione con cui le immagini vengono distribuite dai server di immagini Dynamic Media. Se siete amministratori della società, potete configurare i predefiniti per immagini voi stessi. Dynamic Media Classic viene fornito anche con predefiniti per immagini predefiniti e può essere utilizzato per distribuire dinamicamente le immagini.

Per creare un predefinito per immagini (se sei un amministratore), nella barra di navigazione globale fai clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Predefiniti immagini]**. Quindi fai clic su **[!UICONTROL Aggiungi]** per creare un predefinito per immagini oppure fai clic su **[!UICONTROL Modifica]** per modificare un predefinito per immagini esistente.

Il predefinito immagine creato viene aggiunto al menu Predefinito immagine nella pagina Anteprima. Potete usare il nuovo predefinito per immagini per visualizzare le immagini sui siti Web e sulle applicazioni in modo dinamico. Consultate [Configurazione dei predefiniti per immagini](setting-image-presets.md#setting_up_image_presets).

## 3. Anteprima dei predefiniti immagine

La fase successiva consiste nel visualizzare l’anteprima dei predefiniti per immagini configurati dall’amministratore nelle varie dimensioni.

Per esplorare i predefiniti immagine, nella barra di navigazione globale fai clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**, quindi seleziona un predefinito immagine.

Provate i vari predefiniti per immagini Scopri come viene visualizzata l’immagine quando viene consegnata dinamicamente al sito Web o all’applicazione con dimensioni diverse.

Consultate [Anteprima di una risorsa immagine basata sul suo predefinito per immagini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Pubblicazione delle immagini master

La pubblicazione dei file immagine originali ha due scopi fondamentali:

* Pubblicazione delle immagini master sui server di immagini Dynamic Media in modo che le immagini possano essere distribuite in modo dinamico al sito Web e all’applicazione.
* La pubblicazione attiva le stringhe URL per richiamare le immagini dai server immagini Dynamic Media al sito Web o all&#39;applicazione. Dopo la pubblicazione, puoi copiare e inserire gli URL generati da Dynamic Media Classic, se necessario, nel sito web o nell’applicazione.

Nella barra di navigazione globale, fai clic su **[!UICONTROL Pubblica]** per avviare un processo di pubblicazione. Nella finestra di dialogo Pubblica , fai clic su **[!UICONTROL Invia pubblicazione]**. Consultate [Pubblicazione delle immagini originali](publishing-master-images.md#publishing_master_images).

## 5. Collegamento degli URL all’applicazione web

Dynamic Media Classic crea stringhe di callout URL per le immagini. Quando pubblichi le immagini sui server di immagini Dynamic Media, gli URL diventano attivi. Potete copiare queste stringhe URL dal pannello Sfoglia (in visualizzazione Dettagli) o dalla schermata Anteprima. Dopo aver copiato le stringhe URL, potete usarle nel sito Web o nelle applicazioni. Nel codice della pagina Web, l’URL per il ridimensionamento delle immagini sostituisce il riferimento al nome di un’immagine statica. L’URL fa riferimento al nome di un’immagine originale, che verrà sostituito dal database per ciascuna immagine nuova da visualizzare.

Le stringhe URL generate tramite Predefiniti immagine contengono il nome di un predefinito per immagini. Il nome è racchiuso tra simboli di dollaro (`$`). Ad esempio, `$thumbnail$` può essere il predefinito per immagini progettato per mostrare le immagini master con le dimensioni delle miniature. Consultate [Collegamento degli URL all’applicazione Web](linking-urls-web-application.md#linking_urls_to_your_web_application).
