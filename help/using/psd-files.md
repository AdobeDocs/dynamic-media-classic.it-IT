---
title: Utilizzare i file PSD
description: Scopri come utilizzare i file PSD in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 21%

---

# Utilizzare i file PSD{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

I PSD (Photoshop Document Files) vengono spesso utilizzati in Adobe Dynamic Media Classic per la creazione di modelli. Quando carichi un file PSD, puoi creare automaticamente un modello Adobe Dynamic Media Classic dal file (seleziona l’opzione Crea modello nella schermata Carica).

Adobe Dynamic Media Classic crea più immagini da un file PSD con livelli se utilizzate il file per creare un modello; crea un&#39;immagine per ogni livello.

## Opzioni di caricamento PSD {#psd-upload-options}

Le opzioni per il caricamento di file PSD si trovano in Opzioni Photoshop nella finestra di dialogo Opzioni processo di caricamento. Potete ritagliare un file, scegliere un profilo colore, usare il file per creare un modello e selezionare un ancoraggio.

Quando si carica un file PSD sono disponibili le seguenti opzioni:

* **Opzioni ritaglio**: si trova in **[!UICONTROL Opzioni ritaglio]**. Seleziona **[!UICONTROL Taglia]** per ritagliare automaticamente lo spazio vuoto dai bordi di un file PSD. Selezionare **[!UICONTROL Manuale]** per ritagliare i lati del file PSD:

   * **[!UICONTROL Rifila]**: seleziona il menu **[!UICONTROL Rifila in base a]** e scegli **[!UICONTROL Colore]** o **[!UICONTROL Trasparenza]**.

  Se si sceglie l&#39;opzione **[!UICONTROL Colore]**, selezionare il menu Angolo e scegliere l&#39;angolo del PSD con il colore che meglio rappresenta il colore dello spazio bianco da ritagliare.

  Trascinate il cursore per specificare una tolleranza da 0 a 1. Per rifilare in base al colore, l’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo del file PSD. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. Per tagliare in base alla trasparenza, specificate 0 per ritagliare i pixel solo se sono trasparenti; i numeri più vicini a 1 consentono una maggiore trasparenza.

   * **[!UICONTROL Manuale]**: immettere il numero di pixel da ritagliare da un lato o da un lato dell&#39;immagine. La quantità di immagine che viene ritagliata dipende dall’impostazione ppi (pixel per pollice) nel file immagine. Si supponga, ad esempio, che l&#39;immagine visualizzi 150 ppi. Immettere 75 nelle caselle di testo Superiore, Destra, Inferiore e Sinistra. Ogni lato dell&#39;immagine viene ritagliato, 0,5 pollici.

* **Opzioni profilo colori**: si trova in **[!UICONTROL Opzioni profilo colori]**.

   * **[!UICONTROL Conservazione colore predefinita]**

   * **[!UICONTROL Mantieni spazio colore originale]**: mantiene lo spazio colore originale dell&#39;immagine.

   * **[!UICONTROL Personalizza da]** > **[!UICONTROL A]**: apre i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore standard di Photoshop o uno spazio colore caricato in Adobe Dynamic Media Classic. Consultate [Profili ICC](/help/using/icc-profiles.md).

