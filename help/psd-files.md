---
title: Operazioni con i file PSD
seo-title: Operazioni con i file PSD
description: 'null'
seo-description: Scoprite come lavorare con file PSD.
uuid: 5836 b 660-6 bca -46 e 7-ab 39-1 a 31 d 1 e 0 cff 2
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 4086 e 3 db -5 aca -41 a 0-8 f 15-302 afbf 67 ddb
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Operazioni con i file PSD{#working-with-psd-files}

I file PSD (file di documenti Photoshop) vengono utilizzati più spesso in Media Classic per creare modelli. Quando caricate un file PSD, potete creare automaticamente un modello Dynamic Media Classic dal file (selezionate l'opzione Crea modello nella schermata Carica).

Se create un modello con un file PSD contenente dei livelli, SPS crea più immagini dal file, un’immagine per ogni livello.

## Opzioni di caricamento PSD {#psd-upload-options}

Le opzioni per caricare file PSD si trovano nella sezione Opzioni Photoshop, in Opzioni processo di caricamento. Potete ritagliare un file, scegliere un profilo colore, usare il file per creare un modello e selezionare un ancoraggio.

Quando si carica un file PSD sono disponibili le seguenti opzioni:

**Ritaglia** (si trova in Opzioni di ritaglio). Scegliete Rifila per ritagliare automaticamente lo spazio bianco dai bordi di un file PSD; scegliete Manuale per ritagliare dai lati del file PSD:

**Rifila** Selezionate il menu Rifila in base a e scegliete Colore o Trasparenza.

Se scegliete l’opzione Colore, dal menu Angolo scegliete l’angolo del file PSD con il colore che rappresenta meglio quello dello spazio bianco da ritagliare.

Trascinate il cursore per specificare un valore di tolleranza da 0 a 1.

Per rifilare in base al colore, l’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo del file PSD. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

Per rifilare in base alla trasparenza, l’impostazione 0 ritaglia i pixel solo se sono completamente trasparenti. Con valori più vicini a 1 viene invece tollerata una minore trasparenza. 

**Manuale** Consente di inserire il numero di pixel da ritagliare da ogni lato o da uno dei lati dell'immagine. La quantità di immagine che viene ritagliata dipende dall’impostazione ppi (pixel per pollice) nel file immagine. Ad esempio, se l’immagine viene visualizzata a 150 ppi e immettete 75 nelle caselle di testo, viene ritagliato mezzo pollice da ogni lato dell’immagine.

**Profilo colore** (nella sezione Opzioni profilo colore) Scegliete un’opzione:

**Converti in srgb (predefinito)** Effettua la conversione in srgb (Standard Rosso Verde Blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

**Mantieni spazio colore originale** Conserva lo spazio colore originale dell'immagine.

**Personale Da &gt; Ad** aprire i menu per scegliere uno spazio colore Conversione da e Converti in. Potete scegliere uno spazio colore standard di Photoshop o uno caricato in SPS. Consultate Profili ICC.

**Mantieni livelli** Consente di estrarre i livelli del file PSD in singole risorse. I livelli delle risorse restano associati al file PSD. Per visualizzarli, aprite il file PSD in visualizzazione Dettagli e selezionate il pannello dei livelli. Consultate Visualizzazione e modifica dei livelli in un file PSD.

**Crea modello** Crea un modello dai livelli del file PSD.

**Estrai testo** Estrae il testo in modo che gli utenti possano cercare il testo in un visualizzatore.

**Estendi livelli a dimensione sfondo** Estende le dimensioni dei livelli immagine estratti in base alla dimensione del livello di sfondo.

**I livelli di denominazione** dei livelli nel file PSD vengono caricati come immagini separate. Scegliete un’opzione per denominare queste immagini in Scene7 Publishing System:

**Nome livello** Le immagini vengono denominate in base ai nomi dei rispettivi livelli nel file PSD. Ad esempio, un livello denominato Price Tag nel file PSD originale diventa un’immagine denominata Price Tag. Se però i nomi dei livelli del file PSD sono nomi di livello predefiniti di Photoshop (Sfondo, Livello 1, Livello 2 e così via), le immagini vengono denominate in base al numero del rispettivo livello nel file PSD e non in base al nome predefinito del livello.

**Photoshop e Numero livello** Denomina le immagini in base ai numeri dei rispettivi livelli nel file PSD, ignorando i nomi originali dei livelli. Le immagini vengono denominate con il nome file di Photoshop a cui viene aggiunto un numero di livello. Ad esempio, il secondo livello di un file con nome Spring Ad.psd viene denominato Spring Ad_2 anche se in Photoshop tale livello aveva un nome personalizzato.

**Photoshop e Nome livello** Le immagini vengono denominate dopo il file PSD seguito dal nome del livello o dal numero del livello. Il numero del livello viene usato se il livello nel file PSD ha un nome predefinito di Photoshop. Ad esempio, al livello denominato Price Tag in un file PSD chiamato SpringAd viene assegnato il nome Spring Ad_Price Tag. Al livello con il nome predefinito Layer 2 viene assegnato il nome Spring Ad_2.

**Ancoraggio** Specificate il modo in cui le immagini sono ancorate nei modelli generati dalla composizione a livelli prodotta dal file PSD. Per impostazione predefinita, la posizione di ancoraggio è al centro. L’ancoraggio centrale permette alle immagini sostitutive di riempire in modo ottimale lo spazio, indipendentemente dalle loro proporzioni. In questo modo, facendo riferimento al modello e utilizzano la sostituzione mediante parametri, le immagini sostitutive con proporzioni diverse occupano lo stesso spazio in modo efficace. Usate un’impostazione diversa se la vostra applicazione richiede che le immagini sostitutive riempiano lo spazio allocato nel modello.

## Visualizzazione e modifica dei livelli in un file PSD {#viewing-and-editing-layers-in-a-psd-file}

se al momento di caricare il file PSD selezionate l'opzione Mantieni livelli, Dynamic Media Classic estrae i singoli livelli in risorse. Per visualizzare e modificare i livelli delle risorse appartenenti al file PSD, aprite il file nel pannello Sfoglia in visualizzazione Dettagli.

1. Fate doppio clic sul file PSD completo nel pannello Sfoglia per aprirlo in visualizzazione Dettagli.

   ***Nota**: Accertatevi di aprire la risorsa completa e non uno dei livelli PSD.*

1. Fate clic su Livelli per aprire il pannello Livelli. Nel pannello Livelli, tutti i livelli sono riportati come immagini a sé stanti.
1. Fate doppio clic su un livello per aprirlo ed effettuate una delle seguenti operazioni:

   * Fate clic sull’icona della mappa immagine per creare una mappa immagine sul livello. Consultate [Creazione di mappe immagine](creating-image-maps.md#creating_image_maps).
   * Fate clic sull’icona delle destinazioni zoom per creare le destinazioni zoom sul livello. Consultate [Creazione di destinazioni di zoom per lo zoom guidato](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).
   * Fate clic sull’icona di ritaglio per ritagliare il livello. Consultate [Ritaglio di un’immagine](cropping-image.md#cropping_an_image).
   * Fate clic su Più nitido per aggiungere nitidezza al livello. Consultate [Nitidezza di un’immagine](sharpening-image.md#sharpening_an_image).
   * Fate clic su Regola per regolare il livello. Consultate [Regolazione di un’immagine](adjusting-image.md#adjusting_an_image).

1. Fate clic su Salva o Salva con nome.
1. Per visualizzare o modificare un altro livello, fate clic su una freccia sotto all’anteprima del livello.
1. Per uscire dalla visualizzazione Dettagli del livello, fate clic sull’icona della visualizzazione Griglia.

