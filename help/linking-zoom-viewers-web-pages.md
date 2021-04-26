---
title: Collegamento di visualizzatori zoom alle pagine Web
description: Scopri come collegare i visualizzatori zoom alle pagine web.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Visualizzatori,Zoom
role: Business Practitioner
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
translation-type: tm+mt
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 81%

---

# Collegamento di visualizzatori zoom alle pagine Web{#linking-zoom-viewers-to-your-web-pages}

I siti web e le applicazioni accedono al contenuto di Dynamic Media Image Server, incluse le immagini master e le destinazioni di zoom associate, e ai predefiniti per visualizzatori zoom, tramite stringhe URL o codice incorporato. Queste stringhe URL vengono attivate durante il processo di pubblicazione. Per inserire queste stringhe URL o il codice incorporato nelle pagine web e nelle applicazioni, è necessario copiarle da Dynamic Media Classic.

>[!NOTE]
>
>l’URL non è attivo finché non pubblicate la risorsa.

## Copia dell’URL di un visualizzatore zoom  {#copying-a-zoom-viewer-url}

1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il visualizzatore zoom di cui desiderate copiare l’URL.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Fate clic su **[!UICONTROL Visualizzazione griglia]** o **[!UICONTROL Visualizzazione elenco]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, fate clic su **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato.
   * Fate clic su **[!UICONTROL Visualizzazione griglia]**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, sotto la miniatura, fate clic su **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **[!UICONTROL Copia URL]**.

   * Fate clic su **[!UICONTROL Visualizzazione elenco]**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, a destra della miniatura, fate clic su **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **[!UICONTROL Copia URL]**.

   * Fate clic su **[!UICONTROL Visualizzazione griglia]**, **[!UICONTROL Visualizzazione elenco]** o **[!UICONTROL Visualizzazione dettagli]**. Nella stessa barra degli strumenti, fate clic su **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **[!UICONTROL Copia URL]**.

## Aggiunta degli URL del visualizzatore zoom alla pagina Web  {#adding-zoom-viewer-urls-to-your-web-page}

In genere, i visitatori ingrandiscono le immagini di un sito web selezionando prima un’icona Zoom (spesso l’icona mostra l’immagine di una lente di ingrandimento). Selezionando questa icona, viene avviata una pagina Web dinamica (ASP o JSP) che visualizza l’immagine in una finestra a comparsa. La finestra a comparsa rappresenta il punto in cui i visitatori applicano effettivamente lo zoom all’immagine.

Per ulteriori dettagli ed esempi di codice, consulta [Incorporamento di visualizzatori HTML5 per zoom di base nella Guida di riferimento per visualizzatori di Adobi](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Copia del codice da incorporare di un visualizzatore zoom {#copying-the-embed-copy-of-a-zoom-viewer}

La funzione Incorpora codice permette di analizzare il codice visualizzatore del visualizzatore zoom selezionato. Potete anche copiare il codice negli Appunti per poi incollarlo nelle pagine Web su cui verrà distribuito il visualizzatore. La modifica del codice non è consentita nella finestra di dialogo Incorpora codice.

**Per copiare il codice da incorporare di un visualizzatore zoom:**

1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il visualizzatore zoom di cui desiderate copiare il codice da incorporare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Fate clic su **[!UICONTROL Visualizzazione griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, fate clic su **[!UICONTROL Incorpora codice]** a destra del visualizzatore desiderato.
   * Fate clic su **[!UICONTROL Visualizzazione griglia]**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, sotto la miniatura, fate clic su **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **[!UICONTROL Incorpora codice]**.

   * Fate clic su **[!UICONTROL Visualizzazione elenco]**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, a destra della miniatura, fate clic su **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **[!UICONTROL Incorpora codice]**.

   * Fate clic su **[!UICONTROL Visualizzazione griglia]**, **[!UICONTROL Visualizzazione elenco]** o **[!UICONTROL Visualizzazione dettagli]**. Nella stessa barra degli strumenti, fate clic su **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **[!UICONTROL Incorpora codice]**.

1. Nella finestra di dialogo Codice da incorporare, fate clic su **[!UICONTROL Copia negli Appunti]**.

   La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

1. Fai clic su **[!UICONTROL Chiudi]**.
