---
title: Creazione di un set di offerte
seo-title: Creazione di un set di offerte
description: 'null'
seo-description: Scoprite come creare un set di offerte.
uuid: 6 d 6 a 4 af 9-70 c 0-4 cfa -9 a 8 f -855 d 6 adfcc 8 f
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/target_ classic_ integration
discoiquuid: 59 b 6437 d-c 21 e -4929-9291-3032 dbb 34565
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Creazione di un set di offerte{#creating-an-offer-set}

Potete creare i seguenti tipi di set di offerte:

* Video
* Modello con parametri
* Immagine

For templates, click **Add and Preview**, then set the parameters you choose. Gli altri tipi di set di offerte non dispongono di parametri, ma li potete personalizzare facendo clic su **Anteprima** e cambiando i predefiniti disponibili.

Dynamic Media Classic offre strumenti per la modifica e per creare set di offerte.

>[!NOTE]
>
>Prima di creare un set di offerte, pubblicate tutte le risorse che intendete utilizzare per il set in Scene 7 Publishing System. Consultate [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

## Tipi di set di offerte {#types-of-offer-sets}

Potete creare un set di offerte dai seguenti tipi di set di offerte:

**Immagini** È possibile assemblare le immagini per un set di offerte. Ogni immagine include un'offerta diversa nel set.

**Modello** immagini Potete parametrizzare i modelli immagine in Dynamic Media Classic con il comando Genera &gt; Funzioni di base dei modelli. Attraverso i parametri, potete scambiare e personalizzare i componenti del modello, come il testo all’interno di cornici di testo e le varie immagini. Per un set di offerte potete utilizzare i parametri dei modelli per creare, ad esempio, varianti di una stessa immagine nel set di offerte. Per informazioni sulla creazione e la definizione di parametri per i modelli per immagini, consultate Creazione di parametri per i modelli.

**Video** Potete assemblare un video per un set di offerte. Ciascun video rappresenta una diversa offerta nel set.

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

   Nella pagina Set di offerte di Target Classic sono elencate le offerte del set di offerte. Il primo elemento nell’elenco rappresenta l’oggetto.

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

1. Assemblate immagini o video per il set di offerte. Iniziate nella schermata Set di offerte Classic Classic oppure nella visualizzazione Griglia o Elenco e usate uno dei seguenti metodi:

   **Schermata Set di offerte Classic Classic** Fate clic su Genera &gt; Set di offerte Classic Classic. Trascinate le immagini o i video sulla schermata. Per creare video o immagini di diverse misure, trascinate più copie delle immagini o dei video e impostatene le dimensioni singolarmente.

   **Visualizzazione** Griglia o Elenco Selezionate le immagini o i video, quindi fate clic su Genera &gt; Set di offerte Classic Classic.

1. Facoltativamente, potete selezionare un’immagine o un video e fare clic su **Anteprima**. Nella pagina Anteprima offerte, potete modificare le dimensioni e l'aspetto dell'immagine o del video selezionato. Oppure, potete modificare tutte le immagini o i video del set di offerte.

   * Scegliete un predefinito per cambiare l’aspetto e le dimensioni dell’immagine o del video.
   * Fate clic sulla casella Applica predefinito selezionato a tutti per applicare il predefinito scelto a tutte le offerte del set di offerte.
   Fate clic su **Salva** per salvare le modifiche apportate all’offerta di immagini o video. Then click **Close** to return to the Target Classic Offer Set page.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. Fate clic su **Salva**, immettete un nome per il set di offerte e fate clic su **Salva**.

Prima di chiudere la pagina Set di offerte Classic Classic, inviate il set di offerte a Target Classic. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Modifica di un set di offerte {#editing-an-offer-set}

A seconda se modificate un set pubblicato o non pubblicato, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Il set è già pubblicato | Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio delle modifiche | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono il loro stato pubblicato. Tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione o pubblicazione non pubblicato. |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di offerte**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. Nella pagina Set di offerte di Target Classic, effettuate una delle seguenti operazioni:

   **Rimozione di un’offerta**

   Select the offer, and then click **Delete** to remove an offer from the set.

   **Aggiunta di un’offerta**

   La modalità di aggiunta di un'offerta dipende dal tipo di set di offerte con cui state lavorando:

   * Templates: Click **Add &amp; Preview**, and on the Add &amp; Preview Offers page, create another offer.
   * Immagini e video: Trascinate un'immagine o un video nella pagina Set di offerte Classic Classic.
   ***Nota**: Non potete eliminare un set di offerte associato a una campagna. Per eliminare un set di offerte associate a una campagna, accedete a Target Classic e rimuovete prima le associazioni della campagna. Even after un-associating from a campaign, the asset can only be deleted from Scene7 Publishing System, requiring a login to Target Classic, and not from within Target Classic.*

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

