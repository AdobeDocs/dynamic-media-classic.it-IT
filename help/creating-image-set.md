---
title: Creare un set di immagini
description: Scopri come creare un set di immagini in Adobe Dynamic Media Classic.
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 59%

---

# Creare un set di immagini{#creating-an-image-set}

Per creare un set di immagini a visualizzazione multipla, sono necessarie immagini di uno stesso elemento da più punti di vista o che mostrino diversi aspetti dello stesso elemento. L’obiettivo è quello di presentare agli utenti diverse immagini di un elemento, in modo che possano farsi un’idea concreta dell’aspetto o della funzione di quest’ultimo.

## Creare un set di immagini {#create}

Quando create un set, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** incide su set e relativi membri nei seguenti modi:

| **[!UICONTROL Pubblica dopo il salvataggio]** opzione selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

Quando crei un set di immagini, Adobe consiglia le seguenti best practice e applica i seguenti limiti:

| Tipo di limite | Best practice | Limite imposto |
| --- | --- | --- |
| Numero di risorse duplicate per set | Nessun duplicato | 20 |
| Numero massimo di immagini per set | 5-10 immagini per set | 1000 |

Vedi anche [Limiti Dynamic Media](/help/limitations.md).

**Per creare un set di immagini:**

1. Effettuate una delle seguenti operazioni:

   * **Seleziona prima le immagini** - Nel pannello Sfoglia, seleziona le immagini desiderate per il set di immagini, vai a **[!UICONTROL Crea]** > **[!UICONTROL Set di immagini]**.

   * **Inizia dalla schermata Set di immagini** - Vai a **[!UICONTROL Crea]** > **[!UICONTROL Set di immagini]**. Viene visualizzata la schermata Set immagini. Selezionate una cartella nella Libreria risorse e trascinate le immagini per il set di immagini nella schermata Set immagini.

1. Per modificare l’ordine delle immagini, trascinate queste ultime in nuove posizioni.
1. Verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** (impostazione predefinita) nell’angolo inferiore destro della pagina sia selezionata.
1. Seleziona **[!UICONTROL Salva]**, seleziona una cartella in cui memorizzare il set di immagini, immetti un nome per il set, quindi seleziona **[!UICONTROL Salva]**.
1. Per visualizzare il set di immagini nel visualizzatore dei set di immagini, seleziona **[!UICONTROL Anteprima]** nella schermata Set immagini. È possibile selezionare le miniature dei campioni nel Visualizzatore set di immagini per verificarne il funzionamento.

## Modificare un set di immagini {#editing-an-image-set}

Se modifichi un set pubblicato o non pubblicato, la **[!UICONTROL Pubblica dopo il salvataggio]** influenza i membri set e set nei seguenti modi:

| Il set è già pubblicato | **[!UICONTROL Pubblica dopo il salvataggio]** opzione selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di immagini:**

1. Nella Vista a griglia, individuare un ImageSet e quindi selezionare sotto l&#39;immagine **[!UICONTROL Modifica]**.
1. Effettuate una delle seguenti operazioni:

   * Per aggiungere un’immagine (pubblicata o non pubblicata), trascinatela da una cartella di Aggiungi risorse nella pagina **[!UICONTROL Visualizzazioni]** del set di immagini.
   * Per rimuovere un’immagine, selezionala e seleziona **[!UICONTROL Elimina]** sulla barra degli strumenti.
   * Per riordinare le immagini, trascinate un’immagine fino alla posizione desiderata.

1. Al termine dell’operazione di modifica del set, verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, seleziona una cartella di archiviazione per il set, immetti un nome per il set, quindi seleziona **[!UICONTROL Salva]**.

## Eliminare un set di immagini {#deleting-an-image-set}

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di immagini:**

1. Nella vista Griglia, Elenco o Dettagli, selezionare uno o più set di immagini.
1. Nella barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.
