---
title: Creare un set di offerte
description: Scopri come creare un set di offerte in Adobe Dynamic Media Classic.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '1293'
ht-degree: 35%

---

# Creare un set di offerte {#creating-an-offer-set}

Potete creare i seguenti tipi di set di offerte:

* Video
* Modello con parametri
* Immagine

Per i modelli, selezionare **[!UICONTROL Aggiungi e visualizza anteprima]**, quindi impostare i parametri scelti. Gli altri tipi di set di offerte non includono parametri, ma puoi comunque personalizzarli selezionando **[!UICONTROL Anteprima]** e modificando i predefiniti disponibili.

Adobe Dynamic Media Classic offre strumenti per la modifica e la creazione di set di offerte.

>[!NOTE]
>
>Prima di creare un set di offerte, accertati di pubblicare su Adobe Dynamic Media Classic tutte le risorse che intendi utilizzare per il set. Consultate [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

## Tipi di set di offerte {#types-of-offer-sets}

Potete creare un set di offerte dai seguenti tipi di set di offerte:

* **Immagini**  - Puoi assemblare le immagini per un set di offerte. Ogni immagine include una diversa offerta nel set.

* **Modello immagine**  - È possibile parametrizzare i modelli immagine in Adobe Dynamic Media Classic con il comando  **[!UICONTROL Genera]**  > Nozioni di base sui modelli. Attraverso i parametri, potete scambiare e personalizzare i componenti del modello, come il testo all’interno di cornici di testo e le varie immagini. Per un set di offerte potete utilizzare i parametri dei modelli per creare, ad esempio, varianti di una stessa immagine nel set di offerte. Per informazioni sulla creazione e la parametrizzazione dei modelli immagine, consulta [Creare parametri modello](creating-template-parameters.md#creating_template_parameters).

Guarda anche il video di formazione [Template Basics](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) .

* **Video** : puoi assemblare video per un set di offerte. Ciascun video rappresenta una diversa offerta nel set.

## Creare un set di offerte con un modello con parametri {#creating-an-offer-set-with-a-parameterized-template}

Quando create un eCatalog, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** incide su set e relativi membri nei seguenti modi:

| **[!UICONTROL Pubblica dopo il]** salvataggio, opzione selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di offerte con un modello con parametri:**

1. Selezionare il modello o il banner.
1. Vai a **[!UICONTROL Build]** > **[!UICONTROL Set di offerte Test&amp;Target]**.

   Nella pagina Set di offerte Test&amp;Target sono elencate le offerte nel set di offerte. Il primo elemento nell’elenco rappresenta l’oggetto.

1. Selezionare l&#39;oggetto e selezionare **[!UICONTROL Aggiungi e visualizza anteprima]**.

   Il lato sinistro di questa pagina riporta i parametri presenti nel modello con i rispettivi valori.

1. Per creare l’offerta, modificate i valori dei parametri. Inserite, ad esempio, un testo diverso in un campo di testo, modificate la dimensione di un livello, inserite un’immagine al posto di un’altra oppure scegliete un predefinito per visualizzatori.
1. Seleziona **[!UICONTROL Salva]** o **[!UICONTROL Salva con nome**]** per salvare l&#39;offerta come parte del set di offerte.

   Nella pagina Set di offerte Test&amp;Target sono elencate le offerte create.

1. Ripetete i punti da 3 a 5 per creare più offerte per il set.
1. Al termine, vicino all’angolo inferiore destro della pagina, accertati che l’opzione **[!UICONTROL Pubblica dopo il salvataggio*]** sia selezionata (impostazione predefinita).
1. Seleziona **[!UICONTROL Chiudi]**, immetti un nome per il set di offerte, quindi seleziona **[!UICONTROL Salva]**.

Prima di chiudere la pagina Set di offerte Test&amp;Target, invia il set di offerte ad Adobe Target Standard/Premium. Consultate [Invio dei set di offerte a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Creare un set di offerte con immagini o video {#creating-an-offer-set-with-images-or-videos}

Quando create un eCatalog, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** incide su set e relativi membri nei seguenti modi:

| **[!UICONTROL Pubblica dopo il]** salvataggio, opzione selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di offerte con immagini o video:**

1. Assembla immagini o video per il set di offerte. Inizia nella schermata Set di offerte Test&amp;Target o nella vista Griglia o Elenco e utilizza uno dei seguenti metodi:

   * **Schermata**  Set di offerte Test&amp;Target - Vai a  **[!UICONTROL Genera]**  >  **[!UICONTROL Set di offerte Test&amp;Target]**. Trascinate le immagini o i video sulla schermata. Per creare video o immagini di diverse misure, trascinate più copie delle immagini o dei video e impostatene le dimensioni singolarmente.

   * **Vista a griglia o Vista a elenco**  - Seleziona le immagini o i video, quindi vai a  **[!UICONTROL Genera]**  >  **[!UICONTROL Set di offerte Test&amp;Target]**.

1. Facoltativamente, seleziona un&#39;immagine o un video e seleziona **[!UICONTROL Anteprima]**. Nella pagina Anteprima offerte è possibile modificare le dimensioni e l’aspetto dell’immagine o del video selezionato. In alternativa, puoi modificare tutte le immagini o i video nel set di offerte.

   * Scegliete un predefinito per cambiare l’aspetto e le dimensioni dell’immagine o del video.
   * Per applicare il predefinito scelto a tutte le offerte del set di offerte, seleziona la casella di controllo **[!UICONTROL Seleziona predefiniti per tutti]** .

   Seleziona **[!UICONTROL Salva]** per salvare le modifiche apportate all&#39;immagine o all&#39;offerta video. Quindi seleziona **[!UICONTROL Chiudi]** per tornare alla pagina Set di offerte Test&amp;Target .

1. Dopo aver completato la creazione di offerte per il set di offerte e aver scelto Predefiniti immagini per immagini diverse, accertati che sia selezionato **[!UICONTROL Pubblica dopo il salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]** e immetti un nome per il set di offerte, quindi seleziona **[!UICONTROL Salva]**.

Prima di chiudere la pagina Set di offerte Test&amp;Target, invia il set di offerte ad Adobe Target Standard/Premium. Consulta [Invio di set di offerte a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Modificare un set di offerte {#editing-an-offer-set}

Sia che modifichi un set pubblicato che un set non pubblicato, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** influisce sul set e sui membri impostati nei seguenti modi:

| Il set è già pubblicato | **[!UICONTROL Pubblica dopo il]** salvataggio, opzione selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di offerte:**

1. Per modificare un set di offerte, visualizzalo in Vista griglia o Vista a elenco, quindi seleziona il relativo pulsante di rollover **[!UICONTROL Modifica]**.
1. Nella pagina Set di offerte Test&amp;Target , effettua una delle seguenti operazioni:

   * **Rimozione di un’offerta** : seleziona l’offerta, quindi seleziona  **** Elimina per rimuovere un’offerta dal set.
   * **Aggiunta di un’offerta** : la modalità di aggiunta di un’offerta dipende dal tipo di set di offerte con cui stai lavorando:
      * **Modelli**  - Seleziona  **[!UICONTROL Aggiungi e visualizza anteprima]** e nella pagina Aggiungi e visualizza anteprima offerte crea un’altra offerta.
      * **Immagini e video**  - Trascina un’immagine o un video nella pagina Set di offerte Test&amp;Target .

   >[!NOTE]
   >
   >non potete eliminare un set di offerte associato a una campagna. Per eliminare un set di offerte associato a una campagna, accedi ad Adobe Target Standard/Premium e rimuovi prima le associazioni di campagne. Anche dopo aver annullato l’associazione da una campagna, la risorsa può essere eliminata solo da Adobe Dynamic Media Classic, richiedendo l’accesso ad Adobe Target Standard/Premium e non da Adobe Target Standard/Premium.

1. Al termine della modifica, accertati che nell’angolo in basso a destra della pagina sia selezionato **[!UICONTROL Pubblica dopo aver salvato]** (impostazione predefinita).
1. Selezionare **[!UICONTROL Salva]**, selezionare una cartella di archiviazione, immettere un nome per il set, quindi selezionare **[!UICONTROL Salva]**.

## Eliminare un set di offerte {#deleting-an-offer-set}

Quando eliminate un set di offerte, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un set di offerte:**

1. In Vista griglia, Vista elenco o Vista dettagli, selezionare uno o più set di offerte.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **Elimina**.

>[!MORELIKETHIS]
>
>* [Creazione di parametri per i modelli](creating-template-parameters.md#creating_template_parameters)

