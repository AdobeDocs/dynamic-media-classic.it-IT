---
title: Spostamento, ridenominazione ed eliminazione di risorse
description: Scoprite come spostare, rinominare ed eliminare le risorse.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 66%

---


# Spostamento, ridenominazione ed eliminazione di risorse{#moving-renaming-and-deleting-assets}

Dal pannello Sfoglia potete spostare, rinominare ed eliminare le risorse. Inoltre, potete eliminare più risorse contemporaneamente con un file di testo.

## Spostare le risorse {#move-assets}

Potete spostare le risorse in altre cartelle del pannello Sfoglia.

1. Selezionate la risorsa o le risorse nel pannello Sfoglia, quindi effettuate una delle seguenti operazioni:

   * Nella Libreria risorse, visualizzate la cartella in cui desiderate spostare le risorse e trascinatele in essa.
   * Scegliete File > Sposta, selezionate una cartella nella finestra Sposta risorse, quindi fate clic su Sposta.

## Rinominare le risorse  {#rename-assets}

Per rinominare una risorsa, effettuate le seguenti operazioni:

1. Selezionate la risorsa nel pannello Sfoglia, quindi effettuate una delle seguenti operazioni:

   * Selezionate il nome, digitate un nuovo nome, quindi premete Invio o fate clic in un altro punto della schermata.
   * Scegliete File > Rinomina. Il nome della risorsa viene evidenziato. Immettete un nuovo nome e premete Invio.

Accertatevi di non immettere il nome di una risorsa Dynamic Media Classic esistente.

## Eliminare le risorse {#delete-assets}

Potete eliminare le risorse selezionate nel pannello Sfoglia, nonché intere cartelle. Le risorse e le cartelle eliminate vengono spostate nella cartella Cestino, dove restano per sette giorni prima di essere eliminate definitivamente. 

Quando eliminate un risorsa, vengono anche eliminate tutte le risorse derivate. Ad esempio, se eliminate un’immagine per la quale avete creato delle destinazioni di zoom, anche queste ultime vengono eliminate.

>[!NOTE]
>
>le destinazioni di zoom, gli attributi immagine e le voci della cronologia vengono eliminati definitivamente quando rimuovete le risorse da cui derivano. Poiché non vengono spostate nel Cestino insieme alla risorsa, non possono essere ripristinate dal Cestino.

1. Effettuate una delle seguenti operazioni:

   * Per eliminare una o più risorse, selezionatele nel pannello Sfoglia, quindi premete Canc o scegliete File > Elimina.
   * Per eliminare una cartella, selezionatela nella Libreria risorse e fate clic su **Rimuovi cartella**.

      Se eliminate una cartella, verranno eliminate la cartella, tutte le risorse presenti in essa, nonché tutte le risorse nelle relative sottocartelle.

>[!NOTE]
>
>Dynamic Media Classic consiglia di sovrascrivere i file di risorse invece di eliminarli se intendete sostituire un file di risorse con un altro con lo stesso nome.

## Eliminare più risorse con un file di testo {#delete-multiple-assets-with-a-text-file}

Per eliminare più risorse alla volta nella Libreria risorse, potete elencare le risorse da eliminare in un file di testo e inviare l’elenco ad Dynamic Media Classic.

Create l’elenco degli ID Dynamic Media Classic e salvatelo come file di testo (.txt). Ogni Dynamic Media Classic ID deve essere su una propria riga (seguito da un ritorno a capo).

Una volta creato l’elenco, effettuate le operazioni seguenti:

1. Scegliete File > Elimina elenco risorse.
1. Nella finestra di dialogo Elimina elenco risorse, individuate o digitate il percorso del file di testo contenente l’elenco delle risorse da eliminare.
1. Fate clic sul pulsante Elimina.

Quando eliminate delle risorse con un file di testo, se un ID Dynamic Media Classic non è presente nell’elenco, viene visualizzato un messaggio che informa che Dynamic Media Classic è &quot;Impossibile convalidare queste voci nell’elenco:&quot; insieme all’elenco delle voci. Tuttavia, Dynamic Media Classic non genera un errore nella schermata Processo.

>[!MORELIKETHIS]
>
>* [Selezione delle risorse nel pannello Sfoglia](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparazione delle risorse e delle cartelle per il caricamento](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Ripristino delle risorse dalla cartella Cestino](trash-folder.md#restoring_assets_from_the_trash_folder)

