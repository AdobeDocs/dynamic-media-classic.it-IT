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
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 36%

---

# Utilizzare i PDF{#working-with-pdfs}

I file PDF (Portable Document Format) vengono utilizzati più spesso in Adobe Dynamic Media Classic per la creazione di eCatalog. Quando carichi un file di PDF, Adobe Dynamic Media Classic rasterizza o rimuove le pagine per impostazione predefinita, in modo che possano essere utilizzate per creare contenuti rich media.

Quando carichi un PDF per l’estrazione della pagina, Adobe applica il seguente limite:

| Tipo di limite | Limite imposto | Modifica del limite del 31 dicembre 2022 |
| --- | --- | --- |
| Numero massimo di pagine per un PDF da considerare per l’estrazione | 5000 (per nuovi caricamenti) | 100 (per tutti i PDF) |

Vedi anche [Limitazioni di Dynamic Media](/help/using/limitations.md).

## Opzioni di caricamento PDF {#pdf-upload-options}

Quando caricate un file PDF potete formattarlo in vari modi. Potete ritagliare pagine, estrarre parole di ricerca, immettere un valore di risoluzione in ppi e scegliere uno spazio colore. I file PDF contengono spesso un margine di rifilo, indicatori di taglio, crocini di registro e altri indicatori di stampa. Durante il caricamento di un file PDF potete ritagliare tali indicatori dai lati delle pagine.

Le opzioni per il caricamento dei file di PDF si trovano nella sezione Opzioni di PDF della pagina Carica.

### Opzioni di elaborazione

**[!UICONTROL Rasterizza]** - (Impostazione predefinita) Ripete le pagine nel file PDF e converte gli elementi grafici vettoriali in immagini bitmap. Per creare un eCatalog, scegliere questa opzione.

**[!UICONTROL Estrai parole di ricerca]** - Estrae parole dal file PDF in modo che sia possibile eseguire ricerche per parola chiave in un visualizzatore eCatalog.

**[!UICONTROL Estrai collegamenti]** : estrae collegamenti dai file PDF e li converte in mappe immagini utilizzate in un visualizzatore eCatalog.

**[!UICONTROL Genera automaticamente eCatalog con PDF multipagina]** : crea automaticamente un eCatalog dal file PDF. All’eCatalog viene assegnato un nome in base al file PDF caricato. Questa opzione è disponibile solo se il file PDF viene rasterizzato al momento del caricamento.

### Risoluzione

Specifica l’impostazione della risoluzione. Questa impostazione determina la quantità di pixel visualizzati per pollice nel file PDF. Il valore predefinito è 150.

### Spazio colore di nitidezza

Dal menu Spazio colore scegliete uno spazio colore per il file PDF. La maggior parte dei file PDF contiene immagini a colori sia in RGB che in CMYK. Per la visualizzazione online è preferibile lo spazio colore RGB.

* **[!UICONTROL Rileva automaticamente]** - Mantiene lo spazio colore del file PDF.

* **[!UICONTROL Forza come RGB]** - Converte in spazio colore RGB.

* **[!UICONTROL Forza come CMYK]** - Converte in spazio colore CMYK.

* **[!UICONTROL Forza come gradazioni di grigio]** - Converte lo spazio colore in scala di grigi.

### Opzioni profilo colore

* **[!UICONTROL Converti in sRGB]** - Converte in sRGB (rosso standard, verde, blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

* **[!UICONTROL Mantieni spazio colore originale]** - Mantiene lo spazio colore originale.

* **[!UICONTROL Personalizza da]** > **[!UICONTROL A]** - Apre i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore standard di Photoshop o uno spazio colore caricato in Adobe Dynamic Media Classic.

Consultate anche [Profili ICC](/help/using/icc-profiles.md#icc_profiles).

## Ritaglia spazio vuoto da un file PDF {#cropping-white-space-from-a-pdf-file}

1. Per ritagliare automaticamente i pixel dello spazio bianco da un file PDF mentre lo caricate, selezionate il menu Ritaglio e scegliete Rifila.
1. Specificate le seguenti opzioni:

   * **[!UICONTROL Rifila in base a]** - Scegliere se ritagliare in base al colore o alla trasparenza:

      * **[!UICONTROL Colore]** - Scegliere l&#39;opzione Colore. Quindi seleziona la **[!UICONTROL Angolo]** e scegliete l&#39;angolo del PDF con il colore che meglio rappresenta lo spazio bianco da ritagliare.

      * **[!UICONTROL Trasparenza]** - Scegliere l&#39;opzione Trasparenza.

   * **[!UICONTROL Tolleranza]** - Trascinate il cursore per specificare una tolleranza da 0 a 1.

   * **[!UICONTROL Rifilatura in base al colore]** - Specificate 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell&#39;angolo del PDF. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

   * **[!UICONTROL Rifilatura basata sulla trasparenza]** - Specificate 0 per ritagliare i pixel solo se sono trasparenti; i numeri più vicini a 1 consentono una maggiore trasparenza.

## Ritaglia dai lati delle pagine PDF {#cropping-from-the-sides-of-pdf-pages}

Potete rimuovere manualmente gli indicatori di stampa dai lati delle pagine di un file PDF mentre lo caricate.

1. Dal menu Ritaglia, seleziona **[!UICONTROL Manuale]**.
1. Immettete le impostazioni per i pixel nelle caselle di testo In alto, A destra, In basso e A sinistra per ritagliare dal corrispondente bordo delle pagine.

La quantità di pagina che viene ritagliata dipende dall’impostazione della risoluzione in pixel per pollice immessa per il file PDF. Ad esempio, supponiamo di immettere 150 (valore predefinito) come impostazione Risoluzione PX/Pollici. Quindi ritagliate 75 pixel dai lati delle pagine. In tal caso, 0,5 pollici. è ritagliato. A 150 pixel per pollice, 75 pixel equivalgono a mezzo pollice.
