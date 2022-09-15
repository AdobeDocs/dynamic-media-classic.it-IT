---
title: Ritagliare un’immagine
description: Scopri come ritagliare un’immagine in Adobe Dynamic Media Classic.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 35%

---

# Ritagliare un’immagine{#cropping-an-image}

È possibile ritagliare le immagini in Adobe Dynamic Media Classic. Il sistema conserva le informazioni sulle immagini ritagliate per permettere di riportarle eventualmente al loro stato originale. Potete anche ritagliare un’immagine e salvare la versione ritagliata con un nuovo nome.

Potete ritagliare un’immagine per rimuovere lo spazio bianco che la circonda oppure ritagliare un’area dell’immagine.

>[!NOTE]
>
>Dopo aver ritagliato, potete selezionare **[!UICONTROL Salva con nome]** e salvare una versione ritagliata dell&#39;immagine con un nome diverso. Nella finestra Salva con nome, seleziona **[!UICONTROL Salva come nuovo principale]** per salvare una seconda copia dell&#39;immagine. Seleziona **[!UICONTROL Salva Come Vista Aggiuntiva Della Master]** in modo da poter salvare l&#39;originale e la relativa versione ritagliata con un nome diverso. Seleziona **[!UICONTROL Sostituisci originale]** per eliminare il file originale dal quale è stata ritagliata l&#39;immagine. Quindi immetti un nome per l’immagine e seleziona **[!UICONTROL Invia]**.

## Ritagliare per rimuovere lo spazio bianco intorno a un’immagine {#crop-to-remove-white-space-around-an-image}

Potete eliminare i pixel trasparenti o in tinta unita dal bordo di un’immagine ritagliandoli.

1. Per ritagliare un’immagine, selezionane il rollover **[!UICONTROL Modifica]** quindi seleziona **[!UICONTROL Ritaglio]** oppure visualizzalo nel pannello Sfoglia in Vista dettagli e seleziona la **[!UICONTROL Ritaglio]** pulsante .
1. Nella pagina Editor ritaglio, effettuare una delle seguenti operazioni:

   * Per tagliare i pixel del colore, vai a **[!UICONTROL Rifila]** > **[!UICONTROL Colore]**. In **[!UICONTROL Ritaglio automatico per colore]** seleziona la finestra di dialogo **[!UICONTROL Angolo]** scegliere un angolo con il colore di sfondo che si desidera ritagliare. Quindi inserisci un **[!UICONTROL Tolleranza]** da 0 a 1. L’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo dell’immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. Seleziona **[!UICONTROL Ritaglio]**.
   * Per tagliare i pixel trasparenti, vai a **[!UICONTROL Rifila]** > **[!UICONTROL Trasparente]**. In **[!UICONTROL Ritaglio automatico per trasparenza]** immettere un&#39;impostazione di tolleranza da 0 a 1. L’impostazione 0 ritaglia i pixel solo se sono trasparenti. Con valori più vicini a 1 viene invece tollerata una minore trasparenza. Seleziona **[!UICONTROL Ritaglio]**.

1. Seleziona **[!UICONTROL Salva]**.

>[!NOTE]
>
>Per ripristinare lo stato originale di un’immagine dopo averlo ritagliato, visualizzala nella schermata Editor ritaglio e seleziona **[!UICONTROL Reimposta]**.

## Selezionare un’area da ritagliare {#select-an-area-to-crop}

1. Per ritagliare un’immagine, selezionane il rollover **[!UICONTROL Modifica]** e scegli **[!UICONTROL Ritaglio]** oppure visualizzarla nel pannello Sfoglia in visualizzazione Dettagli e selezionare **[!UICONTROL Ritaglio]**.

1. Nella finestra Editor ritaglio, posizionate la parte dell’immagine da non ritagliare nella casella Ritaglio. Qualsiasi cosa appaia all&#39;interno della casella è ciò che rimarrà dopo aver selezionato **[!UICONTROL Salva]** e ritagliare l&#39;immagine.
1. Per regolare l’area di ritaglio, effettuate una delle seguenti operazioni:

   * Trascinate un lato o un angolo della casella. Tenete premuto il tasto Maiusc mentre trascinate per cambiare le dimensioni ma mantenere le stesse proporzioni (forma) del rettangolo di ritaglio.
   * Immettete le misure in pixel nelle caselle Dimensione.
   * Trascinate per spostare la casella di ritaglio. Spostate il puntatore all’interno della casella. Quando viene visualizzata la freccia a quattro punte, trascinate la casella sull’immagine in una nuova posizione.

1. Seleziona **[!UICONTROL Salva]**.

>[!NOTE]
>
>Per ripristinare lo stato originale di un’immagine dopo averlo ritagliato, visualizzala nella schermata Editor ritaglio e seleziona **[!UICONTROL Reimposta]**.

>[!MORELIKETHIS]
>
>* [Opzioni per la modifica delle immagini al caricamento](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Ritaglio dello spazio bianco da un file PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Ritaglio dai lati delle pagine di PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

