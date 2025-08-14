---
title: Creare un set 360 gradi
description: Scopri come creare un set 360 gradi in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 32%

---

# Creare un set 360 gradi{#creating-a-spin-set}

Per creare un set 360 gradi efficace, assicuratevi di scattare correttamente le immagini. Per creare un set 360 gradi in Adobe Dynamic Media Classic, seleziona il pulsante dei generatori e scegli Set 360 gradi. Nella schermata Set 360 gradi potete modificate i set 360 gradi.

>[!NOTE]
>
>Le versioni precedenti di Adobe Dynamic Media Classic non offrivano set 360 gradi bidimensionali. Se hai creato un set 360 gradi in una versione precedente di Adobe Dynamic Media Classic, salvalo con un nome diverso, potrai salvare il set 360 gradi monodimensionale. Selezionare **[!UICONTROL Salva con nome]** nella schermata Set 360 gradi e immettere un nuovo nome che consenta di modificarlo in Adobe Dynamic Media Classic.

## Linee guida per lo scatto di immagini per set 360 gradi {#guidelines-for-shooting-spin-set-images}

In generale, più immagini si hanno in un set 360 gradi, migliore è l&#39;effetto di rotazione dell&#39;immagine. Tuttavia, se si includono molte immagini nel set si aumenta anche il tempo necessario per il caricamento delle immagini. Adobe Dynamic Media Classic consiglia di seguire queste linee guida per la ripresa di immagini da utilizzare nei set 360 gradi:

* Utilizzare almeno 8-12 immagini in un set 360 gradi monodimensionale e 16-24 immagini in un set 360 gradi bidimensionale.
* Utilizzate un formato senza perdita di dati; si consigliano TIFF e PNG.
* Mascherate tutte le immagini in modo che gli elementi appaiano su uno sfondo bianco puro o su un altro sfondo a elevato contrasto. Se necessario, aggiungete ombre.
* Assicuratevi che i dettagli del prodotto siano ben illuminati e messi a fuoco.
* Per le immagini per un set 360 gradi di capi di abbigliamento, utilizzate un manichino o un indossatore. Spesso il manichino è mascherato (usando un manichino di vetro) o un manichino stilizzato/dressform è mostrato nell&#39;immagine. Potete creare un set 360 gradi sul modello definendo il numero di angoli. Contrassegna ogni angolo con del nastro sul pavimento in modo da guidare il modello a passo e guardare nella direzione di ogni ripresa.

## Creare un set 360 gradi {#create}

L’ordine in cui il set 360 gradi viene creato o creato in Adobe Dynamic Media Classic è importante. A seconda di come ordini le risorse quando trascini e rilasci le immagini nella griglia della pagina Set 360 gradi, il set 360 gradi viene ruotato in una determinata direzione. Pertanto, l’ordine in cui viene visualizzata visivamente nel generatore di è il modo in cui la risorsa viene ruotata quando un utente sposta il puntatore del mouse o il dito, da sinistra a destra.

Quando si crea un set, l&#39;opzione **[!UICONTROL Pubblica dopo un salvataggio]** ha effetto sui membri del set e del set nei modi seguenti:

| **[!UICONTROL Pubblicare dopo aver selezionato un&#39;opzione di salvataggio]** prima di salvare? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually-publishing-assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually-unpublishing-assets).

Quando crei un set 360 gradi, Adobe consiglia la procedura consigliata seguente e applica il seguente limite:

| Tipo limite set 360 gradi | Best practice | Limite imposto |
| --- | --- | --- |
| Numero massimo di righe/colonne per set 2D | 12-18 immagini per set | 1000 |

Vedi anche [Limitazioni di Dynamic Media](/help/using/limitations.md).

Dopo aver salvato un set 360 gradi, potete usare Anteprima nella pagina di generazione del set 360 gradi per vederne l’effetto nel visualizzatore predefinito.

**Per creare un set 360 gradi:**

1. Nel menu a discesa **[!UICONTROL Build]**, seleziona **[!UICONTROL Set 360 gradi]**.
1. Nella finestra di dialogo Dimensione set 360 gradi, impostate il numero di righe e celle desiderato.

   Per creare un set 360 gradi monodimensionale, selezionate una sola riga.

   Per un set bidimensionale, specificate due o più righe.

1. Selezionare **[!UICONTROL OK]**.
1. Trascinate quindi le immagini nella griglia della schermata Set 360 gradi.
1. Al termine, vicino all&#39;angolo inferiore destro della pagina, assicurati che sia selezionato **Pubblica dopo un salvataggio** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**.
1. Nella finestra di dialogo Salva, seleziona una cartella per la memorizzazione del set 360 gradi. Nel campo Nome file immettere il nome del set 360 gradi.
1. Seleziona **[!UICONTROL Salva]**.

## Modificare un set 360 gradi {#editing-a-spin-set}

Sia che si modifichi un set pubblicato o non pubblicato, l&#39;opzione **[!UICONTROL Pubblica dopo un salvataggio]** ha effetto sui membri del set e del set nei modi seguenti:

| Il set è già pubblicato | **[!UICONTROL Pubblicare dopo aver selezionato l&#39;opzione di salvataggio]** prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono lo stato pubblicato. I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually-publishing-assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually-unpublishing-assets).

**Per modificare un set 360 gradi:**

1. Seleziona il pulsante di rollover **[!UICONTROL Modifica]** del set 360 gradi.
1. Effettuate una delle seguenti operazioni:

   * **Rimozione immagini**: selezionare l&#39;immagine, quindi selezionare **[!UICONTROL Elimina]**.

   * **Aggiunta di immagini**: trascinare l&#39;immagine in una cella.

   * **Riordinamento delle righe (set 360 gradi bidimensionali)**: selezionare una casella di selezione delle righe (a sinistra della riga), quindi selezionare **[!UICONTROL Sposta riga giù]** o **[!UICONTROL Sposta riga su]**.

   * **Aggiunta di righe e celle**: immettere un numero nelle caselle Righe e Celle per determinare il numero di righe e il numero di celle in ogni riga.

1. Al termine della modifica, vicino all&#39;angolo inferiore destro della pagina, assicurati che sia selezionato **[!UICONTROL Pubblica dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, seleziona una cartella di archiviazione, immetti un nome per il set, quindi seleziona **[!UICONTROL Salva]**.

## Eliminare un set 360 gradi

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (o &quot;figli&quot;) all&#39;interno di quel set non sono interessati; invece, ciascuno di essi mantiene il proprio stato pubblicato o non pubblicato esistente.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually-publishing-assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually-unpublishing-assets).

**Per eliminare un set 360 gradi:**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più set 360 gradi.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.
