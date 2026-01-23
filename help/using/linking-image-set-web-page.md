---
title: Collegare un set di immagini a una pagina Web
description: Scopri come collegare un set di immagini a una pagina web in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 16%

---

# Collegare un set di immagini a una pagina Web{#linking-an-image-set-to-a-web-page}

Dopo aver pubblicato un set di immagini, è possibile copiarne l&#39;URL associato o il codice di incorporamento da utilizzare nel sito Web o nell&#39;applicazione. È quindi possibile distribuire l&#39;URL o incollare il codice incorporato in base alle esigenze, in modo che gli utenti possano visualizzare il set di immagini nel sito Web o nell&#39;applicazione.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Copiare un URL per set di immagini {#copying-an-image-set-url}

1. Nel pannello Sfoglia risorse, nell&#39;elenco a discesa Mostra, seleziona **[!UICONTROL Set di immagini]**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il set di immagini di cui desiderate copiare il codice incorporato.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello **[!UICONTROL URL e codice di incorporamento]** a destra, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato.
   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]** sotto l&#39;immagine di anteprima.

     Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

   * Selezionare **[!UICONTROL Vista elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell&#39;immagine di anteprima passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

   * Selezionare **[!UICONTROL Visualizzazione griglia]**, **[!UICONTROL Visualizzazione elenco]** o **[!UICONTROL Visualizzazione dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

## Aggiunta degli URL del set di immagini alla pagina Web {#adding-image-set-urls-to-your-web-page}

Il modo più comune per distribuire i set di immagini consiste nell’inserire un collegamento (tramite un’icona di navigazione) nella pagina web. Quando è selezionato, il collegamento avvia una pagina dinamica (JSP) che visualizza il set di immagini in una finestra di zoom popup. Il collegamento di zoom apre una finestra pop-up contenente la funzione di zoom effettiva.

Per ulteriori dettagli ed esempi di codice, vedere il [Visualizzatore zoom di HTML5 incorporato](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2) nella Guida di riferimento dei visualizzatori di Adobe.

## Copiare il codice incorporato di un visualizzatore di set di immagini {#copying-the-embed-code-of-an-image-set-viewer}

L&#39;utilizzo della funzione di codice incorporato consente di esaminare il codice visualizzatore per il set di immagini selezionato. È inoltre possibile copiare il codice negli Appunti in modo da poterlo incollare nelle pagine Web per la distribuzione del visualizzatore. La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

**Per copiare il codice incorporato di un visualizzatore di set di immagini:**

1. Nel pannello Sfoglia risorse, nell&#39;elenco a discesa Mostra, seleziona **[!UICONTROL Set di immagini]**.
1. nel pannello Libreria risorse a sinistra, passa alla cartella delle risorse contenente il set di immagini di cui desideri copiare il codice incorporato.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL a destra, seleziona **[!UICONTROL Incorpora codice]**.
   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]** sotto l&#39;immagine di anteprima.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Vista elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell&#39;immagine di anteprima passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Visualizzazione griglia]**, **Visualizzazione elenco** o **Visualizzazione dettagli**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

1. Nella finestra di dialogo **[!UICONTROL Incorpora codice]**, seleziona **[!UICONTROL Copia negli Appunti]**.

   La modifica del codice non è consentita nella finestra di dialogo **[!UICONTROL Incorpora codice]**.

1. Seleziona **[!UICONTROL Chiudi]**.

>[!MORELIKETHIS]
>
>* [Pubblica](publishing-files.md#publishing_files)
