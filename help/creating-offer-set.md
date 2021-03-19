---
title: Creazione di un set di offerte
description: Scopri come creare un set di offerte.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Ingegnere dati,Amministratore,Professionista aziendale
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1223'
ht-degree: 56%

---


# Creazione di un set di offerte{#creating-an-offer-set}

Potete creare i seguenti tipi di set di offerte:

* Video
* Modello con parametri
* Immagine

Per i modelli, fai clic su **Aggiungi e visualizza anteprima**, quindi imposta i parametri scelti. Gli altri tipi di set di offerte non dispongono di parametri, ma li potete personalizzare facendo clic su **Anteprima** e cambiando i predefiniti disponibili.

Dynamic Media Classic offre strumenti per la modifica e la creazione di set di offerte.

>[!NOTE]
>
>Prima di creare un set di offerte, accertati di pubblicare tutte le risorse che intendi utilizzare per il set in Dynamic Media Classic. Consultate [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

## Tipi di set di offerte {#types-of-offer-sets}

Potete creare un set di offerte dai seguenti tipi di set di offerte:

* ****
ImmaginiPuoi assemblare le immagini per un set di offerte. Ogni immagine include una diversa offerta nel set.

* **Modello**
di immagineÈ possibile parametrizzare i modelli di immagine in Dynamic Media Classic con il comando Genera > Nozioni di base sui modelli. Attraverso i parametri, potete scambiare e personalizzare i componenti del modello, come il testo all’interno di cornici di testo e le varie immagini. Per un set di offerte potete utilizzare i parametri dei modelli per creare, ad esempio, varianti di una stessa immagine nel set di offerte. Per informazioni sulla creazione e la definizione di parametri per i modelli per immagini, consultate Creazione di parametri per i modelli.

* ****
Video: puoi assemblare un video per un set di offerte. Ciascun video rappresenta una diversa offerta nel set.

## Creazione di un set di offerte con un modello con parametri {#creating-an-offer-set-with-a-parameterized-template}

Quando create un eCatalog, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di offerte con un modello con parametri**

1. Selezionare il modello o il banner.
1. Fate clic su **Genera** > **Set di offerte per Test&amp;Target**.

   Nella pagina Set di offerte Test&amp;Target sono elencate le offerte nel set di offerte. Il primo elemento nell’elenco rappresenta l’oggetto.

1. Selezionate l’oggetto e fate clic sul pulsante **Aggiungi e visual. antepr.**.

   Il lato sinistro di questa pagina riporta i parametri presenti nel modello con i rispettivi valori.

1. Per creare l’offerta, modificate i valori dei parametri. Inserite, ad esempio, un testo diverso in un campo di testo, modificate la dimensione di un livello, inserite un’immagine al posto di un’altra oppure scegliete un predefinito per visualizzatori.
1. Per salvare l’offerta come parte del set di offerte, fate clic su **Salva** o **Salva con nome**. 

   Nella pagina Set di offerte Test&amp;Target sono elencate le offerte create.

1. Ripetete i punti da 3 a 5 per creare più offerte per il set.
1. Al termine, vicino all’angolo in basso a destra della pagina, accertati che l’opzione **Pubblica dopo aver salvato** sia selezionata (impostazione predefinita).
1. Fai clic su **Chiudi**, immetti un nome per il set di offerte, quindi fai clic su **Salva**.

Prima di chiudere la pagina Set di offerte Test&amp;Target, invia il set di offerte a Target Standard/Premium. Consultate [Invio dei set di offerte a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Creazione di un set di offerte con immagini o video {#creating-an-offer-set-with-images-or-videos}

Quando create un eCatalog, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di offerte con immagini o video**

1. Assembla immagini o video per il set di offerte. Inizia nella schermata Set di offerte Test&amp;Target o nella vista Griglia o Elenco e utilizza uno dei seguenti metodi:

   * **** Schermata Set di offerte Test&amp;TargetFai clic su  **[!UICONTROL Genera > Set di offerte Test&amp;Target]**. Trascinate le immagini o i video sulla schermata. Per creare video o immagini di diverse misure, trascinate più copie delle immagini o dei video e impostatene le dimensioni singolarmente.

   * **Griglia o** Vista a elencoSeleziona le immagini o i video, quindi fai clic su  **[!UICONTROL Genera > Set di offerte Test&amp;Target]**.

1. Facoltativamente, potete selezionare un’immagine o un video e fare clic su **Anteprima**. Nella pagina Anteprima offerte è possibile modificare le dimensioni e l’aspetto dell’immagine o del video selezionato. In alternativa, puoi modificare tutte le immagini o i video nel set di offerte.

   * Scegliete un predefinito per cambiare l’aspetto e le dimensioni dell’immagine o del video.
   * Fate clic sulla casella Applica predefinito selezionato a tutti per applicare il predefinito scelto a tutte le offerte del set di offerte.

   Fate clic su **Salva** per salvare le modifiche apportate all’offerta di immagini o video. Fate clic su **Chiudi** per tornare alla schermata Set di offerte per Test&amp;Target.

1. Dopo aver completato la creazione di offerte per il set di offerte e aver scelto Predefiniti immagini per immagini diverse, accertati che sia selezionato **Pubblica dopo il salvataggio** (impostazione predefinita).
1. Fate clic su **Salva**, immettete un nome per il set di offerte e fate clic su **Salva**.

Prima di chiudere la pagina Set di offerte Test&amp;Target, invia il set di offerte a Target Standard/Premium. Consultate [Invio dei set di offerte a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Modifica di un set di offerte  {#editing-an-offer-set}

A seconda se modificate un set pubblicato o non pubblicato, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Il set è già pubblicato | Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio delle modifiche | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono il proprio stato di pubblicazione.Tutti i nuovi membri del set aggiunti durante la modifica conservano il proprio stato di pubblicazione o di annullamento della pubblicazione. |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di offerte**

1. Per modificare un set di offerte, visualizzalo nella vista Griglia o Elenco e fai clic sul relativo pulsante di rollover **Modifica**.
1. Nella pagina Set di offerte Test&amp;Target , effettua una delle seguenti operazioni:

   * **Rimozione di un’**
offertaSeleziona l’offerta e fai clic su 
**** Elimina per rimuovere un’offerta dal set.
   * **Aggiunta di un’**
offertaLa modalità di aggiunta di un’offerta dipende dal tipo di set di offerte con cui stai lavorando:
   * ****
TemplatesClick 
**Aggiungi e visualizza anteprima** e crea un’altra offerta nella pagina Aggiungi e visualizza anteprima offerte .
   * **Immagini e**
videoTrascina un’immagine o un video nella pagina Set di offerte Test&amp;Target .
   >[!NOTE]
   >
   >non potete eliminare un set di offerte associato a una campagna. Per eliminare un set di offerte associato a una campagna, accedi a Target Standard/Premium e rimuovi prima le associazioni di campagne. Anche dopo aver annullato l’associazione da una campagna, la risorsa può essere eliminata solo da Dynamic Media Classic, richiedendo l’accesso a Target Standard/Premium e non da Target Standard/Premium.

1. Al termine della modifica, accertati che nell’angolo in basso a destra della pagina sia selezionato **Pubblica dopo aver salvato** (impostazione predefinita).
1. Fate clic su **Salva**, selezionate una cartella di archiviazione, immettete un nome per il set e fate clic su **Salva**.

## Eliminazione di un set di offerte  {#deleting-an-offer-set}

Quando eliminate un set di offerte, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di offerte**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più set di offerte.
1. Nella barra di navigazione globale, fate clic su **File** > **Elimina** > **Elimina**.

>[!MORELIKETHIS]
>
>* [Creazione di parametri per i modelli](creating-template-parameters.md#creating_template_parameters)

