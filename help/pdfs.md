---
title: Utilizzo dei file PDF
seo-title: Utilizzo dei file PDF
description: 'null'
seo-description: Scopri come lavorare con i PDF in Dynamic Media Classic.
uuid: 26 d 70 d 28-9393-49 b 1-9051-d 70456 deca 67
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 5 a 073 de 3-6 b 1 d -4 c 3 e -8 c 03-9182 f 9 f 3874 a
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Utilizzo dei file PDF{#working-with-pdfs}

I file PDF (Portable Document Format) vengono usati più spesso in Dynamic Media Classic per creare ecatalog. Quando caricate un file PDF, per impostazione predefinita Dynamic Media Classic rasterizza o estrae le pagine in modo che le pagine possano essere usate per la creazione di contenuti multimediali.

## Opzioni di caricamento PDF {#pdf-upload-options}

Quando caricate un file PDF potete formattarlo in vari modi. Potete ritagliare pagine, estrarre parole di ricerca, immettere un valore di risoluzione in ppi e scegliere uno spazio colore. I file PDF contengono spesso un margine di rifilo, indicatori di taglio, crocini di registro e altri indicatori di stampa. Durante il caricamento di un file PDF potete ritagliare tali indicatori dai lati delle pagine.

Le opzioni per caricare i file PDF si trovano nella sezione Opzioni PDF della schermata Carica.

**Elaborazione**

Le opzioni di elaborazione sono le seguenti:

**Rasterizza** (Predefinito) Estrae le pagine del file PDF e converte la grafica vettoriale in immagini bitmap. Scegliete questa opzione per creare un eCatalog. 

**Estrai parole ricerca** Estrae le parole dal file PDF per consentire la ricerca del file per parola chiave in un visualizzatore di ecatalog.

**Estrai collegamenti** Estrae i collegamenti dai file PDF e li converte in mappe immagine utilizzate in un visualizzatore di ecatalog.

**Genera automaticamente ecatalog con più** pagine PDF crea automaticamente un ecatalog dal file PDF. All’eCatalog viene assegnato un nome in base al file PDF caricato. Questa opzione è disponibile solo se il file PDF viene rasterizzato al momento del caricamento.

**Risoluzione**

Specifica l’impostazione della risoluzione. Questa impostazione determina la quantità di pixel visualizzati per pollice nel file PDF. Il valore predefinito è 150.

**Spazio colore**

Dal menu Spazio colore scegliete uno spazio colore per il file PDF. La maggior parte dei file PDF contiene immagini a colori sia in RGB che in CMYK. Per la visualizzazione online è preferibile lo spazio colore RGB.

**Rileva automaticamente** lo spazio colore del file PDF.

**Forza come RGB** Effettua la conversione nello spazio colore RGB.

**Forza come CMYK** Effettua la conversione nello spazio colore CMYK.

**Forza come Scala di grigio** effettua la conversione nello spazio colore Scala di grigio.

**Profilo colore**

Scegliete un’opzione Profilo colore:

**Converti in srgb** converte in srgb (Standard Rosso Verde Blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

**Mantieni spazio colore originale** conserva lo spazio colore originale.

**Personale Da &gt; Ad** aprire i menu per scegliere uno spazio colore Conversione da e Converti in. Potete scegliere uno spazio colore standard di Photoshop o uno caricato in SPS. 

Consultate [Profili ICC](icc-profiles.md#icc_profiles).

## Ritaglio dello spazio bianco da un file PDF {#cropping-white-space-from-a-pdf-file}

1. Per ritagliare automaticamente i pixel dello spazio bianco da un file PDF mentre lo caricate, selezionate il menu Ritaglio e scegliete Rifila.
1. Specificate le seguenti opzioni:

   **Rifila in base alla** scelta Se ritagliare in base al colore o alla trasparenza:

   **Colore** Scegliete l'opzione Colore. Dal menu Angolo scegliete quindi l’angolo del PDF con il colore che rappresenta meglio quello dello spazio bianco da ritagliare.

   **Trasparenza** Scegliete l'opzione Trasparenza.

   **Tolleranza** Consente di trascinare il cursore per specificare un valore di tolleranza da 0 a 1.

   **Per ritaglio in base al colore** , l'impostazione 0 ritaglia i pixel solo se corrispondono esattamente al colore selezionato nell'angolo del PDF. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

   **Ritaglio basato sulla trasparenza** Specificate 0 per ritagliare i pixel solo se sono completamente trasparenti; numeri più vicini a 1 consentono una minore trasparenza.

## Ritaglio dai lati delle pagine PDF {#cropping-from-the-sides-of-pdf-pages}

Potete rimuovere manualmente gli indicatori di stampa dai lati delle pagine di un file PDF mentre lo caricate.

1. Dal menu Ritaglio scegliete Manuale.
1. Immettete le impostazioni per i pixel nelle caselle di testo In alto, A destra, In basso e A sinistra per ritagliare dal corrispondente bordo delle pagine.

La quantità di pagina che viene ritagliata dipende dall’impostazione della risoluzione in pixel per pollice immessa per il file PDF. Ad esempio, se immettete 150 (impostazione predefinita) per la risoluzione in pixel per pollice e ritagliate 75 pixel dai lati delle pagine, viene ritagliato mezzo pollice poiché a una risoluzione di 150 ppi, 75 pixel corrisponde a mezzo pollice.
