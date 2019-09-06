---
title: Creazione di un set 360 gradi
seo-title: Creazione di un set 360 gradi
description: 'null'
seo-description: Scoprite come creare un set gradi.
uuid: 697 bd 78 f -5 e 39-46 bf-aa 6 d-ad 8 ab 99 fe 40 e
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/spin_ sets
discoiquuid: 735 b 5867-e 249-4627-a 5 a 5-25 c 19 c 2255 bf
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Creazione di un set 360 gradi{#creating-a-spin-set}

Per creare un set 360 gradi efficace, assicuratevi di scattare correttamente le immagini. Per creare un set gradi in Media Classic, fate clic sul pulsante Genera e scegliete Set gradi. Nella schermata Set 360 gradi potete modificate i set 360 gradi.

>[!NOTE]
>
>Le versioni precedenti di Dynamic Media Classic non offrono set gradi bidimensionali. Se avete creato un set gradi in una versione precedente di Dynamic Media Classic, non potete salvare il set gradi monodimensionale senza salvarlo con un altro nome. Fate clic su Salva con nome nella schermata Set gradi e immettete un nuovo nome per modificarlo in Dynamic Media Classic.

## Linee guida per lo scatto di immagini per set 360 gradi {#guidelines-for-shooting-spin-set-images}

In generale, più sono le immagini contenute in un set 360 gradi, migliore è l’effetto di rotazione dell’immagine. Tuttavia, se si includono molte immagini nel set si aumenta anche il tempo necessario per il caricamento delle immagini. Dynamic Media Classic consiglia le seguenti linee guida per la ripresa di immagini da utilizzare nei set gradi:

* Usate almeno 8-12 immagini in un set gradi monodimensionale e 16-24 in un set gradi bidimensionale.
* Utilizzate un formato senza perdita di dati; si consigliano TIFF e PNG.
* Mascherate tutte le immagini in modo che gli elementi appaiano su uno sfondo bianco puro o su un altro sfondo a elevato contrasto. Se necessario, aggiungete ombre.
* Assicuratevi che i dettagli del prodotto siano ben illuminati e messi a fuoco.
* Per le immagini per un set 360 gradi di capi di abbigliamento, utilizzate un manichino o un indossatore. Il manichino può essere mascherato completamente (utilizzando un manichino in vetro) oppure nell’immagine può essere visibile un manichino o busto da sarta stilizzato. Potete creare un set 360 gradi con un indossatore definendo il numero di angolazioni. Contrassegnate ciascun angolo con nastro sul pavimento per indicare all’indossatore dove spostarsi e come guardare nella direzione di ciascuno scatto. 

## Creazione di un set 360 gradi {#create}

L’ordine con cui è stato generato o creato il set 360 gradi in Scene7 Publishing System è importante. A seconda di come ordinate le risorse quando rilasciate le immagini nella griglia della pagina Set 360 gradi, la rotazione avviene in una determinata direzione. Di conseguenza, l’ordine di visualizzazione nel modulo di generazione corrisponde alla direzione di rotazione delle risorse quando un utente sposta il mouse o il dito, da sinistra a destra.

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

## Modifica di un set 360 gradi {#editing-a-spin-set}

A seconda se modificate un set pubblicato o non pubblicato, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Il set è già pubblicato | Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio delle modifiche | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono il loro stato pubblicato. Tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione o pubblicazione non pubblicato. |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually-publishing-assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually-unpublishing-assets).

**Per modificare un set 360 gradi**

1. Fate clic sul pulsante rollover **Modifica** del set di campioni. 
1. Effettuate una delle seguenti operazioni:

   **Rimozione di immagini**

   Selezionate l’immagine, quindi fate clic su **Elimina**.

   **Aggiunta di immagini**

   Trascinate l’immagine in una cella.

   **Riordinamento delle righe (set 360 gradi bidimensionali)**

   Fate clic su una casella (a sinistra della riga) per selezionare la riga corrispondente, quindi fate clic sul pulsante **Sposta riga in basso** o **Sposta riga in alto**.

   **Aggiunta di righe e celle**

   Inserite un numero nella casella Righe o Celle per determinare il numero di righe o di celle per ogni riga.

1. Al termine dell’operazione di modifica, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **Salva**, selezionate una cartella di archiviazione, immettete un nome per il set e fate clic su **Salva**.

## Eliminazione di un set 360 gradi {#deleting-a-spin-set}

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually-publishing-assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually-unpublishing-assets).

**Per eliminare un set 360 gradi**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più set 360 gradi.
1. Nella barra di navigazione globale, fate clic su **File** &gt; **Elimina** &gt; **Elimina**.

