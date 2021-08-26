---
title: Font
description: Scopri come utilizzare i font in Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: 20a5e54a9f3fa442d3a993afae07aa5b1b13e9c3
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 33%

---

# Font{#fonts}

A volte, Dynamic Media Classic richiede di caricare un file di font per immettere o eseguire il rendering del testo in un particolare font. Ad esempio, per usare un font particolare per un testo su un livello di modello, caricate il file di font. Per visualizzare i numeri della pagina Visualizzatore eCatalog in un font particolare, caricate il file del font.

Dynamic Media Classic supporta i seguenti tipi di font:

* Tutti i font TrueType
* Font PostScript®
* Font OpenType/TrueType
* Font OpenType/PostScript
* PhotoFonts

Dopo aver caricato un file di font, puoi modificarne l’ID Dynamic Media Classic, il nome del font e digitare le informazioni nella schermata Modifica informazioni.

>[!NOTE]
>
>Dynamic Media Classic consiglia di caricare tutti gli stili di font (grassetto, corsivo, grassetto/corsivo e normale) se prevedi di utilizzare i font nei livelli modello. Dynamic Media Classic richiede questi stili di font per elaborare le richieste. Si consiglia anche di caricare tutti i file PostScript/Adobe Type 1 associati a un font, poiché alcuni di questi contengono informazioni dettagliate per la crenatura.

## Caricare file di font {#uploading-font-files}

Caricate i file di font con le stesse tecniche usate per caricare altri file. È possibile memorizzare i file di font in qualsiasi cartella di Dynamic Media Classic. Consultate [Caricamento dei file](uploading-files.md#uploading_your_files).

## Modifica delle informazioni sul file di font {#editing-font-file-information}

È possibile modificare il nome ID di un font e le relative informazioni sul tipo. La modifica di un file di font può essere utile per le ricerche e per identificare i font più facilmente.

Nel pannello Sfoglia, selezionate il file di font che desiderate modificare in visualizzazione Dettagli e scegliete File > Modifica info. Viene visualizzata la schermata Modifica info. Scegli le seguenti opzioni e seleziona **[!UICONTROL Invia]**.

* **[!UICONTROL Nome font]** : questo nome identifica il font quando viene pubblicato.

* **[!UICONTROL Nome]**  PostScript: nome completo del font. Generalmente indica ne lo spessore o stile.

* **[!UICONTROL Nome RTF]**  - Questo nome viene visualizzato in un menu a comparsa nell&#39;editor RTF in cui vengono creati i livelli di testo del modello.

* **[!UICONTROL Font Family Name]**  - Questo nome elenca il nome del font senza l&#39;indicatore di stile, spessore o tipo di carattere.

* **[!UICONTROL Stile carattere]** : le opzioni sono Normale, Grassetto, Corsivo e Grassetto-Corsivo.

* **[!UICONTROL Tipo di carattere]**  - Le opzioni sono TrueType e Adobe Type 1. Per chiamare questi font con un altro nome, immettete il nome desiderato.

* **[!UICONTROL Abbreviazione tipo di carattere]**  - Le opzioni sono le seguenti:

   * **[!UICONTROL TTF]**  - File di font TrueType utilizzati per il rendering PDF/PostScript e il servizio immagini.

   * **[!UICONTROL AFM]**  - File di font Adobe PostScript che contengono informazioni Adobi sulle metriche dei font e vengono utilizzati per il serving delle immagini.

   * **[!UICONTROL PFM]**  - File di font Adobe PostScript che contengono informazioni binarie sulla metrica dei font.

   * **[!UICONTROL PFB]**  - File di font Adobe PostScript che contengono informazioni binarie sulla struttura dei font e vengono utilizzati per il rendering PDF/PostScript e il servizio immagini.
