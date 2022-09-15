---
title: Font
description: Scopri come utilizzare i font in Adobe Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 28%

---

# Font{#fonts}

A volte, Adobe Dynamic Media Classic richiede di caricare un file di font per immettere o eseguire il rendering del testo in un particolare font. Ad esempio, per usare un font particolare per un testo su un livello di modello, caricate il file di font. Per visualizzare i numeri della pagina Visualizzatore eCatalog in un font particolare, caricate il file del font.

Adobe Dynamic Media Classic supporta i seguenti tipi di font:

* Tutti i font TrueType
* Font PostScript®
* Font OpenType/TrueType
* Font OpenType/PostScript
* PhotoFonts

Dopo aver caricato un file di font, puoi modificarne l’ID Adobe Dynamic Media Classic, il nome del font e digitare le informazioni nella schermata Modifica informazioni.

>[!NOTE]
>
>Adobe Dynamic Media Classic consiglia di caricare tutti gli stili di font (grassetto, corsivo, grassetto/corsivo e normale) se prevedi di utilizzare i font nei livelli modello. Adobe Dynamic Media Classic richiede questi stili di font per elaborare le richieste. Si consiglia anche di caricare tutti i file PostScript/Adobe Type 1 associati a un font, poiché alcuni di questi contengono informazioni dettagliate per la crenatura.

## Caricare file di font {#uploading-font-files}

Caricate i file di font con le stesse tecniche usate per caricare altri file. È possibile memorizzare i file di font in qualsiasi cartella Adobe Dynamic Media Classic. Consultate [Caricamento dei file](uploading-files.md#uploading_your_files).

## Modifica delle informazioni sul file di font {#editing-font-file-information}

È possibile modificare il nome ID di un font e le relative informazioni sul tipo. La modifica di un file di font può essere utile per le ricerche e per identificare i font più facilmente.

Nel pannello Sfoglia, selezionare il file di font da modificare in Vista dettagli e scegliere File > Modifica informazioni. Viene visualizzata la schermata Modifica info. Scegli le seguenti opzioni e seleziona **[!UICONTROL Invia]**.

* **[!UICONTROL Nome font]** - Questo nome identifica il font quando viene pubblicato.

* **[!UICONTROL Nome PostScript]** - Questo nome è il nome PostScript completo del font. Generalmente indica ne lo spessore o stile.

* **[!UICONTROL Nome RTF]** - Questo nome viene visualizzato in un menu a comparsa nell&#39;editor RTF in cui vengono creati i livelli di testo del modello.

* **[!UICONTROL Nome famiglia font]** - Questo nome elenca il nome del font senza l&#39;indicatore di stile, spessore o tipo di carattere.

* **[!UICONTROL Stile font]** - Le opzioni disponibili sono Normale, Grassetto, Corsivo e Grassetto-Corsivo.

* **[!UICONTROL Tipo di carattere]** - Le opzioni sono TrueType e Adobe Type 1. Per chiamare questi font con un altro nome, immettete il nome desiderato.

* **[!UICONTROL Abbreviazione tipo di carattere]** - Le opzioni sono le seguenti:

   * **[!UICONTROL TTF]** - File di font TrueType utilizzati per il rendering di PDF/PostScript e per il server di immagini.

   * **[!UICONTROL AFM]** - File di font Adobe PostScript contenenti informazioni Adobi sulle metriche dei font e utilizzati per il serving delle immagini.

   * **[!UICONTROL PFM]** - File di font Adobe PostScript che contengono informazioni binarie sulla metrica dei font.

   * **[!UICONTROL PFB]** - File di font Adobe PostScript che contengono informazioni binarie sulla struttura dei font e vengono utilizzati per il rendering PDF/PostScript e il servizio immagini.
