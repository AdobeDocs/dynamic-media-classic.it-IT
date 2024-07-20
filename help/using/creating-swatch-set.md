---
title: Creazione di un set di campioni
description: Scopri come creare un set di campioni in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 49%

---

# Creazione di un set di campioni{#creating-a-swatch-set}

Un set di campioni offre agli utenti l’opportunità di visualizzare un articolo in un colore, un motivo o una finitura differente. Per creare un set di campioni, è necessario disporre di un’immagine per ciascun colore, motivo o finitura differente che desiderate presentare all’utente. È anche necessario disporre di un campione di colore, motivo o finitura per ciascuno di questi.

Ad esempio, per presentare immagini di berretti con visiere di diversi colori nelle varianti rosso, verde e blu, è necessario effettuare tre scatti dello stesso berretto: uno scatto con la visiera rossa, uno con quella verde e uno con quella blu. È anche necessario disporre di tre campioni colore: uno rosso, uno verde e uno blu. I campioni colore fungono da miniature selezionate dagli utenti nel Visualizzatore set di campioni per visualizzare il cappuccio con fattura rossa, verde o blu.

## Creazione di un set di campioni {#create}

Quando si crea un set, l&#39;opzione **Publish dopo il salvataggio** ha effetto sui membri del set e del set nei modi seguenti:

| **[!UICONTROL Publish dopo aver selezionato un&#39;opzione di salvataggio]** prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di campioni:**

1. Effettuate una delle seguenti operazioni:

   * **Selezionare prima le immagini**: nel pannello Sfoglia, selezionare le immagini, quindi passare a **[!UICONTROL Build]** > **[!UICONTROL Set campioni]**.

   * **Inizia dalla schermata Set campioni**: passa a **[!UICONTROL Build]** > **[!UICONTROL Set campioni]**. Selezionate una cartella nella Libreria risorse e trascinate le immagini per il set di campioni nella pagina Set campioni.

1. Trascinate i colori, i motivi o le finiture campione nella casella segnaposto Campioni nella pagina Set campioni.

   Verificate che il campione di colore, motivo o finitura trascinato in ciascun segnaposto rappresenti il colore, il motivo o la finitura dell’immagine adiacente.

1. Per modificare l’ordine delle immagini nel set di campioni, trascinate queste ultime in nuove posizioni.
1. Nell&#39;angolo inferiore destro della pagina, assicurati che sia selezionato **[!UICONTROL Publish dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, seleziona una cartella per la memorizzazione del set di campioni colore, immetti un nome per il set e seleziona **[!UICONTROL Invia]**.
1. Per visualizzare il set di campioni nel visualizzatore del set di campioni, seleziona **[!UICONTROL Anteprima]** nella schermata Set di campioni. Potete selezionare le miniature dei campioni nel Visualizzatore set di campioni per vedere come si comportano.

## Modifica di un set di campioni {#editing-a-swatch-set}

Sia che si modifichi un set pubblicato o non pubblicato, l&#39;opzione **[!UICONTROL Publish dopo il salvataggio]** ha effetto sui membri del set e del set nei modi seguenti:

| Il set è già pubblicato | **[!UICONTROL Publish dopo aver selezionato l&#39;opzione di salvataggio]** prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato. |
| Sì | No | Pubblicato | I membri del set esistenti mantengono lo stato pubblicato. I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato. |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di campioni:**

1. Nella visualizzazione griglia, individuare un set di campioni e quindi, sotto l&#39;immagine, selezionare **[!UICONTROL Modifica]**.
1. Effettuate una delle seguenti operazioni:

   * Per aggiungere un&#39;immagine (pubblicata o non pubblicata), trascinarla da una cartella in Aggiungi Assets nella pagina **[!UICONTROL Visualizzazioni]** del set di campioni.
   * Per rimuovere un&#39;immagine, selezionarla, quindi selezionare **[!UICONTROL Elimina]** sulla barra degli strumenti.
   * Per riordinare le immagini, trascinate un’immagine fino alla posizione desiderata.

1. Al termine della modifica del set, vicino all&#39;angolo inferiore destro della pagina, assicurati che sia selezionato **[!UICONTROL Publish dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, seleziona una cartella di archiviazione, immetti un nome per il set, quindi seleziona **[!UICONTROL Salva]**.

## Eliminare un set di campioni

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (o &quot;figli&quot;) all&#39;interno di quel set non sono interessati; invece, ciascuno di essi mantiene il proprio stato pubblicato o non pubblicato esistente.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di campioni:**

1. Nella Vista griglia, Vista elenco o Vista dettagli, selezionate uno o più set di campioni.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.
