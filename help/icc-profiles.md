---
title: Profili ICC (International Colore Consortium)
description: Scopri sui profili ICC in Adobe Systems Dynamic Media Classic.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 54%

---

# ICC, profili{#icc-profiles}

Un profilo ICC (International Color Consortium) è un file che descrive come convertire correttamente i file di immagini da uno spazio colore a un altro. I profili ICC consentono di ottenere i colori corretti per le immagini. Ad esempio, per visualizzare correttamente immagini destinate alla stampa sul monitor di un computer, potete scegliere un profilo ICC. Questo profilo consente di convertire l’immagine in un diverso spazio colore e garantisce che i colori vengano visualizzati correttamente online.

In Adobe Systems Dynamic Media Classic, potete scegliere un profilo ICC per convertire immagini in un altro spazio colore quando caricate le immagini. Tutti i profili ICC standard Photoshop sono disponibili per impostazione predefinita su Adobe Systems Dynamic Media Classic. Per visualizzare i nomi dei profili colore nella schermata Carica, selezionate il menu Profilo colore. Quindi scegliete Personale Da > A e scegliete il nome di un profilo ICC nei menu Personale Da e Personale A.

Consulta [ immagine opzioni di modifica al caricamento ](image-editing-options-upload.md#image-editing-options-at-upload) .

Oltre a utilizzare i profili ICC predefiniti, è possibile caricare altri profili ICC per Adobe Systems Dynamic Media Classic e renderli disponibili per la conversione dello spazio colore. Passate ai dettagli Visualizza nel pannello Sfoglia per analizzare la classe di profilo, il tipo di spazio colore e il tipo di PC di un profilo ICC.

## Carica profili ICC {#uploading-icc-profiles}

Caricate profili ICC con le stesse tecniche usate per caricare altri file. Puoi store profili ICC in qualsiasi Adobe Systems Dynamic Media cartella classica.

Consultate [ caricare i file ](uploading-files.md#uploading_your_files) .

## Esaminare un profilo ICC {#examining-an-icc-profile}

Per esaminare un profilo ICC, selezionatelo nel pannello Sfoglia e visualizzatelo in dettaglio Visualizza. Dettagli Visualizza fornisce queste informazioni sui profili ICC:

* **[!UICONTROL Classe]** profile-il ICC (International colore Consortium) definisce ogni classe per coprire un tipo di applicazione. Ad esempio, i profili di Input si applicano a dispositivi quali fotocamere digitali e scanner e i profili di Output si applicano alle stampanti.

* **[!UICONTROL Spazio cromatico Type]** -questo numero è lo spazio colore &quot;input&quot; del profilo, come definito dalla CPI. Il tipo di spazio colore consente di definire il numero di componenti dello spazio colore e l’interpretazione di tali componenti. Ad esempio, RGB è uno spazio colore con tre componenti: rosso, verde e blu. Il tipo di spazio colore non definisce le particolari caratteristiche di colore dello spazio (ad esempio, le cromaticità dei primari).

* **[!UICONTROL Tipo]** di PCS-questo tipo di PCS è lo spazio colore &quot;output&quot; del profilo, ovvero lo spazio di connessione del profilo. Ad esempio, un profilo colore può convertire RGB in PCS, quindi effettua la conversione da PCS a CMYK.

Per un profilo di input, visualizzazione o output utile per assegnare tag a colori o immagini, il tipo PCS è XYZ o Lab. Interpretate questo profilo come lo spazio colore specifico corrispondente definito nella specifica ICC.
