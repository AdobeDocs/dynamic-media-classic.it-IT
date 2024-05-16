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
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 16%

---

# Collegare un modello a una pagina Web{#linking-a-template-to-a-web-page}

I siti Web e le applicazioni accedono al contenuto di Dynamic Medie Image Server tramite stringhe URL. Dopo aver pubblicato un modello, Adobe Dynamic Media Classic attiva una stringa URL che fa riferimento al modello nei server immagini Dynamic Medie. Puoi incollare questo URL in un browser Web per la verifica.

Per inserire stringhe URL nelle pagine Web e nelle applicazioni, copiarle da Adobe Dynamic Media Classic. Per ottenere una stringa dell’URL del modello generata con un predefinito immagine, passa alla schermata Anteprima o al pannello Sfoglia (in Vista dettagli). Quindi selezionate un predefinito immagine e fate clic sul pulsante Copia URL.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Ottenere un URL modello {#obtaining-a-template-url}

Potete ottenere una stringa URL per il modello, generata da un predefinito immagine dalla schermata Anteprima modello. Una volta copiato, l’URL viene inserito negli Appunti ed è pronto per essere incollato. Per ottenere una stringa dell&#39;URL del modello generata con un predefinito immagine dalla pagina Anteprima modello, effettuate le seguenti operazioni:

1. Seleziona il rollover del modello **[!UICONTROL Anteprima]** o vai a **[!UICONTROL File]** > **[!UICONTROL Anteprima]**.
1. Utilizzando i menu del predefinito, scegliete il predefinito immagine con cui desiderate distribuire l&#39;immagine modello. La pagina Anteprima mostra l’aspetto del modello quando viene distribuito dal server.
1. Seleziona **[!UICONTROL Copia URL]** in modo da poter copiare l’URL negli Appunti.

## Aggiungere URL modello alla pagina Web {#adding-template-urls-to-your-web-page}

Per aggiungere un modello alla pagina Web, consultare il team di sviluppo della pagina Web per modificare `<IMG>` nel codice della pagina Web HTML. Utilizza la stringa URL Adobe Dynamic Media Classic per effettuare una richiesta ai server immagini Dynamic Medie. Il codice del motore di e-commerce o della pagina Web dinamica inserisce l&#39;immagine modello nelle dimensioni e con le specifiche di formattazione definite dal predefinito immagine scelto per il modello.

>[!MORELIKETHIS]
>
>* [Aggiungere immagini dinamiche alla pagina Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
