---
title: Impostazione di predefiniti per visualizzatori zoom
seo-title: Impostazione di predefiniti per visualizzatori zoom
description: 'null'
seo-description: Scoprite come impostare i predefiniti per visualizzatori zoom.
uuid: 202 d 80 cb -8282-45 d 4-89 e 8-942 c 8677 aa 93
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/zoom
discoiquuid: 5023 a 933-e 229-4 d 3 c -8 e 91-3 ac 5 e 9 f 4970 b
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Impostazione di predefiniti per visualizzatori zoom{#setting-up-zoom-viewer-presets}

I predefiniti per visualizzatori zoom determinano lo stile, il comportamento e l’aspetto dei visualizzatori zoom. Dynamic Media Classic offre diverse opzioni per personalizzare e inserire in interfacce i visualizzatori. Dynamic Media Classic viene fornito con predefiniti per visualizzatori zoom di base (veloce), a comparsa e personalizzati. Gli amministratori possono creare nuovi predefiniti per visualizzatori zoom della società o modificare un predefinito per visualizzatori preimpostato e salvarlo con un nuovo nome.

Tutti i visualizzatori zoom includono pulsanti per applicare lo zoom in avanti, indietro, la panoramica e per ripristinare le stato originale dell’immagine dopo lo zoom. L’aspetto di questi pulsanti e della finestra dipende dalle selezioni effettuate nei predefiniti per visualizzatori zoom. Potete configurare un predefinito per visualizzatori zoom con diverse impostazioni di colori, bordi, font e immagine. Quando configurate un visualizzatore zoom guidato, potete anche scegliere il percorso di salvataggio delle destinazioni di zoom. Le destinazioni di zoom sono miniature che gli utenti possono selezionare per applicare lo zoom alle aree specificate.

## I predefiniti per visualizzatori zoom {#about-zoom-viewer-presets}

In Media Classic sono disponibili i seguenti predefiniti per visualizzatori zoom:

**Visualizzatore zoom: Base** Fornisce uno zoom di base sull'immagine originale.

**Visualizzatore zoom: A comparsa** Consente di visualizzare una seconda immagine dell'area ingrandita accanto all'immagine originale. Non vi sono controlli; gli utenti devono semplicemente spostare la selezione sull’area da visualizzare.

Quando calcolate l’utilizzo di larghezza di banda totale per questo visualizzatore, tenete presente che nel visualizzatore vengono caricate sia l’immagine principale che l’immagine a comparsa. Le dimensioni dell’immagine a comparsa dipendono da quelle dell’immagine principale (larghezza e altezza dell’area di visualizzazione) e dal fattore di zoom. Per impedire che le dimensioni del file dell’immagine a comparsa diventino eccessive, bilanciate questi due valori: se le dimensioni dell’immagine principale sono grandi, riducete il fattore di zoom. I valori Larghezza a comparsa e Altezza comparsa determinano le dimensioni della finestra a comparsa ma non dell’immagine a comparsa caricata nel visualizzatore.

Ad esempio, se le dimensioni dell’immagine principale sono 350 x 350 pixel, con un fattore di zoom pari a 3 l’immagine a comparsa risultante sarà di 1050 x 1050 pixel. Se le dimensioni dell’immagine principale sono 300 x 300 pixel, con un fattore di zoom pari a 4 l’immagine a comparsa risultante sarà di 1200 x 1200 pixel. In base alla qualità JPEG impostata (impostazioni consigliate: 80-90), potete ridurre sensibilmente le dimensioni del file. I fattori di zoom consigliati sono i valori compresi tra 2,5 e 4, a seconda delle dimensioni dell’immagine principale.

Dynamic Media Classic consiglia questi parametri per i predefiniti per visualizzatori zoom a comparsa:

**Dimensioni** immagini ingrandite circa 1500 x 1500 pixel, non più di 2000 x 2000 pixel.

**Dimensione** immagine pari a 100 KB o inferiore, non superiore a 150 KB (comprimere il file per mantenerlo sotto 150 KB).

**Visualizzatore zoom: Personalizzato** Consente di effettuare zoom guidati o non guidati con immagini, set di immagini con visualizzazioni multiple o set di campioni colore.

## Creazione e modifica dei predefiniti per visualizzatori zoom {#creating-and-editing-zoom-viewer-presets}

Per creare o modificare un predefinito per visualizzatori zoom, effettuate le seguite operazioni:

1. Fate clic su **Configurazione** &gt; **Predefiniti visualizzatore**.
1. Effettuate una delle seguenti operazioni:

   **Creazione di un predefinito** Fate clic su Aggiungi. Nella finestra di dialogo Aggiungi predefinito per visualizzatore, scegliete una piattaforma, selezionate un visualizzatore zoom e fate clic su Aggiungi. Immettete un nome per il predefinito nella casella Nome predefinito.

   **Modifica di un predefinito** Selezionate un predefinito per visualizzatori zoom, quindi fate clic **su Modifica**.

1. Specificate le impostazioni desiderate.

   Per visualizzare la descrizione di un’opzione, fate clic sull’icona Suggerimento  accanto all’opzione.

   Nella schermata di anteprima viene riportato il visualizzatore con le impostazioni aggiornate e modificate.

1. Fate clic su **Salva** o **Salva con nome**.
1. Nella schermata Predefiniti visualizzatore, esaminate il predefinito per visualizzatori zoom o il predefinito per visualizzatori zoom guidato creato. If it needs adjusting, click **Edit**, change settings on the Configure Viewer screen, and click **Save**.

Per informazioni sulla gestione dei predefiniti per visualizzatore nella schermata Predefiniti visualizzatore, consultate [Predefiniti per visualizzatore](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Creazione e modifica dei predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets)

