---
title: Creare un set di file multimediali diversi
description: Scopri come creare un set di file multimediali diversi in Adobe Dynamic Media Classic.
uuid: a0c6e5fa-7a85-4376-b9a3-b72ae63d3d95
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0ff9e763-897c-4ba5-b606-a95d5e45f35e
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 77%

---

# Creare un set di file multimediali diversi{#creating-a-mixed-media-set}

Potete creare un set di file multimediali diversi per combinare più tipi di visualizzatori in un’unica presentazione. Assicuratevi che i file, i set di immagini, i set di campioni e i set 360 gradi siano pronti per la pubblicazione prima di aggiungerli al set di file multimediali diversi.

![Set di file multimediali diversi](/help/assets/mm_mixed_media_set.png)

## Creare un set di file multimediali diversi {#create-a-mixed-media-set}

Quando create un set, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di file multimediali diversi:**

1. Vai a **[!UICONTROL Crea]** > **[!UICONTROL Set di file multimediali diversi]**.
1. Trascinate i video, i set di immagini, i set 360 gradi e i campioni dalla libreria delle risorse alla schermata Set di file multimediali diversi.

   >[!NOTE]
   >
   >Un set di file multimediali diversi non supporta le risorse con nomi di file contenenti uno dei seguenti caratteri: `( ) { }`.

1. Effettuate una delle seguenti operazioni:

   * Per aggiungere una colonna sonora, trascinate un file audio dalla libreria delle risorse alla casella Colonna sonora. La colonna sonora viene riprodotta durante la visualizzazione delle immagini, mentre viene interrotta durante una riproduzione video. 
   * Per cambiare l’ordine dei set, trascinateli nelle nuove posizioni nella schermata Set di file multimediali diversi. L’ordine dei set nella schermata determina l’ordine da sinistra a destra in cui gli utenti vedono i set nel visualizzatore di set di file multimediali diversi.
   * (Facoltativo) Per aggiungere una miniatura personalizzata che rappresenti il video nel visualizzatore, trascinate un file immagine dalla Libreria risorse alla casella segnaposto Miniatura.

1. Verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** (impostazione predefinita) nell’angolo inferiore destro della pagina sia selezionata.
1. Seleziona **[!UICONTROL Salva]**.
1. Seleziona una cartella in cui memorizzare il set di file multimediali diversi, quindi immetti un nome per il set.
1. Seleziona **[!UICONTROL Salva]**.

   Per visualizzare l’aspetto del set di immagini combinato in un visualizzatore di set di immagini, seleziona **[!UICONTROL Anteprima]**.

## Modificare un set di file multimediali diversi {#edit-a-mixed-media-set}

Potete modificare un set di file multimediali diversi. Per modificare un set contenuto in un set di file multimediali diversi, aprite il set desiderato separatamente, modificatelo e salvatelo. Le modifiche saranno riportate anche nel set di file multimediali diversi.

Se modifichi un set pubblicato o non pubblicato, la **[!UICONTROL Pubblica dopo il salvataggio]** influenza i membri set e set nei seguenti modi:

| Il set è già pubblicato | **[!UICONTROL Pubblica dopo il salvataggio]** opzione selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di file multimediali diversi:**

1. Selezionare il rollover del set di file multimediali diversi **[!UICONTROL Modifica]** pulsante .
1. Effettuate una delle seguenti operazioni:

   * Per rimuovere gli elementi, selezionali e seleziona **[!UICONTROL Elimina]**.
   * Per riordinare gli elementi, trascinateli nelle nuove posizioni.

1. Al termine dell’operazione di modifica del set, verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]** o **[!UICONTROL Salva con nome]**.

## Eliminare un set di file multimediali diversi {#deleting-a-mixed-media-set}

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di file multimediali diversi:**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più set di file multimediali diversi.
1. Nella barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.
