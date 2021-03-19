---
title: Profili ICC
description: Scopri i profili ICC.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: Professionista
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 70%

---


# ICC, profili{#icc-profiles}

Un profilo ICC (International Color Consortium) è un file che descrive come convertire correttamente i file di immagini da uno spazio colore a un altro. I profili ICC consentono di ottenere i colori corretti per le immagini. Ad esempio, per visualizzare correttamente immagini destinate alla stampa sul monitor di un computer, potete scegliere un profilo ICC. Questo profilo consente di convertire l’immagine in un diverso spazio colore e garantisce che i colori vengano visualizzati correttamente online.

In Dynamic Media Classic, puoi scegliere un profilo ICC per convertire le immagini in uno spazio colore diverso quando carichi le immagini. Tutti i profili ICC standard di Photoshop sono disponibili per impostazione predefinita in Dynamic Media Classic. Per visualizzare i nomi dei profili colore nella schermata Carica, selezionate il menu Profilo colore. Quindi scegliete Personale Da > A e scegliete il nome di un profilo ICC nei menu Personale Da e Personale A. Consultate [Opzioni di modifica delle immagini al caricamento](image-editing-options-upload.md#image-editing-options-at-upload).

Oltre a utilizzare i profili ICC predefiniti, puoi caricare altri profili ICC in Dynamic Media Classic e renderli disponibili per la conversione dello spazio colore. In visualizzazione Dettagli nel pannello Sfoglia potete vedere la classe del profilo, il tipo di spazio colore e il tipo PCS di un profilo ICC.

## Caricamento di profili ICC  {#uploading-icc-profiles}

Caricate profili ICC con le stesse tecniche usate per caricare altri file. Puoi archiviare i profili ICC in qualsiasi cartella di Dynamic Media Classic. Consultate [Caricamento dei file](uploading-files.md#uploading_your_files).

## Analisi di un profilo ICC  {#examining-an-icc-profile}

Per analizzare un profilo ICC, selezionatelo nel pannello Sfoglia per visualizzarlo in visualizzazione Dettagli. La visualizzazione Dettagli fornisce informazioni sui profili ICC.

**Profilo** ClasseICC (International Color Consortium) definisce ogni classe per coprire un tipo di applicazione. Ad esempio, i profili di Input si applicano a dispositivi quali fotocamere digitali e scanner e i profili di Output si applicano alle stampanti.

**Tipo** di spazio coloreQuesto numero è lo spazio colore &quot;input&quot; del profilo, come definito dalla ICC. Il tipo di spazio colore consente di definire il numero di componenti dello spazio colore e l’interpretazione di tali componenti. Ad esempio, RGB è uno spazio colore con tre componenti: rosso, verde e blu. Il tipo di spazio colore non definisce le particolari caratteristiche di colore dello spazio (ad esempio, le cromaticità dei primari).

**PCS** TypeQuesto tipo di PCS è lo spazio colore &quot;di uscita&quot; del profilo, lo spazio di connessione del profilo. Ad esempio, un profilo colore può convertire RGB in PCS, quindi effettua la conversione da PCS a CMYK.

Per un profilo di input, visualizzazione o output utile per assegnare tag a colori o immagini, il tipo PCS è XYZ o Lab. Interpretate questo profilo come lo spazio colore specifico corrispondente definito nella specifica ICC.
