---
title: Carica file modello
description: Scopri come caricare i file modello in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
topic: Content Management
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 32%

---

# Carica file modello{#uploading-template-files}

Carica i file necessari per il modello in Adobe Dynamic Media Classic prima di iniziare a creare il modello. Puoi creare modelli da un Adobe ® Photoshop® PSD o da un file di immagine. Si consiglia di usare immagini TIFF e PNG poiché consentono la trasparenza.

>[!NOTE]
>
>Adobe Dynamic Media Classic consiglia di utilizzare immagini TIFF o PSD trasparenti nei modelli nelle dimensioni esatte che si desidera visualizzare nel sito Web. Quando pubblicate il modello, richiamate l’immagine mediante un predefinito per immagini che abbia anch’esso le stesse dimensioni. È importante prestare attenzione alle dimensioni per evitare che il modello venga ridimensionato (ricampionato) in dimensioni maggiore o inferiori rispetto alle dimensioni originali.

È possibile creare modelli da file PSD di Adobe Photoshop o file immagine.

Per istruzioni dettagliate sul caricamento dei file, vedere [Carica file](uploading-files.md#uploading_files). Tenete in mente quanto segue per il caricamento dei file modello:

* Se carichi un file PSD, puoi crearne uno nuovo. Adobe Dynamic Media Classic crea un&#39;immagine separata per ogni livello del PSD. Nella finestra di dialogo Opzioni processo di caricamento selezionare **[!UICONTROL Opzioni Photoshop]**, quindi selezionare **[!UICONTROL Gestisci livelli]** e **[!UICONTROL Crea modello]**. Quindi scegli un&#39;opzione dall&#39;elenco a discesa **[!UICONTROL Denominazione livelli]** per denominare le immagini create da Adobe Dynamic Media Classic dai livelli in PSD.
Consultate [Opzioni di caricamento PSD](psd-files.md#psd_upload_options).
<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [Carica i file](uploading-files.md#uploading_your_files)
>* [Utilizzare i file PSD](psd-files.md#working_with_psd_files)
