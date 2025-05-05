---
title: Collegare un eCatalog a una pagina Web
description: Scopri come collegare un eCatalog a una pagina web in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 23%

---

# Collegare un eCatalog a una pagina Web{#linking-an-ecatalog-to-a-web-page}

I siti Web e le applicazioni accedono al contenuto del server immagini di Dynamic Medie, inclusi gli eCatalog, tramite stringhe URL o codice incorporato. Queste stringhe URL vengono attivate durante il processo di pubblicazione. Per inserire la stringa URL o il codice incorporato per l&#39;eCatalog nelle pagine Web e nelle applicazioni, è necessario copiarlo da Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Copiare un URL di eCatalog {#copying-an-ecatalog-url}

1. Nel pannello Sfoglia risorse, nell&#39;elenco a discesa Mostra, seleziona **[!UICONTROL Catalogo]**.
1. nel pannello Libreria risorse a sinistra, passa alla cartella delle risorse contenente l’eCatalog di cui desideri copiare il codice da incorporare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e Codice di incorporamento a destra, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato.
   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]** sotto l&#39;immagine di anteprima.

     Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

   * Selezionare **[!UICONTROL Vista elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell&#39;immagine di anteprima passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

   * Selezionare **[!UICONTROL Visualizzazione griglia]**, **[!UICONTROL Visualizzazione elenco]** o **[!UICONTROL Visualizzazione dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori selezionare **Copia URL** nella colonna Azioni della tabella.

## Aggiungere URL di eCatalog alla pagina Web {#adding-ecatalog-urls-to-your-web-page}

Il modo più comune per distribuire un eCatalog consiste nell&#39;inserire un collegamento sotto forma di una pagina di copertina con miniature di eCatalog nella pagina Web. Consultate il personale IT per fare in modo che l’eCatalog venga avviato in una finestra a comparsa centrata e senza altri contenuti, senza la barra degli strumenti né la barra degli indirizzi nel browser.

Per ulteriori dettagli ed esempi di codice, vedere [Incorporare il visualizzatore eCatalog di HTML5 nella Guida di riferimento dei visualizzatori di Adobi](https://experienceleague.adobe.com/it/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Copiare il codice di incorporamento di un visualizzatore eCatalog {#copying-the-embed-code-of-an-ecatalog-viewer}

La funzione Incorpora codice permette di analizzare il codice visualizzatore dell’eCatalog selezionato. È inoltre possibile copiare il codice negli Appunti in modo da poterlo incollare nelle pagine Web per la distribuzione del visualizzatore. La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

**Per copiare il codice di incorporamento di un visualizzatore eCatalog:**

1. Nel pannello Sfoglia risorse, nell&#39;elenco a discesa Mostra, seleziona **[!UICONTROL Catalogo]**.
1. nel pannello Libreria risorse a sinistra, passa alla cartella delle risorse contenente l’eCatalog di cui desideri copiare il codice da incorporare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL a destra, seleziona **[!UICONTROL Incorpora codice]**.
   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]** sotto l&#39;immagine di anteprima.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Vista elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell&#39;immagine di anteprima passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Visualizzazione griglia]**, **[!UICONTROL Visualizzazione elenco]** o **[!UICONTROL Visualizzazione dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

1. Nella finestra di dialogo Incorpora codice, seleziona **[!UICONTROL Copia negli Appunti]**.

   La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

1. Seleziona **[!UICONTROL Chiudi]**.
