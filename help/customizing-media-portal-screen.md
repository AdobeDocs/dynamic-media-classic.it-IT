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
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 32%

---

# Personalizzare la schermata di Media Portal{#customizing-the-media-portal-screen}

Le impostazioni di stile di Media Portal consentono di personalizzare la schermata di Media Portal con il logo e i colori aziendali. Utilizza le impostazioni di stile per inserire il marchio della tua azienda in Media Portal.

Per accedere alle impostazioni dello stile, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione di Media Portal]** > **[!UICONTROL Impostazioni stile]**. Assicurati di selezionare **[!UICONTROL Salva]** per salvare le impostazioni dopo averle apportate. È possibile selezionare **[!UICONTROL Ripristina]** per ripristinare le impostazioni predefinite. Quando si effettua una scelta, il pannello Anteprima mostra la relativa visualizzazione.

* **[!UICONTROL Logo]** - Seleziona **[!UICONTROL Sfoglia]**, quindi scegliere un grafico nella finestra Seleziona immagine logo .

* **[!UICONTROL Applicazione]** - Crea una blend di colore sfumatura effettuando le scelte sui menu Colori sfumatura sfondo.

* **[!UICONTROL Albero]** - Scegliere un colore di rollover (il colore che appare quando si sposta il puntatore su un elemento) e un colore di selezione (il colore che appare quando si seleziona un elemento).

* **[!UICONTROL Accordion]** - Scegliere i colori di sfondo, uno stile del bordo e i colori rollover e selezionati per il pannello a soffietto che appare sul lato destro dello schermo nella vista Dettagli.

* **[!UICONTROL Intestazione pannello a soffietto]** - Scegliere se fare testo in grassetto intestazione fisarmonica.

* **[!UICONTROL Datagrid]** - Scegliere i colori per la riga di intestazione nelle griglie dati.

* **[!UICONTROL Avviso]** - Scegliere un colore di sfondo per le finestre dei messaggi di avviso.

* **[!UICONTROL Barra di avanzamento]** - Scegli un colore per la barra che indichi l’avanzamento dei caricamenti e dei download.

Affinché gli utenti del Media Portal possano vedere le impostazioni di stile selezionate, devono aggiungere `?company=(company name)` all’URL con cui accedono a Media Portal. Ad esempio, per vedere le impostazioni di stile, gli utenti di Media Portal che accedono alla società PortalCo mediante l’URL seguente:

`https://s7sps1.scene7.com/MediaPortal`

Utilizza invece il seguente URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

L’inclusione del nome della società nell’URL consente a Media Portal di riconoscere la società a cui desidera accedere l’utente e di applicare quindi le relative impostazioni di stile.

È possibile ottenere ulteriori informazioni su come comunicare modifiche di URL agli utenti Media Portal, nonché su come impostare un messaggio e-mail di benvenuto mediante il quale i nuovi utenti possono ricevere l’URL corretto per Media Portal.

Consultate [Impostare il messaggio di benvenuto per gli utenti di Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
