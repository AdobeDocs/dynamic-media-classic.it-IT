---
title: Font
description: Scopri come utilizzare i font in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 23%

---

# Font{#fonts}

A volte, Adobe Dynamic Media Classic richiede di caricare un file di font per immettere o riprodurre il testo in un determinato font. Ad esempio, per usare un font particolare per un testo su un livello di modello, caricate il file di font. Per visualizzare i numeri della pagina Visualizzatore eCatalog in un font particolare, caricate il file del font.

Adobe Dynamic Media Classic supporta i tipi di carattere seguenti:

* Tutti i font TrueType
* PostScript®
* Font OpenType/TrueType
* Font OpenType/PostScript
* PhotoFonts

Dopo il caricamento di un file di caratteri, è possibile modificarne l&#39;ID Adobe Dynamic Media Classic, il nome e le informazioni sul tipo nella schermata Modifica informazioni.

>[!NOTE]
>
>Adobe Dynamic Media Classic consiglia di caricare tutti gli stili di carattere (grassetto, corsivo, grassetto/corsivo e normale) se intendi utilizzare i caratteri nei livelli modello. Adobe Dynamic Media Classic richiede questi stili di carattere per elaborare le richieste. Caricamento di tutto `PostScript/Adobe Type1` file associati a un font è consigliabile, poiché alcuni di questi font contengono informazioni dettagliate sulla crenatura.

## Carica file di font {#uploading-font-files}

Caricate i file di font con le stesse tecniche usate per caricare altri file. È possibile memorizzare i file dei caratteri in qualsiasi cartella di Adobe Dynamic Media Classic. Consultate [Caricamento dei file](uploading-files.md#uploading_your_files).

## Modifica informazioni file font {#editing-font-file-information}

È possibile modificare il nome ID di un tipo di carattere e le relative informazioni sul tipo. La modifica di un file di font può essere utile per le ricerche e per identificare i font più facilmente.

Nel pannello Sfoglia, selezionate il file di font da modificare in Vista dettagli e scegliete File > Modifica informazioni. Viene visualizzata la schermata Modifica info. Scegli le seguenti opzioni, quindi seleziona **[!UICONTROL Invia]**.

* **[!UICONTROL Nome font]**: questo nome identifica il tipo di carattere quando viene pubblicato.

* **[!UICONTROL Nome PostScript]**: nome PostScript completo per il tipo di carattere. Generalmente indica ne lo spessore o stile.

* **[!UICONTROL Nome RTF]**: questo nome viene visualizzato in un menu a comparsa nell’editor RTF in cui vengono creati i livelli di testo del modello.

* **[!UICONTROL Nome famiglia font]**: questo nome elenca il nome del tipo di carattere senza l&#39;indicatore di stile, spessore o tipo di carattere.

* **[!UICONTROL Stile font]**: le opzioni sono Plain, Bold, Italic e Bold-Italic.

* **[!UICONTROL Tipo font]**: le opzioni sono TrueType e Adobi Type 1. Per chiamare questi font con un altro nome, immettete il nome desiderato.

* **[!UICONTROL Abbreviazione tipo font]**: le opzioni sono le seguenti:

   * **[!UICONTROL TTF]**: file di font TrueType utilizzati per il rendering PDF/PostScript e per la gestione delle immagini.

   * **[!UICONTROL AFM]**: file di font di Adobe PostScript che contengono informazioni sulle metriche dei font di Adobe e che vengono utilizzati per la trasmissione delle immagini.

   * **[!UICONTROL PFM]**: file di font Adobe PostScript contenenti informazioni binarie sulle metriche dei font.

   * **[!UICONTROL PFB]**: file di font Adobe PostScript che contengono informazioni binarie sulla struttura del font e che vengono utilizzati per il rendering PDF/PostScript e per il server delle immagini.
