---
title: 'Uso dei file PSD '
description: Scopri come lavorare con i file PSD.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 63%

---


# Uso dei file PSD {#working-with-psd-files}

I file PSD (Photoshop Document Files) sono utilizzati più spesso in Dynamic Media Classic per creare i modelli. Quando carichi un file PSD, puoi creare automaticamente un modello Dynamic Media Classic dal file (seleziona l’opzione Crea modello nella schermata Carica ).

Dynamic Media Classic crea più immagini da un file PSD con livelli, se utilizzate il file per creare un modello; crea un&#39;immagine per ogni livello.

## Opzioni di caricamento PSD {#psd-upload-options}

Le opzioni per caricare file PSD si trovano nella sezione Opzioni Photoshop, in Opzioni processo di caricamento. Potete ritagliare un file, scegliere un profilo colore, usare il file per creare un modello e selezionare un ancoraggio.

Quando si carica un file PSD sono disponibili le seguenti opzioni:

**Ritaglio**  (in Opzioni di ritaglio). Scegliete Rifila per ritagliare automaticamente lo spazio bianco dai bordi di un file PSD; scegliete Manuale per ritagliare dai lati del file PSD:

**** TrimSelezionate il menu Rifila in base a e scegliete Colore o Trasparenza.

Se scegliete l’opzione Colore, dal menu Angolo scegliete l’angolo del file PSD con il colore che rappresenta meglio quello dello spazio bianco da ritagliare.

Trascinate il cursore per specificare un valore di tolleranza da 0 a 1.

Per rifilare in base al colore, l’impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell’angolo del file PSD. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

Per rifilare in base alla trasparenza, l’impostazione 0 ritaglia i pixel solo se sono completamente trasparenti. Con valori più vicini a 1 viene invece tollerata una minore trasparenza. 

**** ManualeImmettere il numero di pixel da ritagliare da qualsiasi lato o lato dell&#39;immagine. La quantità di immagine che viene ritagliata dipende dall’impostazione ppi (pixel per pollice) nel file immagine. Ad esempio, se l’immagine viene visualizzata a 150 ppi e immettete 75 nelle caselle di testo, viene ritagliato mezzo pollice da ogni lato dell’immagine.

**Profilo colore**  (in Opzioni profilo colore). Scegliete un’opzione:

**Converti in sRGB (impostazione predefinita)** Converte in sRGB (Standard Rosso Verde Blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

**Mantieni** spazio colore originaleConserva lo spazio colore originale dell&#39;immagine.

**Personalizzato da >** A aperture menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore Photoshop standard o uno spazio colore caricato in Dynamic Media Classic. Consultate Profili ICC.

**Gestisci** livelliRacchiude i livelli della PSD, se presenti, in singole risorse. I livelli delle risorse restano associati al file PSD. Per visualizzarli, aprite il file PSD in visualizzazione Dettagli e selezionate il pannello dei livelli. Consultate Visualizzazione e modifica dei livelli in un file PSD.

**Crea** modelloCrea un modello dai livelli nel file PSD.

**Extract** TextEstrae il testo in modo che gli utenti possano cercare testo in un Visualizzatore.

**Estendi i livelli alle** dimensioni dello sfondoEstende le dimensioni dei livelli immagine ritagliati alle dimensioni del livello di sfondo.

**I livelli** NamingLayers nel file PSD vengono caricati come immagini separate. Scegli un’opzione per denominare queste immagini in Dynamic Media Classic:

**Livello** NomeDenomina le immagini dopo i loro nomi di livello nel file PSD. Ad esempio, un livello denominato Price Tag nel file PSD originale diventa un’immagine denominata Price Tag. Se però i nomi dei livelli del file PSD sono nomi di livello predefiniti di Photoshop (Sfondo, Livello 1, Livello 2 e così via), le immagini vengono denominate in base al numero del rispettivo livello nel file PSD e non in base al nome predefinito del livello.

**Photoshop e Layer** NumberAssegna un nome alle immagini dopo i numeri dei livelli nel file PSD, ignorando i nomi dei livelli originali. Le immagini vengono denominate con il nome file di Photoshop a cui viene aggiunto un numero di livello. Ad esempio, il secondo livello di un file con nome Spring Ad.psd viene denominato Spring Ad_2 anche se in Photoshop tale livello aveva un nome personalizzato.

**Photoshop e** Nome livelloDenomina le immagini dopo il file PSD seguito dal nome del livello o dal numero del livello. Il numero del livello viene usato se il livello nel file PSD ha un nome predefinito di Photoshop. Ad esempio, al livello denominato Price Tag in un file PSD chiamato SpringAd viene assegnato il nome Spring Ad_Price Tag. Al livello con il nome predefinito Layer 2 viene assegnato il nome Spring Ad_2.

**** AncoraggioConsente di specificare il modo in cui le immagini vengono ancorate nei modelli generati dalla composizione a livelli prodotta dal file PSD. Per impostazione predefinita, la posizione di ancoraggio è al centro. L’ancoraggio centrale permette alle immagini sostitutive di riempire in modo ottimale lo spazio, indipendentemente dalle loro proporzioni. In questo modo, facendo riferimento al modello e utilizzano la sostituzione mediante parametri, le immagini sostitutive con proporzioni diverse occupano lo stesso spazio in modo efficace. Usate un’impostazione diversa se la vostra applicazione richiede che le immagini sostitutive riempiano lo spazio allocato nel modello.

## Visualizzazione e modifica dei livelli in un file PSD  {#viewing-and-editing-layers-in-a-psd-file}

Se hai selezionato l’opzione Mantieni livelli al momento del caricamento del file PSD, Dynamic Media Classic ha suddiviso i singoli livelli in risorse. Per visualizzare e modificare i livelli delle risorse appartenenti al file PSD, aprite il file nel pannello Sfoglia in visualizzazione Dettagli.

1. Fate doppio clic sul file PSD completo nel pannello Sfoglia per aprirlo in visualizzazione Dettagli.

   ***nota **: Assicurati di aprire l’intera risorsa e non uno dei livelli PSD.*

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

