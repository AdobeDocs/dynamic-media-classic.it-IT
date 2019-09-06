---
title: Font
seo-title: Font
description: 'null'
seo-description: Scoprite come utilizzare i font in Dynamic Media Classic.
uuid: bddec 9 c 2-8530-4 bbd -8 db 7-1562 a 347 e 482
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/support_ files
discoiquuid: 97 cecd 6 a -30 aa -44 fe-a 611-fd 71 b 02 fd 5 ae
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Font{#fonts}

In alcuni casi, Scene7 Publishing System richiede di caricare un file di font per immettere o eseguire il rendering di un testo in un font particolare. Ad esempio, per usare un font particolare per un testo su un livello di modello, caricate il file di font. Per visualizzare i numeri della pagina Visualizzatore eCatalog in un font particolare, caricate il file del font.

Dynamic Media Classic supporta i seguenti tipi di font:

* Tutti i font TrueType
* Font postscript®
* Font OpenType/TrueType
* Font OpenType/PostScript
* PhotoFonts

Dopo aver caricato un file di font, potete modificarne l’ID SPS, il nome font e immettere informazioni nella schermata Modifica info.

>[!NOTE]
>
>Dynamic Media Classic consiglia di caricare tutti gli stili di font (grassetto, corsivo, grassetto/corsivo e regolare) se intendete usare i font nei livelli modello. Dynamic Media Classic necessita di questi stili di font per elaborare le richieste. Si consiglia anche di caricare tutti i file PostScript/Adobe Type 1 associati a un font, poiché alcuni di questi contengono informazioni dettagliate per la crenatura.

## Caricamento di file di font {#uploading-font-files}

Caricate i file di font con le stesse tecniche usate per caricare altri file. Potete memorizzarli in qualsiasi cartella SPS. Consultate [Caricamento dei file](uploading-files.md#uploading_your_files).

## Modifica delle informazioni sui file di font {#editing-font-file-information}

Potete modificare il nome ID di un font, nonché le informazioni relative al tipo. La modifica di un file di font può essere utile per le ricerche e per identificare i font più facilmente.

Nel pannello Sfoglia, selezionate il file di font che desiderate modificare in visualizzazione Dettagli e scegliete File &gt; Modifica info. Viene visualizzata la schermata Modifica info. Scegliete le seguenti opzioni e fate clic sul pulsante Invia.

**Nome font** Questo nome identifica il font quando viene pubblicato.

**Nome** postscript Nome completo per il font. Generalmente indica ne lo spessore o stile.

**Nome RTF** Questo nome viene visualizzato in un menu a comparsa nell'editor RTF in cui vengono creati i livelli di testo del modello.

**Nome famiglia font** Questo nome elenca il nome del font senza lo stile, lo spessore o l'indicatore del tipo di font.

**Stile font** Le opzioni sono Normale, Grassetto, Corsivo e Grassetto-Corsivo.

**Tipo font** Le opzioni sono truetype e Adobe Type 1. Per chiamare questi font con un altro nome, immettete il nome desiderato.

**Abbreviazione tipo font** Le opzioni sono le seguenti:

**File di font TTF** truetype utilizzati per il rendering PDF/postscript e per la trasmissione di immagini.

**File di font AFM** Adobe postscript contenenti informazioni Adobe Font Metrics e utilizzati per la trasmissione delle immagini.

**File di font** Adobe postscript contenenti informazioni binarie sulla metrica dei font.

**File di font PFB** Adobe postscript contenenti informazioni binarie sulla struttura dei font e utilizzati per il rendering e la trasmissione di immagini PDF/postscript.
