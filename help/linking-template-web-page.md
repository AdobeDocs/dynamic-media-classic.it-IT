---
title: Collegamento di un modello a una pagina Web
description: Scopri come collegare un modello a una pagina web.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
translation-type: tm+mt
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 50%

---

# Collegamento di un modello a una pagina Web{#linking-a-template-to-a-web-page}

I siti web e le applicazioni accedono al contenuto di Dynamic Media Image Server tramite le stringhe URL. Dopo aver pubblicato un modello, Dynamic Media Classic attiva una stringa URL che fa riferimento al modello sui server di immagini Dynamic Media. Potete incollare questo URL in un browser Web per testarlo.

Per inserire stringhe URL nelle pagine web e nelle applicazioni, copiale da Dynamic Media Classic. Per ottenere una stringa URL generata tramite un predefinito per modelli, passate alla schermata Anteprima o al pannello Sfoglia (in visualizzazione Dettagli). Quindi selezionate un predefinito immagine e fate clic sul pulsante Copia URL.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Ottenimento di un URL per un modello  {#obtaining-a-template-url}

Potete ottenere una stringa URL per il modello, generata da un predefinito immagine dalla schermata Anteprima modello. Una volta copiato, l’URL viene inserito negli Appunti ed è pronto per essere incollato. Per ottenere una stringa URL del modello generata con un predefinito immagine dalla pagina Anteprima modello, procedi come segue:

1. Fai clic sul pulsante rollover del modello **[!UICONTROL Anteprima]** o scegli **[!UICONTROL File]** > **[!UICONTROL Anteprima]**.
1. Usando i menu dei predefiniti, scegliete il predefinito per immagini che desiderate fornire all’immagine modello. La pagina Anteprima mostra l’aspetto del modello quando viene consegnato dal server.
1. Fai clic su **[!UICONTROL Copia URL]** per copiare l&#39;URL negli Appunti.

## Aggiunta di URL modello alla pagina Web {#adding-template-urls-to-your-web-page}

Per aggiungere un modello alla pagina web, rivolgiti al team di sviluppo della pagina web per modificare il tag `<IMG>` nel codice della pagina web HTML. Utilizza la stringa URL Dynamic Media Classic per effettuare una richiesta ai server di immagini Dynamic Media. Il motore del sito commerce o il codice della pagina Web dinamica inserisce l’immagine modello in base alle dimensioni e specifiche di formattazione definite dal predefinito per immagini che scegliete per il modello.

>[!MORELIKETHIS]
>
>* [Aggiunta di immagini dinamiche alla pagina Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

