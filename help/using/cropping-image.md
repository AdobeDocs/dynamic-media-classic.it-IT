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
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 31%

---

# Ritagliare un’immagine{#cropping-an-image}

È possibile ritagliare le immagini in Adobe Dynamic Media Classic. Il sistema conserva le informazioni sulle immagini ritagliate per permettere di riportarle eventualmente al loro stato originale. Potete anche ritagliare un’immagine e salvare la versione ritagliata con un nuovo nome.

Potete ritagliare un’immagine per rimuovere lo spazio bianco che la circonda oppure ritagliare un’area dell’immagine.

>[!NOTE]
>
>Dopo il ritaglio, è possibile selezionare **[!UICONTROL Salva con nome]** e salvare una versione ritagliata dell&#39;immagine con un nome diverso. Nella finestra Salva con nome selezionare **[!UICONTROL Salva come nuovo elemento principale]** per salvare una seconda copia dell&#39;immagine. Selezionare **[!UICONTROL Salva come vista di aggiunta principale]** per salvare l&#39;originale e la versione ritagliata con un nome diverso. Seleziona **[!UICONTROL Sostituisci originale]** per eliminare il file originale da cui hai ritagliato l&#39;immagine. Immettere quindi un nome per l&#39;immagine e selezionare **[!UICONTROL Invia]**.

## Ritagliare per rimuovere lo spazio bianco intorno a un’immagine {#crop-to-remove-white-space-around-an-image}

Potete eliminare i pixel trasparenti o in tinta unita dal bordo di un’immagine ritagliandoli.

1. Per ritagliare un&#39;immagine, selezionarne il pulsante di rollover **[!UICONTROL Modifica]** e quindi selezionare **[!UICONTROL Ritaglia]**, oppure visualizzarla nel pannello Sfoglia in Visualizzazione dettagli e selezionare il pulsante **[!UICONTROL Ritaglia]**.
1. Nella pagina Editor ritaglio eseguire una delle operazioni seguenti:

   * Per tagliare i pixel di colore, passa a **[!UICONTROL Taglia]** > **[!UICONTROL Colore]**. Nella finestra di dialogo **[!UICONTROL Ritaglio automatico per colore]**, selezionare il menu **[!UICONTROL Angolo]** e scegliere un angolo con il colore di sfondo che si desidera ritagliare. Quindi immettere un&#39;impostazione di **[!UICONTROL tolleranza]** da 0 a 1. L’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo dell’immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. Seleziona **[!UICONTROL Ritaglia]**.
   * Per tagliare i pixel trasparenti, vai a **[!UICONTROL Taglia]** > **[!UICONTROL Trasparente]**. Nella finestra di dialogo **[!UICONTROL Ritaglio automatico per trasparenza]** immettere un&#39;impostazione di tolleranza da 0 a 1. L’impostazione 0 ritaglia i pixel solo se sono trasparenti. Con valori più vicini a 1 viene invece tollerata una minore trasparenza. Seleziona **[!UICONTROL Ritaglia]**.

1. Seleziona **[!UICONTROL Salva]**.

>[!NOTE]
>
>Per ripristinare lo stato originale di un&#39;immagine dopo averla ritagliata, visualizzarla nella schermata Editor ritaglio e selezionare **[!UICONTROL Reimposta]**.

## Selezionare un’area da ritagliare {#select-an-area-to-crop}

1. Per ritagliare un&#39;immagine, selezionarne il pulsante di rollover **[!UICONTROL Modifica]** e scegliere **[!UICONTROL Ritaglia]** oppure visualizzarla nel pannello Sfoglia in Visualizzazione dettagli e selezionare **[!UICONTROL Ritaglia]**.

1. Nella finestra Editor ritaglio, posizionate la parte dell&#39;immagine che non desiderate ritagliare nella casella di ritaglio. Qualsiasi cosa venga visualizzata all&#39;interno della casella è ciò che rimarrà dopo aver selezionato **[!UICONTROL Salva]** e ritagliato l&#39;immagine.
1. Per regolare l’area di ritaglio, effettuate una delle seguenti operazioni:

   * Trascinate un lato o un angolo della casella. Tenere premuto il tasto Maiusc mentre si trascina per modificare le dimensioni ma mantenere le proporzioni (la forma) della casella di ritaglio.
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
