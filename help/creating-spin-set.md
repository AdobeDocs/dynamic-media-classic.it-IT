---
title: Creazione di un set 360 gradi
description: Scoprite come creare un set 360 gradi.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 74%

---


# Creazione di un set 360 gradi{#creating-a-spin-set}

Per creare un set 360 gradi efficace, assicuratevi di scattare correttamente le immagini. Per creare un set 360 gradi in Dynamic Media Classic, fate clic sul pulsante Genera e scegliete Set 360 gradi. Nella schermata Set 360 gradi potete modificate i set 360 gradi.

>[!NOTE]
>
>Le versioni precedenti di Dynamic Media Classic non offrirono set 360 gradi bidimensionali. Se avete creato un set 360 gradi in una versione precedente di Dynamic Media Classic, non potete salvare il set 360 gradi monodimensionale senza prima salvarlo con un nome diverso. Fate clic su Salva con nome nella schermata Set 360 gradi e immettete un nuovo nome per modificarlo in Dynamic Media Classic.

## Linee guida per lo scatto di immagini per set 360 gradi {#guidelines-for-shooting-spin-set-images}

In generale, più sono le immagini contenute in un set 360 gradi, migliore è l’effetto di rotazione dell’immagine. Tuttavia, se si includono molte immagini nel set si aumenta anche il tempo necessario per il caricamento delle immagini. Dynamic Media Classic consiglia le seguenti linee guida per lo scatto di immagini da usare nei set 360 gradi:

* Utilizzate almeno 8-12 immagini in un set 360 gradi monodimensionale e 16-24 immagini in un set 360 gradi bidimensionale.
* Utilizzate un formato senza perdita di dati; si consigliano TIFF e PNG.
* Mascherate tutte le immagini in modo che gli elementi appaiano su uno sfondo bianco puro o su un altro sfondo a elevato contrasto. Se necessario, aggiungete ombre.
* Assicuratevi che i dettagli del prodotto siano ben illuminati e messi a fuoco.
* Per le immagini per un set 360 gradi di capi di abbigliamento, utilizzate un manichino o un indossatore. Il manichino può essere mascherato completamente (utilizzando un manichino in vetro) oppure nell’immagine può essere visibile un manichino o busto da sarta stilizzato. Potete creare un set 360 gradi con un indossatore definendo il numero di angolazioni. Contrassegnate ciascun angolo con nastro sul pavimento per indicare all’indossatore dove spostarsi e come guardare nella direzione di ciascuno scatto. 

## Creazione di un set 360 gradi  {#create}

L’ordine in cui il set 360 gradi viene creato o creato in Dynamic Media Classic è importante. A seconda di come ordinate le risorse quando rilasciate le immagini nella griglia della pagina Set 360 gradi, la rotazione avviene in una determinata direzione. Di conseguenza, l’ordine di visualizzazione nel modulo di generazione corrisponde alla direzione di rotazione delle risorse quando un utente sposta il mouse o il dito, da sinistra a destra.

Quando create un set, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually-publishing-assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually-unpublishing-assets).

Dopo aver salvato un set 360 gradi, potete usare Anteprima nella pagina di generazione del set 360 gradi per vederne l’effetto nel visualizzatore predefinito.

**Per creare un set 360 gradi**

1. Scegliete **Set 360 gradi** dal menu a discesa **Genera**.
1. Nella finestra di dialogo Dimensione set 360 gradi, impostate il numero di righe e celle desiderato.

   Per un set monodimensionale, specificate una sola riga.

   Per un set bidimensionale, specificate due o più righe.

1. Fate clic su **OK**.
1. Trascinate quindi le immagini nella griglia della schermata Set 360 gradi.
1. Al termine dell’operazione, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **Salva**.
1. Nella finestra di dialogo Salva, selezionate una cartella in cui salvare il set 360 gradi. Nel campo Nome file, digitate il nome del set.
1. Fate clic su **Salva**.

## Modifica di un set 360 gradi  {#editing-a-spin-set}

A seconda se modificate un set pubblicato o non pubblicato, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Il set è già pubblicato | Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio delle modifiche | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il proprio stato di pubblicazione. Tutti i nuovi membri del set aggiunti durante la modifica conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually-publishing-assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually-unpublishing-assets).

**Per modificare un set 360 gradi**

1. Fate clic sul pulsante rollover **Modifica** del set di campioni. 
1. Effettuate una delle seguenti operazioni:

   * **Rimozione di**
immagini: selezionate l’immagine e fate clic su 
**Elimina**.

   * **Aggiunta di**
immagini: trascinate l’immagine in una cella.

   * **Riordinamento delle righe (set 360 gradi bidimensionali)**
Fare clic su una casella di selezione delle righe (a sinistra della riga), quindi fare clic su 
**Sposta riga** verso il basso e  **sposta riga verso l&#39;alto**.

   * **Aggiunta di righe e**
celleImmettere un numero nella casella Righe e Celle per determinare il numero di righe e il numero di celle in ciascuna riga.

1. Al termine dell’operazione di modifica, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **Salva**, selezionate una cartella di archiviazione, immettete un nome per il set e fate clic su **Salva**.

## Eliminazione di un set 360 gradi  {#deleting-a-spin-set}

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually-publishing-assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually-unpublishing-assets).

**Per eliminare un set 360 gradi**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più set 360 gradi.
1. Nella barra di navigazione globale, fate clic su **File** > **Elimina** > **Elimina**.

