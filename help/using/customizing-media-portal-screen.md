---
title: Personalizzare la schermata Media Portal
description: Scopri come personalizzare la schermata Media Portal in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: 00591bdbe721035e25d3dea245a2110f978d19aa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 17%

---

# Personalizzare la schermata Media Portal{#customizing-the-media-portal-screen}

Le impostazioni di stile di Media Portal consentono di personalizzare la schermata di Media Portal con il logo e i colori aziendali. Utilizza le impostazioni di stile per inserire il marchio della tua azienda in Media Portal.

Per accedere alle impostazioni di stile, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione Media Portal]** > **[!UICONTROL Impostazioni stile]**. Accertati di selezionare **[!UICONTROL Salva]** per salvare le impostazioni dopo averle create. Puoi selezionare **[!UICONTROL Ripristina]** per ripristinare le impostazioni predefinite. Mentre effettuate le scelte, il pannello Anteprima mostra come appaiono.

* **[!UICONTROL Logo]**: Seleziona **[!UICONTROL Sfoglia]** e quindi scegliere un elemento grafico nella finestra Seleziona immagine logo.

* **[!UICONTROL Applicazione]**: consente di creare una fusione di colori sfumati effettuando scelte nei menu dei colori sfumatura di sfondo.

* **[!UICONTROL Albero]**: scegli un colore di rollover e un colore di selezione.

* **[!UICONTROL Accordion]**: scegli i colori di sfondo, lo stile del bordo e il rollover e i colori selezionati per il pannello a soffietto visualizzato sul lato destro dello schermo nella vista Dettagli.

* **[!UICONTROL Intestazione Accordion]**: scegli se creare il testo nel grassetto dell’intestazione del Pannello a soffietto.

* **[!UICONTROL Datagrid]**: scegli i colori per la riga di intestazione nelle griglie dati.

* **[!UICONTROL Avviso]**: consente di scegliere un colore di sfondo per le finestre dei messaggi di avviso.

* **[!UICONTROL Barra di avanzamento]**: scegli un colore per la barra che indica l’avanzamento dei caricamenti e dei download.

Affinché gli utenti di Media Portal possano visualizzare le impostazioni di stile scelte, devono accodare `?company=(company name)` all’URL con cui accedono a Media Portal. Ad esempio, per visualizzare le impostazioni di stile, gli utenti di Media Portal che accedono alla società PortalCo visitano il sito:

`https://s7sps1.scene7.com/MediaPortal`

Utilizza invece il seguente URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

L’inclusione del nome della società nell’URL consente a Media Portal di riconoscere la società a cui un utente desidera accedere e di applicare di conseguenza le impostazioni di stile della società.

È possibile ottenere ulteriori informazioni su come comunicare modifiche di URL agli utenti Media Portal, nonché su come impostare un messaggio e-mail di benvenuto mediante il quale i nuovi utenti possono ricevere l’URL corretto per Media Portal.

Consultate [Impostare il messaggio di benvenuto per gli utenti di Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
