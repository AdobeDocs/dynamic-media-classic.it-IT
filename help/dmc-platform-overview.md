---
title: Panoramica del programma Adobe Dynamic Media Classic
description: Panoramica del programma Adobe Dynamic Media Classic e del processo del flusso di lavoro.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 29%

---

# Panoramica del programma Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic è un ambiente integrato per la gestione, la pubblicazione e il server di contenuti multimediali. I contenuti multimediali possono essere distribuiti a tutti i canali di marketing e vendita, incluso il Web, materiale stampato, campagne e-mail, portali Web, desktop e dispositivi.

## Processo del flusso di lavoro {#workflow-process}

Adobe chiave dei passaggi del flusso di lavoro di Dynamic Media Classic:

* **Carica e gestisci le risorse** : carica le risorse multimediali in Adobe Dynamic Media Classic. Potete organizzare, sfogliare ed effettuare ricerche di risorse nel sistema, nonché applicarvi metadati.

* **Crea rich media** : crea diverse configurazioni delle risorse come eCatalog, set di immagini, set 360 gradi, set di campioni, set di file multimediali diversi, modelli di base e modelli FXG.

* **Pubblica e amministra** : consente di pubblicare risorse nella rete Adobe Dynamic Media Classic SaaS, nonché di monitorare lo stato delle risorse quando vengono pubblicate, amministrare i diritti utente e mantenere la sicurezza.

* **Serve** : fornire contenuti dalla rete SaaS Adobe Dynamic Media Classic alle pagine web, alle applicazioni e ai dispositivi mobili; i supporti sono ottimizzati per le prestazioni e vengono forniti con la memorizzazione in cache CDN. Adobe Dynamic Media Classic fornisce un URL per ogni risorsa. Una volta pubblicata la risorsa, l’URL diviene attivo.

![Il processo del flusso di lavoro Adobe Dynamic Media Classic](/help/assets/gs_workflow.png)

## Singole immagini principali e singoli richiami URL {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic è fondamentalmente diverso dagli altri sistemi perché puoi utilizzare Adobe Dynamic Media Classic per distribuire i contenuti in modo dinamico dalle singole risorse master e dalle chiamate URL.

Le stringhe URL generate con Adobe Dynamic Media Classic includono istruzioni che indicano al server come visualizzare la risorsa quando viene distribuita. Ad esempio, la stessa immagine principale può essere pubblicata in diversi dimensioni, formati, colori e visualizzazioni zoom. Per creare e pubblicare risorse multimediali con Adobe Dynamic Media Classic, è necessario configurare visivamente gli effetti. Durante tale procedura, vengono creati i richiami URL che contengono tutte le informazioni necessarie al server riguardo come presentare la risorsa principale alle applicazioni.

![Ad Adobe, Dynamic Media Classic può distribuire la stessa immagine master a diversi supporti in diverse dimensioni e formati.](/help/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic garantisce che esperienze di qualità e coerenza vengano distribuite a qualsiasi schermo, indipendentemente dalle dimensioni o dalla larghezza di banda.*

## Memorizzazione dei contenuti nella cache {#content-caching}

Le immagini generate dinamicamente da Adobe Dynamic Media Classic sono compatibili con la cache; in genere si tratta di immagini JPEG con chiamate URL univoche che le identificano. Le immagini vengono pubblicate sulla rete CDN (content delivery network, rete di distribuzione dei contenuti), un sistema di server in rete su Internet che consente di trasmettere i contenuti più rapidamente. Le immagini vengono distribuite dai server a livello globale ai computer degli utenti. Quando si implementa un meccanismo di caching utilizzando un fornitore CDN, è sufficiente cambiare il nome del server in modo che indirizzi al server immagini Dynamic Media abilitato per CDN. Tutte le edizioni Adobe Dynamic Media Classic includono il caching della rete CDN in bundle.
