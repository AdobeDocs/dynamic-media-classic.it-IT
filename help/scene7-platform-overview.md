---
title: Panoramica della piattaforma Adobe Dynamic Media Classic
seo-title: Panoramica della piattaforma Adobe Dynamic Media Classic
description: 'null'
seo-description: Panoramica della piattaforma Dynamic Media Classic e del flusso di lavoro.
uuid: e 7 d 3 bfb 3-1 cfe -43 ea-b 862-aae 3 b 3928 c 71
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/getting_ started
discoiquuid: 2 b 134 cfa -7 f 46-4 f 5 f -959 e-b 30 aae 610 bb 9
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Panoramica della piattaforma Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic è un ambiente integrato, di gestione multimediale, pubblicazione e di distribuzione. I contenuti multimediali possono essere distribuiti a tutti i canali di marketing e vendita, incluso il Web, materiale stampato, campagne e-mail, portali Web, desktop e dispositivi.

## Processo del flusso di lavoro {#workflow-process}

I passaggi principali del flusso di lavoro Dynamic Media Classic sono:

**Caricamento e gestione delle risorse** Consente di caricare le risorse multimediali in SPS. Potete organizzare, sfogliare ed effettuare ricerche di risorse nel sistema, nonché applicarvi metadati. Se installate l’applicazione desktop Adobe Scene7 Publishing System, potete caricare i file e le cartelle trascinandoli dal desktop a una cartella di caricamento.

**Creazione di contenuti multimediali** diversi Create configurazioni diverse di risorse come ecatalog, Set di immagini, Set gradi, Set di campioni, Set di file multimediali diversi, Modelli di base e Modelli FXG. Per ulteriori informazioni, consultate I contenuti multimediali.

**Pubblicate e amministrate** le risorse pubblicate nella rete Dynamic Media Saas, e monitorate lo stato delle risorse pubblicate, amministrate i diritti degli utenti e mantenete la sicurezza.

**Trasmettere** contenuti multimediali dalla rete Saas Dynamic Media Classic a pagine Web, applicazioni e dispositivi mobili; i contenuti multimediali sono ottimizzati per le prestazioni e vengono distribuiti con cache CDN. Dynamic Media Classic fornisce un URL per ciascuna risorsa. Una volta pubblicata la risorsa, l’URL diviene attivo.

![Processo Flusso di lavoro Dynamic Media Classic](/help/assets/gs_workflow.png)

## Singole immagini principali e singoli richiami URL {#single-master-images-and-single-url-calls}

Dynamic Media Classic è sostanzialmente diverso da altri sistemi perché potete utilizzare Dynamic Media Classic per distribuire contenuti multimediali in modo dinamico da singole risorse principali e chiamate URL.

Le stringhe URL generate con Dynamic Media Classic includono istruzioni che informano il server su come visualizzare la risorsa quando viene pubblicata. Ad esempio, la stessa immagine principale può essere pubblicata in diversi dimensioni, formati, colori e visualizzazioni zoom. Per la creazione e la pubblicazione di risorse multimediali con Dynamic Media Classic, potete configurare visivamente gli effetti. Durante tale procedura, vengono creati i richiami URL che contengono tutte le informazioni necessarie al server riguardo come presentare la risorsa principale alle applicazioni.

![Dynamic Media Classic può trasmettere la stessa immagine principale a diversi supporti in diversi formati e formati.](/help/assets/gs_dynamic_publishing.png)

## Memorizzazione dei contenuti nella cache {#content-caching}

Le immagini generate da Dynamic Media Classic sono basate su cache, nella maggior parte dei casi, si tratta di immagini JPEG con chiamate URL univoche che li identificano. Le immagini vengono pubblicate sulla rete CDN (content delivery network, rete di distribuzione dei contenuti), un sistema di server in rete su Internet che consente di trasmettere i contenuti più rapidamente. Le immagini vengono distribuite dai server a livello globale ai computer degli utenti. Quando implementate un meccanismo di cache utilizzando un operatore CDN, dovete semplicemente cambiare il nome del server in modo che punti al server di immagini Dynamic Media per CDN abilitato. Tutte le edizioni Dynamic Media Classic includono la cache CDN fornita.
