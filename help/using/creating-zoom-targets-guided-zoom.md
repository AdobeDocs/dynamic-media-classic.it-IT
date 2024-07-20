---
title: Creare destinazioni di zoom per lo zoom guidato
description: Scopri come creare destinazioni di zoom per lo zoom guidato in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 27%

---

# Creare destinazioni di zoom per lo zoom guidato{#creating-zoom-targets-for-guided-zoom}

Le destinazioni di zoom guidano gli utenti su determinate parti di un’immagine. Oltre allo zoom in formato libero, gli utenti possono selezionare una miniatura di destinazione di zoom e ingrandire la parte dell&#39;immagine su cui si desidera mettere a fuoco. Le destinazioni di zoom consentono di evidenziare le parti accattivanti o interessanti di un’immagine.

![Crea destinazioni zoom per zoom guidato](/help/using/assets/zo_guided_zoom.png)

## Destinazioni zoom {#about-zoom-targets}

La percentuale di zoom massima di Target di Zoom è 100%. La percentuale di zoom minima varia in base alle dimensioni del visualizzatore e dell’immagine, come illustrato nella seguente tabella:

| Dimensione immagine | Dimensioni visualizzatore | Percentuale zoom  |
| --- | --- | --- |
| Grande | Più piccolo | Più piccolo minimo |
| Piccolo | Più grande | Più grande minimo |

È possibile modificare le dimensioni del Visualizzatore zoom in modo che corrispondano a quelle utilizzate nella pagina Web. È possibile modificare in modo permanente questa impostazione modificando le dimensioni del visualizzatore nella schermata Configurazione (se si è un amministratore). Consulta [Configurare i predefiniti visualizzatore zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Creare e modificare le destinazioni di zoom {#creating-and-editing-zoom-targets}

Creare e modificare Destinazioni di zoom nella schermata Editor destinazioni di zoom. Per aprire questa schermata, selezionate un’immagine ed effettuate una delle seguenti operazioni:

* Selezionare il pulsante di rollover **[!UICONTROL Modifica]** e scegliere Destinazioni zoom.
* Nel pannello Sfoglia, visualizza l&#39;immagine in **[!UICONTROL Visualizzazione dettagli]**, quindi seleziona **[!UICONTROL Destinazioni zoom]**.

Nella schermata Editor destinazioni di zoom, selezionare il pulsante **[!UICONTROL Seleziona destinazione]** (freccia) per selezionare una destinazione prima di modificarne le dimensioni o la posizione. Per creare una destinazione di zoom sull&#39;immagine, selezionare **[!UICONTROL Aggiungi destinazioni]** (rettangolo). La pagina Editor destinazioni di zoom offre inoltre strumenti per l&#39;eliminazione, la copia e la denominazione delle destinazioni di zoom.

### Creare una destinazione di zoom {#creating-a-zoom-target}

Per creare una destinazione di zoom, aprire la pagina Editor destinazione di zoom ed effettuare le seguenti operazioni:

1. Seleziona **[!UICONTROL Aggiungi destinazioni]** (rettangolo), sposta il puntatore sull&#39;immagine e seleziona la destinazione di zoom.

   Nel pannello a destra della schermata viene visualizzata una miniatura della destinazione di zoom.

1. Selezionare **[!UICONTROL Seleziona destinazione]** (freccia), quindi selezionare la destinazione di zoom creata e regolare la dimensione e la posizione della destinazione.

   * **Ridimensiona**: sposta il puntatore su un angolo della destinazione di zoom e trascina per ingrandire o ridurre la destinazione.

   * **Posizione**: spostare il puntatore sulla destinazione di zoom e trascinarlo in un&#39;altra posizione.

1. Digitate un nome per la destinazione di zoom nella casella Nome.

   >[!NOTE]
   >
   >quanto inserite nella casella Nome è più di un nome: quando gli utenti passano il cursore sulla destinazione di zoom, viene visualizzato quello che avete inserito nella casella Nome. Potete quindi inserire una breve descrizione della destinazione di zoom nella casella Nome che possa essere utile agli utenti.

1. Facoltativamente, potete immettere dei dati utente nel campo Dati utente. Questo campo consente ai progettisti di siti Web di aggiungere informazioni alla destinazione di zoom.
1. Seleziona **[!UICONTROL Salva]**.

   Le coordinate e il livello di zoom della destinazione di zoom vengono salvate. Nella parte destra della schermata viene visualizzata una miniatura della destinazione di zoom accompagnata dal testo inserito nella casella Nome.

>[!NOTE]
>
>Per visualizzare l&#39;aspetto delle destinazioni di zoom in un Visualizzatore zoom, selezionare il pulsante **[!UICONTROL Anteprima]** nella schermata Editor destinazioni zoom. Scegliere quindi un Visualizzatore zoom nella schermata Anteprima. Per ulteriori informazioni su questa schermata, vedere [Anteprima di immagini con diversi visualizzatori di zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Modifica destinazioni di zoom {#editing-zoom-targets}

Per modificare le destinazioni di zoom, utilizzare le tecniche riportate di seguito nella pagina Editor destinazioni di zoom.

* **Riposiziona**: con il pulsante Seleziona destinazione (la freccia), seleziona la destinazione. Trascinate quindi la destinazione in un’altra posizione.

* **Ridimensiona**: con il pulsante Seleziona destinazione (la freccia), seleziona la destinazione. Per ingrandire o ridurre la destinazione, spostare il puntatore su un angolo della destinazione di zoom e trascinare.

* **Elimina**: seleziona l&#39;immagine miniatura di destinazione sul lato destro dello schermo. Quindi selezionare **[!UICONTROL Elimina destinazione]**.

* **Ridenominazione**: seleziona l&#39;immagine miniatura di destinazione sul lato destro dello schermo. Immetti un nome nel campo di testo **[!UICONTROL Nome]** e seleziona **[!UICONTROL Salva]**.

### Copia destinazioni di zoom {#copying-zoom-targets}

Potete copiare le destinazioni di zoom da un&#39;immagine a un&#39;altra. Copiare le destinazioni quando due immagini presentano contenuti simili e le relative destinazioni di zoom appartengono alle stesse posizioni. Per copiare le destinazioni di zoom in un&#39;altra immagine, effettuare le seguenti operazioni:

1. Aprite l&#39;immagine con le destinazioni di zoom da copiare nella schermata Editor destinazioni di zoom.
1. Seleziona **[!UICONTROL Copia Destinazioni In]**.
1. Nella finestra di dialogo Seleziona immagini selezionare un&#39;immagine e scegliere **[!UICONTROL Seleziona]**.
