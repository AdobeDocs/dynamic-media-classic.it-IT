---
title: Creazione di un set di offerte
seo-title: Creazione di un set di offerte
description: 'null'
seo-description: Scoprite come creare un set di offerte.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 57%

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
>Prima di creare un set di offerte, accertatevi di pubblicare tutte le risorse che intendete utilizzare per il set su Dynamic Media Classic. Consultate [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

## Tipi di set di offerte {#types-of-offer-sets}

Potete creare un set di offerte dai seguenti tipi di set di offerte:

* **Immagini** Potete assemblare le immagini per un set di offerte. Ogni immagine include un’offerta diversa nel set.

* **Modello** immagine È possibile parametrizzare i modelli per immagini in Dynamic Media Classic con il comando Genera > Funzioni di base dei modelli. Attraverso i parametri, potete scambiare e personalizzare i componenti del modello, come il testo all’interno di cornici di testo e le varie immagini. Per un set di offerte potete utilizzare i parametri dei modelli per creare, ad esempio, varianti di una stessa immagine nel set di offerte. Per informazioni sulla creazione e la definizione di parametri per i modelli per immagini, consultate Creazione di parametri per i modelli.

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
1. Fate clic su **Genera** > **Set di offerte per Test&amp;Target**.

   La pagina Set di offerte Test&amp;Target elenca le offerte nel set di offerte. Il primo elemento nell’elenco rappresenta l’oggetto.

1. Selezionate l’oggetto e fate clic sul pulsante **Aggiungi e visual. antepr.**.

   Il lato sinistro di questa pagina riporta i parametri presenti nel modello con i rispettivi valori.

1. Per creare l’offerta, modificate i valori dei parametri. Inserite, ad esempio, un testo diverso in un campo di testo, modificate la dimensione di un livello, inserite un’immagine al posto di un’altra oppure scegliete un predefinito per visualizzatori.
1. Per salvare l’offerta come parte del set di offerte, fate clic su **Salva** o **Salva con nome**. 

   Nella pagina Set di offerte Test&amp;Target sono elencate le offerte create.

1. Ripetete i punti da 3 a 5 per creare più offerte per il set.
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

Prima di chiudere la pagina Set di offerte Test&amp;Target, inviate il set di offerte a Target Standard/Premium. Consultate [Invio dei set di offerte a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Creating an offer set with images or videos {#creating-an-offer-set-with-images-or-videos}

Quando create un eCatalog, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di offerte con immagini o video**

1. Assemblate immagini o video per il set di offerte. Iniziate nella schermata Set di offerte Test&amp;Target oppure nella vista Griglia o Elenco e usate uno dei seguenti metodi:

   * **Schermata** Set di offerte Test&amp;Target Fate clic su **[!UICONTROL Genera > Set]** di offerte Test&amp;Target. Trascinate le immagini o i video sulla schermata. Per creare video o immagini di diverse misure, trascinate più copie delle immagini o dei video e impostatene le dimensioni singolarmente.

   * **Visualizzazione** Griglia o Elenco Selezionate le immagini o i video, quindi fate clic su **[!UICONTROL Genera > Set]** di offerte Test&amp;Target.

1. Facoltativamente, potete selezionare un’immagine o un video e fare clic su **Anteprima**. Nella pagina Anteprima offerte potete modificare le dimensioni e l’aspetto dell’immagine o del video selezionato. Oppure potete modificare tutte le immagini o i video del set di offerte.

   * Scegliete un predefinito per cambiare l’aspetto e le dimensioni dell’immagine o del video.
   * Fate clic sulla casella Applica predefinito selezionato a tutti per applicare il predefinito scelto a tutte le offerte del set di offerte.

   Fate clic su **Salva** per salvare le modifiche apportate all’offerta di immagini o video. Fate clic su **Chiudi** per tornare alla schermata Set di offerte per Test&amp;Target.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. Fate clic su **Salva**, immettete un nome per il set di offerte e fate clic su **Salva**.

Prima di chiudere la pagina Set di offerte Test&amp;Target, inviate il set di offerte a Target Standard/Premium. Consultate [Invio dei set di offerte a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

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
1. Nella pagina Set di offerte per Test&amp;Target, effettuate una delle seguenti operazioni:

   * **Rimozione di un&#39;offerta** Selezionate l&#39;offerta, quindi fate clic su 
**Elimina** per rimuovere un&#39;offerta dal set.
   * **L’aggiunta di un’offerta** La modalità di aggiunta di un’offerta dipende dal tipo di set di offerte con cui state lavorando:
   * **Modelli** Click 
**Aggiungi e visualizza anteprima** e crea un’altra offerta nella pagina Aggiungi offerte e visualizza anteprima.
   * **Immagini e video** Trascinate un’immagine o un video nella pagina Set di offerte per Test&amp;Target.
   >[!NOTE]
   >
   >non potete eliminare un set di offerte associato a una campagna. Per eliminare un set di offerte associato a una campagna, accedete a Target Standard/Premium e rimuovete prima le associazioni della campagna. Anche dopo aver interrotto l&#39;associazione da una campagna, la risorsa può essere eliminata solo da Dynamic Media Classic, richiedendo l&#39;accesso a Target Standard/Premium e non da Target Standard/Premium.

1. When you finish editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Fate clic su **Salva**, selezionate una cartella di archiviazione, immettete un nome per il set e fate clic su **Salva**.

## Eliminazione di un set di offerte {#deleting-an-offer-set}

Quando eliminate un set di offerte, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di offerte**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più set di offerte.
1. Nella barra di navigazione globale, fate clic su **File** > **Elimina** > **Elimina**.

>[!MORELIKETHIS]
>
>* [Creazione di parametri per i modelli](creating-template-parameters.md#creating_template_parameters)

