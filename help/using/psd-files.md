---
title: Utilizzare i file PSD
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
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 25%

---

# Utilizzare i file PSD{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

I PSD (Photoshop Document Files) vengono spesso utilizzati in Adobe Dynamic Media Classic per la creazione di modelli. Quando carichi un file di PSD, puoi creare automaticamente un modello di Adobe Dynamic Media Classic dal file (seleziona l’opzione Crea modello nella schermata Carica ).

Adobe Dynamic Media Classic crea più immagini da un file PSD con livelli se utilizzate il file per creare un modello; crea un&#39;immagine per ogni livello.

## Opzioni di caricamento PSD {#psd-upload-options}

Le opzioni per il caricamento di file PSD si trovano in Opzioni Photoshop nella finestra di dialogo Opzioni processo di caricamento. Potete ritagliare un file, scegliere un profilo colore, usare il file per creare un modello e selezionare un ancoraggio.

Quando si carica un file PSD sono disponibili le seguenti opzioni:

* **Opzioni di ritaglio** - Situato sotto **[!UICONTROL Opzioni di ritaglio]**. Seleziona **[!UICONTROL Rifila]** per ritagliare automaticamente lo spazio vuoto dai bordi di un file PSD; selezionate **[!UICONTROL Manuale]** per ritagliare i lati del file PSD:

   * **[!UICONTROL Rifila]** - Selezionare la **[!UICONTROL Rifila in base a]** e scegliere **[!UICONTROL Colore]** o **[!UICONTROL Trasparenza]**.
   Se si sceglie **[!UICONTROL Colore]** , selezionare il menu Angolo e scegliere l&#39;angolo del PSD con il colore che meglio rappresenta lo spazio bianco che si desidera ritagliare.

   Trascinate il cursore per specificare una tolleranza da 0 a 1. Per rifilare in base al colore, l’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo del file PSD. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. Per tagliare in base alla trasparenza, specificate 0 per ritagliare i pixel solo se sono trasparenti; i numeri più vicini a 1 consentono una maggiore trasparenza.

   * **[!UICONTROL Manuale]** - Immetti il numero di pixel da ritagliare da un lato o da ciascun lato dell&#39;immagine. La quantità di immagine che viene ritagliata dipende dall’impostazione ppi (pixel per pollice) nel file immagine. Ad esempio, se l&#39;immagine visualizza 150 ppi e si immette 75 nelle caselle di testo Superiore, Destra, Inferiore e Sinistra, 0,5 pollici. viene ritagliato da ciascun lato dell&#39;immagine.


* **Opzioni profilo colore** - Situato sotto **[!UICONTROL Opzioni profilo colore]**.

   * **[!UICONTROL Mantenimento colore predefinito]**

   * **[!UICONTROL Mantieni spazio colore originale]** - Mantiene lo spazio colore originale dell&#39;immagine.

   * **[!UICONTROL Personalizza da]** > **[!UICONTROL A]** - Apre i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore standard di Photoshop o uno spazio colore caricato in Adobe Dynamic Media Classic. Consultate [Profili ICC](/help/using/icc-profiles.md).

