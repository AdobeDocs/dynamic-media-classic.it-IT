---
title: Operazioni con i file PSD
description: Scopri come utilizzare i file PSD in Adobe Dynamic Media Classic.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: dc1ec666b208cec8fffe836d64ed501f6ccf4e7b
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 25%

---

# Operazioni con i file PSD{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD (file di documenti Photoshop) viene utilizzato più spesso in Adobe Dynamic Media Classic per creare modelli. Quando carichi un file PSD, puoi creare automaticamente un modello Adobe Dynamic Media Classic dal file (seleziona l’opzione Crea modello nella schermata Carica ).

Adobe Dynamic Media Classic crea più immagini da un file PSD con livelli se utilizzi il file per creare un modello; crea un&#39;immagine per ogni livello.

## Opzioni di caricamento PSD {#psd-upload-options}

Le opzioni per il caricamento di file PSD si trovano in Opzioni Photoshop nella finestra di dialogo Opzioni processo di caricamento. Potete ritagliare un file, scegliere un profilo colore, usare il file per creare un modello e selezionare un ancoraggio.

Quando si carica un file PSD sono disponibili le seguenti opzioni:

* **Opzioni di ritaglio** - Situato in **[!UICONTROL Opzioni di ritaglio]**. Seleziona **[!UICONTROL Rifila]** ritagliare automaticamente lo spazio bianco dai bordi di un file PSD; select **[!UICONTROL Manuale]** per ritagliare i lati del file PSD:

   * **[!UICONTROL Rifila]** - Seleziona la **[!UICONTROL Rifila in base a]** e scegli **[!UICONTROL Colore]** o **[!UICONTROL Trasparenza]**.
   Se scegli la **[!UICONTROL Colore]** selezionate il menu Angolo (Corner) e scegliete l’angolo del PSD con il colore che rappresenta meglio lo spazio bianco da ritagliare.

   Trascinare il cursore per specificare una tolleranza da 0 a 1. Per rifilare in base al colore, l’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo del file PSD. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. Per tagliare in base alla trasparenza, specificare 0 per ritagliare i pixel solo se sono trasparenti; numeri più vicini a 1 assicurano una maggiore trasparenza.

   * **[!UICONTROL Manuale]** - Immettere il numero di pixel da ritagliare da qualsiasi lato o lato dell&#39;immagine. La quantità di immagine che viene ritagliata dipende dall’impostazione ppi (pixel per pollice) nel file immagine. Ad esempio, se l’immagine viene visualizzata a 150 ppi e immetti 75 nelle caselle di testo In alto, A destra, In basso e A sinistra, 0,5 pollici. viene ritagliato da ogni lato dell&#39;immagine.


* **Opzioni del profilo colore** - Situato in **[!UICONTROL Opzioni del profilo colore]**.

   * **[!UICONTROL Mantenimento colore predefinito]**

   * **[!UICONTROL Mantieni spazio colore originale]** - Mantiene lo spazio colore originale dell&#39;immagine.

   * **[!UICONTROL Personalizzato da]** > **[!UICONTROL A]** - Apre i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore Photoshop standard o uno spazio colore caricato su Adobe Dynamic Media Classic. Consultate [Profili ICC](/help/icc-profiles.md).

