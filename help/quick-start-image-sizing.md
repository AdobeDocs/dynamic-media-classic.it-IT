---
title: '"Avvio rapido: ridimensionamento delle immagini"'
description: Introduzione e rapida alle dimensioni dell’immagine per aiutarti a iniziare rapidamente a usare le tecniche di dimensionamento dell’immagine.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 56%

---


# Avvio rapido: ridimensionamento delle immagini{#quick-start-image-sizing}

Il dimensionamento dell&#39;immagine si riferisce alla capacità di Dynamic Media Classic di creare più immagini derivate basate su un&#39;unica immagine ad alta risoluzione. Invece di creare manualmente diverse immagini (ad esempio, una miniatura e un’immagine ingrandita) per il sito Web o l’applicazione, fornisci un’unica immagine principale. Dynamic Media Classic genera tutte le immagini modificate come richiesto. I vantaggi di poter offrire immagini in modo dinamico da una singola immagine originale sono notevoli:

* Non è necessario creare manualmente più copie dell’immagine in diversi formati. Fornisci un’immagine principale a Dynamic Media Classic e Dynamic Media Classic genera derivati di dimensioni diverse dall’immagine principale.
* Potete rapidamente modificare le dimensioni di un tipo di immagine usato nell’intero sito Web o nell’applicazione. Ad esempio, per modificare tutte le miniature, è sufficiente modificare il relativo predefinito. Un predefinito per immagini, paragonabile a una macro, consiste in un insieme di attributi di dimensione e formattazione. Per modificare la dimensione di tutte le miniature nel sito Web o nell’applicazione, potete modificare il predefinito per immagini “Miniatura”.
* Non è necessario gestire le immagini originali e tutte le varie immagini derivate nei vari sistemi di gestione di contenuti e risorse interni o esterni.

![È possibile creare più immagini derivate di dimensioni diverse dallo stesso file master ad alta risoluzione.](/help/assets/is_derivative_sizes_popup.png)

**Guida introduttiva**

Questa guida rapida alle dimensioni delle immagini è stata progettata per aiutarti a iniziare rapidamente a usare le tecniche di dimensionamento delle immagini in Dynamic Media Classic. Segui i punti da 1 a 5. Inoltre, per ogni passaggio è riportato un riferimento incrociato in cui potete trovare ulteriori informazioni.

**1. Caricamento delle immagini originali**

Per iniziare, carica le immagini principali in Dynamic Media Classic. Per quanto riguarda le dimensioni, Dynamic Media Classic consiglia di utilizzare immagini di dimensioni maggiori che si prevede di utilizzare sul sito Web o sull&#39;applicazione. Ad esempio, se desiderate che gli utenti possano eseguire uno zoom sulle immagini, caricate immagini di cui il lato maggiore sia di almeno 2000 pixel. Dynamic Media Classic supporta molti formati di file immagine, ma si consiglia di utilizzare immagini TIFF e PNG senza perdita di dati.

Seleziona il pulsante Carica nella barra di navigazione globale per caricare i file dal computer in una cartella in Dynamic Media Classic. Consultate [Caricamento delle immagini originali](uploading-master-images.md#uploading_master_images).

**2. Configurazione dei predefiniti immagine**

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Un predefinito per immagini regola le dimensioni e la formattazione con cui le immagini vengono distribuite dai server di immagini Dynamic Media. Se siete amministratori della società, potete configurare i predefiniti per immagini voi stessi. Dynamic Media Classic viene fornito anche con predefiniti per immagini predefiniti e può essere utilizzato per distribuire dinamicamente le immagini.

Per creare una predefinito per immagini, scegliete Configurazione > Impostazione applicazione (se siete amministratore). Nella schermata Configurazione, visualizzate le opzioni di impostazione dell’applicazione e scegliete Predefiniti immagine. Quindi fai clic su **Aggiungi** o **Modifica** per creare un predefinito per immagini.

Il predefinito per immagini creato viene aggiunto al menu Predefinito immagine della schermata Anteprima. Potete usare il nuovo predefinito per immagini per visualizzare le immagini sui siti Web e sulle applicazioni in modo dinamico. Consultate [Configurazione dei predefiniti per immagini](setting-image-presets.md#setting_up_image_presets).

**3. Anteprima dei predefiniti per immagini**

La fase successiva consiste nel visualizzare l’anteprima dei predefiniti per immagini configurati dall’amministratore nelle varie dimensioni.

Per esplorare i predefiniti immagine, fai clic su **Configurazione** > **Predefiniti immagine**, quindi seleziona un predefinito immagine.

Provate i vari predefiniti per immagini per vedere come si presenta l’immagine quando viene trasmessa in modo dinamico sul sito Web o sull’applicazione in dimensioni diverse. 

Consultate [Anteprima di una risorsa immagine basata sul suo predefinito per immagini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Pubblicazione delle immagini originali**

La pubblicazione dei file immagine originali ha due scopi fondamentali:

* Pubblicazione delle immagini master sui server di immagini Dynamic Media in modo che le immagini possano essere distribuite in modo dinamico al sito Web e all’applicazione.
* La pubblicazione attiva le stringhe URL per richiamare le immagini dai server immagini Dynamic Media al sito Web o all&#39;applicazione. Dopo la pubblicazione, puoi copiare e inserire gli URL generati da Dynamic Media Classic, se necessario, nel sito web o nell’applicazione.

Per avviare una pubblicazione, fate clic sul pulsante Pubblica nella barra di navigazione globale. Nella schermata Pubblica, fate clic sul pulsante Avvia pubblicazione. Consultate [Pubblicazione delle immagini originali](publishing-master-images.md#publishing_master_images).

**5. Collegamento degli URL all’applicazione Web**

Dynamic Media Classic crea stringhe di callout URL per le immagini. Quando pubblichi le immagini sui server di immagini Dynamic Media, gli URL diventano attivi. Potete copiare queste stringhe URL dal pannello Sfoglia (in visualizzazione Dettagli) o dalla schermata Anteprima. Dopo aver copiato le stringhe URL, potete usarle nel sito Web o nelle applicazioni. Nel codice della pagina Web, l’URL per il ridimensionamento delle immagini sostituisce il riferimento al nome di un’immagine statica. L’URL fa riferimento al nome di un’immagine originale, che verrà sostituito dal database per ciascuna immagine nuova da visualizzare.

Le stringhe URL generate tramite Predefiniti immagine contengono il nome di un predefinito per immagini. Il nome è racchiuso tra simboli di dollaro (`$`). Ad esempio, `$thumbnail$` può essere il predefinito per immagini progettato per mostrare le immagini master con le dimensioni delle miniature. Consultate [Collegamento degli URL all’applicazione Web](linking-urls-web-application.md#linking_urls_to_your_web_application).
