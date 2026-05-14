---
title: Informazioni sui contenuti generati dagli utenti in Adobe Dynamic Media Classic
description: Introduzione ai contenuti generati dagli utenti.
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
feature: Dynamic Media Classic
role: Admin,User
exl-id: 14729192-7b9d-4f42-99da-6564a3f35959
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:34:44.287Z'
TQID: 'https://experienceleague.adobe.com/SwNEO6U33qx45AECK79nff9f9kABWuOdq91d4X8SHd0'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 179
ht-degree: 33%

---

# Informazioni sui contenuti generati dagli utenti in Adobe Dynamic Media Classic {#about-user-generated-content}

L’utilizzo di contenuti generati dagli utenti (UGC, User-Generated Content) consiste nel caricare le risorse in un archivio di storage Adobe Dynamic Media Classic dedicato ed eseguire le operazioni correlate.

UGC supporta i formati di file immagine raster BMP, GIF, JPG, PNG, PSD, TIFF.

>[!IMPORTANT]
>
>A partire dal 1° maggio 2023, le risorse UGC in Dynamic Media saranno disponibili per l’uso fino a 60 giorni dalla data di caricamento. Dopo 60 giorni, le risorse verranno rimosse.

<!-- * Vector: AI, EPS (EPS files from Adobe Illustrator 2018 are not supported), PDF (only when the PDF file is previously opened and saved in Adobe Illustrator CS6) -->

>[!NOTE]
>
>Il supporto per risorse di immagini vettoriali UGC nuove o esistenti in Adobe Dynamic Media Classic è terminato il 30 settembre 2021.

Prima di caricare le risorse, dovete ottenere una chiave segreta condivisa Usate questa chiave per ottenere un token di caricamento. Il token di caricamento verrà quindi fornito al momento di caricare le risorse ed eseguire altre operazioni UGC.

Una volta ottenuta la chiave segreta condivisa e caricato il token, potete eseguire le seguenti operazioni relative a contenuti generati dall’utente:

* Carica una risorsa.
* Ottenere i metadati di una risorsa immagine.
* Eliminare una risorsa caricata.
* Informazioni sull&#39;utilizzo dello spazio su disco di un&#39;azienda.
