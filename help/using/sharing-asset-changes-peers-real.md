---
title: Condividere in tempo reale le modifiche apportate alle risorse con altri utenti
description: Scopri come condividere in tempo reale le modifiche apportate alle risorse con colleghi in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
autotag-review: '2026-05-13T20:12:54.992Z'
TQID: 'https://experienceleague.adobe.com/Yn5GsnQ4cM3Byk18iEB8Z4uGsTt9FjEZOBP17Yt-K8M'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 281
ht-degree: 26%

---

# Condividere in tempo reale le modifiche apportate alle risorse con altri utenti{#sharing-asset-changes-with-peers-in-real-time}

Si supponga di disporre di più copie di Adobe Dynamic Media Classic in esecuzione su computer della stessa società. In questo scenario, le seguenti azioni di qualsiasi client Dynamic Media Classic vengono aggiornate in tempo reale con tutti i client peer:

* Modificare una risorsa (generatore, editor di immagini e così via)
* Rinominare una risorsa
* Eliminare una risorsa
* Spostare una risorsa
* Caricare una o più risorse (sia desktop che FTP)
* Creare, eliminare o rinominare una cartella

Dopo aver apportato una modifica nel client di origine, tutti i client peer connessi alla stessa azienda vengono aggiornati con la modifica. Le modifiche vengono applicate ai client peer senza alcuna notifica, a meno che non sia in corsa la modifica di una delle risorse da aggiornare negli editor di immagini o negli strumenti di generazione.

Quando hai effettuato l’accesso, ti è stato chiesto di consentire o negare gli aggiornamenti peer. È possibile ricordare la scelta ed evitare così che tale notifica venga successivamente riproposta. Per annullare la scelta, eliminate il sito appropriato dal pannello Connettività peer-to-peer in Impostazioni globali.

Se stavi modificando una risorsa modificata da un peer, ti viene richiesto di inserire la modifica nel generatore o nell’editor. Se si sceglie **[!UICONTROL Sì]**, il generatore o l&#39;editor ignora eventuali modifiche apportate alla risorsa e importa la risorsa aggiornata. Se si sceglie **[!UICONTROL No]**, la risorsa rimane invariata nel generatore o nell&#39;editor e le modifiche apportate persistono nella sessione.

Quando hai salvato la risorsa, ti è stato notificato che esiste una versione più recente e ti è stato chiesto se desideri sovrascrivere la risorsa con le modifiche apportate.
