---
title: Collegamento di un modello a una pagina Web
seo-title: Collegamento di un modello a una pagina Web
description: 'null'
seo-description: Scopri come collegare un modello a una pagina Web.
uuid: f 111 ef 06-4 afc -454 c -86 ce -5 d 640236 d 40 b
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/template_ basics
discoiquuid: 989 dba 07-448 a -45 b 1-b 157-af 50 abb 5359 a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Collegamento di un modello a una pagina Web{#linking-a-template-to-a-web-page}

I siti Web e le applicazioni accedono al contenuto del server di immagini Dynamic Media tramite stringhe URL. Dopo aver pubblicato un modello, Dynamic Media Classic attiva una stringa URL che fa riferimento al modello sui server immagini Dynamic Media. Potete incollare questo URL in un browser Web per testarlo.

Per inserire queste stringhe di URL nelle pagine Web e nelle applicazioni, copiatele da Scene7 Publishing System. Per ottenere una stringa URL generata tramite un predefinito per modelli, passate alla schermata Anteprima o al pannello Sfoglia (in visualizzazione Dettagli). Quindi selezionate un predefinito immagine e fate clic sul pulsante Copia URL.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Ottenimento di un URL per un modello {#obtaining-a-template-url}

Potete ottenere una stringa URL per il modello, generata da un predefinito immagine dalla schermata Anteprima modello. Una volta copiato, l’URL viene inserito negli Appunti ed è pronto per essere incollato. Per ottenere una stringa URL per il modello, generata tramite un predefinito per modelli dalla schermata Anteprima, effettuate le seguenti operazioni:

1. Fate clic sul pulsante rollover Anteprima o scegliete File &gt; Anteprima. Viene visualizzata la schermata Anteprima.
1. Usando i menu dei predefiniti, scegliete il predefinito per immagini che desiderate fornire all’immagine modello. Nella schermata Anteprima viene visualizzato l’aspetto del modello che verrà trasmesso dal server.
1. Per copiare l’URL negli Appunti, fate clic sul pulsante Copia URL.

## Aggiunta di URL modello alla pagina Web {#adding-template-urls-to-your-web-page}

To add a template to your web page, consult with your web page development team to modify the `<IMG>` tag in your HTML web page code using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. Il motore del sito commerce o il codice della pagina Web dinamica inserisce l’immagine modello in base alle dimensioni e specifiche di formattazione definite dal predefinito per immagini che scegliete per il modello.

>[!MORELIKETHIS]
>
>* [Aggiunta di immagini dinamiche alla pagina Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

