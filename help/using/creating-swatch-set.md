---
title: Creazione di un set di campioni
description: Scopri come creare un set di campioni in Adobe Dynamic Media Classic.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 67%

---

# Creazione di un set di campioni{#creating-a-swatch-set}

Un set di campioni offre agli utenti l’opportunità di visualizzare un articolo in un colore, un motivo o una finitura differente. Per creare un set di campioni, è necessario disporre di un’immagine per ciascun colore, motivo o finitura differente che desiderate presentare all’utente. È anche necessario disporre di un campione di colore, motivo o finitura per ciascuno di questi.

Ad esempio, per presentare immagini di berretti con visiere di diversi colori nelle varianti rosso, verde e blu, è necessario effettuare tre scatti dello stesso berretto: uno scatto con la visiera rossa, uno con quella verde e uno con quella blu. È anche necessario disporre di tre campioni colore: uno rosso, uno verde e uno blu. I campioni colore fungono da miniature selezionate dagli utenti nel Visualizzatore set di campioni per visualizzare il cappuccio con fattura rossa, verde o blu.

## Creazione di un set di campioni {#create}

Quando create un set, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| **[!UICONTROL Pubblica dopo il salvataggio]** opzione selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di campioni:**

1. Effettuate una delle seguenti operazioni:

   * **Seleziona prima le immagini** - Nel pannello Sfoglia, selezionare le immagini, quindi passare a **[!UICONTROL Genera]** > **[!UICONTROL Set campioni]**.

   * **Inizia dalla schermata Set campioni** - Vai a **[!UICONTROL Genera]** > **[!UICONTROL Set campioni]**. Selezionate una cartella nella Libreria risorse e trascinate le immagini per il set di campioni nella pagina Set campioni.

1. Trascinate i colori, i motivi o le finiture campione nella casella segnaposto Campioni nella pagina Set campioni.

   Verificate che il campione di colore, motivo o finitura trascinato in ciascun segnaposto rappresenti il colore, il motivo o la finitura dell’immagine adiacente.

1. Per modificare l’ordine delle immagini nel set di campioni, trascinate queste ultime in nuove posizioni.
1. Verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** (impostazione predefinita) nell’angolo inferiore destro della pagina sia selezionata.
1. Seleziona **[!UICONTROL Salva]**, selezionate una cartella per la memorizzazione del set di campioni colore, immettete un nome per il set e selezionate **[!UICONTROL Invia]**.
1. Per visualizzare il set di campioni nel visualizzatore del set di campioni, seleziona **[!UICONTROL Anteprima]** nella schermata Set campioni. Potete selezionare le miniature dei campioni nel Visualizzatore set di campioni per vedere come si comportano.

## Modifica di un set di campioni {#editing-a-swatch-set}

Sia che si modifichi un set pubblicato o non pubblicato, il **[!UICONTROL Pubblica dopo il salvataggio]** influisce sui membri set e set nei modi seguenti:

| Il set è già pubblicato | **[!UICONTROL Pubblica dopo]** salvare l’opzione selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di campioni:**

1. Nella Vista griglia, individuate un set di campioni e, sotto l&#39;immagine, selezionate **[!UICONTROL Modifica]**.
1. Effettuate una delle seguenti operazioni:

   * Per aggiungere un’immagine (pubblicata o non pubblicata), trascinatela da una cartella di Aggiungi risorse nella pagina **[!UICONTROL Visualizzazioni]** del set di campioni.
   * Per rimuovere un&#39;immagine, selezionarla e quindi selezionare **[!UICONTROL Elimina]** sulla barra degli strumenti.
   * Per riordinare le immagini, trascinate un’immagine fino alla posizione desiderata.

1. Al termine dell’operazione di modifica del set, verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, selezionare una cartella di archiviazione, immettere un nome per il set e quindi selezionare **[!UICONTROL Salva]**.

## Eliminare un set di campioni {#deleting-a-swatch-set}

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di campioni:**

1. Nella Vista griglia, Vista elenco o Vista dettagli, selezionate uno o più set di campioni.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.
