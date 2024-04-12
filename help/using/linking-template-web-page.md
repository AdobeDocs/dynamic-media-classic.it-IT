---
title: Collegare un modello a una pagina Web
description: Scopri come collegare un modello a una pagina web in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 32%

---

# Collegare un modello a una pagina Web{#linking-a-template-to-a-web-page}

I siti Web e le applicazioni accedono al contenuto di Dynamic Medie Image Server tramite stringhe URL. Dopo aver pubblicato un modello, Adobe Dynamic Media Classic attiva una stringa URL che fa riferimento al modello nei server immagini Dynamic Medie. Potete incollare questo URL in un browser Web per testarlo.

Per inserire stringhe URL nelle pagine Web e nelle applicazioni, copiale da Adobe Dynamic Media Classic. Per ottenere una stringa dell’URL del modello generata con un predefinito immagine, passa alla schermata Anteprima o al pannello Sfoglia (in Vista dettagli). Quindi selezionate un predefinito immagine e fate clic sul pulsante Copia URL.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Ottenere un URL modello {#obtaining-a-template-url}

Potete ottenere una stringa URL per il modello, generata da un predefinito immagine dalla schermata Anteprima modello. Una volta copiato, l’URL viene inserito negli Appunti ed è pronto per essere incollato. Per ottenere una stringa dell&#39;URL del modello generata con un predefinito immagine dalla pagina Anteprima modello, effettuate le seguenti operazioni:

1. Seleziona il rollover del modello **[!UICONTROL Anteprima]** o vai a **[!UICONTROL File]** > **[!UICONTROL Anteprima]**.
1. Utilizzando i menu del predefinito, scegliete il predefinito immagine con cui desiderate distribuire l&#39;immagine modello. La pagina Anteprima mostra l’aspetto del modello quando viene distribuito dal server.
1. Seleziona **[!UICONTROL Copia URL]** in modo da poter copiare l’URL negli Appunti.

## Aggiungere gli URL del modello alla pagina web {#adding-template-urls-to-your-web-page}

Per aggiungere un modello alla pagina web, rivolgiti al team di sviluppo della pagina web per modificare `<IMG>` nel codice della pagina web HTML. Utilizza la stringa URL Adobe Dynamic Media Classic per effettuare una richiesta ai server immagini Dynamic Medie. Il motore del sito commerce o il codice della pagina Web dinamica inserisce l’immagine modello in base alle dimensioni e specifiche di formattazione definite dal predefinito per immagini che scegliete per il modello.

>[!MORELIKETHIS]
>
>* [Aggiungere immagini dinamiche alla pagina web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
