---
title: Spostamento, ridenominazione ed eliminazione di risorse
seo-title: Spostamento, ridenominazione ed eliminazione di risorse
description: 'null'
seo-description: Scoprite come spostare, rinominare ed eliminare le risorse.
uuid: deff 6521-0 ad 0-4 db 9-b 4 e 0-e 3211 ff 97740
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: 1 c 9 e 29 f 0-3083-4 d 22-a 439-2 a 01 faf 59683
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Spostamento, ridenominazione ed eliminazione di risorse{#moving-renaming-and-deleting-assets}

Dal pannello Sfoglia potete spostare, rinominare ed eliminare le risorse. Inoltre, potete eliminare più risorse contemporaneamente con un file di testo.

## Spostare le risorse {#move-assets}

Potete spostare le risorse in altre cartelle del pannello Sfoglia.

1. Selezionate la risorsa o le risorse nel pannello Sfoglia, quindi effettuate una delle seguenti operazioni:

   * Nella Libreria risorse, visualizzate la cartella in cui desiderate spostare le risorse e trascinatele in essa.
   * Scegliete File &gt; Sposta, selezionate una cartella nella finestra Sposta risorse, quindi fate clic su Sposta.

## Rinominare le risorse {#rename-assets}

Per rinominare una risorsa, effettuate le seguenti operazioni:

1. Selezionate la risorsa nel pannello Sfoglia, quindi effettuate una delle seguenti operazioni:

   * Selezionate il nome, digitate un nuovo nome, quindi premete Invio o fate clic in un altro punto della schermata.
   * Scegliete File &gt; Rinomina. Il nome della risorsa viene evidenziato. Immettete un nuovo nome e premete Invio.

Accertatevi di non inserire il nome di un risorsa esistente di Scene7 Publishing System.

## Eliminare le risorse {#delete-assets}

Potete eliminare le risorse selezionate nel pannello Sfoglia, nonché intere cartelle. Le risorse e le cartelle eliminate vengono spostate nella cartella Cestino, dove restano per sette giorni prima di essere eliminate definitivamente. 

Quando eliminate un risorsa, vengono anche eliminate tutte le risorse derivate. Ad esempio, se eliminate un’immagine per la quale avete creato delle destinazioni di zoom, anche queste ultime vengono eliminate.

>[!NOTE]
>
>le destinazioni di zoom, gli attributi immagine e le voci della cronologia vengono eliminati definitivamente quando rimuovete le risorse da cui derivano. Poiché non vengono spostate nel Cestino insieme alla risorsa, non possono essere ripristinate dal Cestino.

1. Effettuate una delle seguenti operazioni:

   * Per eliminare una o più risorse, selezionatele nel pannello Sfoglia, quindi premete Canc o scegliete File &gt; Elimina.
   * To delete a folder, select the folder in the Asset Library, and click **Remove Folder**.

      Se eliminate una cartella, verranno eliminate la cartella, tutte le risorse presenti in essa, nonché tutte le risorse nelle relative sottocartelle.

>[!NOTE]
>
>Dynamic Media Classic consiglia di sovrascrivere i file di risorse invece di eliminarli se il motivo per eliminare un file di risorsa consiste nell'sostituirlo con un altro nome.

## Eliminare più risorse con un file di testo {#delete-multiple-assets-with-a-text-file}

Per eliminare più risorse contemporaneamente nella Libreria risorse, potete elencare le risorse da eliminare in un file di testo e inviare l'elenco a Dynamic Media Classic.

Create un elenco di ID Scene7 Publishing System e salvatelo come file di testo (.txt). Ogni ID Scene7 Publishing System deve essere su una propria riga (seguito da un ritorno a capo).

Una volta creato l’elenco, effettuate le operazioni seguenti:

1. Scegliete File &gt; Elimina elenco risorse.
1. Nella finestra di dialogo Elimina elenco risorse, individuate o digitate il percorso del file di testo contenente l’elenco delle risorse da eliminare.
1. Fate clic sul pulsante Elimina.

Quando eliminate le risorse con un file di testo, se un ID Scene 7 Publishing System non è presente nell'elenco, viene visualizzato un messaggio che informa che Dynamic Media Classic è impossibile convalidare le voci nell'elenco: » insieme all'elenco delle voci. Tuttavia, Dynamic Media Classic non genera un errore nella schermata Processo.

>[!MORELIKETHIS]
>
>* [Selezione delle risorse nel pannello Sfoglia](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparazione delle risorse e delle cartelle per il caricamento](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Ripristino delle risorse dalla cartella Cestino](trash-folder.md#restoring_assets_from_the_trash_folder)

