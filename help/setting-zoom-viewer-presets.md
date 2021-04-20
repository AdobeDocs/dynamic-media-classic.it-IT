---
title: Impostazione di predefiniti per visualizzatori zoom
description: Scopri come impostare i predefiniti per visualizzatori zoom.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Classic,Viewers,Zoom
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 68%

---


# Impostazione di predefiniti per visualizzatori zoom{#setting-up-zoom-viewer-presets}

I predefiniti per visualizzatori zoom determinano lo stile, il comportamento e l’aspetto dei visualizzatori zoom. Dynamic Media Classic offre diverse opzioni per personalizzare e skin dei visualizzatori. Dynamic Media Classic viene fornito con predefiniti per visualizzatori zoom di base (veloci), a comparsa e personalizzati. Gli amministratori possono creare nuovi predefiniti per visualizzatori zoom della società o modificare un predefinito per visualizzatori preimpostato e salvarlo con un nuovo nome.

Tutti i visualizzatori zoom includono pulsanti per applicare lo zoom in avanti, indietro, la panoramica e per ripristinare le stato originale dell’immagine dopo lo zoom. L’aspetto di questi pulsanti e della finestra dipende dalle selezioni effettuate nei predefiniti per visualizzatori zoom. Potete configurare un predefinito per visualizzatori zoom con diverse impostazioni di colori, bordi, font e immagine. Quando configurate un visualizzatore zoom guidato, potete anche scegliere il percorso di salvataggio delle destinazioni di zoom. Le destinazioni di zoom sono miniature che gli utenti possono selezionare per applicare lo zoom alle aree specificate.

## I predefiniti per visualizzatori zoom {#about-zoom-viewer-presets}

In Dynamic Media Classic sono disponibili i seguenti predefiniti per visualizzatori zoom:

* **Visualizzatore zoom:**
BaseFornisce uno zoom di base sull&#39;immagine originale.

* **Visualizzatore zoom: Visualizzazione**
a comparsaVisualizza una seconda immagine dell&#39;area ingrandita accanto all&#39;immagine originale. Non vi sono controlli; gli utenti devono semplicemente spostare la selezione sull’area da visualizzare.

Quando calcolate l’utilizzo di larghezza di banda totale per questo visualizzatore, tenete presente che nel visualizzatore vengono caricate sia l’immagine principale che l’immagine a comparsa. Le dimensioni dell’immagine a comparsa dipendono da quelle dell’immagine principale (larghezza e altezza dell’area di visualizzazione) e dal fattore di zoom. Per impedire che le dimensioni del file dell’immagine a comparsa diventino eccessive, bilanciate questi due valori: se le dimensioni dell’immagine principale sono grandi, riducete il fattore di zoom. I valori Larghezza a comparsa e Altezza comparsa determinano le dimensioni della finestra a comparsa ma non dell’immagine a comparsa caricata nel visualizzatore.

Ad esempio, se le dimensioni dell’immagine principale sono 350 x 350 pixel, con un fattore di zoom pari a 3 l’immagine a comparsa risultante sarà di 1050 x 1050 pixel. Se le dimensioni dell’immagine principale sono 300 x 300 pixel, con un fattore di zoom pari a 4 l’immagine a comparsa risultante sarà di 1200 x 1200 pixel. In base alla qualità JPEG impostata (impostazioni consigliate: 80-90), potete ridurre sensibilmente le dimensioni del file. I fattori di zoom consigliati sono i valori compresi tra 2,5 e 4, a seconda delle dimensioni dell’immagine principale.

Dynamic Media Classic consiglia questi parametri per i predefiniti visualizzatore zoom a comparsa:

* **Dimensione**
dell&#39;immagine ingranditaCirca 1500 x 1500 pixel, non superiore a 2000 x 2000 pixel.

* **Dimensione dell&#39;immagine**
100 KB o inferiore, non superiore a 150 KB (comprimere il file per mantenerlo sotto i 150 KB).

* **Visualizzatore zoom:**
PersonalizzatoFornisce lo zoom guidato o non guidato con immagini, set di immagini con più viste o set di campioni di colore.

## Creazione e modifica dei predefiniti per visualizzatori zoom {#creating-and-editing-zoom-viewer-presets}

Per creare o modificare un predefinito per visualizzatori zoom, effettuate le seguite operazioni:

1. Fate clic su **Configurazione** > **Predefiniti visualizzatore**.
1. Effettuate una delle seguenti operazioni:

   * **Creazione di un**
predefinitoFai clic su Aggiungi. Nella finestra di dialogo Aggiungi predefinito visualizzatore scegliere una piattaforma, scegliere un visualizzatore zoom e quindi fare clic su Aggiungi. Immetti un nome per il predefinito nella casella Nome predefinito .

   * **Modifica di un**
predefinitoSeleziona un predefinito per visualizzatori zoom, quindi fai clic su 
**Modifica**.

1. Specificate le impostazioni desiderate.

   Per visualizzare la descrizione di un’opzione, fate clic sull’icona Suggerimento  accanto all’opzione.

   Nella schermata di anteprima viene riportato il visualizzatore con le impostazioni aggiornate e modificate.

1. Fate clic su **Salva** o **Salva con nome**.
1. Nella schermata Predefiniti visualizzatore, esaminate il predefinito per visualizzatori zoom o il predefinito per visualizzatori zoom guidato creato. Se è necessario eseguire le regolazioni, fare clic su **Modifica**, modificare le impostazioni nella schermata Configura visualizzatore e fare clic su **Salva**.

Per informazioni sulla gestione dei predefiniti per visualizzatore nella schermata Predefiniti visualizzatore, consultate [Predefiniti per visualizzatore](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Creazione e modifica dei predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets)

