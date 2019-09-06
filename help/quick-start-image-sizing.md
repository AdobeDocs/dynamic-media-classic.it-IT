---
title: '"Avvio rapido: ridimensionamento delle immagini"'
seo-title: '"Avvio rapido: ridimensionamento delle immagini"'
description: 'null'
seo-description: Introduzione e Avvio rapido al ridimensionamento delle immagini per imparare a usare le tecniche di ridimensionamento delle immagini.
uuid: 6 c 4 ad 4 b 7-549 d -4 daa-b 6 b 9-5997 a 8427 af 8
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/image_ sizing
discoiquuid: dcaa 9 b 21-b 925-4 dbb -865 e -7918 cdbda 50 c
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Avvio rapido: ridimensionamento delle immagini{#quick-start-image-sizing}

Il ridimensionamento delle immagini si riferisce alla capacità di Dynamic Media Classic di creare più immagini derivate in base a una singola immagine ad alta risoluzione. Invece di creare manualmente diverse immagini, ad esempio una miniatura e un'immagine ingrandita, per il sito Web o l'applicazione, fornite una singola immagine originale. Dynamic Media Classic genera tutte le immagini modificate come richiesto. I vantaggi di poter offrire immagini in modo dinamico da una singola immagine originale sono notevoli:

* Non è necessario creare manualmente più copie dell’immagine in diversi formati. Fornite un'immagine principale a Dynamic Media Classic, mentre Dynamic Media Classic genera derivati diversi da quelli dell'immagine principale.
* Potete rapidamente modificare le dimensioni di un tipo di immagine usato nell’intero sito Web o nell’applicazione. Ad esempio, per modificare tutte le miniature, è sufficiente modificare il relativo predefinito. Un predefinito per immagini, paragonabile a una macro, consiste in un insieme di attributi di dimensione e formattazione. Per modificare la dimensione di tutte le miniature nel sito Web o nell’applicazione, potete modificare il predefinito per immagini “Miniatura”.
* Non è necessario gestire le immagini originali e tutte le varie immagini derivate nei vari sistemi di gestione di contenuti e risorse interni o esterni.

![Potete creare più immagini derivate in dimensioni diverse dallo stesso file principale ad alta risoluzione.](/help/assets/is_derivative_sizes_popup.png)

**Avvio rapido**

Questa sezione è stata progettata per punto di partenza per imparare a usare le funzioni di ridimensionamento rapido delle immagini in Scene7 Publishing System. Seguite i passaggi da a. Inoltre, per ogni passaggio è riportato un riferimento incrociato in cui potete trovare ulteriori informazioni.

**1. Caricamento delle immagini originali**

Per iniziare, caricate le immagini originali in Scene7 Publishing System. Per le dimensioni, Dynamic Media Classic consiglia di usare immagini che sono la dimensione più grande prevista utilizzando nel sito Web o nell'applicazione. Ad esempio, se desiderate che gli utenti possano eseguire uno zoom sulle immagini, caricate immagini di cui il lato maggiore sia di almeno 2000 pixel. Dynamic Media Classic supporta molti formati di file immagine, ma si consiglia di usare immagini senza perdita di dati TIFF e PNG.

Per caricare il file dal computer a una cartella del Scene7 Publishing System, fate clic sul pulsante Carica nella barra di navigazione globale. Consultate [Caricamento delle immagini originali](uploading-master-images.md#uploading_master_images).

**2. Configurazione dei predefiniti immagine**

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Un predefinito per immagini regola le dimensioni e la formattazione con cui le immagini vengono trasmesse dai server immagini Dynamic Media. Se siete amministratori della società, potete configurare i predefiniti per immagini voi stessi. Dynamic Media Classic viene fornito anche con predefiniti per immagini predefiniti, che potete usare per distribuire in modo dinamico immagini.

Per creare una predefinito per immagini, scegliete Configurazione &gt; Impostazione applicazione (se siete amministratore). Nella schermata Configurazione, visualizzate le opzioni di impostazione dell’applicazione e scegliete Predefiniti immagine. Quindi fate clic **su Aggiungi** o **Modifica** per creare un predefinito per immagini.

Il predefinito per immagini creato viene aggiunto al menu Predefinito immagine della schermata Anteprima. Potete usare il nuovo predefinito per immagini per visualizzare le immagini sui siti Web e sulle applicazioni in modo dinamico. Consultate [Configurazione dei predefiniti per immagini](setting-image-presets.md#setting_up_image_presets).

**3. Anteprima dei predefiniti per immagini**

La fase successiva consiste nel visualizzare l’anteprima dei predefiniti per immagini configurati dall’amministratore nelle varie dimensioni.

To explore Image Presets, click **Setup** &gt; **Image Presets**, and then browse to an Image Preset.

Provate i vari predefiniti per immagini per vedere come si presenta l’immagine quando viene trasmessa in modo dinamico sul sito Web o sull’applicazione in dimensioni diverse. 

Consultate [Anteprima di una risorsa immagine basata sul suo predefinito per immagini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Pubblicazione delle immagini originali**

La pubblicazione dei file immagine originali ha due scopi fondamentali:

* Pubblicare le immagini originali nei server immagini per contenuti multimediali dinamici in modo che le immagini possano essere distribuite in modo dinamico al sito Web e all'applicazione.
* La pubblicazione attiva le stringhe URL per la chiamata delle immagini dai server immagini Dynamic Media al sito Web o all'applicazione. Dopo la pubblicazione, potete copiare e inserire gli URL generati da Dynamic Media Classic nel sito Web o nell'applicazione.

Per avviare una pubblicazione, fate clic sul pulsante Pubblica nella barra di navigazione globale. Nella schermata Pubblica, fate clic sul pulsante Avvia pubblicazione. Consultate [Pubblicazione delle immagini originali](publishing-master-images.md#publishing_master_images).

**5. Collegamento degli URL all’applicazione Web**

Dynamic Media Classic crea stringhe URL per le immagini. Quando pubblicate le immagini su server di immagini multimediali dinamici, gli URL diventano attivi. Potete copiare queste stringhe URL dal pannello Sfoglia (in visualizzazione Dettagli) o dalla schermata Anteprima. Dopo aver copiato le stringhe URL, potete usarle nel sito Web o nelle applicazioni. Nel codice della pagina Web, l’URL per il ridimensionamento delle immagini sostituisce il riferimento al nome di un’immagine statica. L’URL fa riferimento al nome di un’immagine originale, che verrà sostituito dal database per ciascuna immagine nuova da visualizzare.

Le stringhe URL generate tramite Predefiniti immagine contengono il nome di un predefinito per immagini. Il nome è racchiuso tra simboli di dollaro (`$`). For example, `$thumbnail$` can be the Image Preset designed to show master images at thumbnail size. Consultate [Collegamento degli URL all’applicazione Web](linking-urls-web-application.md#linking_urls_to_your_web_application).
