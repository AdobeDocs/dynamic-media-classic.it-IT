---
title: Utilizzare i PDF
description: Scopri come utilizzare i PDF in Adobe Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 36%

---

# Utilizzare i PDF{#working-with-pdfs}

I file PDF (Portable Document Format) vengono utilizzati più spesso in Adobe Dynamic Media Classic per creare eCatalog. Quando carichi un file PDF, Adobe Dynamic Media Classic rasterizza o copia le pagine per impostazione predefinita, in modo che possano essere utilizzate per creare contenuti multimediali complessi.

Quando carichi un PDF per l’estrazione della pagina, Adobe applica il seguente limite:

| Tipo di limite | Limite imposto | Modifica del limite il 31 dicembre 2022 |
| --- | --- | --- |
| Numero massimo di pagine per un PDF da considerare per l’estrazione | 5000 (per nuovi caricamenti) | 100 (per tutti i PDF) |

Vedi anche [Limiti Dynamic Media](/help/limitations.md).

## Opzioni di caricamento PDF {#pdf-upload-options}

Quando caricate un file PDF potete formattarlo in vari modi. Potete ritagliare pagine, estrarre parole di ricerca, immettere un valore di risoluzione in ppi e scegliere uno spazio colore. I file PDF contengono spesso un margine di rifilo, indicatori di taglio, crocini di registro e altri indicatori di stampa. Durante il caricamento di un file PDF potete ritagliare tali indicatori dai lati delle pagine.

Le opzioni per il caricamento dei file di PDF si trovano nella pagina Carica in Opzioni di PDF.

### Opzioni di elaborazione

**[!UICONTROL Rasterizza]** - (Impostazione predefinita) Esegue l’striping delle pagine nel file PDF e converte la grafica vettoriale in immagini bitmap. Per creare un eCatalog, scegli questa opzione.

**[!UICONTROL Estrai parole di ricerca]** - Estrae le parole dal file PDF in modo che la ricerca nel file possa essere eseguita per parola chiave in un visualizzatore di eCatalog.

**[!UICONTROL Estrai collegamenti]** - Estrae i collegamenti dai file PDF e li converte in mappe immagine utilizzate in un visualizzatore di eCatalog.

**[!UICONTROL Genera automaticamente eCatalog con PDF multipagina]** - Crea automaticamente un eCatalog dal file PDF. All’eCatalog viene assegnato un nome in base al file PDF caricato. Questa opzione è disponibile solo se il file PDF viene rasterizzato al momento del caricamento.

### Risoluzione

Specifica l’impostazione della risoluzione. Questa impostazione determina la quantità di pixel visualizzati per pollice nel file PDF. Il valore predefinito è 150.

### Spazio colore di nitidezza

Dal menu Spazio colore scegliete uno spazio colore per il file PDF. La maggior parte dei file PDF contiene immagini a colori sia in RGB che in CMYK. Per la visualizzazione online è preferibile lo spazio colore RGB.

* **[!UICONTROL Rileva automaticamente]** - Mantiene lo spazio colore del file PDF.

* **[!UICONTROL Forza come RGB]** - Si converte nello spazio colore RGB.

* **[!UICONTROL Forza come CMYK]** - Si converte nello spazio colore CMYK.

* **[!UICONTROL Forza come scala di grigi]** - Converte lo spazio colore in scala di grigi.

### Opzioni del profilo colore

* **[!UICONTROL Converti in sRGB]** - Converte in sRGB (Standard Rosso Verde Blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

* **[!UICONTROL Mantieni spazio colore originale]** - Mantiene lo spazio colore originale.

* **[!UICONTROL Personalizzato da]** > **[!UICONTROL A]** - Apre i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore Photoshop standard o uno spazio colore caricato su Adobe Dynamic Media Classic.

Consultate anche [Profili ICC](/help/icc-profiles.md#icc_profiles).

## Ritaglio dello spazio bianco da un file PDF {#cropping-white-space-from-a-pdf-file}

1. Per ritagliare automaticamente i pixel dello spazio bianco da un file PDF mentre lo caricate, selezionate il menu Ritaglio e scegliete Rifila.
1. Specificate le seguenti opzioni:

   * **[!UICONTROL Rifila in base a]** - Scegli se ritagliare in base al colore o alla trasparenza:

      * **[!UICONTROL Colore]** - Scegliere l&#39;opzione Colore. Quindi seleziona la **[!UICONTROL Angolo]** scegliere l’angolo del PDF con il colore che rappresenta meglio lo spazio bianco da ritagliare.

      * **[!UICONTROL Trasparenza]** - Scegliere l&#39;opzione Trasparenza.
   * **[!UICONTROL Tolleranza]** - Trascinare il cursore per specificare una tolleranza da 0 a 1.

   * **[!UICONTROL Rifilatura in base al colore]** - Specificare 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell&#39;angolo del PDF. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

   * **[!UICONTROL Rifilatura basata sulla trasparenza]** - Specificare 0 per ritagliare i pixel solo se sono trasparenti; numeri più vicini a 1 assicurano una maggiore trasparenza.


## Ritaglio dai lati delle pagine di PDF {#cropping-from-the-sides-of-pdf-pages}

Potete rimuovere manualmente gli indicatori di stampa dai lati delle pagine di un file PDF mentre lo caricate.

1. Dal menu Ritaglio, selezionate **[!UICONTROL Manuale]**.
1. Immettete le impostazioni per i pixel nelle caselle di testo In alto, A destra, In basso e A sinistra per ritagliare dal corrispondente bordo delle pagine.

La quantità di pagina che viene ritagliata dipende dall’impostazione della risoluzione in pixel per pollice immessa per il file PDF. Ad esempio, supponiamo che immetti 150 (impostazione predefinita) come impostazione Risoluzione PX/Inch. Quindi ritagliate 75 pixel dai lati delle pagine. In tal caso, 0,5 pollici. è ritagliato. A 150 pixel per pollice, 75 pixel equivale a mezzo pollice.
