---
title: Creare un set di offerte
description: Scopri come creare un set di offerte in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 21%

---

# Creare un set di offerte {#creating-an-offer-set}

Potete creare uno dei seguenti tipi di serie di offerte:

* Video
* Modello con parametri
* Immagine

Per i modelli, seleziona **[!UICONTROL Aggiungi e visualizza anteprima]**, quindi impostare i parametri selezionati. Altri tipi di serie di offerte non includono parametri, ma puoi comunque personalizzarli selezionando **[!UICONTROL Anteprima]** e la modifica dei predefiniti disponibili.

Adobe Dynamic Media Classic offre strumenti per la modifica e la creazione di set di offerte.

>[!NOTE]
>
>Prima di creare una serie di offerte, assicurati di pubblicare su Adobe Dynamic Media Classic tutte le risorse che intendi utilizzare per il set. Consultate [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

## Tipi di set di offerte {#types-of-offer-sets}

Creare una serie di offerte dai seguenti tipi di serie di offerte:

* **Immagini**: puoi assemblare immagini per un set di offerte. Ogni immagine include un’offerta diversa nel set.

* **Modello immagine**: puoi parametrizzare i modelli di immagine in Adobe Dynamic Media Classic con il **[!UICONTROL Genera]** > Comando di base del modello. Attraverso parametri, componenti del modello, il testo nelle cornici di testo, le diverse immagini, possono essere scambiati e personalizzati. Per una serie di offerte, puoi utilizzare i parametri del modello per creare varianti sulla stessa immagine nella serie di offerte, ad esempio. Per informazioni sulla creazione e la parametrizzazione dei modelli di immagine, consultate [Creare i parametri del modello](creating-template-parameters.md#creating_template_parameters).

Vedi anche [Nozioni di base sui modelli](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) video di formazione.

* **Video**: puoi assemblare un video per un set di offerte. Ciascun video rappresenta una diversa offerta nel set.

## Creare un set di offerte con un modello con parametri {#creating-an-offer-set-with-a-parameterized-template}

Quando si crea una serie di offerte, **[!UICONTROL Pubblica dopo un salvataggio]** influisce sui membri set e set nei modi seguenti:

| **[!UICONTROL Pubblica dopo un salvataggio]** opzione selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di offerte con un modello con parametri:**

1. Selezionare il modello o il banner.
1. Vai a **[!UICONTROL Genera]** > **[!UICONTROL Set di offerte Test&amp;Target]**.

   La pagina Set di offerte Test&amp;Target elenca le offerte incluse nel set di offerte. Il primo elemento nell’elenco rappresenta l’oggetto.

1. Selezionare l&#39;oggetto e selezionare **[!UICONTROL Aggiungi e visualizza anteprima]**.

   Il lato sinistro di questa pagina riporta i parametri presenti nel modello con i rispettivi valori.

1. Per creare l’offerta, modificate i valori dei parametri. Ad esempio, immettete un testo diverso in un campo di testo, modificate le dimensioni di un livello, scambiate un&#39;immagine per un&#39;altra oppure scegliete un predefinito visualizzatore diverso.
1. Seleziona **[!UICONTROL Salva]** o **[!UICONTROL Salva con nome**]** per salvare l’offerta come parte del set di offerte.

   Nella pagina Set di offerte Test&amp;Target sono elencate le offerte create.

1. Ripetete i punti da 3 a 5 per creare più offerte per il set.
1. Al termine, vicino all’angolo inferiore destro della pagina, assicurati che **[!UICONTROL Pubblica dopo un salvataggio*]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Chiudi]**, immetti un nome per la serie di offerte, quindi seleziona **[!UICONTROL Salva]**.

Prima di chiudere la pagina Set di offerte Test&amp;Target, invia il set di offerte ad Adobe Target Standard/Premium. Consulta [Invia set di offerte a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Creare un set di offerte con immagini o video {#creating-an-offer-set-with-images-or-videos}

Quando si crea una serie di offerte, **[!UICONTROL Pubblica dopo un salvataggio]** influisce sui membri set e set nei modi seguenti:

| **[!UICONTROL Pubblica dopo un salvataggio]** opzione selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un set di offerte con immagini o video:**

1. Assembla immagini o video per il set di offerte. Iniziare nella schermata Set offerte Test&amp;Target o nella Vista griglia o Vista elenco e utilizzare uno dei metodi seguenti:

   * **Schermata Set offerte Test&amp;Target**: vai a **[!UICONTROL Genera]** > **[!UICONTROL Set di offerte Test&amp;Target]**. Trascinate le immagini o i video sulla schermata. Per creare video o immagini di diverse misure, trascinate più copie delle immagini o dei video e impostatene le dimensioni singolarmente.

   * **Visualizzazione griglia o visualizzazione elenco**: seleziona le immagini o i video, quindi vai a **[!UICONTROL Genera]** > **[!UICONTROL Set di offerte Test&amp;Target]**.

1. Se necessario, seleziona un’immagine o un video e fai clic su **[!UICONTROL Anteprima]**. Nella pagina Anteprima offerte è possibile modificare le dimensioni e l&#39;aspetto dell&#39;immagine o del video selezionato. In alternativa, puoi modificare tutte le immagini o i video nel Set di offerte.

   * Scegliete un predefinito per cambiare l’aspetto e le dimensioni dell’immagine o del video.
   * Per applicare il predefinito scelto a tutte le offerte del set di offerte, seleziona la **[!UICONTROL Seleziona predefiniti per tutti]** casella di controllo.

   Seleziona **[!UICONTROL Salva]** per salvare le modifiche apportate all’offerta immagine o video. Quindi seleziona **[!UICONTROL Chiudi]** per tornare alla pagina Set di offerte Test&amp;Target.

1. Dopo aver completato la creazione delle offerte per il set di offerte e aver scelto i predefiniti immagine per le diverse immagini, assicurati che **[!UICONTROL Pubblica dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]** e inserisci un nome per la serie di offerte, quindi seleziona **[!UICONTROL Salva]**.

Prima di chiudere la pagina Set di offerte Test&amp;Target, invia il set di offerte ad Adobe Target Standard/Premium. Consulta [Invia set di offerte a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Modificare un set di offerte {#editing-an-offer-set}

Sia che si modifichi un set pubblicato o un set non pubblicato, il **[!UICONTROL Pubblica dopo un salvataggio]** influisce sui membri set e set nei modi seguenti:

| Il set è già pubblicato | **[!UICONTROL Pubblica dopo un salvataggio]** opzione selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono lo stato pubblicato. I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare una serie di offerte:**

1. Per modificare una serie di offerte, visualizzarla in Vista griglia o Vista elenco, quindi selezionarne una **[!UICONTROL Modifica]** pulsante di rollover.
1. Nella pagina Set di offerte Test&amp;Target eseguire una delle operazioni seguenti:

   * **Rimozione di un’offerta**: seleziona l’offerta, quindi seleziona **[!UICONTROL Elimina]** per rimuovere un’offerta dal set.
   * **Aggiunta di un’offerta**: la modalità di aggiunta di un’offerta dipende dal tipo di Set di offerte con cui stai lavorando:
      * **Modelli**: Seleziona **[!UICONTROL Aggiungi e visualizza anteprima]**, e nella pagina Aggiungi e visualizza anteprima offerte, crea un’altra offerta.
      * **Immagini e video**: trascina un’immagine o un video nella pagina Set di offerte Test&amp;Target.

   >[!NOTE]
   >
   >Non puoi eliminare un set di offerte associato a una campagna. Per eliminare un set di offerte associato a una campagna, accedi ad Adobe Target Standard/Premium e rimuovi le associazioni alle campagne. Anche dopo l’annullamento dell’associazione a una campagna, la risorsa può essere eliminata solo da Adobe Dynamic Media Classic, richiedendo l’accesso a Adobe Target Standard/Premium e non da Adobe Target Standard/Premium.

1. Al termine della modifica, vicino all’angolo inferiore destro della pagina, assicurati che **[!UICONTROL Pubblica dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, selezionare una cartella di archiviazione, immettere un nome per il set e quindi selezionare **[!UICONTROL Salva]**.

## Eliminare un set di offerte {#delet-an-offer-set}

Quando eliminate un set di offerte, viene spostato nel cestino. Tuttavia, i membri (o &quot;figli&quot;) all&#39;interno di quel set non sono interessati; invece, ciascuno di essi mantiene il proprio stato pubblicato o non pubblicato esistente.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare una serie di offerte:**

1. Nella Vista griglia, Vista elenco o Vista dettagli, seleziona una o più serie di offerte.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **Elimina**.

>[!MORELIKETHIS]
>
>* [Creazione di parametri di modello](creating-template-parameters.md#creating_template_parameters)
