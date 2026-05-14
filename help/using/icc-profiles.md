---
title: Profili ICC (International Color Consortium)
description: Scopri i profili ICC in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
autotag-review: '2026-05-13T19:59:42.608Z'
TQID: 'https://experienceleague.adobe.com/eGKamqA47mITzfyTuHoFYLfWEXOP0jAl5XWDpihGjZA'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 528
ht-degree: 31%

---

# Profili ICC{#icc-profiles}

Un profilo ICC (International Color Consortium) è un file che descrive come convertire correttamente i file immagine da uno spazio colore all&#39;altro. I profili ICC consentono di ottenere i colori corretti per le immagini. Ad esempio, per visualizzare correttamente le immagini progettate per la stampa su un monitor, è possibile scegliere un profilo ICC. Questo profilo consente di convertire l’immagine in un diverso spazio colore e garantisce che i colori vengano visualizzati correttamente online.

In Adobe Dynamic Media Classic, potete scegliere un profilo ICC per convertire le immagini in uno spazio colore diverso quando caricate le immagini. Tutti i profili ICC standard di Photoshop sono disponibili per impostazione predefinita su Adobe Dynamic Media Classic. Per visualizzare i nomi dei profili colore nella schermata Carica, selezionate il menu Profilo colore. Quindi scegliete Personale Da > A e scegliete il nome di un profilo ICC nei menu Personale Da e Personale A.

Consulta [Opzioni di modifica immagine al caricamento](image-editing-options-upload.md#image-editing-options-at-upload).

Oltre a utilizzare i profili ICC predefiniti, potete caricare altri profili ICC in Adobe Dynamic Media Classic e renderli disponibili per la conversione dello spazio colore. Passate alla Vista dettagli nel pannello Sfoglia per esaminare la Classe profilo, il tipo di spazio colore e il Tipo PCS di un profilo ICC.

In sintesi, i punti chiave per i profili ICC sono i seguenti:

* I profili ICC consentono la conversione corretta dei colori tra spazi di colore diversi per i file di immagine.
* Adobe Dynamic Media Classic incorpora tutti i profili Photoshop ICC standard per una conversione delle immagini affidabile.
* I profili ICC personalizzati offrono maggiore flessibilità per le esigenze avanzate di conversione dello spazio colore.
* La visualizzazione di dettagli quali la classe di profilo e il tipo di PCS nella vista dei dettagli consente di gestire le impostazioni ICC.
* Il caricamento dei profili ICC è semplice e garantisce l’accesso tra le cartelle in Dynamic Media Classic.


## Carica profili ICC {#uploading-icc-profiles}

Caricate profili ICC con le stesse tecniche usate per caricare altri file. È possibile memorizzare i profili ICC in qualsiasi cartella Adobe Dynamic Media Classic.

Consulta [Caricare i file](uploading-files.md#uploading_your_files).

## Esamina un profilo ICC {#examining-an-icc-profile}

Per esaminare un profilo ICC, selezionatelo nel pannello Sfoglia e visualizzatelo in Vista dettagli. La Vista dettagli fornisce queste informazioni sui profili ICC:

* **[!UICONTROL Classe profilo]**: l&#39;ICC definisce ogni classe per coprire un tipo di applicazione. Ad esempio, i profili di input si applicano ai dispositivi, come fotocamere digitali e scanner. I profili di output si applicano alle stampanti.

* **[!UICONTROL Tipo di spazio colore]**: questo numero è lo spazio colore &quot;di input&quot; del profilo, come definito dall&#39;ICC. Il tipo di spazio colore consente di definire il numero di componenti dello spazio colore e l’interpretazione di tali componenti. Ad esempio, RGB è uno spazio colore con tre componenti: rosso, verde e blu. Il tipo di spazio colore non definisce le particolari caratteristiche di colore dello spazio (ad esempio, le cromaticità dei primari).

* **[!UICONTROL Tipo PCS]**: questo tipo PCS è lo spazio colore &quot;output&quot; del profilo, ovvero lo spazio di connessione del profilo. Ad esempio, un profilo colore può convertire RGB in PCS, quindi effettua la conversione da PCS a CMYK.

Per un profilo di ingresso, visualizzazione o uscita utile per l&#39;assegnazione di tag a colori o immagini, il tipo di PCS è XYZ o Lab. Interpretate questo profilo come lo spazio colore specifico corrispondente definito nella specifica ICC.
