---
title: Configurazione predefiniti immagine
description: Scopri come impostare i predefiniti per immagini in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 37%

---

# Configurazione predefiniti immagine{#setting-up-image-presets}

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Per capire come funzionano i predefiniti immagine, supponiamo che il sito web richieda che ogni immagine del prodotto sia visualizzata in due dimensioni diverse: 500 × 500 pixel e 150 × 150 pixel. Si creano due predefiniti per le immagini, uno denominato &quot;Ingrandisci&quot; per visualizzare le immagini a 500x500 pixel e uno denominato &quot;Miniatura&quot; per visualizzare le immagini a 150 × 150 pixel. Per distribuire immagini con le dimensioni &quot;Ingrandisci&quot; e &quot;Miniatura&quot;, un server immagini Dynamic Medie cerca la definizione di &quot;Predefinito immagine ingrandita&quot; e &quot;Predefinito immagine miniatura&quot;. Quindi il server genera in modo dinamico un’immagine secondo le specifiche di ridimensionamento e formattazione di ciascun predefinito per immagini.

Adobe Dynamic Media Classic viene fornito con diversi predefiniti immagine &quot;best practice&quot; già configurati per l’utilizzo. Gli amministratori possono anche creare predefiniti per immagini. Per creare un predefinito per immagini, potete partire da zero o iniziare da uno esistente e salvarlo con un nuovo nome.

Le immagini la cui dimensione viene ridotta quando vengono trasmesse da un server in modo dinamico possono perdere nitidezza e dettaglio. Per questa ragione, ciascun predefinito per immagini contiene controlli di formattazione per ottimizzare l’immagine quando questa viene trasmessa in una determinata dimensione. Grazie a tali controlli, le immagini trasmesse al sito Web o all’applicazione restano nitide e chiare.

## Creare un predefinito immagine {#creating-an-image-preset}

Se siete l’amministratore della società, potete creare dei predefiniti per immagini in base alle vostre specifiche esigenze. Potete creare predefiniti immagine o iniziare con un predefinito immagine predefinito fornito da Adobe Dynamic Media Classic, modificarlo e salvarlo con un nuovo nome.

**Per creare un predefinito immagine:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**.

   Per un’anteprima di un predefinito per immagini esistente, selezionatene il nome in questa schermata. Quando selezionate un nome di predefinito per immagini, l’immagine campione nella finestra Anteprima cambia di conseguenza, assumendo la dimensione e l’aspetto specificati dal predefinito.

1. Effettuate una delle seguenti operazioni:

   * **Creare un predefinito immagine** - Seleziona **[!UICONTROL Aggiungi]**.
   * **Modificare un predefinito immagine** : individua il predefinito immagine più simile a quello che desideri creare, quindi seleziona **[!UICONTROL Modifica]**.

1. Immettete un nome per il predefinito per immagini.
1. Immettete i valori Larghezza e Altezza in pixel. Tali valori determinano la dimensione in cui verranno trasmesse le immagini.
1. Compilate la schermata Aggiungi predefinito o Modifica predefinito. Per informazioni, consultate [Opzioni dei predefiniti per immagini](application-setup.md#image_preset_options).

   Adobe Dynamic Media Classic consiglia di avviare le seguenti opzioni di &quot;best practice&quot;:

   * **[!UICONTROL Formato]** - Scegli JPEG o un altro formato che soddisfi le tue esigenze. Tutti i browser web supportano il formato immagine JPEG, che offre un buon equilibrio tra dimensioni ridotte dei file e qualità delle immagini. Tuttavia, le immagini JPEG utilizzano uno schema di compressione con perdita di dati che può introdurre artefatti di immagine indesiderati se l’impostazione di compressione è troppo bassa. Per questo motivo, Adobe Dynamic Media Classic consiglia di impostare la qualità di compressione (sul dispositivo di scorrimento) su 75. Questa impostazione offre il giusto compromesso tra qualità delle immagini e dimensione ridotta dei file.

   * **[!UICONTROL Nitidezza]** - Non selezionare Nitidezza (questo filtro di nitidezza offre un controllo inferiore rispetto a **[!UICONTROL Maschera di contrasto]** ).

   * **[!UICONTROL Modalità di ricampionamento]** - Scegli **[!UICONTROL Bicubico]**.

   * **[!UICONTROL Maschera di contrasto]** (USM) - Immettere le impostazioni seguenti:

   | Tipo predefinito | Dimensione | USM: Fattore | USM: Raggio | USM: Soglia |
   | --- | --- | --- | --- | --- |
   | Oggetti correlati (mini miniature) | 75 × 75 | 1,5 | 0,8 | 5 |
   | Miniatura | 150 × 150 | 1,1 | 1 | 5 |
   | Principale | 350 × 350 | 1 | 1 | 6 |
   | Ingrandimento | 500 × 500 | 1,2 | 1,2 | 5 |

1. Seleziona **[!UICONTROL Salva]**.

Le opzioni consigliate di Adobe Dynamic Media Classic per la creazione di predefiniti immagine qui elencate sono generali. La nitidezza è altamente soggettiva. Queste impostazioni di &quot;best practice&quot; si basavano su un&#39;immagine primaria da 2000 × 2000; le impostazioni per i file primari più grandi o più piccoli possono essere diverse. Se si desidera regolare le impostazioni Maschera di contrasto, Adobe Dynamic Media Classic consiglia i seguenti intervalli:

* **[!UICONTROL Quantità]** - Tra 0,8 e 1,5.

* **[!UICONTROL Raggio]** - Tra 0,6 e 2.

* **[!UICONTROL Soglia]** - Da 1 a 6.

Per eliminare un predefinito immagine, selezionatelo nella schermata Predefiniti immagine, quindi selezionate **[!UICONTROL Elimina]**.

>[!MORELIKETHIS]
>
>* [Creare e modificare i predefiniti immagine](application-setup.md#creating_and_editing_image_presets)
>* [Opzioni predefinito immagine](application-setup.md#image_preset_options)
>* [Visualizzare in anteprima una risorsa immagine in base al suo predefinito immagine](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
