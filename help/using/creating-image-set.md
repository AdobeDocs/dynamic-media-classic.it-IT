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
source-git-commit: edd893482cbafd9674a44cf9878b8ee3079d98f7
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 46%

---

# Creare un set di immagini{#creating-an-image-set}

Per creare un set di immagini a visualizzazione multipla, sono necessarie immagini di uno stesso elemento da più punti di vista o che mostrino diversi aspetti dello stesso elemento. L’obiettivo è quello di presentare agli utenti diverse immagini di un elemento, in modo che possano farsi un’idea concreta dell’aspetto o della funzione di quest’ultimo.

## Creare un set di immagini {#create}

Quando create un set, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** incide su set e relativi membri nei seguenti modi:

| **[!UICONTROL `Publish after save`]** opzione selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
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

   * **Seleziona prima le immagini** - Nel pannello Sfoglia, selezionare le immagini desiderate per il set di immagini, andare a **[!UICONTROL Genera]** > **[!UICONTROL Set di immagini]**.

   * **Inizia dalla schermata Set di immagini** - Vai a **[!UICONTROL Genera]** > **[!UICONTROL Set di immagini]**. Viene visualizzata la schermata Set immagini. Selezionate una cartella nella Libreria risorse e trascinate le immagini per il set di immagini nella schermata Set immagini.

1. Per modificare l’ordine delle immagini, trascinate queste ultime in nuove posizioni.
1. Verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** (impostazione predefinita) nell’angolo inferiore destro della pagina sia selezionata.
1. Seleziona **[!UICONTROL Salva]**, selezionare una cartella per la memorizzazione del set di immagini, immettere un nome per il set e quindi selezionare **[!UICONTROL Salva]**.
1. Per visualizzare il set di immagini nel Visualizzatore set di immagini, seleziona **[!UICONTROL Anteprima]** nella schermata Image Set. Per vedere come si comportano, potete selezionare le miniature dei campioni nel Visualizzatore set di immagini.

## Modificare un set di immagini {#editing-an-image-set}

Sia che si modifichi un set pubblicato o non pubblicato, il **[!UICONTROL Pubblica dopo il salvataggio]** influisce sui membri set e set nei modi seguenti:

| Il set è già pubblicato | **[!UICONTROL `Publish after save`]** opzione selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono lo stato pubblicato. I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di immagini:**

1. Nella visualizzazione griglia, passare a un set di immagini, quindi selezionare sotto l&#39;immagine **[!UICONTROL Modifica]**.
1. Effettuate una delle seguenti operazioni:

   * Per aggiungere un’immagine (pubblicata o non pubblicata), trascinala da una cartella in Aggiungi risorse al set di immagini **[!UICONTROL Visualizzazioni]** pagina.
   * Per rimuovere un&#39;immagine, selezionarla e quindi selezionare **[!UICONTROL Elimina]** sulla barra degli strumenti.
   * Per riordinare le immagini, trascinate un’immagine fino alla posizione desiderata.

1. Al termine dell’operazione di modifica del set, verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, selezionare una cartella di archiviazione per il set, immettere un nome per il set e quindi selezionare **[!UICONTROL Salva]**.

## Eliminare un set di immagini

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (o &quot;figli&quot;) all&#39;interno di quel set non sono interessati; invece, ciascuno di essi mantiene il proprio stato pubblicato o non pubblicato esistente.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di immagini:**

1. In Vista griglia, Vista elenco o Vista dettagli, selezionare uno o più set di immagini.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.
