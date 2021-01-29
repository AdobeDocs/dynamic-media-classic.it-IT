---
title: Condivisione di modifiche di risorse con client peer in tempo reale
description: Scoprite come condividere le modifiche alle risorse con altri utenti in tempo reale.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 70%

---


# Condivisione di modifiche di risorse con client peer in tempo reale{#sharing-asset-changes-with-peers-in-real-time}

Con più copie di Dynamic Media Classic in esecuzione su uno o più computer della stessa società, le seguenti azioni da qualsiasi client Dynamic Media Classic vengono aggiornate in tempo reale con tutti i client peer:

* Modifica di una risorsa (strumento di generazione, editor di immagini, ecc.)
* Rinominare una risorsa
* Eliminare una risorsa
* Spostare una risorsa
* Caricare una o più risorse (sia desktop che FTP)
* Creare, eliminare o rinominare una cartella

Dopo aver apportato una modifica nel client di origine, tutti i client peer firmati nella stessa società vengono aggiornati di conseguenza. Le modifiche vengono applicate ai client peer senza alcuna notifica, a meno che non sia in corsa la modifica di una delle risorse da aggiornare negli editor di immagini o negli strumenti di generazione.

Quando effettuate l’accesso, vi viene richiesto di consentire o negare gli aggiornamenti peer. È possibile ricordare la scelta ed evitare così che tale notifica venga successivamente riproposta. Per annullare la scelta, eliminate il sito appropriato dal pannello Connettività peer-to-peer in Impostazioni globali.

Se state modificando una risorsa modificata da un utente peer, viene richiesto di inserire la modifica nello strumento di generazione o nell’editor. Se scegliete Sì, le modifiche apportate alla risorsa vengono eliminate e viene reimportata la risorsa aggiornata. Se scegliete No, la risorsa resta inalterata nel modulo di generazione o nell’editor e vengono mantenute le modifiche che avete apportato nella sessione corrente.

Quando salvate la risorsa, viene visualizzato un avviso di nuova versione e potete scegliere se sovrascrivere la risorsa con le modifiche che avete apportato.
