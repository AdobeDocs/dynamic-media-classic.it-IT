---
title: Creare un set di immagini
description: Scopri come creare un set di immagini in Adobe Systems Dynamic Media Classic.
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

| **[!UICONTROL Publish dopo l&#39;opzione Salva]** selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

Quando crei un Immagine insieme, Adobe Systems consiglia le seguenti Best practice e impone i seguenti limiti:

| Tipo limite | Best practice | Limite imposto |
| --- | --- | --- |
| Numero di risorse duplicati per insieme | Nessun duplicato | 20 |
| Numero massimo di immagini per insieme | 5-10 immagini per insieme | 1000 |

Vedi anche [ Dynamic Media limitazioni ](/help/limitations.md) .

**Per creare un set di immagini:**

1. Effettuate una delle seguenti operazioni:

   * **Seleziona prima** le immagini-nel pannello Sfoglia, seleziona le immagini desiderate per il tuo immagine set, vai a **[!UICONTROL Build]** > **[!UICONTROL immagine sets]** .

   * **Inizia dalla schermata** immagine set-vai a **[!UICONTROL Build]** > **[!UICONTROL immagine set]** . Viene visualizzata la schermata Set immagini. Selezionate una cartella nella Libreria risorse e trascinate le immagini per il set di immagini nella schermata Set immagini.

1. Per modificare l’ordine delle immagini, trascinate queste ultime in nuove posizioni.
1. Verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** (impostazione predefinita) nell’angolo inferiore destro della pagina sia selezionata.
1. Seleziona **[!UICONTROL Salva]** , seleziona una cartella per memorizzare il immagine insieme, immetti un nome per il gruppo, quindi seleziona **[!UICONTROL Salva]** .
1. Per visualizzare il Immagine impostati nel Visualizzatore di Immagine insieme, selezionare **[!UICONTROL Anteprima]** nella schermata immagine impostazione. Puoi selezionare campione miniature nel Visualizzatore di Immagine insieme per vedere come si comportano.

## Modificare un set di immagini {#editing-an-image-set}

Se modifichi un insieme pubblicato o non pubblicato, l&#39; **[!UICONTROL opzione Publish dopo il salvataggio]** influisce sui membri impostati e impostati nei seguenti modi:

| Il set è già pubblicato | **[!UICONTROL Publish dopo aver selezionato l&#39;opzione Salva]** prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di immagini:**

1. Nella Visualizza griglia, individuate un set di immagini e, quindi, sotto l&#39;immagine, selezionate **[!UICONTROL modifica]** .
1. Effettuate una delle seguenti operazioni:

   * Per aggiungere un’immagine (pubblicata o non pubblicata), trascinatela da una cartella di Aggiungi risorse nella pagina **[!UICONTROL Visualizzazioni]** del set di immagini.
   * Per rimuovere un&#39;immagine, selezionatela e fate clic **[!UICONTROL su Elimina]** sulla barra degli strumenti.
   * Per riordinare le immagini, trascinate un’immagine fino alla posizione desiderata.

1. Al termine dell’operazione di modifica del set, verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]** , seleziona una cartella di archiviazione per il tuo insieme, immetti un nome per il gruppo, quindi seleziona **[!UICONTROL Salva]** .

## Elimina un Immagine insieme {#deleting-an-image-set}

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di immagini:**

1. Nella Visualizza griglia, elenca Visualizza o dettagli Visualizza, seleziona un Immagine insieme o più.
1. Nella barra di navigazione globale, vai a **[!UICONTROL file]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]** .
