---
title: Creare un set di immagini
description: Scopri come creare un set di immagini in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 38%

---

# Creare un set di immagini{#creating-an-image-set}

Per creare un set di immagini a visualizzazione multipla, sono necessarie immagini di uno stesso elemento da più punti di vista o che mostrino diversi aspetti dello stesso elemento. L’obiettivo è quello di presentare agli utenti diverse immagini di un elemento, in modo che possano farsi un’idea concreta dell’aspetto o della funzione di quest’ultimo.

## Creare un set di immagini {#create}

Quando si crea un set, l&#39;opzione **[!UICONTROL Publish dopo il salvataggio]** ha effetto sui membri del set e del set nei modi seguenti:

| Opzione **[!UICONTROL `Publish after a save`]** selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

Quando crei un set di immagini, Adobe consiglia le seguenti best practice e applica i seguenti limiti:

| Tipo di limite | Best practice | Limite imposto |
| --- | --- | --- |
| Numero di risorse duplicate per set | Nessun duplicato | 20‡ |
| Numero massimo di immagini per set | 5-10 immagini per set | 1000 |

‡ Si consiglia di non avere risorse duplicate in un set. Il limite è di 20 duplicati per una singola risorsa. Se, all’interno del set, aggiungi un altro duplicato per tale risorsa, la richiesta restituisce un errore o ignora il duplicato.

Vedi anche [Limitazioni di Dynamic Medie](/help/using/limitations.md).

**Per creare un set di immagini:**

1. Effettuate una delle seguenti operazioni:

   * **Seleziona prima le immagini**: nel pannello Sfoglia, seleziona le immagini desiderate per il set di immagini, passa a **[!UICONTROL Build]** > **[!UICONTROL Set di immagini]**.

   * **Inizia dalla schermata Set immagini**: passa a **[!UICONTROL Build]** > **[!UICONTROL Set immagini]**. Viene visualizzata la schermata Set immagini. Selezionate una cartella nella Libreria risorse e trascinate le immagini per il set di immagini nella schermata Set immagini.

1. Per modificare l’ordine delle immagini, trascinate queste ultime in nuove posizioni.
1. Nell&#39;angolo inferiore destro della pagina, assicurati che sia selezionato **[!UICONTROL Publish dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, seleziona una cartella per l&#39;archiviazione del set di immagini, immetti un nome per il set, quindi seleziona **[!UICONTROL Salva]**.
1. Per visualizzare il set di immagini nel visualizzatore set di immagini, seleziona **[!UICONTROL Anteprima]** nella schermata set di immagini. Per vedere come si comportano, potete selezionare le miniature dei campioni nel Visualizzatore set di immagini.

## Modificare un set di immagini {#editing-an-image-set}

Sia che si modifichi un set pubblicato o non pubblicato, l&#39;opzione **[!UICONTROL Publish dopo il salvataggio]** ha effetto sui membri del set e del set nei modi seguenti:

| Il set è già pubblicato | Opzione **[!UICONTROL `Publish after a save`]** selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono lo stato pubblicato. I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di immagini:**

1. Nella visualizzazione griglia, passare a un set di immagini, quindi selezionare **[!UICONTROL Modifica]** sotto l&#39;immagine.
1. Effettuate una delle seguenti operazioni:

   * Per aggiungere un&#39;immagine (pubblicata o non pubblicata), trascinarla da una cartella in Aggiungi Assets nella pagina **[!UICONTROL Visualizzazioni]** del set di immagini.
   * Per rimuovere un&#39;immagine, selezionarla, quindi selezionare **[!UICONTROL Elimina]** sulla barra degli strumenti.
   * Per riordinare le immagini, trascinate un’immagine fino alla posizione desiderata.

1. Al termine della modifica del set, vicino all&#39;angolo inferiore destro della pagina, assicurati che sia selezionato **[!UICONTROL Publish dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, seleziona una cartella di archiviazione per il set, immetti un nome per il set, quindi seleziona **[!UICONTROL Salva]**.

## Eliminare un set di immagini

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (o &quot;figli&quot;) all&#39;interno di quel set non sono interessati; invece, ciascuno di essi mantiene il proprio stato pubblicato o non pubblicato esistente.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di immagini:**

1. In Vista griglia, Vista elenco o Vista dettagli, selezionare uno o più set di immagini.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.
