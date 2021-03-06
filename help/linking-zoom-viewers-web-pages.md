---
title: Collegare i visualizzatori zoom alle pagine web
description: Scopri come collegare i visualizzatori zoom alle pagine web in Adobe Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 34%

---

# Collegare i visualizzatori zoom alle pagine web{#linking-zoom-viewers-to-your-web-pages}

I siti web e le applicazioni accedono al contenuto di Dynamic Media Image Server, incluse le immagini master e le destinazioni di zoom associate, e ai predefiniti per visualizzatori zoom, tramite stringhe URL o codice incorporato. Queste stringhe URL vengono attivate durante il processo di pubblicazione. Per inserire queste stringhe URL o il codice incorporato nelle pagine web e nelle applicazioni, è necessario copiarle da Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Copiare l’URL di un visualizzatore zoom {#copying-a-zoom-viewer-url}

1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il visualizzatore zoom di cui desiderate copiare l’URL.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Vista griglia]** o **[!UICONTROL Vista a elenco]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato.
   * Selezionare **[!UICONTROL Vista griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi, sotto l’immagine miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Copia URL]**.

   * Selezionare **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi, a destra della miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Copia URL]**.

   * Selezionare **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]** o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Copia URL]**.

## Aggiungere gli URL del visualizzatore zoom alla pagina web {#adding-zoom-viewer-urls-to-your-web-page}

In genere, i visitatori ingrandiscono le immagini di un sito web selezionando prima un’icona Zoom (spesso l’icona mostra l’immagine di una lente di ingrandimento). Selezionando questa icona, viene avviata una pagina Web dinamica (ASP o JSP) che visualizza l’immagine in una finestra a comparsa. La finestra a comparsa rappresenta il punto in cui i visitatori applicano effettivamente lo zoom all’immagine.

Per ulteriori dettagli ed esempi di codice, consulta [Incorporare HTML5 Basic Zoom Viewer nella Guida di riferimento dei visualizzatori di Adobi](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Copiare la copia da incorporare di un visualizzatore zoom {#copying-the-embed-copy-of-a-zoom-viewer}

La funzione Incorpora codice permette di analizzare il codice visualizzatore del visualizzatore zoom selezionato. Potete anche copiare il codice negli Appunti per poi incollarlo nelle pagine Web su cui verrà distribuito il visualizzatore. La modifica del codice non è consentita nella finestra di dialogo Incorpora codice.

**Per copiare il codice da incorporare di un visualizzatore zoom:**

1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il visualizzatore zoom di cui desiderate copiare il codice da incorporare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Vista griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, seleziona **[!UICONTROL Codice da incorporare]** a destra del visualizzatore desiderato.
   * Selezionare **[!UICONTROL Vista griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi, sotto l’immagine miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi, a destra della miniatura, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

   * Selezionare **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]** o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, selezionare **[!UICONTROL Codice di incorporamento]**.

1. Nella finestra di dialogo Incorpora codice selezionare **[!UICONTROL Copia negli Appunti]**.

   La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

1. Selezionare **[!UICONTROL Chiudi]**.
