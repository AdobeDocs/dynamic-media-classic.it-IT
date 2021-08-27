---
title: Creare destinazioni di zoom per lo zoom guidato
description: Scopri come creare destinazioni di zoom per lo zoom guidato in Adobe Dynamic Media Classic.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 44%

---

# Creare destinazioni di zoom per lo zoom guidato{#creating-zoom-targets-for-guided-zoom}

Le destinazioni di zoom guidano gli utenti su determinate parti di un’immagine. Oltre allo zoom a forma libera, gli spettatori possono selezionare una miniatura di destinazione dello zoom e lo zoom sulla parte dell&#39;immagine su cui si desidera mettere a fuoco. Le destinazioni di zoom consentono di evidenziare le parti accattivanti o interessanti di un’immagine.

![Creare destinazioni di zoom per lo zoom guidato](/help/assets/zo_guided_zoom.png)

## Destinazioni di zoom {#about-zoom-targets}

La percentuale massima di zoom delle destinazioni di zoom è 100 percento. La percentuale di zoom minima varia in base alle dimensioni del visualizzatore e dell’immagine, come illustrato nella seguente tabella:

| Dimensione immagine | Dimensioni visualizzatore | Percentuale zoom  |
| --- | --- | --- |
| Grande | Più piccolo | Più piccolo minimo |
| Piccolo | Più grande | Più grande minimo |

Potete modificare le dimensioni del visualizzatore zoom in modo che corrispondano a quelle usate sulla pagina Web. Solo gli amministratori possono modificare questa impostazione in maniera permanente, modificando le dimensioni del visualizzatore nella schermata Configurazione. Consulta [Configurazione predefiniti visualizzatore zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Creare e modificare le destinazioni di zoom {#creating-and-editing-zoom-targets}

Potete creare e modificare le destinazioni di zoom nella schermata Editor destinazioni di zoom. Per aprire questa schermata, selezionate un’immagine ed effettuate una delle seguenti operazioni:

* Selezionare il pulsante rollover **[!UICONTROL Modifica]** e scegliere Destinazioni zoom.
* Nel pannello Sfoglia, visualizza l&#39;immagine in **[!UICONTROL Vista dettagli]**, quindi seleziona **[!UICONTROL Destinazioni zoom]**.

Nella schermata Editor di destinazione zoom, seleziona il pulsante **[!UICONTROL Seleziona destinazione]** (freccia) per selezionare una destinazione prima di modificarne le dimensioni o la posizione. Per creare una destinazione di zoom sull&#39;immagine, seleziona **[!UICONTROL Aggiungi destinazioni]** (rettangolo). La pagina Editor di destinazione zoom offre anche strumenti per eliminare, copiare e denominare le destinazioni di zoom.

### Creare una destinazione di zoom {#creating-a-zoom-target}

Per creare una destinazione di zoom, apri la pagina Editor destinazione di zoom ed effettua le seguenti operazioni:

1. Selezionare **[!UICONTROL Aggiungi destinazioni]** (rettangolo), spostare il puntatore sull&#39;immagine e selezionare il punto in cui si desidera impostare la destinazione di zoom.

   Nel pannello a destra della schermata viene visualizzata una miniatura della destinazione di zoom.

1. Scegli **[!UICONTROL Seleziona destinazione]** (freccia), quindi seleziona la destinazione di zoom creata e regola le dimensioni e la posizione della destinazione.

   * **Ridimensiona** : sposta il puntatore su un angolo della destinazione di zoom e trascina per ingrandire o ridurre la destinazione.

   * **Posizione** : spostare il puntatore sulla destinazione dello zoom e trascinarlo in un&#39;altra posizione.

1. Digitate un nome per la destinazione di zoom nella casella Nome.

   >[!NOTE]
   >
   >quanto inserite nella casella Nome è più di un nome: quando gli utenti passano il cursore sulla destinazione di zoom, viene visualizzato quello che avete inserito nella casella Nome. Potete quindi inserire una breve descrizione della destinazione di zoom nella casella Nome che possa essere utile agli utenti.

1. Facoltativamente, potete immettere dei dati utente nel campo Dati utente. Questo campo è destinato ai Web designer che possono aggiungere informazioni sulla destinazione di zoom.
1. Selezionare **[!UICONTROL Salva]**.

   Le coordinate e il livello di zoom della destinazione di zoom vengono salvate. Nella parte destra della schermata viene visualizzata una miniatura della destinazione di zoom accompagnata dal testo inserito nella casella Nome.

>[!NOTE]
>
>Per visualizzare l’aspetto delle destinazioni di zoom in un visualizzatore zoom, selezionare il pulsante **[!UICONTROL Anteprima]** nella schermata Editor di destinazione zoom e scegliere un visualizzatore zoom nella schermata Anteprima. Per informazioni su questa schermata, vedere [Anteprima delle immagini con diversi visualizzatori zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Modificare le destinazioni di zoom {#editing-zoom-targets}

Per modificare le destinazioni di zoom, utilizza le seguenti tecniche nella pagina Editor di destinazione zoom:

* **Riposiziona** : con il pulsante Seleziona destinazione (la freccia), seleziona la destinazione. Trascinate quindi la destinazione in un’altra posizione.

* **Ridimensiona** : con il pulsante Seleziona destinazione (la freccia), seleziona la destinazione. Per ingrandire o ridurre la destinazione, spostare il puntatore su un angolo della destinazione di zoom e trascinare.

* **Elimina** : seleziona l’immagine in miniatura della destinazione sul lato destro dello schermo. Quindi seleziona **[!UICONTROL Elimina Target]**.

* **Ridenominazione** : seleziona l’immagine in miniatura della destinazione sul lato destro dello schermo. Quindi inserisci un nome nel campo di testo **[!UICONTROL Nome]** e seleziona **[!UICONTROL Salva]**.

### Copiare le destinazioni di zoom {#copying-zoom-targets}

Potete copiare le destinazioni di zoom da un’immagine a un’altra. Questo risulta utile nel caso in cui due immagini presentano contenuto simile e le rispettive destinazioni di zoom appartengono alle stesse posizioni. Per copiare le destinazioni di zoom in un’altra immagine, procedi come segue:

1. Aprite l’immagine con le destinazioni di zoom che desiderate copiare nella schermata Editor destinazioni di zoom. 
1. Seleziona **[!UICONTROL Copia destinazioni in]**.
1. Nella finestra di dialogo Seleziona immagini , seleziona un’immagine e scegli **[!UICONTROL Seleziona]**.
