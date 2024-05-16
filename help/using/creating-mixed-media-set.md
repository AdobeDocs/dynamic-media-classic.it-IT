---
title: Creare un set di file multimediali diversi
description: Scopri come creare un set di file multimediali diversi in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 56%

---

# Creare un set di file multimediali diversi{#creating-a-mixed-media-set}

Potete creare un set di file multimediali diversi per combinare più tipi di visualizzatori in un’unica presentazione. Assicuratevi che i file, i set di immagini, i set di campioni e i set 360 gradi siano pronti per la pubblicazione prima di aggiungerli al set di file multimediali diversi.

![Set di file multimediali diversi](/help/using/assets/mm_mixed_media_set.png)

## Creare un set di file multimediali diversi {#create-a-mixed-media-set}

Quando si crea un set, **Pubblica dopo un salvataggio** influisce sui membri set e set nei modi seguenti:

| Opzione &quot;Pubblica dopo un salvataggio&quot; selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di file multimediali diversi:**

1. Vai a **[!UICONTROL Genera]** > **[!UICONTROL Set di file multimediali diversi]**.
1. Trascinate i video, i set di immagini, i set 360 gradi e i campioni dalla libreria delle risorse alla schermata Set di file multimediali diversi.

   >[!NOTE]
   >
   >Un set di file multimediali diversi non supporta le risorse con nomi di file che contengono i seguenti caratteri: `( ) { }`.

1. Effettuate una delle seguenti operazioni:

   * Per aggiungere una colonna sonora, trascinate un file audio dalla libreria delle risorse alla casella Colonna sonora. La colonna sonora viene riprodotta durante la visualizzazione delle immagini, Si interrompe durante la riproduzione di un video.
   * Per cambiare l’ordine dei set, trascinateli nelle nuove posizioni nella schermata Set di file multimediali diversi. L’ordine dei set nella schermata determina l’ordine da sinistra a destra in cui gli utenti vedono i set nel visualizzatore di set di file multimediali diversi.
   * (Facoltativo) Per aggiungere una miniatura personalizzata che rappresenti il video nel visualizzatore, trascinate un file immagine dalla Libreria risorse alla casella segnaposto Miniatura.

1. Nell’angolo inferiore destro della pagina, assicurati che **[!UICONTROL Pubblica dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**.
1. Seleziona una cartella per l’archiviazione del set di file multimediali diversi, quindi immetti un nome per il set.
1. Seleziona **[!UICONTROL Salva]**.

   Per visualizzare l&#39;aspetto del set di immagini combinato in un visualizzatore di set di immagini, selezionare **[!UICONTROL Anteprima]**.

## Modificare un set di file multimediali diversi {#edit-a-mixed-media-set}

Potete modificare un set di file multimediali diversi. Per modificare un set contenuto in un set di file multimediali diversi, aprite il set desiderato separatamente, modificatelo e salvatelo. Le modifiche vengono visualizzate nel set di file multimediali diversi.

Sia che si modifichi un set pubblicato o non pubblicato, il **[!UICONTROL Pubblica dopo un salvataggio]** influisce sui membri set e set nei modi seguenti:

| Il set è già pubblicato | **[!UICONTROL Pubblica dopo un salvataggio]** opzione selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono lo stato pubblicato. I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di file multimediali diversi:**

1. Seleziona il rollover del set di file multimediali diversi **[!UICONTROL Modifica]** pulsante.
1. Effettuate una delle seguenti operazioni:

   * Per rimuovere gli elementi, selezionali e seleziona **[!UICONTROL Elimina]**.
   * Per riordinare gli elementi, trascinateli nelle nuove posizioni.

1. Al termine della modifica del set, vicino all’angolo inferiore destro della pagina, assicurati che **[!UICONTROL Pubblica dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]** o **[!UICONTROL Salva con nome]**.

## Eliminare un set di file multimediali diversi

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (o &quot;figli&quot;) all&#39;interno di quel set non sono interessati; invece, ciascuno di essi mantiene il proprio stato pubblicato o non pubblicato esistente.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di file multimediali diversi:**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più set di file multimediali diversi.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.
