---
title: Utilizzare i file PSD
description: Scopri come lavorare con i file PSD in Adobe Dynamic Media Classic.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 28%

---

# Utilizzare i file PSD{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

I file PSD (Photoshop Document Files) sono utilizzati più spesso in Adobe Dynamic Media Classic per creare i modelli. Quando carichi un file PSD, puoi creare automaticamente un modello Adobe Dynamic Media Classic dal file (seleziona l’opzione Crea modello nella schermata Carica ).

Ad Adobe, Dynamic Media Classic crea più immagini da un file PSD con livelli se utilizzi il file per creare un modello; crea un&#39;immagine per ogni livello.

## Opzioni di caricamento PSD {#psd-upload-options}

Le opzioni per il caricamento di file PSD si trovano in Opzioni Photoshop nella finestra di dialogo Opzioni processo di caricamento. Potete ritagliare un file, scegliere un profilo colore, usare il file per creare un modello e selezionare un ancoraggio.

Quando si carica un file PSD sono disponibili le seguenti opzioni:

* **Opzioni**  di ritaglio - Situato in Opzioni  **[!UICONTROL di ritaglio]**. Selezionare **[!UICONTROL Trim]** per ritagliare automaticamente lo spazio bianco dai bordi di un file PSD; selezionare **[!UICONTROL Manuale]** per ritagliare i lati del file PSD:

   * **[!UICONTROL Taglia]**  - Selezionate il menu di  **[!UICONTROL scelta rapida basato su]** rifilo e scegliete  **** Colore  **[!UICONTROL trasparenza]**.

      Se scegli l&#39;opzione **[!UICONTROL Colore]**, seleziona il menu Angolo e scegli l&#39;angolo della PSD con il colore che rappresenta meglio lo spazio bianco da ritagliare.

      Trascinare il cursore per specificare una tolleranza da 0 a 1. Per rifilare in base al colore, l’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo del file PSD. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. Per tagliare in base alla trasparenza, specificare 0 per ritagliare i pixel solo se sono trasparenti; numeri più vicini a 1 assicurano una maggiore trasparenza.

   * **[!UICONTROL Manuale]** : immetti il numero di pixel da ritagliare da qualsiasi lato o lato dell’immagine. La quantità di immagine che viene ritagliata dipende dall’impostazione ppi (pixel per pollice) nel file immagine. Ad esempio, se l’immagine viene visualizzata a 150 ppi e immettete 75 nelle caselle di testo, viene ritagliato mezzo pollice da ogni lato dell’immagine.

* **Opzioni**  del profilo colore: si trova in Opzioni  **[!UICONTROL del profilo colore]**.

   * **[!UICONTROL Mantenimento colore predefinito]**

   * **[!UICONTROL Mantieni spazio colore originale]** : mantiene lo spazio colore originale dell&#39;immagine.

   * **[!UICONTROL Personalizzato da]**  >  **[!UICONTROL a]** : apre i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. È possibile scegliere uno spazio colore Photoshop standard o uno spazio colore caricato in Adobe Dynamic Media Classic. Consultate [Profili ICC](/help/icc-profiles.md).

