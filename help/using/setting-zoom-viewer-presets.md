---
title: Impostare i predefiniti per visualizzatore zoom
description: Scopri come impostare i predefiniti per visualizzatore zoom in Adobe Dynamic Media Classic.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 47%

---

# Impostare i predefiniti per visualizzatore zoom{#setting-up-zoom-viewer-presets}

I predefiniti per visualizzatori zoom determinano lo stile, il comportamento e l’aspetto dei visualizzatori zoom. Adobe Dynamic Media Classic offre molte opzioni per personalizzare e affiancare i visualizzatori. Adobe Dynamic Media Classic viene fornito con predefiniti di base (veloci), fly-out e predefiniti personalizzati per visualizzatori zoom. Se siete amministratori, potete creare predefiniti visualizzatore zoom per la società o modificare un predefinito predefinito predefinito e salvarlo con un nuovo nome.

Tutti i visualizzatori zoom includono pulsanti per applicare lo zoom in avanti, indietro, la panoramica e per ripristinare le stato originale dell’immagine dopo lo zoom. L&#39;aspetto di questi pulsanti e la modalità di visualizzazione della finestra dipendono dall&#39;impostazione dei predefiniti per visualizzatore zoom. Potete configurare un predefinito per visualizzatori zoom con diverse impostazioni di colori, bordi, font e immagine. Quando configurate un visualizzatore zoom guidato, potete anche scegliere il percorso di salvataggio delle destinazioni di zoom. Le destinazioni di zoom sono miniature che gli utenti possono selezionare per applicare lo zoom alle aree specificate.

## I predefiniti per visualizzatori zoom {#about-zoom-viewer-presets}

Adobe Dynamic Media Classic offre i seguenti predefiniti visualizzatore zoom:

* **Visualizzatore zoom: di base** - Fornisce uno zoom di base sull&#39;immagine originale.

* **Visualizzatore zoom: a comparsa** - Visualizza una seconda immagine dell&#39;area ingrandita accanto all&#39;immagine originale. Non vi sono controlli; gli utenti devono semplicemente spostare la selezione sull’area da visualizzare.

Quando calcolate l’utilizzo di larghezza di banda totale per questo visualizzatore, tenete presente che nel visualizzatore vengono caricate sia l’immagine principale che l’immagine a comparsa. Le dimensioni dell’immagine a comparsa dipendono da quelle dell’immagine principale (larghezza e altezza dell’area di visualizzazione) e dal fattore di zoom. Per impedire che le dimensioni del file dell’immagine a comparsa diventino eccessive, bilanciate questi due valori: se le dimensioni dell’immagine principale sono grandi, riducete il fattore di zoom. I valori Larghezza a comparsa e Altezza comparsa determinano le dimensioni della finestra a comparsa ma non dell’immagine a comparsa caricata nel visualizzatore.

Ad esempio, se le dimensioni dell’immagine principale sono 350 x 350 pixel, con un fattore di zoom pari a 3 l’immagine a comparsa risultante sarà di 1050 x 1050 pixel. Se le dimensioni dell’immagine principale sono 300 x 300 pixel, con un fattore di zoom pari a 4 l’immagine a comparsa risultante sarà di 1200 x 1200 pixel. In base alla qualità JPEG impostata (impostazioni consigliate: 80-90), potete ridurre sensibilmente le dimensioni del file. I fattori di zoom consigliati sono i valori compresi tra 2,5 e 4, a seconda delle dimensioni dell’immagine principale.

Adobe Dynamic Media Classic consiglia i seguenti parametri per i predefiniti visualizzatore zoom a comparsa:

* **Dimensioni immagine ingrandite** - circa 1500 x 1500 pixel, senza superare i 2000 x 2000 pixel.

* **Dimensioni immagine** - 100 KB o meno, non superare i 150 KB (comprimere il file per mantenerlo sotto i 150 KB).

* **Visualizzatore zoom: personalizzato** - Zoom guidato o non guidato con immagini, set di immagini con più viste o set di campioni colore.

## Creare e modificare i predefiniti visualizzatore zoom {#creating-and-editing-zoom-viewer-presets}

1. Sulla barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Effettuate una delle seguenti operazioni:

   * **Creare un predefinito** - Seleziona **[!UICONTROL Aggiungi]**. Nella finestra di dialogo Aggiungi predefinito visualizzatore, scegli una piattaforma, scegli un Visualizzatore zoom, quindi seleziona **[!UICONTROL Aggiungi]**. Immettete un nome per il predefinito nella casella Nome predefinito.

   * **Modificare un predefinito** - Selezionate un predefinito visualizzatore zoom, quindi selezionate **[!UICONTROL Modifica]**.

1. Specificate le impostazioni desiderate.

   Per visualizzare una descrizione di un&#39;opzione, selezionare **[!UICONTROL Suggerimento]** accanto all’opzione.

   Nella pagina Anteprima viene visualizzato il visualizzatore durante l&#39;aggiornamento e la modifica delle impostazioni.

1. Seleziona **[!UICONTROL Salva]** o **[!UICONTROL Salva con nome]**.
1. Nella pagina Predefiniti visualizzatore esaminare il predefinito visualizzatore zoom o il predefinito visualizzatore zoom guidato creato. Se è necessario apportare modifiche, selezionare **[!UICONTROL Modifica]**, modificare le impostazioni nella pagina Configura visualizzatore e quindi selezionare **[!UICONTROL Salva]**.

Per informazioni sulla gestione dei predefiniti per visualizzatore nella schermata Predefiniti visualizzatore, consultate [Predefiniti per visualizzatore](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Creare e modificare i predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets)
