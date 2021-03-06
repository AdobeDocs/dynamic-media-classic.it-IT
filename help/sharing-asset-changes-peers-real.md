---
title: Condividere le modifiche delle risorse con i peer in tempo reale
description: Scopri come condividere le modifiche alle risorse con i colleghi in tempo reale in Adobe Dynamic Media Classic.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 44%

---

# Condividere le modifiche delle risorse con i peer in tempo reale{#sharing-asset-changes-with-peers-in-real-time}

Con più copie di Adobe Dynamic Media Classic in esecuzione su più computer della stessa azienda, le azioni seguenti di qualsiasi client Dynamic Media Classic di Adobe vengono aggiornate in tempo reale con tutti i client peer:

* Modificare una risorsa (generatore, editor di immagini e così via)
* Rinominare una risorsa
* Eliminare una risorsa
* Spostare una risorsa
* Caricare una o più risorse (sia desktop che FTP)
* Creare, eliminare o rinominare una cartella

Dopo aver apportato una modifica nel client di origine, tutti i client peer firmati nella stessa società vengono aggiornati con la modifica. Le modifiche vengono applicate ai client peer senza alcuna notifica, a meno che non sia in corsa la modifica di una delle risorse da aggiornare negli editor di immagini o negli strumenti di generazione.

Quando effettui l’accesso, ti viene richiesto di consentire o negare gli aggiornamenti peer. È possibile ricordare la scelta ed evitare così che tale notifica venga successivamente riproposta. Per annullare la scelta, eliminate il sito appropriato dal pannello Connettività peer-to-peer in Impostazioni globali.

Se state modificando una risorsa modificata da un utente peer, viene richiesto di inserire la modifica nello strumento di generazione o nell’editor. Se scegli **[!UICONTROL Sì]**, il generatore o l’editor elimina le modifiche apportate alla risorsa e importa la risorsa aggiornata. Se scegli **[!UICONTROL No]**, la risorsa rimane invariata nel generatore o nell’editor e le eventuali modifiche apportate persistono in quella sessione.

Quando salvate la risorsa, viene visualizzato un avviso di nuova versione e potete scegliere se sovrascrivere la risorsa con le modifiche che avete apportato.
