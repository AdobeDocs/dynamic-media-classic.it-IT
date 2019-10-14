---
title: Creazione di un set di offerte
seo-title: Creazione di un set di offerte
description: 'null'
seo-description: Scoprite come creare un set di offerte.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/Categories/target_classic_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Creazione di un set di offerte{#creating-an-offer-set}

Potete creare i seguenti tipi di set di offerte:

* Video
* Modello con parametri
* Immagine

For templates, click **Add and Preview**, then set the parameters you choose. Gli altri tipi di set di offerte non dispongono di parametri, ma li potete personalizzare facendo clic su **Anteprima** e cambiando i predefiniti disponibili.

Dynamic Media Classic offre strumenti per la modifica e la creazione di set di offerte.

>[!NOTE]
>
>Prima di creare un set di offerte, accertatevi di pubblicare tutte le risorse che intendete utilizzare per il set in Scene7 Publishing System. Consultate [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

## Tipi di set di offerte {#types-of-offer-sets}

Potete creare un set di offerte dai seguenti tipi di set di offerte:

* **Immagini** Potete assemblare le immagini per un set di offerte. Ogni immagine include un’offerta diversa nel set.

* **Modello** immagine È possibile parametrizzare i modelli per immagini in Dynamic Media Classic con il comando Genera &gt; Funzioni di base dei modelli. Attraverso i parametri, potete scambiare e personalizzare i componenti del modello, come il testo all’interno di cornici di testo e le varie immagini. Per un set di offerte potete utilizzare i parametri dei modelli per creare, ad esempio, varianti di una stessa immagine nel set di offerte. Per informazioni sulla creazione e la definizione di parametri per i modelli per immagini, consultate Creazione di parametri per i modelli.

* **Video** Potete assemblare i video per un set di offerte. Ciascun video rappresenta una diversa offerta nel set.

## Creazione di un set di offerte con un modello con parametri {#creating-an-offer-set-with-a-parameterized-template}

Quando create un eCatalog, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di offerte con un modello con parametri**

1. Selezionate il modello o il banner.
1. Click **Build** &gt; **Target Classic Offer Set**.

   La pagina Set di offerte di Target Classic elenca le offerte nel set di offerte. Il primo elemento nell’elenco rappresenta l’oggetto.

1. Selezionate l’oggetto e fate clic sul pulsante **Aggiungi e visual. antepr.**.

   Il lato sinistro di questa pagina riporta i parametri presenti nel modello con i rispettivi valori.

1. Per creare l’offerta, modificate i valori dei parametri. Inserite, ad esempio, un testo diverso in un campo di testo, modificate la dimensione di un livello, inserite un’immagine al posto di un’altra oppure scegliete un predefinito per visualizzatori.
1. Per salvare l’offerta come parte del set di offerte, fate clic su **Salva** o **Salva con nome**. 

   Nella pagina Set di offerte di Target Classic sono elencate le offerte create.

1. Ripetete i punti da 3 a 5 per creare più offerte per il set.
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

Prima di chiudere la pagina Set di offerte di Target Classic, inviate il set di offerte a Target Classic. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Creating an offer set with images or videos {#creating-an-offer-set-with-images-or-videos}

Quando create un eCatalog, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di offerte con immagini o video**

1. Assemblate immagini o video per il set di offerte. Iniziate nella schermata Set di offerte di Target Classic oppure nella vista Griglia o Elenco e usate uno dei seguenti metodi:

   * **Schermata** Set di offerte per Target Classic Fate clic su Genera &gt; Set di offerte per Target Classic. Trascinate le immagini o i video sulla schermata. Per creare video o immagini di diverse misure, trascinate più copie delle immagini o dei video e impostatene le dimensioni singolarmente.

   * **Visualizzazione** Griglia o Elenco Selezionate le immagini o i video, quindi fate clic su Genera &gt; Set di offerte per Target Classic.

1. Facoltativamente, potete selezionare un’immagine o un video e fare clic su **Anteprima**. Nella pagina Anteprima offerte potete modificare le dimensioni e l’aspetto dell’immagine o del video selezionato. Oppure potete modificare tutte le immagini o i video del set di offerte.

   * Scegliete un predefinito per cambiare l’aspetto e le dimensioni dell’immagine o del video.
   * Fate clic sulla casella Applica predefinito selezionato a tutti per applicare il predefinito scelto a tutte le offerte del set di offerte.
   Fate clic su **Salva** per salvare le modifiche apportate all’offerta di immagini o video. Then click **Close** to return to the Target Classic Offer Set page.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. Fate clic su **Salva**, immettete un nome per il set di offerte e fate clic su **Salva**.

Prima di chiudere la pagina Set di offerte di Target Classic, inviate il set di offerte a Target Classic. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Modifica di un set di offerte {#editing-an-offer-set}

A seconda se modificate un set pubblicato o non pubblicato, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Il set è già pubblicato | Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio delle modifiche | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il proprio stato di pubblicazione. Tutti i nuovi membri del set aggiunti durante la modifica conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di offerte**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. Nella pagina Set di offerte di Target Classic, effettuate una delle seguenti operazioni:

   * **Rimozione di un'offerta** Selezionate l'offerta, quindi fate clic su **Elimina** per rimuovere un'offerta dal set.
   * **L’aggiunta di un’offerta** La modalità di aggiunta di un’offerta dipende dal tipo di set di offerte con cui state lavorando:
   * **Modelli** Fate clic su **Aggiungi e visualizza anteprima**, quindi create un’altra offerta nella pagina Aggiungi offerte e visualizza anteprima.
   * **Immagini e video** Trascinate un’immagine o un video nella pagina Set di offerte per Target Classic.
   >[!NOTE]
   >
   >non potete eliminare un set di offerte associato a una campagna. Per eliminare un set di offerte associato a una campagna, accedete a Target Classic e rimuovete prima le associazioni della campagna. Anche dopo aver interrotto l’associazione da una campagna, la risorsa può essere eliminata solo da Scene7 Publishing System, richiedendo l’accesso a Target Classic e non da Target Classic.

1. When you finish editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Fate clic su **Salva**, selezionate una cartella di archiviazione, immettete un nome per il set e fate clic su **Salva**.

## Eliminazione di un set di offerte {#deleting-an-offer-set}

Quando eliminate un set di offerte, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di offerte**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più set di offerte.
1. Nella barra di navigazione globale, fate clic su **File** &gt; **Elimina** &gt; **Elimina**.

>[!MORELIKETHIS]
>
>* [Creazione di parametri per i modelli](creating-template-parameters.md#creating_template_parameters)

