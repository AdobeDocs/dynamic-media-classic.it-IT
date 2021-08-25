---
title: Ritaglio di un’immagine
description: Scopri come ritagliare un’immagine.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Gestione risorse
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: 7be3f63bfadeafa71eeb2567f982f579ccb85975
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 39%

---

# Ritagliare un’immagine{#cropping-an-image}

È possibile ritagliare le immagini in Dynamic Media Classic. Il sistema conserva le informazioni sulle immagini ritagliate per permettere di riportarle eventualmente al loro stato originale. Potete anche ritagliare un’immagine e salvare la versione ritagliata con un nuovo nome.

Potete ritagliare un’immagine per rimuovere lo spazio bianco che la circonda oppure ritagliare un’area dell’immagine.

>[!NOTE]
>
>Dopo aver ritagliato l&#39;immagine, puoi selezionare **[!UICONTROL Salva con nome]** e salvare una versione ritagliata dell&#39;immagine con un nome diverso. Nella finestra Salva con nome, scegliete Salva come nuovo elemento principale per salvare una seconda copia dell’immagine. Seleziona **[!UICONTROL Salva come visualizzazione di aggiunta del principale]** in modo da salvare l&#39;originale e la relativa versione ritagliata con un nome diverso. Selezionare **[!UICONTROL Sostituisci originale]** per eliminare il file originale dal quale è stata ritagliata l&#39;immagine. Quindi immetti un nome per l&#39;immagine e seleziona **[!UICONTROL Invia]**.

## Ritagliare per rimuovere lo spazio bianco intorno a un’immagine {#crop-to-remove-white-space-around-an-image}

Potete eliminare i pixel trasparenti o in tinta unita dal bordo di un’immagine ritagliandoli.

1. Per ritagliare un&#39;immagine, selezionarne il pulsante rollover **[!UICONTROL Modifica]** e scegliere **[!UICONTROL Ritaglia]**, oppure visualizzarlo nel pannello Sfoglia in visualizzazione Dettagli e selezionare il pulsante **[!UICONTROL Ritaglia]**.
1. Nella pagina Editor ritaglio, effettuare una delle seguenti operazioni:

   * Per tagliare i pixel dei colori, vai a **[!UICONTROL Trim]** > **[!UICONTROL Colore]**. Nella finestra di dialogo **[!UICONTROL Ritaglio automatico per colore]**, selezionate il menu **[!UICONTROL Angolo]** e scegliete un angolo con il colore di sfondo da ritagliare. Quindi immetti un&#39;impostazione **[!UICONTROL Tolleranza]** da 0 a 1. L’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo dell’immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. Selezionare **[!UICONTROL Ritaglia]**.
   * Per tagliare i pixel trasparenti, vai su **[!UICONTROL Trim]** > **[!UICONTROL Trasparente]**. Nella finestra di dialogo **[!UICONTROL Ritaglio automatico per trasparenza]**, immettere un&#39;impostazione di tolleranza da 0 a 1. L’impostazione 0 ritaglia i pixel solo se sono trasparenti. Con valori più vicini a 1 viene invece tollerata una minore trasparenza. Selezionare **[!UICONTROL Ritaglia]**.

1. Selezionare **[!UICONTROL Salva]**.

>[!NOTE]
>
>Per ripristinare lo stato originale di un&#39;immagine dopo averlo ritagliato, visualizzala nella schermata Editor ritaglio e seleziona **[!UICONTROL Ripristina]**.

## Selezionare un’area da ritagliare {#select-an-area-to-crop}

1. Per ritagliare un&#39;immagine, selezionane il pulsante rollover **[!UICONTROL Modifica]** e scegli **[!UICONTROL Ritaglia]**, oppure visualizzalo nel pannello Sfoglia in visualizzazione Dettagli e seleziona **[!UICONTROL Ritaglia]**.

1. Nella finestra Editor ritaglio, posizionate la parte dell’immagine da non ritagliare nella casella Ritaglio. Qualsiasi cosa appaia all&#39;interno della casella è ciò che rimarrà dopo aver selezionato **[!UICONTROL Salva]** e ritagliato l&#39;immagine.
1. Per regolare l’area di ritaglio, effettuate una delle seguenti operazioni:

   * Trascinate un lato o un angolo della casella. Tenete premuto il tasto Maiusc mentre trascinate per cambiare le dimensioni ma mantenere le stesse proporzioni (forma) del rettangolo di ritaglio.
   * Immettete le misure in pixel nelle caselle Dimensione.
   * Trascinate per spostare la casella di ritaglio. Spostate il puntatore all’interno della casella. Quando viene visualizzata la freccia a quattro punte, trascinate la casella sull’immagine in una nuova posizione.

1. Selezionare **[!UICONTROL Salva]**.

>[!NOTE]
>
>Per ripristinare lo stato originale di un&#39;immagine dopo averlo ritagliato, visualizzala nella schermata Editor ritaglio e seleziona **[!UICONTROL Ripristina]**.

>[!MORELIKETHIS]
>
>* [Opzioni per la modifica delle immagini al caricamento](image-editing-options-upload.md#image-editing-options-at-upload)
* [Ritaglio di spazio bianco da un file PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
* [Ritaglio dai lati delle pagine PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

