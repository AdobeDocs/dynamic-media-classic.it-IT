---
title: Condivisione di modifiche di risorse con client peer in tempo reale
seo-title: Condivisione di modifiche di risorse con client peer in tempo reale
description: 'null'
seo-description: Scopri come condividere le modifiche di risorse con i colleghi in tempo reale.
uuid: 13 fa 4 f 6 e -66 bf -4682-96 a 9-0 e 7040706 f 53
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: ca 7 c 8 a 7 f -76 f 4-4 a 25-8 c 36-617 a 029 e 55 be
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Condivisione di modifiche di risorse con client peer in tempo reale{#sharing-asset-changes-with-peers-in-real-time}

Con più copie di Dynamic Media Classic eseguite su uno o più computer della stessa società, le seguenti azioni da qualsiasi client Dynamic Media Classic vengono aggiornate in tempo reale con tutti i client peer:

* Modifica di una risorsa (strumento di generazione, editor di immagini, ecc.)
* Rinominare una risorsa
* Eliminare una risorsa
* Spostare una risorsa
* Caricare una o più risorse (sia desktop che FTP)
* Creare, eliminare o rinominare una cartella

Dopo che viene apportata una modifica nel client di origine, tutti i client peer connessi nella stessa società vengono aggiornati di conseguenza. Le modifiche vengono applicate ai client peer senza alcuna notifica, a meno che non sia in corsa la modifica di una delle risorse da aggiornare negli editor di immagini o negli strumenti di generazione.

Quando effettuate l’accesso, una notifica di Flash Player richiede se accettare o rifiutare gli aggiornamenti peer. È possibile ricordare la scelta ed evitare così che tale notifica venga successivamente riproposta. Per annullare la scelta, eliminate il sito appropriato dal pannello Connettività peer-to-peer in Impostazioni globali.

Se state modificando una risorsa modificata da un utente peer, viene richiesto di inserire la modifica nello strumento di generazione o nell’editor. Se scegliete Sì, le modifiche apportate alla risorsa vengono eliminate e viene reimportata la risorsa aggiornata. Se scegliete No, la risorsa resta inalterata nel modulo di generazione o nell’editor e vengono mantenute le modifiche che avete apportato nella sessione corrente.

Quando salvate la risorsa, viene visualizzato un avviso di nuova versione e potete scegliere se sovrascrivere la risorsa con le modifiche che avete apportato.
