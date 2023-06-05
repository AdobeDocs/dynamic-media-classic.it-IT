---
title: Personalizzare la schermata di Media Portal
description: Scopri come personalizzare la schermata Media Portal in Adobe Dynamic Media Classic.
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 32%

---

# Personalizzare la schermata di Media Portal{#customizing-the-media-portal-screen}

Le impostazioni di stile di Media Portal consentono di personalizzare la schermata di Media Portal con il logo e i colori aziendali. Utilizza le impostazioni di stile per inserire il marchio della tua azienda in Media Portal.

Per accedere alle impostazioni di stile, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione Media Portal]** > **[!UICONTROL Impostazioni stile]**. Accertati di selezionare **[!UICONTROL Salva]** per salvare le impostazioni dopo averle create. Puoi selezionare **[!UICONTROL Ripristina]** per ripristinare le impostazioni predefinite. Mentre effettuate le scelte, il pannello Anteprima mostra come appaiono.

* **[!UICONTROL Logo]** - Seleziona **[!UICONTROL Sfoglia]** e quindi scegliere un elemento grafico nella finestra Seleziona immagine logo.

* **[!UICONTROL Applicazione]** - Creare una fusione di colori sfumati effettuando le scelte desiderate nei menu Colori sfumatura sfondo.

* **[!UICONTROL Albero]** - Scegliere un colore di rollover (il colore visualizzato quando si sposta il puntatore su un elemento) e un colore di selezione (il colore visualizzato quando si seleziona un elemento).

* **[!UICONTROL Accordion]** - Scegliere i colori di sfondo, lo stile del bordo, il rollover e i colori selezionati per il pannello a soffietto visualizzato sul lato destro dello schermo nella visualizzazione Dettagli.

* **[!UICONTROL Intestazione Accordion]** - Scegli se rendere il testo nel grassetto dell’intestazione del Pannello a soffietto.

* **[!UICONTROL Datagrid]** - Scegliere i colori per la riga di intestazione nelle griglie dati.

* **[!UICONTROL Avviso]** - Scegliere un colore di sfondo per le finestre di messaggio di avviso.

* **[!UICONTROL Barra di avanzamento]** : scegli un colore per la barra che indica l’avanzamento dei caricamenti e dei download.

Affinché gli utenti di Media Portal possano visualizzare le impostazioni di stile scelte, devono accodare `?company=(company name)` all’URL con cui accedono a Media Portal. Ad esempio, per vedere le impostazioni di stile, gli utenti di Media Portal che accedono alla società PortalCo mediante l’URL seguente:

`https://s7sps1.scene7.com/MediaPortal`

Utilizza invece il seguente URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

L’inclusione del nome della società nell’URL consente a Media Portal di riconoscere la società a cui desidera accedere l’utente e di applicare quindi le relative impostazioni di stile.

È possibile ottenere ulteriori informazioni su come comunicare modifiche di URL agli utenti Media Portal, nonché su come impostare un messaggio e-mail di benvenuto mediante il quale i nuovi utenti possono ricevere l’URL corretto per Media Portal.

Consultate [Impostare il messaggio di benvenuto per gli utenti di Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
