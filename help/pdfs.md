---
title: Utilizzo dei file PDF
description: Scopri come utilizzare i PDF in Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Gestione risorse
role: Professionista
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 55%

---


# Utilizzo dei file PDF{#working-with-pdfs}

I file PDF (Portable Document Format) vengono utilizzati più spesso in Dynamic Media Classic per creare gli eCatalog. Quando carichi un file PDF, per impostazione predefinita Dynamic Media Classic rasterizza, o copia, le pagine in modo che possano essere utilizzate per generare contenuti multimediali.

## Opzioni di caricamento PDF {#pdf-upload-options}

Quando caricate un file PDF potete formattarlo in vari modi. Potete ritagliare pagine, estrarre parole di ricerca, immettere un valore di risoluzione in ppi e scegliere uno spazio colore. I file PDF contengono spesso un margine di rifilo, indicatori di taglio, crocini di registro e altri indicatori di stampa. Durante il caricamento di un file PDF potete ritagliare tali indicatori dai lati delle pagine.

Le opzioni per caricare i file PDF si trovano nella sezione Opzioni PDF della schermata Carica.

**Elaborazione**

Le opzioni di elaborazione sono le seguenti:

**Rasterizza**  (impostazione predefinita) Rimuove le pagine dal file PDF e converte la grafica vettoriale in immagini bitmap. Scegliete questa opzione per creare un eCatalog. 

**Estrai** parole di ricercaEstrae le parole dal file PDF in modo che la ricerca nel file possa essere eseguita per parola chiave in un visualizzatore di eCatalog.

**Estrai** collegamentiEstrae i collegamenti dai file PDF e li converte in mappe immagine utilizzate in un visualizzatore di eCatalog.

**Genera automaticamente eCatalog con più pagine** PDFAcrea automaticamente un eCatalog dal file PDF. All’eCatalog viene assegnato un nome in base al file PDF caricato. Questa opzione è disponibile solo se il file PDF viene rasterizzato al momento del caricamento.

**Risoluzione**

Specifica l’impostazione della risoluzione. Questa impostazione determina la quantità di pixel visualizzati per pollice nel file PDF. Il valore predefinito è 150.

**Spazio colore**

Dal menu Spazio colore scegliete uno spazio colore per il file PDF. La maggior parte dei file PDF contiene immagini a colori sia in RGB che in CMYK. Per la visualizzazione online è preferibile lo spazio colore RGB.

**Rileva** automaticamenteConserva lo spazio colore del file PDF.

**Force As** RGBConverts nello spazio colore RGB.

**Forza come** CMYKConverts nello spazio colore CMYK.

**Forza come** scala di grigiConverte lo spazio colore in scala di grigi.

**Profilo colore**

Scegliete un’opzione Profilo colore:

**Converti in** sRGBConverts in sRGB (Standard Rosso Verde Blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

**Mantieni** spazio colore originaleConserva lo spazio colore originale.

**Personalizzato da >** A aperture menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore Photoshop standard o uno spazio colore caricato in Dynamic Media Classic.

Consultate [Profili ICC](icc-profiles.md#icc_profiles).

## Ritaglio dello spazio bianco da un file PDF  {#cropping-white-space-from-a-pdf-file}

1. Per ritagliare automaticamente i pixel dello spazio bianco da un file PDF mentre lo caricate, selezionate il menu Ritaglio e scegliete Rifila.
1. Specificate le seguenti opzioni:

   **Rifila in base** aScegli se ritagliare in base a colore o trasparenza:

   **** ColoreScegli l’opzione Colore. Dal menu Angolo scegliete quindi l’angolo del PDF con il colore che rappresenta meglio quello dello spazio bianco da ritagliare.

   **** TrasparenzaScegli l’opzione Trasparenza.

   **** TolleranzaTrascinate il cursore per specificare una tolleranza da 0 a 1:

   **Taglio in base al** coloreSpecificare 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell’angolo del PDF. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

   **Ritaglio basato sulla** trasparenzaSpecificare 0 per ritagliare i pixel solo se sono completamente trasparenti; numeri più vicini a 1 assicurano una maggiore trasparenza.

## Ritaglio dai lati delle pagine PDF {#cropping-from-the-sides-of-pdf-pages}

Potete rimuovere manualmente gli indicatori di stampa dai lati delle pagine di un file PDF mentre lo caricate.

1. Dal menu Ritaglio scegliete Manuale.
1. Immettete le impostazioni per i pixel nelle caselle di testo In alto, A destra, In basso e A sinistra per ritagliare dal corrispondente bordo delle pagine.

La quantità di pagina che viene ritagliata dipende dall’impostazione della risoluzione in pixel per pollice immessa per il file PDF. Ad esempio, se immettete 150 (impostazione predefinita) per la risoluzione in pixel per pollice e ritagliate 75 pixel dai lati delle pagine, viene ritagliato mezzo pollice poiché a una risoluzione di 150 ppi, 75 pixel corrisponde a mezzo pollice.
