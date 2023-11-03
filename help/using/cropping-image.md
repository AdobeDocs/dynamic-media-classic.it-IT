---
title: Ritagliare un’immagine
description: Scopri come ritagliare un’immagine in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 35%

---

# Ritagliare un’immagine{#cropping-an-image}

È possibile ritagliare le immagini in Adobe Dynamic Media Classic. Il sistema conserva le informazioni sulle immagini ritagliate per permettere di riportarle eventualmente al loro stato originale. Potete anche ritagliare un’immagine e salvare la versione ritagliata con un nuovo nome.

Potete ritagliare un’immagine per rimuovere lo spazio bianco che la circonda oppure ritagliare un’area dell’immagine.

>[!NOTE]
>
>Dopo il ritaglio, puoi selezionare **[!UICONTROL Salva con nome]** e salvare una versione ritagliata dell&#39;immagine con un nome diverso. Nella finestra Salva con nome, seleziona **[!UICONTROL Salva come nuovo elemento principale]** per salvare una seconda copia dell&#39;immagine. Seleziona **[!UICONTROL Salva come vista aggiuntiva dell&#39;elemento principale]** in modo da poter salvare l’originale e la relativa versione ritagliata con un nome diverso. Seleziona **[!UICONTROL Sostituisci originale]** per eliminare il file originale da cui è stata ritagliata l&#39;immagine. Quindi immetti un nome per l’immagine e seleziona **[!UICONTROL Invia]**.

## Ritagliare per rimuovere lo spazio bianco intorno a un’immagine {#crop-to-remove-white-space-around-an-image}

Potete eliminare i pixel trasparenti o in tinta unita dal bordo di un’immagine ritagliandoli.

1. Per ritagliare un’immagine, selezionane il rollover **[!UICONTROL Modifica]** e quindi selezionare **[!UICONTROL Ritaglio]** o visualizzarlo nel pannello Sfoglia in Visualizzazione dettagli e selezionare **[!UICONTROL Ritaglio]** pulsante.
1. Nella pagina Editor ritaglio eseguire una delle operazioni seguenti:

   * Per tagliare i pixel di colore, vai a **[!UICONTROL Rifila]** > **[!UICONTROL Colore]**. In **[!UICONTROL Ritaglio automatico per colore]** , selezionare la **[!UICONTROL Angolo]** e scegliete un angolo con il colore di sfondo da ritagliare. Quindi inserisci un **[!UICONTROL Tolleranza]** da 0 a 1. L’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo dell’immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. Seleziona **[!UICONTROL Ritaglio]**.
   * Per tagliare i pixel trasparenti, vai a **[!UICONTROL Rifila]** > **[!UICONTROL Trasparente]**. In **[!UICONTROL Ritaglio automatico in base a trasparenza]** immettete un&#39;impostazione di tolleranza da 0 a 1. L’impostazione 0 ritaglia i pixel solo se sono trasparenti. Con valori più vicini a 1 viene invece tollerata una minore trasparenza. Seleziona **[!UICONTROL Ritaglio]**.

1. Seleziona **[!UICONTROL Salva]**.

>[!NOTE]
>
>Per ripristinare lo stato originale di un&#39;immagine dopo averla ritagliata, visualizzarla nella schermata Editor ritaglio e selezionare **[!UICONTROL Reimposta]**.

## Selezionare un’area da ritagliare {#select-an-area-to-crop}

1. Per ritagliare un’immagine, selezionane il rollover **[!UICONTROL Modifica]** e scegliere **[!UICONTROL Ritaglio]** o visualizzarlo nel pannello Sfoglia in Visualizzazione dettagli e selezionare **[!UICONTROL Ritaglio]**.

1. Nella finestra Editor ritaglio, posizionate la parte dell&#39;immagine che non desiderate ritagliare nella casella di ritaglio. Qualsiasi cosa venga visualizzata all&#39;interno della casella è ciò che rimarrà dopo aver selezionato **[!UICONTROL Salva]** e ritagliare l&#39;immagine.
1. Per regolare l’area di ritaglio, effettuate una delle seguenti operazioni:

   * Trascinate un lato o un angolo della casella. Tenete premuto il tasto Maiusc mentre trascinate per cambiare le dimensioni ma mantenere le stesse proporzioni (forma) del rettangolo di ritaglio.
   * Immettete le misure in pixel nelle caselle Dimensione.
   * Trascinate per spostare la casella di ritaglio. Spostate il puntatore all’interno della casella. Quando viene visualizzata la freccia a quattro punte, trascinate la casella sull’immagine in una nuova posizione.

1. Seleziona **[!UICONTROL Salva]**.

>[!NOTE]
>
>Per ripristinare lo stato originale di un&#39;immagine dopo averla ritagliata, visualizzarla nella schermata Editor ritaglio e selezionare **[!UICONTROL Reimposta]**.

>[!MORELIKETHIS]
>
>* [Opzioni per la modifica delle immagini al caricamento](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Ritaglia spazio vuoto da un file PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Ritaglia dai lati delle pagine PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)