* **Opzioni Photoshop**

   * **[!UICONTROL Mantieni livelli]** - Ripete i livelli nel PSD, se presenti, in singole risorse. I livelli delle risorse restano associati al file PSD. Per visualizzarli, aprite il file PSD in Vista dettagli (Detail View) e selezionate il pannello dei livelli. Consultate Visualizzazione e modifica dei livelli in un file PSD.

   * **[!UICONTROL Crea modello]** - Crea un modello dai livelli nel file PSD.

   * **[!UICONTROL Estrai testo]** - Estrae il testo in modo che gli utenti possano cercare il testo in un visualizzatore.

   * **[!UICONTROL Estendi livelli a dimensioni sfondo]** - Estende le dimensioni dei livelli immagine strappati alle dimensioni del livello di sfondo.

   * **[!UICONTROL Denominazione livelli]** - I livelli nel file PSD vengono caricati come immagini separate. Per denominare queste immagini in Adobe Dynamic Media Classic, scegliere una delle opzioni seguenti:

      * **[!UICONTROL Nome livello]** - Assegna alle immagini i nomi dei livelli nel file PSD. Ad esempio, un livello denominato Price Tag nel file PSD originale diventa un’immagine denominata Price Tag. Tuttavia, se i nomi dei livelli nel file PSD sono nomi di livello predefiniti di Photoshop (Sfondo, Livello 1, Livello 2 e così via), le immagini vengono denominate in base ai numeri dei livelli nel file PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop e numero livello]** - Assegna alle immagini un nome dopo il numero del livello nel file PSD, ignorando i nomi dei livelli originali. Le immagini vengono denominate con il nome file di Photoshop a cui viene aggiunto un numero di livello. Ad esempio, il secondo livello di un file denominato `Spring Ad.psd` è denominato `Spring Ad_2` anche se aveva un nome non predefinito in Photoshop.

      * **[!UICONTROL Photoshop e nome livello]** - Assegna alle immagini un nome dopo il file PSD seguito dal nome o dal numero del livello. Il numero del livello viene usato se il livello nel file PSD ha un nome predefinito di Photoshop. Ad esempio, un livello denominato `Price Tag` in un file PSD denominato `SpringAd` è denominato `Spring Ad_Price Tag`. Un livello con il nome di default Livello 2 è chiamato `Spring Ad_2`.
   * **[!UICONTROL Ancoraggio]** : specifica in che modo le immagini vengono ancorate nei modelli generati dalla composizione a livelli prodotta dal file PSD. Per impostazione predefinita, la posizione di ancoraggio è al centro. L’ancoraggio centrale permette alle immagini sostitutive di riempire in modo ottimale lo spazio, indipendentemente dalle loro proporzioni. In questo modo, facendo riferimento al modello e utilizzano la sostituzione mediante parametri, le immagini sostitutive con proporzioni diverse occupano lo stesso spazio in modo efficace. Usate un’impostazione diversa se la vostra applicazione richiede che le immagini sostitutive riempiano lo spazio allocato nel modello.


## Visualizzare e modificare i livelli in un file PSD {#viewing-and-editing-layers-in-a-psd-file}

Se al momento del caricamento del PSD hai selezionato l’opzione Mantieni livelli, Adobe Dynamic Media Classic ha copiato i singoli livelli nelle risorse. Per visualizzare e modificare i livelli di risorse appartenenti a un file PSD, apri il file nel pannello Sfoglia in Vista dettagli.

>[!NOTE]
>
>Adobe Dynamic Media Classic supporta fino a cinque livelli in un gruppo di livelli nidificato.

1. Fare doppio clic sul file di PSD completo nel pannello Sfoglia. Il file viene aperto in Vista dettagli (Detail View).

   >[!NOTE]
   >
   >assicuratevi di aprire la risorsa completa e non uno dei livelli del file PSD.

1. Seleziona **[!UICONTROL Livelli]**. Nel pannello Livelli, tutti i livelli sono riportati come immagini a sé stanti.
1. Fate doppio clic su un livello ed effettuate una delle seguenti operazioni:

   * Per creare una mappa immagine sul livello, selezionate **[!UICONTROL Mappa immagine]** icona. (vedere [Creare mappe immagine](creating-image-maps.md#creating_image_maps).)
   * Per creare destinazioni di zoom sul livello, selezionate **[!UICONTROL Destinazioni di zoom]** icona. (vedere [Creare destinazioni di zoom per lo zoom guidato](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Per ritagliare il livello, selezionate **[!UICONTROL Ritaglio]** icona. (vedere [Ritagliare un’immagine](cropping-image.md#cropping_an_image).)
   * Per rendere più nitido il livello, selezionate **[!UICONTROL Nitidezza]**. (vedere [Nitidezza di un&#39;immagine](sharpening-image.md#sharpening_an_image).)
   * Per regolare il livello, selezionate **[!UICONTROL Regola]**. (vedere [Regolare un’immagine](adjusting-image.md#adjusting_an_image).)

1. Seleziona **[!UICONTROL Salva]** o **[!UICONTROL Salva con nome]**.
1. Per visualizzare o modificare un livello diverso, selezionate una freccia nella parte inferiore dell&#39;anteprima del livello.
1. Per uscire dalla vista di dettaglio del livello, selezionate **[!UICONTROL Vista griglia]** icona.
