---
title: Collegare un modello a una pagina Web
description: Scopri come collegare un modello a una pagina Web in Adobe Systems Dynamic Media Classic.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 37%

---

# Collegare un modello a una pagina Web{#linking-a-template-to-a-web-page}

I siti Web e le applicazioni accesso Dynamic Media Immagine server contenuto a mezzo di stringhe URL. Dopo aver pubblicare un modello, Adobe Systems Dynamic Media Classic attiva una stringa di URL che fa riferimento al modello su Dynamic Media Immagine server. Potete incollare questo URL in un browser Web per testarlo.

Per inserire URL stringhe nelle pagine Web e applicazioni, copiarle da Adobe Systems Dynamic Media Classic. Per ottenere un modello URL stringa generata con un Immagine predefinito, passate alla schermata Anteprima o al pannello Sfoglia (in dettaglio Visualizza). Quindi selezionate un predefinito immagine e fate clic sul pulsante Copia URL.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Ottenere un modello URL {#obtaining-a-template-url}

Potete ottenere una stringa URL per il modello, generata da un predefinito immagine dalla schermata Anteprima modello. Una volta copiato, l’URL viene inserito negli Appunti ed è pronto per essere incollato. Per ottenere un modello URL stringa generata con un Immagine predefinito dalla pagina Anteprima modello, effettuate le seguenti operazioni:

1. Seleziona il Anteprima ]**di rollover**[!UICONTROL  del modello pulsante o vai a **[!UICONTROL file]** > **[!UICONTROL Anteprima]** .
1. Usando i menu dei predefiniti, scegliete il predefinito per immagini che desiderate fornire all’immagine modello. La pagina Anteprima Mostra l&#39;aspetto del modello like quando viene consegnato dal server.
1. Selezionate **[!UICONTROL copia URL]** in modo da poter copiare il URL in Appunti.

## Aggiungere URL modello alla pagina Web {#adding-template-urls-to-your-web-page}

Per aggiungere un modello alla pagina Web, consulta il team di sviluppo della pagina Web per modificare le tag nel codice della `<IMG>` pagina Web HTML. Utilizza la stringa Adobe Systems Dynamic Media URL classica per creare un richiesta per Dynamic Media immagine server. Il motore del sito commerce o il codice della pagina Web dinamica inserisce l’immagine modello in base alle dimensioni e specifiche di formattazione definite dal predefinito per immagini che scegliete per il modello.

>[!MORELIKETHIS]
>
>* [Aggiungere immagini dinamiche alla pagina Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

