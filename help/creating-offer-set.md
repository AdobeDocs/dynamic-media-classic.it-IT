---
title: Creare un set di offerte
description: Scopri come creare un set di offerte in Adobe Dynamic Media Classic.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1294'
ht-degree: 35%

---

# Creare un set di offerte {#creating-an-offer-set}

Potete creare i seguenti tipi di set di offerte:

* Video
* Modello con parametri
* Immagine

Per i modelli, seleziona **[!UICONTROL Aggiungi e visualizza anteprima]**, quindi imposta i parametri scelti. Gli altri tipi di set di offerte non includono parametri, ma puoi comunque personalizzarli selezionando **[!UICONTROL Anteprima]** e la modifica dei predefiniti disponibili.

Adobe Dynamic Media Classic offre strumenti per la modifica e la creazione di set di offerte.

>[!NOTE]
>
>Prima di creare un set di offerte, accertati di pubblicare su Adobe Dynamic Media Classic tutte le risorse che intendi utilizzare per il set. Consultate [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

## Tipi di set di offerte {#types-of-offer-sets}

Potete creare un set di offerte dai seguenti tipi di set di offerte:

* **Immagini** - È possibile assemblare le immagini per un set di offerte. Ogni immagine include una diversa offerta nel set.

* **Modello immagini** - È possibile parametrizzare i modelli di immagine in Adobe Dynamic Media Classic con **[!UICONTROL Crea]** > Comando Nozioni di base sui modelli. Attraverso i parametri, potete scambiare e personalizzare i componenti del modello, come il testo all’interno di cornici di testo e le varie immagini. Per un set di offerte potete utilizzare i parametri dei modelli per creare, ad esempio, varianti di una stessa immagine nel set di offerte. Per informazioni sulla creazione e la parametrizzazione dei modelli immagine, consulta [Creare parametri di modello](creating-template-parameters.md#creating_template_parameters).

Vedi anche [Nozioni di base sui modelli](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) video di formazione.

* **Video** - È possibile assemblare video per un set di offerte. Ciascun video rappresenta una diversa offerta nel set.

## Creare un set di offerte con un modello con parametri {#creating-an-offer-set-with-a-parameterized-template}

Quando create un eCatalog, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** incide su set e relativi membri nei seguenti modi:

| **[!UICONTROL Pubblica dopo il salvataggio]** opzione selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di offerte con un modello con parametri:**

1. Selezionare il modello o il banner.
1. Vai a **[!UICONTROL Crea]** > **[!UICONTROL Set di offerte Test&amp;Target]**.

   Nella pagina Set di offerte Test&amp;Target sono elencate le offerte nel set di offerte. Il primo elemento nell’elenco rappresenta l’oggetto.

1. Selezionare l’oggetto e **[!UICONTROL Aggiungi e visualizza anteprima]**.

   Il lato sinistro di questa pagina riporta i parametri presenti nel modello con i rispettivi valori.

1. Per creare l’offerta, modificate i valori dei parametri. Inserite, ad esempio, un testo diverso in un campo di testo, modificate la dimensione di un livello, inserite un’immagine al posto di un’altra oppure scegliete un predefinito per visualizzatori.
1. Seleziona **[!UICONTROL Salva]** o **[!UICONTROL Salva con nome**]** per salvare l’offerta come parte del set di offerte.

   Nella pagina Set di offerte Test&amp;Target sono elencate le offerte create.

1. Ripetete i punti da 3 a 5 per creare più offerte per il set.
1. Al termine, vicino all’angolo inferiore destro della pagina, assicurati che **[!UICONTROL Pubblica dopo il salvataggio*]** è selezionato (predefinito).
1. Seleziona **[!UICONTROL Chiudi]**, immetti un nome per il set di offerte, quindi seleziona **[!UICONTROL Salva]**.

Prima di chiudere la pagina Set di offerte Test&amp;Target, invia il set di offerte ad Adobe Target Standard/Premium. Vedi [Invia set di offerte a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Creare un set di offerte con immagini o video {#creating-an-offer-set-with-images-or-videos}

Quando create un eCatalog, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** incide su set e relativi membri nei seguenti modi:

| **[!UICONTROL Pubblica dopo il salvataggio]** opzione selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di offerte con immagini o video:**

1. Assembla immagini o video per il set di offerte. Inizia nella schermata Set di offerte Test&amp;Target o nella vista Griglia o Elenco e utilizza uno dei metodi seguenti:

   * **Schermata Set di offerte Test&amp;Target** - Vai a **[!UICONTROL Crea]** > **[!UICONTROL Set di offerte Test&amp;Target]**. Trascinate le immagini o i video sulla schermata. Per creare video o immagini di diverse misure, trascinate più copie delle immagini o dei video e impostatene le dimensioni singolarmente.

   * **Vista a griglia o vista a elenco** - Seleziona le immagini o i video e vai a **[!UICONTROL Crea]** > **[!UICONTROL Set di offerte Test&amp;Target]**.

1. Facoltativamente, seleziona un’immagine o un video e seleziona **[!UICONTROL Anteprima]**. Nella pagina Anteprima offerte è possibile modificare le dimensioni e l’aspetto dell’immagine o del video selezionato. In alternativa, puoi modificare tutte le immagini o i video nel set di offerte.

   * Scegliete un predefinito per cambiare l’aspetto e le dimensioni dell’immagine o del video.
   * Per applicare il predefinito scelto a tutte le offerte del set di offerte, seleziona la **[!UICONTROL Seleziona predefiniti per tutti]** casella di controllo.

   Seleziona **[!UICONTROL Salva]** per salvare le modifiche apportate all’offerta immagine o video. Quindi seleziona **[!UICONTROL Chiudi]** per tornare alla pagina Set di offerte Test&amp;Target .

1. Dopo aver completato la creazione di offerte per il set di offerte e scelto Predefiniti immagini per diverse immagini, assicurati che **[!UICONTROL Pubblica dopo il salvataggio]** è selezionato (predefinito).
1. Seleziona **[!UICONTROL Salva]** e immetti un nome per il set di offerte, quindi seleziona **[!UICONTROL Salva]**.

Prima di chiudere la pagina Set di offerte Test&amp;Target, invia il set di offerte ad Adobe Target Standard/Premium. Vedi [Invia set di offerte a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Modificare un set di offerte {#editing-an-offer-set}

Se modifichi un set pubblicato o un set non pubblicato, la **[!UICONTROL Pubblica dopo il salvataggio]** influenza i membri set e set nei seguenti modi:

| Il set è già pubblicato | **[!UICONTROL Pubblica dopo il salvataggio]** opzione selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di offerte:**

1. Per modificare un set di offerte, visualizzalo in Vista a griglia o Vista a elenco e selezionane uno **[!UICONTROL Modifica]** pulsante rollover.
1. Nella pagina Set di offerte Test&amp;Target , effettua una delle seguenti operazioni:

   * **Rimozione di un’offerta** - Seleziona l’offerta, quindi seleziona **[!UICONTROL Elimina]** per rimuovere un’offerta dal set.
   * **Aggiunta di un’offerta** - La modalità di aggiunta di un’offerta dipende dal tipo di set di offerte con cui stai lavorando:
      * **Modelli** - Seleziona **[!UICONTROL Aggiungi e visualizza anteprima]**, e nella pagina Aggiungi e visualizza anteprima offerte , crea un’altra offerta.
      * **Immagini e video** - Trascina un’immagine o un video nella pagina Set di offerte Test&amp;Target .

   >[!NOTE]
   >
   >non potete eliminare un set di offerte associato a una campagna. Per eliminare un set di offerte associato a una campagna, accedi ad Adobe Target Standard/Premium e rimuovi prima le associazioni di campagne. Anche dopo aver annullato l’associazione da una campagna, la risorsa può essere eliminata solo da Adobe Dynamic Media Classic, richiedendo l’accesso ad Adobe Target Standard/Premium e non da Adobe Target Standard/Premium.

1. Al termine della modifica, accertati di **[!UICONTROL Pubblica dopo il salvataggio]** è selezionato (predefinito).
1. Seleziona **[!UICONTROL Salva]**, seleziona una cartella di archiviazione, immetti un nome per il set, quindi seleziona **[!UICONTROL Salva]**.

## Eliminare un set di offerte {#deleting-an-offer-set}

Quando eliminate un set di offerte, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di offerte:**

1. In Vista griglia, Vista elenco o Vista dettagli, selezionare uno o più set di offerte.
1. Nella barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **Elimina**.

>[!MORELIKETHIS]
>
>* [Creazione di parametri per i modelli](creating-template-parameters.md#creating_template_parameters)

