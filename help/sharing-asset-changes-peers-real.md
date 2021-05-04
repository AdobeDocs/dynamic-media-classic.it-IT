---
title: Condivisione di modifiche di risorse con client peer in tempo reale
description: Scopri come condividere in tempo reale i cambiamenti delle risorse con i colleghi.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic, Gestione risorse, Collaborazione
role: Administrator,Business Practitioner
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
translation-type: tm+mt
source-git-commit: 9d73e74ffc4a1e7e31c84720a9bae105b6afb1ae
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 50%

---

# Condivisione di modifiche di risorse con client peer in tempo reale{#sharing-asset-changes-with-peers-in-real-time}

Con più copie di Dynamic Media Classic in esecuzione su uno o più computer della stessa azienda, le seguenti azioni di qualsiasi client Dynamic Media Classic vengono aggiornate in tempo reale con tutti i client peer:

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
