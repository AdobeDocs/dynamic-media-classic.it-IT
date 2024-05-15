---
title: Panoramica del programma Adobe Dynamic Media Classic
description: Panoramica del programma Adobe Dynamic Media Classic e dell'intero processo di workflow.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: edd893482cbafd9674a44cf9878b8ee3079d98f7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 12%

---

# Panoramica del programma Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic è un ambiente integrato di gestione, pubblicazione e distribuzione di contenuti rich media. I rich media possono essere distribuiti a tutti i canali di marketing e vendita. Questi canali includono il web, il materiale per la stampa, le campagne e-mail, i portali web, i desktop e i dispositivi.

Vedi anche [Panoramica della piattaforma](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) video di formazione.

## Processo del flusso di lavoro {#workflow-process}

I passaggi chiave del flusso di lavoro di Adobe Dynamic Media Classic sono i seguenti:

* **Caricare e gestire le risorse** - Carica le risorse multimediali in Adobe Dynamic Media Classic. Potete organizzare, sfogliare ed effettuare ricerche di risorse nel sistema, Puoi anche applicare i metadati alle risorse.

* **Creare rich media** : crea diverse configurazioni delle risorse, ad esempio eCatalog, Set di immagini, Set 360 gradi, Set di campioni, Set di file multimediali diversi, Modelli di base e Modelli FXG.

* **Pubblicare e amministrare** - Pubblicare risorse sulla rete SaaS di Adobe Dynamic Media Classic. Monitora lo stato delle risorse quando vengono pubblicate. Amministra i diritti utente e mantieni la sicurezza.

* **Serve** - Distribuisci contenuti multimediali dalla rete Adobe Dynamic Media Classic SaaS a pagine web, applicazioni e dispositivi mobili; i contenuti multimediali sono ottimizzati in termini di prestazioni e vengono forniti con caching CDN. Adobe Dynamic Media Classic fornisce un URL per ogni risorsa. Una volta pubblicata la risorsa, l’URL diviene attivo.

![Il processo del flusso di lavoro di Adobe Dynamic Media Classic](/help/using/assets/gs_workflow.png)

## Immagini primarie singole e chiamate URL singole {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic è fondamentalmente diverso da altri sistemi perché puoi utilizzare Adobe Dynamic Media Classic per distribuire i contenuti multimediali in modo dinamico da singole risorse primarie e chiamate URL.

Le stringhe URL generate con Adobe Dynamic Media Classic includono istruzioni che indicano al server come visualizzare la risorsa quando viene distribuita. Ad esempio, la stessa immagine primaria può essere distribuita in diverse visualizzazioni di dimensioni, formati, pesi, colori e zoom. Come parte della creazione e pubblicazione di risorse multimediali con Adobe Dynamic Media Classic, puoi configurare visivamente gli effetti. In questo modo, puoi creare le chiamate URL che indicano correttamente al server come presentare la risorsa principale alle applicazioni.

![Adobe Dynamic Media Classic è in grado di fornire la stessa immagine primaria a supporti diversi in formati e dimensioni diversi.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic garantisce che esperienze coerenti e di qualità vengano trasmesse a qualsiasi schermo, indipendentemente dalle dimensioni o dalla larghezza di banda.*

## Memorizzazione dei contenuti nella cache {#content-caching}

Le immagini generate dinamicamente da Adobe Dynamic Media Classic sono favorevoli alla cache; in genere, sono immagini JPEG con chiamate URL univoche che le identificano. Le immagini vengono pubblicate sulla rete CDN (content delivery network, rete di distribuzione dei contenuti), un sistema di server in rete su Internet che consente di trasmettere i contenuti più rapidamente. Le immagini vengono distribuite dai server a livello globale ai computer degli utenti. Quando si implementa un meccanismo di caching utilizzando un fornitore CDN, è sufficiente modificare il nome del server in modo che punti al server immagini Dynamic Medie abilitato per CDN. Tutte le edizioni di Adobe Dynamic Media Classic includono il caching CDN in bundle.
