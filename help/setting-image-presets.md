---
title: Impostazione dei predefiniti per immagini
description: Scopri come impostare i predefiniti per immagini in Adobe Dynamic Media Classic.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 54%

---

# Impostazione dei predefiniti per immagini{#setting-up-image-presets}

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Per comprendere il funzionamento dei predefiniti per immagini, supponiamo che il sito web richieda che ogni immagine del prodotto venga visualizzata in due dimensioni diverse: 500 x 500 pixel e 150 x 150 pixel. In questo caso dovrete creare due predefiniti per immagini, uno denominato “Ingrandimento” e l’altro “Miniatura” per visualizzare le immagini rispettivamente a 500 x 500 e 150 x 150 pixel. Per fornire immagini con le dimensioni &quot;Ingrandisci&quot; e &quot;Miniature&quot;, un server di immagini Dynamic Media cerca la definizione di Ingrandisci predefinito immagine e Predefinito immagine miniatura. Quindi il server genera in modo dinamico un’immagine secondo le specifiche di ridimensionamento e formattazione di ciascun predefinito per immagini.

Ad Adobe, Dynamic Media Classic include diversi predefiniti immagine &quot;best practice&quot; già configurati per l’utilizzo. Gli amministratori possono creare anche predefiniti per immagini. Per creare un predefinito per immagini, potete partire da zero o iniziare da uno esistente e salvarlo con un nuovo nome.

Le immagini la cui dimensione viene ridotta quando vengono trasmesse da un server in modo dinamico possono perdere nitidezza e dettaglio. Per questa ragione, ciascun predefinito per immagini contiene controlli di formattazione per ottimizzare l’immagine quando questa viene trasmessa in una determinata dimensione. Grazie a tali controlli, le immagini trasmesse al sito Web o all’applicazione restano nitide e chiare.

## Creare un predefinito per immagini {#creating-an-image-preset}

Se siete l’amministratore della società, potete creare dei predefiniti per immagini in base alle vostre specifiche esigenze. È possibile creare predefiniti per immagini o iniziare con un predefinito per immagini predefinito fornito da Adobe Dynamic Media Classic, modificarlo e salvarlo con un nuovo nome.

**Per creare un predefinito per immagini:**

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagini]**.

   Per un’anteprima di un predefinito per immagini esistente, selezionatene il nome in questa schermata. Quando selezionate un nome di predefinito per immagini, l’immagine campione nella finestra Anteprima cambia di conseguenza, assumendo la dimensione e l’aspetto specificati dal predefinito.

1. Effettuate una delle seguenti operazioni:

   * **Crea un predefinito**  per immagini - Seleziona  **[!UICONTROL Aggiungi]**.
   * **Modifica un predefinito immagine** : seleziona il predefinito immagine più simile a quello che desideri creare, quindi seleziona  **[!UICONTROL Modifica]**.

1. Immettete un nome per il predefinito per immagini.
1. Immettete i valori Larghezza e Altezza in pixel. Tali valori determinano la dimensione in cui verranno trasmesse le immagini.
1. Compilate la schermata Aggiungi predefinito o Modifica predefinito. Per informazioni, consultate [Opzioni dei predefiniti per immagini](application-setup.md#image_preset_options).

   Ad Adobe, Dynamic Media Classic consiglia di iniziare con le seguenti opzioni di &quot;best practice&quot;:

   * **[!UICONTROL Formato]** : scegli JPEG o un altro formato che soddisfi le tue esigenze. Tutti i browser web supportano il formato immagine JPEG, in quanto offre un buon compromesso tra dimensioni ridotte dei file e qualità delle immagini. Tuttavia, le immagini in formato JPEG usano uno schema di compressione che causa la perdita di dati, con possibile introduzione di artefatti di immagine indesiderati, qualora l’impostazione di compressione sia troppo bassa. Per questo motivo, Adobe Dynamic Media Classic consiglia di impostare la qualità di compressione (sul cursore) su 75. Questa impostazione offre un buon compromesso tra la qualità delle immagini e le dimensioni ridotte dei file.

   * **[!UICONTROL Nitidezza]**  - Non selezionare Nitidezza (il filtro di nitidezza offre un controllo inferiore rispetto alle impostazioni  **[!UICONTROL Maschera definizione dettagli]** ).

   * **[!UICONTROL Modalità]**  di campionamento - Scegli  **[!UICONTROL Bi-Cubic]**.

   * **[!UICONTROL Maschera definizione dettagli]**  (USM) - Inserisci le seguenti impostazioni:

   | Tipo predefinito | Dimensione | USM: Fattore | USM: Raggio | USM: Soglia |
   | --- | --- | --- | --- | --- |
   | Oggetti correlati (mini miniature) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniatura | 150 x 150 | 1,1 | 1 | 5 |
   | Principale | 350 x 350 | 1 | 1 | 6 |
   | Ingrandimento | 500 x 500 | 1,2 | 1,2 | 5 |

1. Selezionare **[!UICONTROL Salva]**.

L’Adobe delle opzioni di &quot;best practice&quot; di Dynamic Media Classic per la creazione di predefiniti per immagini elencate di seguito offre raccomandazioni generali; la nitidezza è molto soggettiva. Queste impostazioni si basano su un’immagine originale 2000 x 2000 e potrebbero pertanto differire per originali di dimensioni maggiori o minori. Per regolare le impostazioni Maschera definizione dettagli, ad Adobe Dynamic Media Classic consiglia gli intervalli seguenti:

* **[!UICONTROL Importo]**  - Tra 0,8 e 1,5.

* **[!UICONTROL Raggio]**  - Tra 0,6 e 2.

* **[!UICONTROL Soglia]**  - Da 1 a 6.

Per eliminare un predefinito immagine, selezionalo nella schermata Predefiniti immagine, quindi seleziona **[!UICONTROL Elimina]**.

>[!MORELIKETHIS]
>
>* [Creare e modificare i predefiniti immagine](application-setup.md#creating_and_editing_image_presets)
>* [Opzioni dei predefiniti immagine](application-setup.md#image_preset_options)
>* [Visualizzare in anteprima una risorsa immagine in base al relativo predefinito per immagini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

