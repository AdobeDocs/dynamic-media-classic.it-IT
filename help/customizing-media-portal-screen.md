---
title: Personalizzazione della schermata di Media Portal
description: Scopri come personalizzare la schermata Media Portal.
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaborazione,Gestione risorse
role: Administrator,Business Practitioner
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
source-git-commit: 4e79c98b92dfa4e1a9890ed8a291cdf564126466
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 46%

---

# Personalizzazione della schermata di Media Portal{#customizing-the-media-portal-screen}

Le impostazioni di stile di Media Portal consentono di personalizzare la schermata di Media Portal con il logo e i colori aziendali. Utilizza le impostazioni di stile per inserire il marchio della tua azienda in Media Portal.

Per accedere alle impostazioni di stile, scegliete **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione Media Portal]** > **[!UICONTROL Impostazioni stile]**. Accertatevi di fare clic su **[!UICONTROL Salva]** per salvare le impostazioni modificate. Se necessario, per ripristinare le impostazioni predefinite potete fare clic su **[!UICONTROL Ripristina]**. Mentre selezionate le opzioni desiderate, nel pannello Anteprima viene riportato il relativo risultato.

* **Logo**  - Fai clic su  **** Browser e scegli un grafico nella finestra Seleziona immagine logo.

* **Applicazione** : consente di creare una blend di colore sfumato effettuando le scelte sui menu Colori sfumatura sfondo.

* **Struttura** : consente di scegliere un colore di rollover (il colore visualizzato quando si sposta il puntatore su un elemento) e un colore di selezione (il colore visualizzato quando si seleziona un elemento).

* **Pannello a soffietto**  - Consente di scegliere i colori di sfondo, uno stile del bordo e i colori rollover e selezionati per il pannello a soffietto visualizzato sul lato destro dello schermo nella vista Dettagli.

* **Intestazione pannello a soffietto**  - Consente di scegliere se creare testo nel grassetto dell’intestazione del pannello a soffietto.

* **Datagrid**  - Consente di scegliere i colori per la riga di intestazione nelle griglie dati.

* **Avviso** : scegli un colore di sfondo per le finestre dei messaggi di avviso.

* **Barra di avanzamento** : scegli un colore per la barra che indica l’avanzamento dei caricamenti e dei download.

Affinché gli utenti del Media Portal possano vedere le impostazioni di stile scelte, devono aggiungere `?company=(company name)` all’URL con cui accedono a Media Portal. Ad esempio, per vedere le impostazioni di stile, gli utenti di Media Portal che accedono alla società PortalCo mediante l’URL seguente:

`https://s7sps1.scene7.com/MediaPortal`

Utilizza invece il seguente URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

L’inclusione del nome della società nell’URL consente a Media Portal di riconoscere la società a cui desidera accedere l’utente e di applicare quindi le relative impostazioni di stile.

È possibile ottenere ulteriori informazioni su come comunicare modifiche di URL agli utenti Media Portal, nonché su come impostare un messaggio e-mail di benvenuto mediante il quale i nuovi utenti possono ricevere l’URL corretto per Media Portal.

Consultate [Impostare il messaggio di benvenuto per gli utenti di Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
