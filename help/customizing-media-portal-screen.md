---
title: Personalizzazione della schermata di Media Portal
description: Scopri come personalizzare la schermata Media Portal.
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 51%

---


# Personalizzazione della schermata di Media Portal{#customizing-the-media-portal-screen}

Le impostazioni di stile di Media Portal consentono di personalizzare la schermata di Media Portal con il logo e i colori aziendali. Utilizzate le impostazioni di stile per inserire in Media Portal il vostro logo aziendale. 

Per accedere alle impostazioni di stile, scegliete **Configurazione** > **Configurazione Media Portal** > **Impostazioni stile**. Accertatevi di fare clic su **Salva** per salvare le impostazioni modificate. Se necessario, per ripristinare le impostazioni predefinite potete fare clic su **Ripristina**. Mentre selezionate le opzioni desiderate, nel pannello Anteprima viene riportato il relativo risultato.

**** LogoFai clic su Sfoglia e scegli un grafico nella finestra Seleziona immagine logo.

**** ApplicazioneCreate una blend di colore con sfumatura effettuando le scelte sui menu Colori sfumatura sfondo.

**** AlberoScegli un colore di rollover (il colore visualizzato quando il puntatore viene spostato su un elemento) e un colore di selezione (il colore visualizzato quando selezioni un elemento).

**** Pannello a soffiettoScegli i colori di sfondo, uno stile del bordo e i colori rollover e selezionati per il pannello a soffietto che appare sul lato destro dello schermo nella vista Dettagli.

**Intestazione** pannello a soffiettoScegliere se creare testo nel grassetto dell&#39;intestazione del pannello a soffietto.

**** DatagridScegli i colori per la riga di intestazione nelle griglie dati.

**** AvvisoScegliere un colore di sfondo per le finestre dei messaggi di avviso.

**Barra** di avanzamentoScegli un colore per la barra che indica l’avanzamento dei caricamenti e dei download.

Affinché gli utenti del Media Portal possano vedere le impostazioni di stile selezionate, devono aggiungere `?company=(company name)` all’URL con cui accedono a Media Portal. Ad esempio, per vedere le impostazioni di stile, gli utenti di Media Portal che accedono alla società PortalCo mediante l’URL seguente:

`https://s7sps1.scene7.com/MediaPortal`

devono utilizzare invece il seguente URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

L’inclusione del nome della società nell’URL consente a Media Portal di riconoscere la società a cui desidera accedere l’utente e di applicare quindi le relative impostazioni di stile.

È possibile ottenere ulteriori informazioni su come comunicare modifiche di URL agli utenti Media Portal, nonché su come impostare un messaggio e-mail di benvenuto mediante il quale i nuovi utenti possono ricevere l’URL corretto per Media Portal.

Consultate [Impostare il messaggio di benvenuto per gli utenti di Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
