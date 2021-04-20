---
title: Panoramica della piattaforma Adobe Dynamic Media Classic
description: Panoramica del processo di piattaforma e flusso di lavoro di Dynamic Media Classic.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 32%

---


# Adobe Panoramica della piattaforma Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic è un ambiente integrato di gestione, pubblicazione e distribuzione di contenuti multimediali. I contenuti multimediali possono essere distribuiti a tutti i canali di marketing e vendita, incluso il Web, materiale stampato, campagne e-mail, portali Web, desktop e dispositivi.

## Processo del flusso di lavoro  {#workflow-process}

I passaggi chiave del flusso di lavoro di Dynamic Media Classic sono i seguenti:

* **Carica e gestisci le**
risorseCarica le risorse multimediali in Dynamic Media Classic. Potete organizzare, sfogliare ed effettuare ricerche di risorse nel sistema, nonché applicarvi metadati.

* **Crea**
contenuti multimediali avanzatiCrea configurazioni diverse delle risorse come eCatalog, set di immagini, set 360 gradi, set di campioni, set di file multimediali diversi, modelli di base e modelli FXG. Per ulteriori informazioni, consultate I contenuti multimediali.

* **Pubblicare e**
amministrare le risorsePubblicare sulla rete Saas di Dynamic Media Classic, nonché monitorare lo stato delle risorse quando vengono pubblicate, amministrare i diritti utente e mantenere la sicurezza.

* ****
Distribuzione di contenuti multimediali dalla rete SaaS di Dynamic Media Classic a pagine web, applicazioni e dispositivi mobili; i supporti sono ottimizzati per le prestazioni e vengono forniti con la memorizzazione in cache CDN. Dynamic Media Classic fornisce un URL per ogni risorsa. Una volta pubblicata la risorsa, l’URL diviene attivo.

![Il processo del flusso di lavoro di Dynamic Media Classic](/help/assets/gs_workflow.png)

## Singole immagini principali e singoli richiami URL {#single-master-images-and-single-url-calls}

Dynamic Media Classic è fondamentalmente diverso dagli altri sistemi perché è possibile utilizzare Dynamic Media Classic per distribuire i contenuti in modo dinamico dalle singole risorse master e dalle chiamate URL.

Le stringhe URL generate con Dynamic Media Classic includono istruzioni che indicano al server come visualizzare la risorsa quando viene distribuita. Ad esempio, la stessa immagine principale può essere pubblicata in diversi dimensioni, formati, colori e visualizzazioni zoom. Per creare e pubblicare risorse multimediali con Dynamic Media Classic, è necessario configurare visivamente gli effetti. Durante tale procedura, vengono creati i richiami URL che contengono tutte le informazioni necessarie al server riguardo come presentare la risorsa principale alle applicazioni.

![Dynamic Media Classic è in grado di fornire la stessa immagine master a diversi supporti in diverse dimensioni e formati.](/help/assets/gs_dynamic_publishing.png)

## Memorizzazione dei contenuti nella cache {#content-caching}

Le immagini generate dinamicamente da Dynamic Media Classic sono compatibili con la cache; nella maggior parte dei casi si tratta di immagini JPEG con chiamate URL univoche che le identificano. Le immagini vengono pubblicate sulla rete CDN (content delivery network, rete di distribuzione dei contenuti), un sistema di server in rete su Internet che consente di trasmettere i contenuti più rapidamente. Le immagini vengono distribuite dai server a livello globale ai computer degli utenti. Quando si implementa un meccanismo di caching utilizzando un fornitore CDN, è sufficiente cambiare il nome del server in modo che indirizzi al server immagini Dynamic Media abilitato per CDN. Tutte le edizioni di Dynamic Media Classic includono il caching CDN in bundle.
