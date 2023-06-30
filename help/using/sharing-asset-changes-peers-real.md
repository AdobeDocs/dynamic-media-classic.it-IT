---
title: Condividere in tempo reale le modifiche apportate alle risorse con altri utenti
description: Scopri come condividere in tempo reale le modifiche apportate alle risorse con colleghi in Adobe Dynamic Media Classic.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 44%

---

# Condividere in tempo reale le modifiche apportate alle risorse con altri utenti{#sharing-asset-changes-with-peers-in-real-time}

Con più copie di Adobe Dynamic Media Classic in esecuzione su più computer della stessa società, le azioni seguenti di qualsiasi client Adobe Dynamic Media Classic vengono aggiornate in tempo reale con tutti i client peer:

* Modificare una risorsa (generatore, editor di immagini e così via)
* Rinominare una risorsa
* Eliminare una risorsa
* Spostare una risorsa
* Caricare una o più risorse (sia desktop che FTP)
* Creare, eliminare o rinominare una cartella

Dopo aver apportato una modifica nel client di origine, tutti i client peer connessi alla stessa azienda vengono aggiornati con la modifica. Le modifiche vengono applicate ai client peer senza alcuna notifica, a meno che non sia in corsa la modifica di una delle risorse da aggiornare negli editor di immagini o negli strumenti di generazione.

Quando si esegue l&#39;accesso, viene richiesto di consentire o negare gli aggiornamenti peer. È possibile ricordare la scelta ed evitare così che tale notifica venga successivamente riproposta. Per annullare la scelta, eliminate il sito appropriato dal pannello Connettività peer-to-peer in Impostazioni globali.

Se state modificando una risorsa modificata da un utente peer, viene richiesto di inserire la modifica nello strumento di generazione o nell’editor. Se si sceglie **[!UICONTROL Sì]** Quindi il generatore o l’editor elimina eventuali modifiche apportate alla risorsa e importa la risorsa aggiornata. Se si sceglie **[!UICONTROL No]**, la risorsa rimane invariata nel generatore o nell’editor e tutte le modifiche apportate persistono in quella sessione.

Quando salvate la risorsa, viene visualizzato un avviso di nuova versione e potete scegliere se sovrascrivere la risorsa con le modifiche che avete apportato.
