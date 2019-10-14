---
title: Creazione di destinazioni di zoom per lo zoom guidato
seo-title: Creazione di destinazioni di zoom per lo zoom guidato
description: 'null'
seo-description: Scoprite come creare destinazioni di zoom per lo zoom guidato.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/category/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
translation-type: tm+mt
source-git-commit: 6ff0141d1e8e96278b95f61c00602780984aaf67

---


# Creazione di destinazioni di zoom per lo zoom guidato{#creating-zoom-targets-for-guided-zoom}

Le destinazioni di zoom guidano gli utenti su determinate parti di un’immagine. Come nel caso dello zoom libero, gli utenti possono fare clic su una miniatura di destinazione di zoom per applicare lo zoom alla porzione dell’immagine che desiderano evidenziare. Le destinazioni di zoom consentono di evidenziare le parti accattivanti o interessanti di un’immagine.

![Creazione di destinazioni di zoom per lo zoom guidato](/help/assets/zo_guided_zoom.png)

## Destinazioni di zoom {#about-zoom-targets}

La percentuale massima di zoom delle destinazioni di zoom è 100 percento. La percentuale di zoom minima varia in base alle dimensioni del visualizzatore e dell’immagine, come illustrato nella seguente tabella:

| Dimensione immagine | Dimensioni visualizzatore | Percentuale zoom  |
|--- |--- |--- |
| Grande | Più piccolo | Più piccolo minimo |
| Piccolo | Più grande | Più grande minimo |

Potete modificare le dimensioni del visualizzatore zoom in modo che corrispondano a quelle usate sulla pagina Web. Solo gli amministratori possono modificare questa impostazione in maniera permanente, modificando le dimensioni del visualizzatore nella schermata Configurazione. Consultate [Impostazione dei predefiniti per il visualizzatore zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Creazione e modifica delle destinazioni di zoom {#creating-and-editing-zoom-targets}

Potete creare e modificare le destinazioni di zoom nella schermata Editor destinazioni di zoom. Per aprire questa schermata, selezionate un’immagine ed effettuate una delle seguenti operazioni:

* Click the rollover **[!UICONTROL Edit]** button and choose Zoom Targets.
* In the Browse Panel, display the image in **[!UICONTROL Detail View]**, then click **[!UICONTROL Zoom Targets]**.

On the Zoom Target Editor screen, click **[!UICONTROL Select Target]** button (arrow) to select a target before changing its size or position. Click **[!UICONTROL Add Targets]** (rectangle) to create a zoom target on the image. La schermata Editor destinazioni di zoom contiene anche strumenti per eliminare, copiare e denominare destinazioni di zoom.

### Creazione di una destinazione di zoom {#creating-a-zoom-target}

Per creare una destinazione di zoom, aprite la schermata Editor destinazioni di zoom ed effettuate le seguenti operazioni: 

1. Click **[!UICONTROL Add Targets]** (rectangle), move the pointer over the image, and click where you want to the zoom target to be.

   Nel pannello a destra della schermata viene visualizzata una miniatura della destinazione di zoom.

1. Click **[!UICONTROL Select Target]** (arrow), click to select the zoom target you created, and adjust the size and position of the target.

   * **Ridimensionamento** Spostate il puntatore su un angolo della destinazione di zoom e trascinate per ingrandire o ridurre la destinazione.

   * **Posizionamento** Spostate il puntatore sulla destinazione di zoom e trascinatela in un’altra posizione.

1. Digitate un nome per la destinazione di zoom nella casella Nome.

   >[!NOTE]
   >
   >quanto inserite nella casella Nome è più di un nome: quando gli utenti passano il cursore sulla destinazione di zoom, viene visualizzato quello che avete inserito nella casella Nome. Potete quindi inserire una breve descrizione della destinazione di zoom nella casella Nome che possa essere utile agli utenti.

1. Facoltativamente, potete immettere dei dati utente nel campo Dati utente. Questo campo è destinato ai Web designer che possono aggiungere informazioni sulla destinazione di zoom.
1. Fate clic su **[!UICONTROL Salva]**.

   Le coordinate e il livello di zoom della destinazione di zoom vengono salvate. Nella parte destra della schermata viene visualizzata una miniatura della destinazione di zoom accompagnata dal testo inserito nella casella Nome.

>[!NOTE]
>
>Per visualizzare l’aspetto delle destinazioni di zoom in un visualizzatore zoom, fate clic sul pulsante Anteprima nella schermata Editor destinazioni di zoom e scegliete un visualizzatore zoom nella schermata Anteprima. Per informazioni su questa schermata, consultate [Anteprima delle immagini con diversi visualizzatori zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Modifica delle destinazioni di zoom {#editing-zoom-targets}

Per modificare le destinazioni di zoom, utilizzate le seguenti tecniche nella schermata Editor destinazioni di zoom.

* **Riposizionamento** Con il pulsante Seleziona destinazione (la freccia), fate clic sulla destinazione per selezionarla. Trascinate quindi la destinazione in un’altra posizione.

* **Ridimensionamento** Con il pulsante Seleziona destinazione (la freccia), fate clic sulla destinazione per selezionarla. Portate il cursore su un angolo della destinazione di zoom e trascinate per ingrandire o ridurre la destinazione.

* **Eliminazione** Fate clic sulla miniatura della destinazione sul lato destro della schermata. Fate clic su **[!UICONTROL Elimina destinazione]**.

* **Ridenominazione** Fate clic sulla miniatura della destinazione sul lato destro della schermata. Then enter a name in the **[!UICONTROL Name]** text field and click **[!UICONTROL Save]**.

### Copia delle destinazioni di zoom {#copying-zoom-targets}

Potete copiare le destinazioni di zoom da un’immagine a un’altra. Questo risulta utile nel caso in cui due immagini presentano contenuto simile e le rispettive destinazioni di zoom appartengono alle stesse posizioni. Per copiare le destinazioni di zoom in un’altra immagine, effettuate le seguenti operazioni.

1. Aprite l’immagine con le destinazioni di zoom che desiderate copiare nella schermata Editor destinazioni di zoom. 
1. Fate clic su **[!UICONTROL Copia destinazioni in]**.
1. In the Select Images dialog box, select an image and click **[!UICONTROL Select]**.

