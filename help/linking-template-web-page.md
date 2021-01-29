---
title: Collegamento di un modello a una pagina Web
description: Scoprite come collegare un modello a una pagina Web.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 69%

---


# Collegamento di un modello a una pagina Web{#linking-a-template-to-a-web-page}

I siti Web e le applicazioni accedono al contenuto di Dynamic Media Image Server tramite le stringhe URL. Dopo aver pubblicato un modello, Dynamic Media Classic attiva una stringa URL che fa riferimento al modello sui server immagini Dynamic Media. Potete incollare questo URL in un browser Web per testarlo.

Per inserire stringhe URL nelle pagine Web e nelle applicazioni, copiatele da Dynamic Media Classic. Per ottenere una stringa URL generata tramite un predefinito per modelli, passate alla schermata Anteprima o al pannello Sfoglia (in visualizzazione Dettagli). Quindi selezionate un predefinito immagine e fate clic sul pulsante Copia URL.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Ottenimento di un URL per un modello  {#obtaining-a-template-url}

Potete ottenere una stringa URL per il modello, generata da un predefinito immagine dalla schermata Anteprima modello. Una volta copiato, l’URL viene inserito negli Appunti ed è pronto per essere incollato. Per ottenere una stringa URL per il modello, generata tramite un predefinito per modelli dalla schermata Anteprima, effettuate le seguenti operazioni:

1. Fate clic sul pulsante rollover Anteprima o scegliete File > Anteprima. Viene visualizzata la schermata Anteprima.
1. Usando i menu dei predefiniti, scegliete il predefinito per immagini che desiderate fornire all’immagine modello. Nella schermata Anteprima viene visualizzato l’aspetto del modello che verrà trasmesso dal server.
1. Per copiare l’URL negli Appunti, fate clic sul pulsante Copia URL.

## Aggiunta di URL modello alla pagina Web  {#adding-template-urls-to-your-web-page}

Per aggiungere un modello alla pagina Web, rivolgetevi al team di sviluppo Web per modificare il tag `<IMG>` nel codice HTML della pagina Web utilizzando la stringa URL Dynamic Media Classic per effettuare una richiesta ai server immagini Dynamic Media. Il motore del sito commerce o il codice della pagina Web dinamica inserisce l’immagine modello in base alle dimensioni e specifiche di formattazione definite dal predefinito per immagini che scegliete per il modello.

>[!MORELIKETHIS]
>
>* [Aggiunta di immagini dinamiche alla pagina Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

