---
title: Spostare, rinominare ed eliminare le risorse
description: Scopri come spostare, rinominare ed eliminare le risorse in Adobe Dynamic Media Classic.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 31%

---

# Spostare, rinominare ed eliminare le risorse{#moving-renaming-and-deleting-assets}

Dal pannello Sfoglia potete spostare, rinominare ed eliminare le risorse. Inoltre, potete eliminare più risorse contemporaneamente con un file di testo.

## Spostare le risorse {#move-assets}

Potete spostare le risorse in altre cartelle del pannello Sfoglia.

**Per spostare le risorse:**

1. Selezionate la risorsa o le risorse nel pannello Sfoglia, quindi effettuate una delle seguenti operazioni:

   * Visualizza la cartella in cui desideri spostare le risorse nella Libreria risorse e trascina le risorse nella cartella.
   * Vai a **[!UICONTROL File]** > **[!UICONTROL Sposta]**, seleziona una cartella nella finestra Sposta risorse e seleziona **[!UICONTROL Sposta]**.

## Rinominare le risorse {#rename-assets}

1. Selezionate la risorsa nel pannello Sfoglia, quindi effettuate una delle seguenti operazioni:

   * Selezionare il nome, digitare un nuovo nome e premere **[!UICONTROL Invio]** oppure selezionala lontano dal nome.
   * Vai a **[!UICONTROL File]** > **[!UICONTROL Rinomina]**. Il nome della risorsa viene evidenziato. Inserisci un nuovo nome e premi **[!UICONTROL Invio]**. Assicurati di non inserire il nome di una risorsa Adobe Dynamic Media Classic esistente.

## Eliminare le risorse {#delete-assets}

Puoi eliminare le risorse selezionate nel pannello Sfoglia ed eliminare intere cartelle. Le risorse e le cartelle eliminate vengono spostate nella cartella Cestino, dove restano per sette giorni prima di essere eliminate definitivamente. 

Quando eliminate un risorsa, vengono anche eliminate tutte le risorse derivate. Ad esempio, se eliminate un’immagine per la quale avete creato delle destinazioni di zoom, anche queste ultime vengono eliminate.

le destinazioni di zoom, gli attributi immagine e le voci della cronologia vengono eliminati definitivamente quando rimuovete le risorse da cui derivano. Poiché non vengono spostate nel Cestino insieme alla risorsa, non possono essere ripristinate dal Cestino.

>[!IMPORTANT]
>
>L’eliminazione in blocco è un’operazione intensiva. Assicurati di eseguire le eliminazioni in blocco in sequenza anziché come operazioni di eliminazione simultanee e complesse. L’Adobe consiglia di limitare le operazioni di eliminazione a un massimo di 5000 eliminazioni di risorse all’ora. Un numero superiore a 5000 all&#39;ora può causare una limitazione della velocità.

**Per eliminare le risorse:**

1. Effettuate una delle seguenti operazioni:

   * Per eliminare una o più risorse, selezionale nel pannello Sfoglia e premi **[!UICONTROL Elimina]** o vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]**.
   * Per eliminare una cartella, selezionala nella Libreria risorse, quindi fai clic su **[!UICONTROL Rimuovi cartella]**.

     Quando si elimina una cartella, vengono eliminati anche la cartella, tutte le risorse presenti nella cartella e tutte le risorse presenti nelle relative sottocartelle.

Adobe Dynamic Media Classic consiglia di sovrascrivere i file di risorse anziché eliminarli se il motivo per cui si elimina un file di risorse è quello di sostituirlo con un altro con lo stesso nome.

## Eliminare più risorse con un file di testo {#delete-multiple-assets-with-a-text-file}

Per eliminare più risorse contemporaneamente in tutta la Libreria risorse, puoi elencare le risorse da eliminare in un file di testo e inviare l’elenco a Adobe Dynamic Media Classic.

Crea l&#39;elenco degli ID Adobe Dynamic Media Classic e salvalo come file di testo (.txt). Ogni Adobe Dynamic Media Classic ID deve trovarsi sulla propria riga (seguita da un ritorno a capo).

Una volta creato l’elenco, effettuate le operazioni seguenti:

1. Vai a **[!UICONTROL File]** > **[!UICONTROL Elimina elenco risorse]**.
1. Nella finestra di dialogo Elimina elenco risorse, sfoglia o digita il percorso del file di testo con l’elenco delle risorse da eliminare.
1. Seleziona **[!UICONTROL Elimina]**.

Quando elimini le risorse con un file di testo, se nell’elenco non è presente alcun ID Adobe Dynamic Media Classic, viene visualizzato il messaggio &quot;Impossibile convalidare queste voci nell’elenco:&quot;. Viene inoltre visualizzato l&#39;elenco delle voci. Tuttavia, Adobe Dynamic Media Classic non genera un errore nella pagina Job (Processo).

>[!MORELIKETHIS]
>
>* [Selezionare le risorse nel pannello Sfoglia](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparare risorse e cartelle per il caricamento](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Ripristinare le risorse dalla cartella Cestino](trash-folder.md#restoring_assets_from_the_trash_folder)
