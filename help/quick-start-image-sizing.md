---
title: '"Avvio rapido: ridimensionamento delle immagini"'
seo-title: '"Avvio rapido: ridimensionamento delle immagini"'
description: 'null'
seo-description: Introduzione e avvio rapido al ridimensionamento delle immagini per imparare a usare rapidamente le tecniche di ridimensionamento delle immagini.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 56%

---


# Avvio rapido: ridimensionamento delle immagini{#quick-start-image-sizing}

Per ridimensionamento delle immagini si intende la capacità di Dynamic Media Classic di creare più immagini derivate da un’unica immagine ad alta risoluzione. Invece di creare manualmente diverse immagini per il sito Web o l’applicazione, ad esempio una miniatura e un’immagine ingrandita, potete fornire una singola immagine originale. Dynamic Media Classic genera tutte le immagini modificate come richiesto. I vantaggi di poter offrire immagini in modo dinamico da una singola immagine originale sono notevoli:

* Non è necessario creare manualmente più copie dell’immagine in diversi formati. Potete fornire un’immagine principale ad Dynamic Media Classic e Dynamic Media Classic genera derivati di dimensioni diverse dall’immagine principale.
* Potete rapidamente modificare le dimensioni di un tipo di immagine usato nell’intero sito Web o nell’applicazione. Ad esempio, per modificare tutte le miniature, è sufficiente modificare il relativo predefinito. Un predefinito per immagini, paragonabile a una macro, consiste in un insieme di attributi di dimensione e formattazione. Per modificare la dimensione di tutte le miniature nel sito Web o nell’applicazione, potete modificare il predefinito per immagini “Miniatura”.
* Non è necessario gestire le immagini originali e tutte le varie immagini derivate nei vari sistemi di gestione di contenuti e risorse interni o esterni.

![Potete creare più immagini derivate di dimensioni diverse dallo stesso file principale ad alta risoluzione.](/help/assets/is_derivative_sizes_popup.png)

**Avvio rapido**

Questa sezione è stata progettata come punto di partenza per imparare a usare le funzioni di ridimensionamento delle immagini di Dynamic Media Classic. Seguite i passaggi da 1 a 5. Inoltre, per ogni passaggio è riportato un riferimento incrociato in cui potete trovare ulteriori informazioni.

**1. Caricamento delle immagini originali**

Per iniziare, caricate le immagini originali in Dynamic Media Classic. Per quanto riguarda le dimensioni, Dynamic Media Classic consiglia di utilizzare immagini delle dimensioni maggiori che si prevede di utilizzare sul sito Web o l&#39;applicazione. Ad esempio, se desiderate che gli utenti possano eseguire uno zoom sulle immagini, caricate immagini di cui il lato maggiore sia di almeno 2000 pixel. Dynamic Media Classic supporta molti formati di file immagine, ma si consigliano immagini senza perdita di dati TIFF e PNG.

Per caricare i file dal computer a una cartella di Dynamic Media Classic, fate clic sul pulsante Carica nella barra di navigazione globale. Consultate [Caricamento delle immagini originali](uploading-master-images.md#uploading_master_images).

**2. Configurazione dei predefiniti immagine**

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Un predefinito per immagini regola le dimensioni e la formattazione con cui le immagini vengono trasmesse dai server immagini di Dynamic Media. Se siete amministratori della società, potete configurare i predefiniti per immagini voi stessi. Dynamic Media Classic viene fornito anche con predefiniti per immagini predefiniti che potete usare per distribuire le immagini in modo dinamico.

Per creare una predefinito per immagini, scegliete Configurazione > Impostazione applicazione (se siete amministratore). Nella schermata Configurazione, visualizzate le opzioni di impostazione dell’applicazione e scegliete Predefiniti immagine. Fate clic su **Aggiungi** o **Modifica** per creare un predefinito per immagini.

Il predefinito per immagini creato viene aggiunto al menu Predefinito immagine della schermata Anteprima. Potete usare il nuovo predefinito per immagini per visualizzare le immagini sui siti Web e sulle applicazioni in modo dinamico. Consultate [Configurazione dei predefiniti per immagini](setting-image-presets.md#setting_up_image_presets).

**3. Anteprima dei predefiniti per immagini**

La fase successiva consiste nel visualizzare l’anteprima dei predefiniti per immagini configurati dall’amministratore nelle varie dimensioni.

To explore Image Presets, click **Setup** > **Image Presets**, and then browse to an Image Preset.

Provate i vari predefiniti per immagini per vedere come si presenta l’immagine quando viene trasmessa in modo dinamico sul sito Web o sull’applicazione in dimensioni diverse. 

Consultate [Anteprima di una risorsa immagine basata sul suo predefinito per immagini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Pubblicazione delle immagini originali**

La pubblicazione dei file immagine originali ha due scopi fondamentali:

* Pubblicare le immagini originali sui server immagini Dynamic Media in modo che possano essere distribuite in modo dinamico al sito Web e all’applicazione.
* Con la pubblicazione vengono attivate le stringhe URL necessarie per trasmettere le immagini dai server immagini Dynamic Media al sito Web o all’applicazione. Dopo la pubblicazione, potete copiare e inserire gli URL generati da Dynamic Media Classic, se necessario, nel sito Web o nell’applicazione.

Per avviare una pubblicazione, fate clic sul pulsante Pubblica nella barra di navigazione globale. Nella schermata Pubblica, fate clic sul pulsante Avvia pubblicazione. Consultate [Pubblicazione delle immagini originali](publishing-master-images.md#publishing_master_images).

**5. Collegamento degli URL all’applicazione Web**

Dynamic Media Classic crea le stringhe URL per richiamare le immagini. Quando pubblicate le immagini sui server immagini Dynamic Media, gli URL diventano attivi. Potete copiare queste stringhe URL dal pannello Sfoglia (in visualizzazione Dettagli) o dalla schermata Anteprima. Dopo aver copiato le stringhe URL, potete usarle nel sito Web o nelle applicazioni. Nel codice della pagina Web, l’URL per il ridimensionamento delle immagini sostituisce il riferimento al nome di un’immagine statica. L’URL fa riferimento al nome di un’immagine originale, che verrà sostituito dal database per ciascuna immagine nuova da visualizzare.

Le stringhe URL generate tramite Predefiniti immagine contengono il nome di un predefinito per immagini. Il nome è racchiuso tra simboli di dollaro (`$`). For example, `$thumbnail$` can be the Image Preset designed to show master images at thumbnail size. Consultate [Collegamento degli URL all’applicazione Web](linking-urls-web-application.md#linking_urls_to_your_web_application).
