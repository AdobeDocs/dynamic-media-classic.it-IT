---
title: Utilizzare i PDF
description: Scopri come utilizzare i PDF in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 25%

---

# Utilizzare i PDF{#working-with-pdfs}

I file PDF (Portable Document Format) vengono spesso utilizzati in Adobe Dynamic Media Classic per la creazione di eCatalog. Quando carichi un file PDF, Adobe Dynamic Media Classic rasterizza o rimuove le pagine per impostazione predefinita, in modo che possano essere utilizzate per creare rich media.

Quando carichi un PDF per l’estrazione della pagina, Adobe applica il seguente limite:

| Tipo di limite | Limite imposto | Modifica del limite del 31 dicembre 2022 |
| --- | --- | --- |
| Numero massimo di pagine per un PDF da considerare per l’estrazione | 5000 (per nuovi caricamenti) | 100 (per tutti i PDF) |

Vedi anche [Limitazioni di Dynamic Media](/help/using/limitations.md).

## Opzioni di caricamento PDF {#pdf-upload-options}

Quando caricate un file PDF potete formattarlo in vari modi. Potete ritagliare pagine, estrarre parole di ricerca, immettere un valore di risoluzione in ppi e scegliere uno spazio colore. I file PDF spesso contengono un margine di ritaglio, indicatori di ritaglio, indicatori di registrazione e altri indicatori della stampante. Durante il caricamento di un file PDF potete ritagliare tali indicatori dai lati delle pagine.

Le opzioni per il caricamento dei file PDF si trovano nella sezione Opzioni di PDF della pagina Carica.

### Opzioni di elaborazione

**[!UICONTROL Rasterizza]**: (impostazione predefinita) esegue il riping delle pagine nel file PDF e converte gli elementi grafici vettoriali in immagini bitmap. Per creare un eCatalog, scegliere questa opzione.

**[!UICONTROL Estrai parole di ricerca]**: estrae parole dal file PDF in modo che le parole chiave nel file possano essere cercate in un visualizzatore eCatalog.

**[!UICONTROL Estrai collegamenti]**: estrae i collegamenti dai file di PDF e li converte in mappe immagine utilizzate in un visualizzatore eCatalog.

**[!UICONTROL Generazione automatica eCatalog con PDF a più pagine]**: crea automaticamente un eCatalog dal file PDF. All’eCatalog viene assegnato un nome in base al file PDF caricato. Questa opzione è disponibile solo se il file PDF viene rasterizzato al momento del caricamento.

### Risoluzione

Specifica l’impostazione della risoluzione. Questa impostazione determina la quantità di pixel visualizzati per pollice nel file PDF. Il valore predefinito è 150.

### Opzioni spazio colore

Dal menu Spazio colore scegliete uno spazio colore per il file PDF. La maggior parte dei file PDF contiene immagini a colori sia in RGB che in CMYK. Per la visualizzazione online è preferibile lo spazio colore RGB.

* **[!UICONTROL Rileva automaticamente]**: mantiene lo spazio colore del file PDF.

* **[!UICONTROL Forza come RGB]**: viene convertito nello spazio colore di RGB.

* **[!UICONTROL Forza come CMYK]**: viene convertito nello spazio colore CMYK.

* **[!UICONTROL Forza come scala di grigio]**: converte lo spazio colore della scala di grigio.

### Opzioni profilo colore

* **[!UICONTROL Converti in sRGB]**: viene convertito in sRGB (blu rosso verde standard). sRGB è lo spazio colore consigliato per la visualizzazione di immagini in una pagina Web.

* **[!UICONTROL Mantieni spazio colore originale]**: mantiene lo spazio colore originale.

* **[!UICONTROL Personalizza da]** > **[!UICONTROL A]**: apre i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore standard di Photoshop o uno spazio colore caricato in Adobe Dynamic Media Classic.

Consultate anche [Profili ICC](/help/using/icc-profiles.md#icc_profiles).

## Ritaglia spazio vuoto da un file PDF {#cropping-white-space-from-a-pdf-file}

Puoi ritagliare automaticamente i pixel dello spazio vuoto da un file PDF durante il caricamento.

1. Selezionate il menu Ritaglia (Crop) e scegliete Rifila (Trim).
1. Specificate le seguenti opzioni:

   * **[!UICONTROL Rifila in base a]**: scegli se ritagliare in base al colore o alla trasparenza:

      * **[!UICONTROL Colore]**: scegliere l&#39;opzione Colore. Quindi seleziona il menu **[!UICONTROL Angolo]** e scegli l&#39;angolo del PDF con il colore che meglio rappresenta il colore dello spazio bianco da ritagliare.

      * **[!UICONTROL Trasparenza]**: scegliere l&#39;opzione Trasparenza.

   * **[!UICONTROL Tolleranza]**: trascinare il dispositivo di scorrimento per specificare una tolleranza da 0 a 1.

   * **[!UICONTROL Rifilatura in base al colore]**: specificare 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell&#39;angolo di PDF. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

   * **[!UICONTROL Taglio basato sulla trasparenza]**: specificare 0 per ritagliare i pixel solo se sono trasparenti; i numeri più vicini a 1 consentono una maggiore trasparenza.

## Ritaglia dai lati delle pagine PDF {#cropping-from-the-sides-of-pdf-pages}

È possibile rimuovere manualmente i contrassegni della stampante dai lati delle pagine di un file PDF durante il caricamento.

1. Dal menu Ritaglio, selezionare **[!UICONTROL Manuale]**.
1. Immettete le impostazioni per i pixel nelle caselle di testo In alto, A destra, In basso e A sinistra per ritagliare dal corrispondente bordo delle pagine.

La quantità di pagina che viene ritagliata dipende dall’impostazione della risoluzione in pixel per pollice immessa per il file PDF. Ad esempio, supponiamo di immettere 150 (valore predefinito) come impostazione Risoluzione PX/Pollici. Quindi ritagliate 75 pixel dai lati delle pagine. In tal caso, 0,5 pollici. è ritagliato. A 150 pixel per pollice, 75 pixel equivalgono a mezzo pollice.
