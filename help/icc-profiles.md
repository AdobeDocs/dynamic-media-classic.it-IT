---
title: Profili ICC
seo-title: ICC, profili
description: 'null'
seo-description: Informazioni sui profili ICC.
uuid: 708 ff 2 ad -9 a 47-4 e 3 e-b 643-5 b 19648 f 726 b
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/support_ files
discoiquuid: 44 f 1 b 4 c 4-6 d 7 f -4 e 0 f -84 ce -11 d 26745 e 0 f 0
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# ICC, profili{#icc-profiles}

Un profilo ICC (International Color Consortium) è un file che descrive come convertire correttamente i file di immagini da uno spazio colore a un altro. I profili ICC consentono di ottenere i colori corretti per le immagini. Ad esempio, per visualizzare correttamente immagini destinate alla stampa sul monitor di un computer, potete scegliere un profilo ICC. Questo profilo consente di convertire l’immagine in un diverso spazio colore e garantisce che i colori vengano visualizzati correttamente online.

In Scene7 Publishing System, potete scegliere un profilo ICC per convertire immagini in un diverso spazio colore in fase di caricamento. Tutti i profili ICC standard di Photoshop sono disponibili per impostazione predefinita in SPS. Per visualizzare i nomi dei profili colore nella schermata Carica, selezionate il menu Profilo colore. Quindi scegliete Personale Da &gt; A e scegliete il nome di un profilo ICC nei menu Personale Da e Personale A. Consultate [Opzioni di modifica delle immagini al caricamento](image-editing-options-upload.md#image-editing-options-at-upload).

Anche usando i profili ICC predefiniti, potete caricare altri profili ICC in SPS e renderli disponibili per la conversione dello spazio colore. In visualizzazione Dettagli nel pannello Sfoglia potete vedere la classe del profilo, il tipo di spazio colore e il tipo PCS di un profilo ICC.

## Caricamento di profili ICC {#uploading-icc-profiles}

Caricate profili ICC con le stesse tecniche usate per caricare altri file. Potete memorizzarli in qualsiasi cartella SPS. Consultate [Caricamento dei file](uploading-files.md#uploading_your_files).

## Analisi di un profilo ICC {#examining-an-icc-profile}

Per analizzare un profilo ICC, selezionatelo nel pannello Sfoglia per visualizzarlo in visualizzazione Dettagli. La visualizzazione Dettagli fornisce informazioni sui profili ICC.

**Profile Class** the ICC (International Color Consortium) definisce ciascuna classe per la copertura di un tipo di applicazione. Ad esempio, i profili di Input si applicano a dispositivi quali fotocamere digitali e scanner e i profili di Output si applicano alle stampanti.

**Tipo** di spazio colore Questo numero è lo spazio colore «input» del profilo, come definito da ICC. Il tipo di spazio colore consente di definire il numero di componenti dello spazio colore e l’interpretazione di tali componenti. Ad esempio, RGB è uno spazio colore con tre componenti: rosso, verde e blu. Il tipo di spazio colore non definisce le particolari caratteristiche di colore dello spazio (ad esempio, le cromaticità dei primari).

**Tipo** PCS Questo tipo PCS è lo spazio colore «output» del profilo, ossia lo spazio di connessione del profilo. Ad esempio, un profilo colore può convertire RGB in PCS, quindi effettua la conversione da PCS a CMYK.

Per un profilo di input, visualizzazione o output utile per assegnare tag a colori o immagini, il tipo PCS è XYZ o Lab. Interpretate questo profilo come lo spazio colore specifico corrispondente definito nella specifica ICC.
