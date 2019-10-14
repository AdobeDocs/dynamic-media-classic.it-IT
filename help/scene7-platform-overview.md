---
title: Panoramica della piattaforma Adobe Dynamic Media Classic
seo-title: Panoramica della piattaforma Adobe Dynamic Media Classic
description: 'null'
seo-description: Panoramica della piattaforma e del processo di workflow Dynamic Media Classic.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/Categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Panoramica della piattaforma Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic è un ambiente integrato per la gestione, la pubblicazione e la distribuzione di contenuti multimediali avanzati. I contenuti multimediali possono essere distribuiti a tutti i canali di marketing e vendita, incluso il Web, materiale stampato, campagne e-mail, portali Web, desktop e dispositivi.

## Processo del flusso di lavoro {#workflow-process}

I passaggi principali del flusso di lavoro per Dynamic Media Classic sono:

* **Caricate e gestite le risorse** Caricate le risorse multimediali in SPS. Potete organizzare, sfogliare ed effettuare ricerche di risorse nel sistema, nonché applicarvi metadati. Se installate l’applicazione desktop Adobe Scene7 Publishing System, potete caricare i file e le cartelle trascinandoli dal desktop a una cartella di caricamento.

* **Creazione di contenuti multimediali** Create configurazioni diverse delle risorse disponibili, ad esempio eCatalog, set di immagini, set 360 gradi, set di campioni, set di file multimediali diversi, modelli di base e modelli FXG. Per ulteriori informazioni, consultate I contenuti multimediali.

* **Pubblicate e amministrate** le risorse Pubblica sulla rete Saas di Dynamic Media Classic, nonché monitorate lo stato delle risorse al momento della pubblicazione, amministrate i diritti utente e mantenete la sicurezza.

* **Trasmettere** contenuti dalla rete SaaS di Dynamic Media Classic a pagine Web, applicazioni e dispositivi mobili; i supporti sono ottimizzati per le prestazioni e vengono distribuiti con la memorizzazione cache CDN. Dynamic Media Classic fornisce un URL per ciascuna risorsa. Una volta pubblicata la risorsa, l’URL diviene attivo.

![Processo del flusso di lavoro Dynamic Media Classic](/help/assets/gs_workflow.png)

## Singole immagini principali e singoli richiami URL {#single-master-images-and-single-url-calls}

Dynamic Media Classic è fondamentalmente diverso dagli altri sistemi perché è possibile utilizzare Dynamic Media Classic per distribuire i contenuti multimediali in modo dinamico da singole risorse principali e da richiami URL.

Le stringhe URL generate con Dynamic Media Classic includono istruzioni che informano il server su come visualizzare la risorsa quando viene distribuita. Ad esempio, la stessa immagine principale può essere pubblicata in diversi dimensioni, formati, colori e visualizzazioni zoom. Per creare e pubblicare risorse multimediali con Dynamic Media Classic, potete configurare visivamente gli effetti. Durante tale procedura, vengono creati i richiami URL che contengono tutte le informazioni necessarie al server riguardo come presentare la risorsa principale alle applicazioni.

![Dynamic Media Classic consente di distribuire la stessa immagine principale a diversi supporti in dimensioni e formati diversi.](/help/assets/gs_dynamic_publishing.png)

## Memorizzazione dei contenuti nella cache {#content-caching}

Le immagini generate dinamicamente da Dynamic Media Classic sono compatibili con la cache; nella maggior parte dei casi, si tratta di immagini JPEG con richiami URL univoci che le identificano. Le immagini vengono pubblicate sulla rete CDN (content delivery network, rete di distribuzione dei contenuti), un sistema di server in rete su Internet che consente di trasmettere i contenuti più rapidamente. Le immagini vengono distribuite dai server a livello globale ai computer degli utenti. Quando si implementa un meccanismo di caching utilizzando un fornitore CDN, è sufficiente cambiare il nome del server in modo da puntare al server di immagini per file multimediali dinamici abilitato per CDN. Tutte le edizioni Dynamic Media Classic includono il caching CDN incluso nel pacchetto.
