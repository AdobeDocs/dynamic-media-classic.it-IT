---
title: Font
seo-title: Font
description: 'null'
seo-description: Scoprite come utilizzare i font in Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 40%

---


# Font{#fonts}

In alcuni casi, Dynamic Media Classic richiede di caricare un file di font per immettere o eseguire il rendering del testo in un font particolare. Ad esempio, per usare un font particolare per un testo su un livello di modello, caricate il file di font. Per visualizzare i numeri della pagina Visualizzatore eCatalog in un font particolare, caricate il file del font.

Dynamic Media Classic supporta i seguenti tipi di font:

* Tutti i font TrueType
* PostScript® fonts
* Font OpenType/TrueType
* Font OpenType/PostScript
* PhotoFonts

Dopo aver caricato un file di font, potete modificarne l’ID Dynamic Media Classic, il nome del font e digitare le informazioni nella schermata Modifica info.

>[!NOTE]
>
>Dynamic Media Classic consiglia di caricare tutti gli stili di font (grassetto, corsivo, grassetto/corsivo e normale) se prevedete di utilizzare i font nei livelli modello. Dynamic Media Classic necessita di questi stili di font per elaborare le richieste. Si consiglia anche di caricare tutti i file PostScript/Adobe Type 1 associati a un font, poiché alcuni di questi contengono informazioni dettagliate per la crenatura.

## Caricamento di file di font {#uploading-font-files}

Caricate i file di font con le stesse tecniche usate per caricare altri file. È possibile archiviare i file di font in qualsiasi cartella di Dynamic Media Classic. Consultate [Caricamento dei file](uploading-files.md#uploading_your_files).

## Modifica delle informazioni sui file di font {#editing-font-file-information}

Potete modificare il nome ID di un font, nonché le informazioni relative al tipo. La modifica di un file di font può essere utile per le ricerche e per identificare i font più facilmente.

Nel pannello Sfoglia, selezionate il file di font che desiderate modificare in visualizzazione Dettagli e scegliete File > Modifica info. Viene visualizzata la schermata Modifica info. Scegliete le seguenti opzioni e fate clic sul pulsante Invia.

**Nome** font Questo nome identifica il font quando viene pubblicato.

**Nome** PostScript Questo nome è il nome PostScript completo per il font. Generalmente indica ne lo spessore o stile.

**Nome** RTF Questo nome viene visualizzato in un menu a comparsa nell’editor RTF in cui vengono creati i livelli di testo del modello.

**Nome** famiglia font Questo nome riporta il nome del font senza l&#39;indicatore dello stile, dello spessore o del tipo di font.

**Stile** font Le opzioni sono Normale, Grassetto, Corsivo e Grassetto-Corsivo.

**Tipo** di font Le opzioni sono TrueType e Adobe Type 1. Per chiamare questi font con un altro nome, immettete il nome desiderato.

**Abbreviazione** tipo di carattere Le opzioni sono le seguenti:

**File di font TTF** TrueType utilizzati per il rendering e la trasmissione delle immagini PDF/PostScript.

**File di font AFM** Adobe PostScript contenenti informazioni Adobe Font Metrics e utilizzati per la trasmissione delle immagini.

**File di font Adobe PostScript PFM** che contengono informazioni binarie sulla metrica dei font.

**File di font Adobe PostScript PFB** contenenti informazioni binarie sul contorno dei font e utilizzati per il rendering e la trasmissione delle immagini PDF/PostScript.