* **Opzioni Photoshop**

   * **[!UICONTROL Mantieni livelli]**: esegue il riping dei livelli nel PSD, se presenti, in singole risorse. I livelli delle risorse restano associati al file PSD. Per visualizzarli, aprite il file PSD in Vista dettagli (Detail View) e selezionate il pannello dei livelli. Consultate Visualizzare e modificare i livelli in un file PSD.

   * **[!UICONTROL Crea modello]**: crea un modello dai livelli nel file PSD.

   * **[!UICONTROL Estrai testo]**: estrae il testo in modo che gli utenti possano cercare il testo in un visualizzatore.

   * **[!UICONTROL Estendi livelli alle dimensioni di sfondo]**: estende le dimensioni dei livelli immagine copiati da CD alle dimensioni del livello di sfondo.

   * **[!UICONTROL Denominazione livelli]**: i livelli nel file PSD vengono caricati come immagini separate. Per denominare queste immagini in Adobe Dynamic Media Classic, scegliere una delle opzioni seguenti:

      * **[!UICONTROL Nome livello]**: assegna alle immagini un nome dopo i nomi dei livelli nel file PSD. Ad esempio, un livello denominato Price Tag nel file PSD originale diventa un’immagine denominata Price Tag. Tuttavia, se i nomi dei livelli nel file PSD sono nomi di livello predefiniti di Photoshop (Sfondo, Livello 1, Livello 2 e così via), le immagini vengono denominate in base ai numeri dei livelli nel file PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop e numero livello]**: assegna alle immagini un nome dopo il numero di livello nel file PSD, ignorando i nomi di livello originali. Le immagini vengono denominate con il nome file di Photoshop a cui viene aggiunto un numero di livello. Il secondo livello di un file denominato `Spring Ad.psd`, ad esempio, è denominato `Spring Ad_2` anche se in Photoshop è presente un nome non predefinito.

      * **[!UICONTROL Photoshop e nome livello]**: assegna un nome alle immagini dopo il file PSD seguito dal nome o dal numero del livello. Il numero del livello viene usato se il livello nel file PSD ha un nome predefinito di Photoshop. Ad esempio, un livello denominato `Price Tag` in un file PSD denominato `SpringAd` è denominato `Spring Ad_Price Tag`. Un livello con il nome predefinito Livello 2 è denominato `Spring Ad_2`.

   * **[!UICONTROL Ancoraggio]**: specificare il modo in cui le immagini vengono ancorate nei modelli generati dalla composizione con livelli prodotta dal file PSD. Per impostazione predefinita, la posizione di ancoraggio è al centro. Un ancoraggio centrale consente di utilizzare immagini sostitutive in grado di riempire lo stesso spazio, indipendentemente dalle proporzioni dell&#39;immagine sostitutiva. In questo modo, facendo riferimento al modello e utilizzano la sostituzione mediante parametri, le immagini sostitutive con proporzioni diverse occupano lo stesso spazio in modo efficace. Usate un’impostazione diversa se la vostra applicazione richiede che le immagini sostitutive riempiano lo spazio allocato nel modello.

## Visualizzare e modificare i livelli in un file PSD {#viewing-and-editing-layers-in-a-psd-file}

Se al momento del caricamento del PSD hai selezionato l&#39;opzione **[!UICONTROL Mantieni livelli]**, Adobe Dynamic Media Classic ha copiato i singoli livelli nelle risorse. Per visualizzare e modificare i livelli di risorse appartenenti a un file PSD, apri il file nel pannello Sfoglia in Vista dettagli.

>[!NOTE]
>
>Adobe Dynamic Media Classic supporta fino a cinque livelli in un gruppo di livelli nidificato.

1. Fate doppio clic sul file PSD completo nel pannello Sfoglia. Il file viene aperto in Vista dettagli (Detail View).

   >[!NOTE]
   >
   >assicuratevi di aprire la risorsa completa e non uno dei livelli del file PSD.

1. Seleziona **[!UICONTROL Livelli]**. Nel pannello Livelli, tutti i livelli sono riportati come immagini a sé stanti.
1. Fate doppio clic su un livello ed effettuate una delle seguenti operazioni:

   * Per creare una mappa immagine sul livello, seleziona l&#39;icona **[!UICONTROL Mappa immagine]**. (Vedi [Creare mappe immagine](creating-image-maps.md#creating_image_maps).)
   * Per creare destinazioni di zoom sul livello, selezionare l&#39;icona **[!UICONTROL Destinazioni di zoom]**. (Vedi [Crea destinazioni di zoom per zoom guidato](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Per ritagliare il livello, seleziona l&#39;icona **[!UICONTROL Ritaglia]**. (Vedi [Ritagliare un&#39;immagine](cropping-image.md#cropping_an_image).)
   * Per rendere più nitido il livello, selezionare **[!UICONTROL Contrasta]**. (Vedi [Contrasta un&#39;immagine](sharpening-image.md#sharpening_an_image).)
   * Per regolare il livello, selezionare **[!UICONTROL Regola]**. (Vedi [Regolare un&#39;immagine](adjusting-image.md#adjusting_an_image).)

1. Selezionare **[!UICONTROL Salva]** o **[!UICONTROL Salva con nome]**.
1. Per visualizzare o modificare un livello diverso, selezionate una freccia nella parte inferiore dell&#39;anteprima del livello.
1. Per uscire dalla Vista dettagli livello, selezionare l&#39;icona **[!UICONTROL Vista griglia]**.
