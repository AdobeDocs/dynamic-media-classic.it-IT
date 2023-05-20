---
title: Creare un set 360 gradi
description: Scopri come creare un set 360 gradi in Adobe Dynamic Media Classic.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 50%

---

# Creare un set 360 gradi{#creating-a-spin-set}

Per creare un set 360 gradi efficace, assicuratevi di scattare correttamente le immagini. Per creare un set 360 gradi in Adobe Dynamic Media Classic, seleziona il pulsante dei generatori e scegli Set 360 gradi. Nella schermata Set 360 gradi potete modificate i set 360 gradi.

>[!NOTE]
>
>Le versioni precedenti di Adobe Dynamic Media Classic non offrivano set 360 gradi bidimensionali. Se hai creato un set 360 gradi in una versione precedente di Adobe Dynamic Media Classic, non puoi salvare il set 360 gradi monodimensionale senza prima salvarlo con un nome diverso. Seleziona **[!UICONTROL Salva con nome]** nella schermata Set 360 gradi e immetti un nuovo nome che potrai modificare in Adobe Dynamic Media Classic.

## Linee guida per lo scatto di immagini per set 360 gradi {#guidelines-for-shooting-spin-set-images}

In generale, più immagini si hanno in un set 360 gradi, migliore è l&#39;effetto di rotazione dell&#39;immagine. Tuttavia, se si includono molte immagini nel set si aumenta anche il tempo necessario per il caricamento delle immagini. Adobe Dynamic Media Classic consiglia di seguire queste linee guida per la ripresa di immagini da utilizzare nei set 360 gradi:

* Utilizzare almeno 8-12 immagini in un set 360 gradi monodimensionale e 16-24 immagini in un set 360 gradi bidimensionale.
* Utilizzate un formato senza perdita di dati; si consigliano TIFF e PNG.
* Mascherate tutte le immagini in modo che gli elementi appaiano su uno sfondo bianco puro o su un altro sfondo a elevato contrasto. Se necessario, aggiungete ombre.
* Assicuratevi che i dettagli del prodotto siano ben illuminati e messi a fuoco.
* Per le immagini per un set 360 gradi di capi di abbigliamento, utilizzate un manichino o un indossatore. Spesso il manichino è mascherato (usando un manichino di vetro) o un manichino stilizzato/dressform è mostrato nell&#39;immagine. Potete creare un set 360 gradi su modello definendo il numero di angoli. Contrassegna ogni angolo con del nastro sul pavimento in modo da guidare il modello a passo e guardare nella direzione di ogni ripresa.

## Creare un set 360 gradi {#create}

L’ordine in cui il set 360 gradi viene creato o creato in Adobe Dynamic Media Classic è importante. A seconda di come ordinate le risorse quando rilasciate le immagini nella griglia della pagina Set 360 gradi, la rotazione avviene in una determinata direzione. Pertanto, l’ordine in cui viene visualizzata visivamente nel generatore di è il modo in cui la risorsa viene ruotata quando un utente sposta il puntatore del mouse o il dito, da sinistra a destra.

Quando create un set, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** incide su set e relativi membri nei seguenti modi:

| **[!UICONTROL Pubblica dopo il salvataggio]** opzione selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually-publishing-assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually-unpublishing-assets).

Quando crei un set 360 gradi, Adobe consiglia la procedura consigliata seguente e applica il seguente limite:

| Tipo limite set 360 gradi | Best practice | Limite imposto |
| --- | --- | --- |
| Numero massimo di righe/colonne per set 2D | 12-18 immagini per set | 1000 |

Vedi anche [Limitazioni di Dynamic Media](/help/limitations.md).

Dopo aver salvato un set 360 gradi, potete usare Anteprima nella pagina di generazione del set 360 gradi per vederne l’effetto nel visualizzatore predefinito.

**Per creare un set 360 gradi:**

1. Il giorno **[!UICONTROL Genera]** menu a discesa, seleziona **[!UICONTROL Set 360 gradi]**.
1. Nella finestra di dialogo Dimensione set 360 gradi, impostate il numero di righe e celle desiderato.

   Per un set monodimensionale, specificate una sola riga.

   Per un set bidimensionale, specificate due o più righe.

1. Seleziona **[!UICONTROL OK]**.
1. Trascinate quindi le immagini nella griglia della schermata Set 360 gradi.
1. Al termine dell’operazione, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**.
1. Nella finestra di dialogo Salva, selezionate una cartella in cui salvare il set 360 gradi. Nel campo Nome file, digitate il nome del set.
1. Seleziona **[!UICONTROL Salva]**.

## Modificare un set 360 gradi {#editing-a-spin-set}

Sia che si modifichi un set pubblicato o un set non pubblicato, il **[!UICONTROL Pubblica dopo il salvataggio]** influisce sui membri set e set nei modi seguenti:

| Il set è già pubblicato | **[!UICONTROL Pubblica dopo il salvataggio]** opzione selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually-publishing-assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually-unpublishing-assets).

**Per modificare un set 360 gradi:**

1. Seleziona il rollover del set 360 gradi **[!UICONTROL Modifica]** pulsante.
1. Effettuate una delle seguenti operazioni:

   * **Rimozione di immagini** - Selezionare l&#39;immagine, quindi selezionare **[!UICONTROL Elimina]**.

   * **Aggiunta di immagini** : trascina l’immagine in una cella.

   * **Riordinamento delle righe (set 360 gradi bidimensionali)** - Selezionare una casella di selezione delle righe (a sinistra della riga), quindi selezionare **[!UICONTROL Sposta riga in basso]** o **[!UICONTROL Sposta riga in alto]**.

   * **Aggiunta di righe e celle** - Immettere un numero nelle caselle Righe e Celle per determinare il numero di righe e il numero di celle in ogni riga.

1. Al termine dell’operazione di modifica, verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, selezionare una cartella di archiviazione, immettere un nome per il set e quindi selezionare **[!UICONTROL Salva]**.

## Eliminare un set 360 gradi {#deleting-a-spin-set}

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually-publishing-assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually-unpublishing-assets).

**Per eliminare un set 360 gradi:**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più set 360 gradi.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.
