---
title: Creazione di un set di file multimediali diversi
description: Scopri come creare un set di file multimediali diversi.
uuid: a0c6e5fa-7a85-4376-b9a3-b72ae63d3d95
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0ff9e763-897c-4ba5-b606-a95d5e45f35e
feature: Dynamic Media Classic,Visualizzatori,Set Di File Multimediali Diversi
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
source-git-commit: f99832bc9660a16b06e63b19f9ead1267dab0f35
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 88%

---

# Creazione di un set di file multimediali diversi{#creating-a-mixed-media-set}

Potete creare un set di file multimediali diversi per combinare più tipi di visualizzatori in un’unica presentazione. Assicuratevi che i file, i set di immagini, i set di campioni e i set 360 gradi siano pronti per la pubblicazione prima di aggiungerli al set di file multimediali diversi.

![Set di file multimediali diversi](/help/assets/mm_mixed_media_set.png)

## Creare un set di file multimediali diversi {#create-a-mixed-media-set}

Quando create un set, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di file multimediali diversi:**

1. Fate clic su **[!UICONTROL Genera]** > **[!UICONTROL Set di file multimediali diversi]**.
1. Trascinate i video, i set di immagini, i set 360 gradi e i campioni dalla libreria delle risorse alla schermata Set di file multimediali diversi.

   >[!NOTE]
   >
   >Un set di file multimediali diversi non supporta le risorse con nomi di file contenenti uno dei seguenti caratteri: `( ) { }`.

1. Effettuate una delle seguenti operazioni:

   * Per aggiungere una colonna sonora, trascinate un file audio dalla libreria delle risorse alla casella Colonna sonora. La colonna sonora viene riprodotta durante la visualizzazione delle immagini, mentre viene interrotta durante una riproduzione video. 
   * Per cambiare l’ordine dei set, trascinateli nelle nuove posizioni nella schermata Set di file multimediali diversi. L’ordine dei set nella schermata determina l’ordine da sinistra a destra in cui gli utenti vedono i set nel visualizzatore di set di file multimediali diversi.
   * (Facoltativo) Per aggiungere una miniatura personalizzata che rappresenti il video nel visualizzatore, trascinate un file immagine dalla Libreria risorse alla casella segnaposto Miniatura.

1. Verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** (impostazione predefinita) nell’angolo inferiore destro della pagina sia selezionata.
1. Fate clic su **[!UICONTROL Salva]**, selezionate una cartella in cui memorizzare il set di file multimediali diversi, immettete un nome per il set, quindi fate clic su **[!UICONTROL Salva]**.

   Per visualizzare l&#39;aspetto del set di immagini combinato in un visualizzatore di set di immagini, fare clic su **[!UICONTROL Anteprima]**.

## Modificare un set di file multimediali diversi {#edit-a-mixed-media-set}

Potete modificare un set di file multimediali diversi. Per modificare un set contenuto in un set di file multimediali diversi, aprite il set desiderato separatamente, modificatelo e salvatelo. Le modifiche saranno riportate anche nel set di file multimediali diversi.

Sia che modifichi un set pubblicato che non pubblicato, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** influisce sul set e sui membri impostati nei seguenti modi:

| Il set è già pubblicato | Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio delle modifiche | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di file multimediali diversi:**

1. Fate clic sul pulsante rollover **[!UICONTROL Modifica]** del set di file multimediali diversi. 
1. Effettuate una delle seguenti operazioni:

   * Per rimuovere degli elementi, selezionateli e fate clic su **[!UICONTROL Elimina]**.
   * Per riordinare gli elementi, trascinateli nelle nuove posizioni.

1. Al termine dell’operazione di modifica del set, verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **[!UICONTROL Salva]** o **[!UICONTROL Salva con nome]**.

## Eliminare un set di file multimediali diversi {#deleting-a-mixed-media-set}

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di file multimediali diversi:**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più set di file multimediali diversi.
1. Nella barra di navigazione globale, fate clic su **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.