* **Opzioni Photoshop**

   * **[!UICONTROL Gestisci livelli]** - Racchiude gli eventuali livelli in PSD in singole risorse. I livelli delle risorse restano associati al file PSD. Per visualizzarli, aprite il file PSD in Vista dettagli e selezionate il pannello dei livelli. Consultate Visualizzazione e modifica dei livelli in un file PSD.

   * **[!UICONTROL Crea modello]** - Crea un modello dai livelli nel file PSD.

   * **[!UICONTROL Estrai testo]** - Estrae il testo in modo che gli utenti possano cercare il testo in un visualizzatore.

   * **[!UICONTROL Estendi i livelli alle dimensioni dello sfondo]** - Estende le dimensioni dei livelli immagine strappati alle dimensioni del livello di sfondo.

   * **[!UICONTROL Denominazione dei livelli]** - I livelli nel file PSD vengono caricati come immagini separate. Per denominare queste immagini in Adobe Dynamic Media Classic, scegli una delle seguenti opzioni:

      * **[!UICONTROL Nome livello]** - Assegna un nome alle immagini dopo i relativi nomi di livello nel file PSD. Ad esempio, un livello denominato Price Tag nel file PSD originale diventa un’immagine denominata Price Tag. Tuttavia, se i nomi dei livelli nel file PSD sono nomi di livello Photoshop predefiniti (Sfondo, Livello 1, Livello 2 e così via), le immagini vengono denominate in base ai numeri dei rispettivi livelli nel file PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop e numero di livello]** - Assegna un nome alle immagini dopo i relativi numeri di livello nel file PSD, ignorando i nomi dei livelli originali. Le immagini vengono denominate con il nome file di Photoshop a cui viene aggiunto un numero di livello. Ad esempio, il secondo livello di un file denominato `Spring Ad.psd` è denominato `Spring Ad_2` anche se aveva un nome non predefinito in Photoshop.

      * **[!UICONTROL Nome Photoshop e livello]** - Assegna un nome alle immagini dopo il file PSD seguito dal nome del livello o dal numero del livello. Il numero del livello viene usato se il livello nel file PSD ha un nome predefinito di Photoshop. Ad esempio, un livello denominato `Price Tag` in un file PSD denominato `SpringAd` è denominato `Spring Ad_Price Tag`. Viene chiamato un livello con il nome predefinito Livello 2 `Spring Ad_2`.
   * **[!UICONTROL Ancoraggio]** - Specificare il modo in cui le immagini vengono ancorate nei modelli generati dalla composizione a livelli prodotta dal file PSD. Per impostazione predefinita, la posizione di ancoraggio è al centro. L’ancoraggio centrale permette alle immagini sostitutive di riempire in modo ottimale lo spazio, indipendentemente dalle loro proporzioni. In questo modo, facendo riferimento al modello e utilizzano la sostituzione mediante parametri, le immagini sostitutive con proporzioni diverse occupano lo stesso spazio in modo efficace. Usate un’impostazione diversa se la vostra applicazione richiede che le immagini sostitutive riempiano lo spazio allocato nel modello.


## Visualizzare e modificare i livelli in un file PSD {#viewing-and-editing-layers-in-a-psd-file}

Se hai selezionato l’opzione Mantieni livelli al momento del caricamento del PSD, Adobe Dynamic Media Classic suddivideva i singoli livelli in risorse. Per visualizzare e modificare i livelli delle risorse appartenenti a un file PSD, apri il file nel pannello Sfoglia in visualizzazione Dettagli.

>[!NOTE]
>
>Adobe Dynamic Media Classic supporta fino a cinque livelli in un gruppo di livelli nidificato.

1. Fare doppio clic sul file PSD completo nel pannello Sfoglia. Il file viene aperto in Vista dettagli.

   >[!NOTE]
   >
   >assicuratevi di aprire la risorsa completa e non uno dei livelli del file PSD.

1. Seleziona **[!UICONTROL Livelli]**. Nel pannello Livelli, tutti i livelli sono riportati come immagini a sé stanti.
1. Fate doppio clic su un livello ed effettuate una delle seguenti operazioni:

   * Per creare una mappa immagine sul livello, seleziona **[!UICONTROL Mappa immagine]** icona. (Vedi [Creare mappe immagine](creating-image-maps.md#creating_image_maps).)
   * Per creare le destinazioni di zoom sul livello, seleziona **[!UICONTROL Destinazioni di zoom]** icona. (Vedi [Creare destinazioni di zoom per lo zoom guidato](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Per ritagliare il livello, selezionate **[!UICONTROL Ritaglio]** icona. (Vedi [Ritagliare un’immagine](cropping-image.md#cropping_an_image).)
   * Per aumentare l’nitidezza del livello, selezionate **[!UICONTROL Nitidezza]**. (Vedi [Rendere più nitida un’immagine](sharpening-image.md#sharpening_an_image).)
   * Per regolare il livello, selezionate **[!UICONTROL Regola]**. (Vedi [Regolare un’immagine](adjusting-image.md#adjusting_an_image).)

1. Seleziona **[!UICONTROL Salva]** o **[!UICONTROL Salva con nome]**.
1. Per visualizzare o modificare un livello diverso, selezionate una freccia nella parte inferiore dell’anteprima del livello.
1. Per uscire dalla Vista dettagli livello, selezionate la **[!UICONTROL Vista a griglia]** icona.
