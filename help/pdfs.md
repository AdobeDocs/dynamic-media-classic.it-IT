---
title: Utilizzo dei file PDF
seo-title: Utilizzo dei file PDF
description: 'null'
seo-description: Scoprite come utilizzare i PDF in Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 56%

---


# Utilizzo dei file PDF{#working-with-pdfs}

I file PDF (Portable Document Format) vengono utilizzati più spesso in Dynamic Media Classic per creare eCatalog. Quando caricate un file PDF, per impostazione predefinita le pagine vengono rasterizzate (ossia ne vengono estratti i dati) da Dynamic Media Classic in modo che possano essere utilizzate per la creazione di contenuti multimediali.

## Opzioni di caricamento PDF {#pdf-upload-options}

Quando caricate un file PDF potete formattarlo in vari modi. Potete ritagliare pagine, estrarre parole di ricerca, immettere un valore di risoluzione in ppi e scegliere uno spazio colore. I file PDF contengono spesso un margine di rifilo, indicatori di taglio, crocini di registro e altri indicatori di stampa. Durante il caricamento di un file PDF potete ritagliare tali indicatori dai lati delle pagine.

Le opzioni per caricare i file PDF si trovano nella sezione Opzioni PDF della schermata Carica.

**Elaborazione**

Le opzioni di elaborazione sono le seguenti:

**Rasterizza** (impostazione predefinita) Rimuove l’ordine delle pagine nel file PDF e converte la grafica vettoriale in immagini bitmap. Scegliete questa opzione per creare un eCatalog. 

**Estrai termini** di ricerca Estrai le parole dal file PDF in modo che sia possibile effettuare ricerche nel file mediante parole chiave in un visualizzatore di eCatalog.

**Estrai collegamenti** Estrae i collegamenti dai file PDF e li converte in mappe immagine utilizzate in un visualizzatore di eCatalog.

**Genera automaticamente eCatalog con PDF** con più pagine Crea automaticamente un eCatalog dal file PDF. All’eCatalog viene assegnato un nome in base al file PDF caricato. Questa opzione è disponibile solo se il file PDF viene rasterizzato al momento del caricamento.

**Risoluzione**

Specifica l’impostazione della risoluzione. Questa impostazione determina la quantità di pixel visualizzati per pollice nel file PDF. Il valore predefinito è 150.

**Spazio colore**

Dal menu Spazio colore scegliete uno spazio colore per il file PDF. La maggior parte dei file PDF contiene immagini a colori sia in RGB che in CMYK. Per la visualizzazione online è preferibile lo spazio colore RGB.

**Rileva automaticamente** Conserva lo spazio colore del file PDF.

**Forza come RGB** Converte nello spazio colore RGB.

**Forza come CMYK** Converte nello spazio colore CMYK.

**Forza come scala di grigio** Consente di convertire nello spazio colore Scala di grigio.

**Profilo colore**

Scegliete un’opzione Profilo colore:

**Converti in sRGB** Converte in sRGB (Standard Rosso Verde Blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

**Mantieni spazio** colore originale Conserva lo spazio colore originale.

**Personalizzato da > Per** aprire i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Potete scegliere uno spazio colore Photoshop standard o uno spazio colore caricato in Dynamic Media Classic.

Consultate [Profili ICC](icc-profiles.md#icc_profiles).

## Ritaglio dello spazio bianco da un file PDF {#cropping-white-space-from-a-pdf-file}

1. Per ritagliare automaticamente i pixel dello spazio bianco da un file PDF mentre lo caricate, selezionate il menu Ritaglio e scegliete Rifila.
1. Specificate le seguenti opzioni:

   **RifilaBasato su** Consente di scegliere se ritagliare in base al colore o alla trasparenza:

   **Colore** Scegliete l’opzione Colore. Dal menu Angolo scegliete quindi l’angolo del PDF con il colore che rappresenta meglio quello dello spazio bianco da ritagliare.

   **Trasparenza** Scegliere l&#39;opzione Trasparenza.

   **Tolleranza** Trascinate il cursore per specificare una tolleranza da 0 a 1:

   **Ritaglio in base al colore** Specificate 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell’angolo del PDF. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

   **Ritaglio in base alla trasparenza** Specificate 0 per ritagliare i pixel solo se sono completamente trasparenti; Con valori più vicini a 1 viene invece tollerata una minore trasparenza.

## Ritaglio dai lati delle pagine PDF {#cropping-from-the-sides-of-pdf-pages}

Potete rimuovere manualmente gli indicatori di stampa dai lati delle pagine di un file PDF mentre lo caricate.

1. Dal menu Ritaglio scegliete Manuale.
1. Immettete le impostazioni per i pixel nelle caselle di testo In alto, A destra, In basso e A sinistra per ritagliare dal corrispondente bordo delle pagine.

La quantità di pagina che viene ritagliata dipende dall’impostazione della risoluzione in pixel per pollice immessa per il file PDF. Ad esempio, se immettete 150 (impostazione predefinita) per la risoluzione in pixel per pollice e ritagliate 75 pixel dai lati delle pagine, viene ritagliato mezzo pollice poiché a una risoluzione di 150 ppi, 75 pixel corrisponde a mezzo pollice.
