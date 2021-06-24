---
title: Spostamento, ridenominazione ed eliminazione di risorse
description: Scopri come spostare, rinominare ed eliminare le risorse.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Gestione risorse
role: Business Practitioner
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 44%

---

# Spostamento, ridenominazione ed eliminazione di risorse{#moving-renaming-and-deleting-assets}

Dal pannello Sfoglia potete spostare, rinominare ed eliminare le risorse. Inoltre, potete eliminare più risorse contemporaneamente con un file di testo.

## Spostare le risorse {#move-assets}

Potete spostare le risorse in altre cartelle del pannello Sfoglia.

1. Selezionate la risorsa o le risorse nel pannello Sfoglia, quindi effettuate una delle seguenti operazioni:

   * Nella Libreria risorse, visualizzate la cartella in cui desiderate spostare le risorse e trascinatele in essa.
   * Fai clic su **[!UICONTROL File]** > **[!UICONTROL Sposta]**, seleziona una cartella nella finestra Sposta risorse e seleziona **[!UICONTROL Sposta]**.

## Rinominare le risorse {#rename-assets}

1. Selezionate la risorsa nel pannello Sfoglia, quindi effettuate una delle seguenti operazioni:

   * Seleziona il nome, digita un nuovo nome e premi **[!UICONTROL Invio]** oppure fai clic lontano dal nome.
   * Fare clic su **[!UICONTROL File]** > **[!UICONTROL Rinomina]**. Il nome della risorsa viene evidenziato. Immettere un nuovo nome e premere **[!UICONTROL Invio]**.

Assicurati di non inserire il nome di una risorsa Dynamic Media Classic esistente.

## Eliminare le risorse {#delete-assets}

Potete eliminare le risorse selezionate nel pannello Sfoglia ed eliminare intere cartelle. Le risorse e le cartelle eliminate vengono spostate nella cartella Cestino, dove restano per sette giorni prima di essere eliminate definitivamente. 

Quando eliminate un risorsa, vengono anche eliminate tutte le risorse derivate. Ad esempio, se eliminate un’immagine per la quale avete creato delle destinazioni di zoom, anche queste ultime vengono eliminate.

>[!NOTE]
>
>le destinazioni di zoom, gli attributi immagine e le voci della cronologia vengono eliminati definitivamente quando rimuovete le risorse da cui derivano. Poiché non vengono spostate nel Cestino insieme alla risorsa, non possono essere ripristinate dal Cestino.

1. Effettuate una delle seguenti operazioni:

   * Per eliminare una o più risorse, selezionale nel pannello Sfoglia e premi **[!UICONTROL Elimina]** oppure fai clic su **[!UICONTROL File]** > **[!UICONTROL Elimina]**.
   * Per eliminare una cartella, selezionala nella Libreria risorse e fai clic su **[!UICONTROL Rimuovi cartella]**.

      Se si elimina una cartella, vengono eliminate tutte le risorse presenti nella cartella e tutte le relative sottocartelle.

>[!NOTE]
>
>Dynamic Media Classic consiglia di sovrascrivere i file di risorse anziché eliminarli se si desidera sostituire un file di risorse con un altro con lo stesso nome.

## Eliminare più risorse con un file di testo {#delete-multiple-assets-with-a-text-file}

Per eliminare più risorse contemporaneamente nella libreria delle risorse, puoi elencare le risorse da eliminare in un file di testo e inviare l’elenco a Dynamic Media Classic.

Crea l’elenco degli ID di Dynamic Media Classic e salvalo come file di testo (.txt). Ogni ID Dynamic Media Classic deve trovarsi sulla propria riga (seguito da un ritorno a capo).

Una volta creato l’elenco, effettuate le operazioni seguenti:

1. Fai clic su **[!UICONTROL File]** > **[!UICONTROL Elimina elenco risorse]**.
1. Nella finestra di dialogo Elimina elenco risorse , sfoglia o digita il percorso del file di testo con l’elenco delle risorse da eliminare.
1. Fate clic su **[!UICONTROL Elimina]**.

Quando elimini le risorse con un file di testo, se un ID Dynamic Media Classic non è presente nell’elenco, viene visualizzato il messaggio &quot;Impossibile convalidare queste voci nell’elenco:&quot; e l’elenco delle voci. Tuttavia, Dynamic Media Classic non genera un errore nella pagina Processo.

>[!MORELIKETHIS]
>
>* [Selezione delle risorse nel pannello Sfoglia](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
* [Preparazione delle risorse e delle cartelle per il caricamento](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
* [Ripristino delle risorse dalla cartella Cestino](trash-folder.md#restoring_assets_from_the_trash_folder)

