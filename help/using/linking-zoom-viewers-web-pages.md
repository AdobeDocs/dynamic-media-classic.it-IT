---
title: Collegare i visualizzatori Zoom alle pagine Web
description: Scopri come collegare i visualizzatori Zoom alle pagine web in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
topic: Administration, Content Management, Development
level: Intermediate
autotag-review: '2026-05-13T20:03:57.696Z'
TQID: 'https://experienceleague.adobe.com/Urf0qGJqj7tCCGDfNwprZnxf6YfDgavWb44pThwds0I'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 698
ht-degree: 20%

---

# Collegare i visualizzatori Zoom alle pagine Web{#linking-zoom-viewers-to-your-web-pages}

I siti Web e le applicazioni accedono al contenuto di Dynamic Media Image Server tramite stringhe URL o codice incorporato. Tale accesso include le immagini primarie e le destinazioni di zoom associate. Sono inclusi anche i predefiniti visualizzatore zoom. Queste stringhe URL vengono attivate durante il processo di pubblicazione. Per inserire queste stringhe URL o il codice incorporato nelle pagine Web e nelle applicazioni, copiale da Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Copiare un URL di visualizzatore Zoom {#copying-a-zoom-viewer-url}

1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il visualizzatore zoom di cui desiderate copiare l’URL.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Visualizzazione griglia]** o **[!UICONTROL Visualizzazione elenco]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e Codice di incorporamento a destra, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato.
   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]** sotto l&#39;immagine di anteprima.

     Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

   * Selezionare **[!UICONTROL Vista elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell&#39;immagine di anteprima passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

   * Selezionare **[!UICONTROL Visualizzazione griglia]**, **[!UICONTROL Visualizzazione elenco]** o **[!UICONTROL Visualizzazione dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

## Aggiungere gli URL del visualizzatore Zoom alla pagina Web {#adding-zoom-viewer-urls-to-your-web-page}

In genere, i visitatori ingrandiscono le immagini su un sito web selezionando prima un’icona Zoom (spesso l’icona mostra l’immagine di una lente di ingrandimento). Se si seleziona questa icona, viene avviata una pagina Web dinamica (ASP o JSP) che visualizza l&#39;immagine in una finestra popup. La finestra a comparsa rappresenta il punto in cui i visitatori applicano effettivamente lo zoom all’immagine.

Per ulteriori dettagli ed esempi di codice, vedere il [Visualizzatore zoom di base integrato di HTML5](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2) nella Guida di riferimento dei visualizzatori di Adobe.

## Copiare la copia incorporata di un visualizzatore Zoom {#copying-the-embed-copy-of-a-zoom-viewer}

L&#39;utilizzo della funzione del codice incorporato consente di esaminare il codice del visualizzatore Zoom selezionato. È inoltre possibile copiare il codice negli Appunti in modo da poterlo incollare nelle pagine Web per la distribuzione del visualizzatore. La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

**Per copiare il codice incorporato di un visualizzatore Zoom:**

1. nel pannello Libreria risorse, a sinistra, accedi alla cartella risorse contenente il visualizzatore Zoom di cui desideri copiare il codice da incorporare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e Codice di incorporamento a destra, seleziona **[!UICONTROL Codice di incorporamento]** a destra del visualizzatore desiderato.
   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]** sotto l&#39;immagine di anteprima.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Vista elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell&#39;immagine di anteprima passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Visualizzazione griglia]**, **[!UICONTROL Visualizzazione elenco]** o **[!UICONTROL Visualizzazione dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

1. Nella finestra di dialogo Incorpora codice, seleziona **[!UICONTROL Copia negli Appunti]**.

   La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

1. Seleziona **[!UICONTROL Chiudi]**.
