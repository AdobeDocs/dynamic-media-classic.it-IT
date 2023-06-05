---
title: Profili ICC (International Color Consortium)
description: Scopri i profili ICC in Adobe Dynamic Media Classic.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 54%

---

# ICC, profili{#icc-profiles}

Un profilo ICC (International Color Consortium) è un file che descrive come convertire correttamente i file di immagini da uno spazio colore a un altro. I profili ICC consentono di ottenere i colori corretti per le immagini. Ad esempio, per visualizzare correttamente immagini destinate alla stampa sul monitor di un computer, potete scegliere un profilo ICC. Questo profilo consente di convertire l’immagine in un diverso spazio colore e garantisce che i colori vengano visualizzati correttamente online.

In Adobe Dynamic Media Classic, potete scegliere un profilo ICC per convertire le immagini in uno spazio colore diverso quando caricate le immagini. Tutti i profili ICC standard di Photoshop sono disponibili per impostazione predefinita su Adobe Dynamic Media Classic. Per visualizzare i nomi dei profili colore nella schermata Carica, selezionate il menu Profilo colore. Quindi scegliete Personale Da > A e scegliete il nome di un profilo ICC nei menu Personale Da e Personale A.

Consulta [Opzioni di modifica immagine al caricamento](image-editing-options-upload.md#image-editing-options-at-upload).

Oltre a utilizzare i profili ICC predefiniti, potete caricare altri profili ICC in Adobe Dynamic Media Classic e renderli disponibili per la conversione dello spazio colore. Passate alla Vista dettagli nel pannello Sfoglia per esaminare la classe di profilo, il tipo di spazio colore e il tipo PCS di un profilo ICC.

## Carica profili ICC {#uploading-icc-profiles}

Caricate profili ICC con le stesse tecniche usate per caricare altri file. È possibile memorizzare i profili ICC in qualsiasi cartella Adobe Dynamic Media Classic.

Consulta [Caricare i file](uploading-files.md#uploading_your_files).

## Esamina un profilo ICC {#examining-an-icc-profile}

Per esaminare un profilo ICC, selezionarlo nel pannello Sfoglia e visualizzarlo in Vista dettagli. La Vista dettagli fornisce queste informazioni sui profili ICC:

* **[!UICONTROL Classe profilo]** - L&#39;ICC (International Color Consortium) definisce ogni classe per coprire un tipo di applicazione. Ad esempio, i profili di Input si applicano a dispositivi quali fotocamere digitali e scanner e i profili di Output si applicano alle stampanti.

* **[!UICONTROL Tipo di spazio colore]** - Questo numero è lo spazio colore &quot;di input&quot; del profilo, come definito dall&#39;ICC. Il tipo di spazio colore consente di definire il numero di componenti dello spazio colore e l’interpretazione di tali componenti. Ad esempio, RGB è uno spazio colore con tre componenti: rosso, verde e blu. Il tipo di spazio colore non definisce le particolari caratteristiche di colore dello spazio (ad esempio, le cromaticità dei primari).

* **[!UICONTROL Tipo PCS]** - Questo tipo PCS è lo spazio colore &quot;di output&quot; del profilo, cioè lo spazio di connessione del profilo. Ad esempio, un profilo colore può convertire RGB in PCS, quindi effettua la conversione da PCS a CMYK.

Per un profilo di input, visualizzazione o output utile per assegnare tag a colori o immagini, il tipo PCS è XYZ o Lab. Interpretate questo profilo come lo spazio colore specifico corrispondente definito nella specifica ICC.