* **Opzioni Photoshop**

   * **[!UICONTROL Gestisci livelli]** : consente di rimuovere gli eventuali livelli del file PSD in singole risorse. I livelli delle risorse restano associati al file PSD. Per visualizzarli, aprite il file PSD in Vista dettagli e selezionate il pannello dei livelli. Consultate Visualizzazione e modifica dei livelli in un file PSD.

   * **[!UICONTROL Crea modello]** : crea un modello dai livelli nel file PSD.

   * **[!UICONTROL Estrai testo]** : estrae il testo in modo che gli utenti possano cercare il testo in un visualizzatore.

   * **[!UICONTROL Estendi i livelli alle dimensioni dello sfondo]** : consente di estendere le dimensioni dei livelli immagine ritagliati alle dimensioni del livello di sfondo.

   * **[!UICONTROL Denominazione livello]** : i livelli nel file PSD vengono caricati come immagini separate. Per assegnare un nome a queste immagini in Adobe Dynamic Media Classic, scegli tra le seguenti opzioni:

      * **[!UICONTROL Nome livello]** : assegna un nome alle immagini dopo i loro nomi di livello nel file PSD. Ad esempio, un livello denominato Price Tag nel file PSD originale diventa un’immagine denominata Price Tag. Tuttavia, se i nomi dei livelli nel file PSD sono nomi di livello Photoshop predefiniti (Sfondo, Livello 1, Livello 2 e così via), le immagini vengono denominate in base ai numeri dei rispettivi livelli nel file PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop e numero]**  di livello: assegna un nome alle immagini dopo i numeri di livello nel file PSD, ignorando i nomi di livello originali. Le immagini vengono denominate con il nome file di Photoshop a cui viene aggiunto un numero di livello. Ad esempio, il secondo livello di un file denominato `Spring Ad.psd` viene denominato `Spring Ad_2` anche se in Photoshop è presente un nome non predefinito.

      * **[!UICONTROL Photoshop e nome del livello]** : assegna un nome alle immagini dopo il file PSD seguito dal nome del livello o dal numero del livello. Il numero del livello viene usato se il livello nel file PSD ha un nome predefinito di Photoshop. Ad esempio, un livello denominato `Price Tag` in un file PSD denominato `SpringAd` viene denominato `Spring Ad_Price Tag`. Un livello con il nome predefinito Livello 2 è denominato `Spring Ad_2`.
   * **[!UICONTROL Ancoraggio]**  - Consente di specificare il modo in cui le immagini vengono ancorate nei modelli generati dalla composizione a livelli prodotta dal file PSD. Per impostazione predefinita, la posizione di ancoraggio è al centro. L’ancoraggio centrale permette alle immagini sostitutive di riempire in modo ottimale lo spazio, indipendentemente dalle loro proporzioni. In questo modo, facendo riferimento al modello e utilizzano la sostituzione mediante parametri, le immagini sostitutive con proporzioni diverse occupano lo stesso spazio in modo efficace. Usate un’impostazione diversa se la vostra applicazione richiede che le immagini sostitutive riempiano lo spazio allocato nel modello.


## Visualizzare e modificare i livelli in un file PSD {#viewing-and-editing-layers-in-a-psd-file}

Se hai selezionato l’opzione Mantieni livelli al momento del caricamento del file PSD, Adobe Dynamic Media Classic ha suddiviso i singoli livelli in risorse. Per visualizzare e modificare i livelli delle risorse appartenenti a un file PSD, aprite il file nel pannello Sfoglia in visualizzazione Dettagli.

1. Fare doppio clic sul file PSD completo nel pannello Sfoglia. Il file viene aperto in Vista dettagli.

   >[!NOTE]
   >
   >assicuratevi di aprire la risorsa completa e non uno dei livelli del file PSD.

1. Selezionare **[!UICONTROL Livelli]**. Nel pannello Livelli, tutti i livelli sono riportati come immagini a sé stanti.
1. Fate doppio clic su un livello ed effettuate una delle seguenti operazioni:

   * Per creare una mappa immagine sul livello, seleziona l’icona **[!UICONTROL Mappa immagine]** . (Consulta [Creare mappe immagine](creating-image-maps.md#creating_image_maps).)
   * Per creare le destinazioni di zoom sul livello, seleziona l’icona **[!UICONTROL Destinazioni di zoom]** . (Consultare [Creazione di destinazioni di zoom per Zoom guidato](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Per ritagliare il livello, seleziona l’icona **[!UICONTROL Ritaglia]** . (Vedere [Ritagliare un&#39;immagine](cropping-image.md#cropping_an_image).)
   * Per aumentare l&#39;nitidezza del livello, selezionare **[!UICONTROL Nitidezza]**. (Consultare [Nitidezza di un&#39;immagine](sharpening-image.md#sharpening_an_image).)
   * Per regolare il livello, selezionare **[!UICONTROL Regola]**. (Consultare [Regolare un&#39;immagine](adjusting-image.md#adjusting_an_image).)

1. Selezionare **[!UICONTROL Salva]** o **[!UICONTROL Salva con nome]**.
1. Per visualizzare o modificare un livello diverso, selezionate una freccia nella parte inferiore dell’anteprima del livello.
1. Per uscire dalla Vista dettagli livello, selezionare l&#39;icona **[!UICONTROL Vista griglia]**.
