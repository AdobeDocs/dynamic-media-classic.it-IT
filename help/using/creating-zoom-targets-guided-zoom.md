---
title: Creare destinazioni di zoom per lo zoom guidato
description: Scopri come creare destinazioni di zoom per lo zoom guidato in Adobe Dynamic Media Classic.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 41%

---

# Creare destinazioni di zoom per lo zoom guidato{#creating-zoom-targets-for-guided-zoom}

Le destinazioni di zoom guidano gli utenti su determinate parti di un’immagine. Oltre allo zoom in formato libero, gli utenti possono selezionare una miniatura di destinazione di zoom e ingrandire la parte dell&#39;immagine su cui si desidera mettere a fuoco. Le destinazioni di zoom consentono di evidenziare le parti accattivanti o interessanti di un’immagine.

![Creare destinazioni di zoom per lo zoom guidato](/help/using/assets/zo_guided_zoom.png)

## Destinazioni di zoom {#about-zoom-targets}

La percentuale massima di zoom delle destinazioni di zoom è 100 percento. La percentuale di zoom minima varia in base alle dimensioni del visualizzatore e dell’immagine, come illustrato nella seguente tabella:

| Dimensione immagine | Dimensioni visualizzatore | Percentuale zoom  |
| --- | --- | --- |
| Grande | Più piccolo | Più piccolo minimo |
| Piccolo | Più grande | Più grande minimo |

Potete modificare le dimensioni del visualizzatore zoom in modo che corrispondano a quelle usate sulla pagina Web. Solo gli amministratori possono modificare questa impostazione in maniera permanente, modificando le dimensioni del visualizzatore nella schermata Configurazione. Consulta [Impostare i predefiniti per visualizzatore zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Creare e modificare le destinazioni di zoom {#creating-and-editing-zoom-targets}

Potete creare e modificare le destinazioni di zoom nella schermata Editor destinazioni di zoom. Per aprire questa schermata, selezionate un’immagine ed effettuate una delle seguenti operazioni:

* Seleziona il rollover **[!UICONTROL Modifica]** e scegliere Destinazioni zoom.
* Nel pannello Sfoglia, visualizzare l&#39;immagine in **[!UICONTROL Vista dettagli]**, quindi seleziona **[!UICONTROL Destinazioni di zoom]**.

Nella schermata Editor destinazioni di zoom, seleziona **[!UICONTROL Seleziona destinazione]** (freccia) per selezionare una destinazione prima di modificarne le dimensioni o la posizione. Per creare una destinazione di zoom sull&#39;immagine, selezionare **[!UICONTROL Aggiungi destinazioni]** (rettangolo). La pagina Editor destinazioni di zoom offre inoltre strumenti per l&#39;eliminazione, la copia e la denominazione delle destinazioni di zoom.

### Creare una destinazione di zoom {#creating-a-zoom-target}

Per creare una destinazione di zoom, aprire la pagina Editor destinazione di zoom ed effettuare le seguenti operazioni:

1. Seleziona **[!UICONTROL Aggiungi destinazioni]** (rettangolo), spostate il puntatore sull&#39;immagine e selezionate la posizione in cui desiderate posizionare la destinazione di zoom.

   Nel pannello a destra della schermata viene visualizzata una miniatura della destinazione di zoom.

1. Scegli **[!UICONTROL Seleziona destinazione]** (freccia), quindi selezionare la destinazione di zoom creata e regolare la dimensione e la posizione della destinazione.

   * **Ridimensiona** - Spostate il puntatore su un angolo della destinazione di zoom e trascinate per ingrandire o ridurre la destinazione.

   * **Posizione** - Spostare il puntatore sulla destinazione di zoom e trascinarlo in una posizione diversa.

1. Digitate un nome per la destinazione di zoom nella casella Nome.

   >[!NOTE]
   >
   >quanto inserite nella casella Nome è più di un nome: quando gli utenti passano il cursore sulla destinazione di zoom, viene visualizzato quello che avete inserito nella casella Nome. Potete quindi inserire una breve descrizione della destinazione di zoom nella casella Nome che possa essere utile agli utenti.

1. Facoltativamente, potete immettere dei dati utente nel campo Dati utente. Questo campo è destinato ai Web designer che possono aggiungere informazioni sulla destinazione di zoom.
1. Seleziona **[!UICONTROL Salva]**.

   Le coordinate e il livello di zoom della destinazione di zoom vengono salvate. Nella parte destra della schermata viene visualizzata una miniatura della destinazione di zoom accompagnata dal testo inserito nella casella Nome.

>[!NOTE]
>
>Per visualizzare l&#39;aspetto delle destinazioni di zoom in un Visualizzatore zoom, selezionare **[!UICONTROL Anteprima]** nella schermata Zoom Target Editor e scegliere un Visualizzatore zoom nella schermata Preview. Per informazioni su questa schermata, vedi [Anteprima di immagini con diversi visualizzatori zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Modifica destinazioni di zoom {#editing-zoom-targets}

Per modificare le destinazioni di zoom, utilizzare le tecniche riportate di seguito nella pagina Editor destinazioni di zoom.

* **Riposiziona** - Con il pulsante Seleziona destinazione (la freccia), selezionare la destinazione. Trascinate quindi la destinazione in un’altra posizione.

* **Ridimensiona** - Con il pulsante Seleziona destinazione (la freccia), selezionare la destinazione. Per ingrandire o ridurre la destinazione, spostare il puntatore su un angolo della destinazione di zoom e trascinare.

* **Elimina** - Selezionare l&#39;immagine miniatura del target sul lato destro dello schermo. Quindi seleziona **[!UICONTROL Elimina destinazione]**.

* **Ridenominazione** - Selezionare l&#39;immagine miniatura del target sul lato destro dello schermo. Quindi inserisci un nome in **[!UICONTROL Nome]** campo di testo e selezione **[!UICONTROL Salva]**.

### Copia destinazioni di zoom {#copying-zoom-targets}

Potete copiare le destinazioni di zoom da un’immagine a un’altra. Questo risulta utile nel caso in cui due immagini presentano contenuto simile e le rispettive destinazioni di zoom appartengono alle stesse posizioni. Per copiare le destinazioni di zoom in un&#39;altra immagine, effettuare le seguenti operazioni:

1. Aprire l&#39;immagine con le destinazioni di zoom da copiare nella schermata Editor destinazioni di zoom.
1. Seleziona **[!UICONTROL Copia destinazioni in]**.
1. Nella finestra di dialogo Seleziona immagini, selezionate un&#39;immagine e fate clic su **[!UICONTROL Seleziona]**.
