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
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 38%

---

# Collegare un eCatalog a una pagina Web{#linking-an-ecatalog-to-a-web-page}

I siti Web e le applicazioni consentono di accedere ai contenuti di Dynamic Medie Image Server, inclusi gli eCatalog, tramite stringhe URL o codice incorporato. Queste stringhe URL vengono attivate durante il processo di pubblicazione. Per inserire la stringa URL o il codice incorporato per l’eCatalog nelle pagine web e nelle applicazioni, è necessario copiarlo da Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Copiare un URL di eCatalog {#copying-an-ecatalog-url}

1. Nel pannello Sfoglia risorse, nell’elenco a discesa Mostra, seleziona **[!UICONTROL Catalogo]**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene l’eCatalog di cui desiderate copiare il codice incorporato.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Vista griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e Codice di incorporamento a destra, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato.
   * Seleziona **[!UICONTROL Vista griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi sotto l’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Copia URL]**.

   * Seleziona **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Copia URL]**.

   * Seleziona **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]**, o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **Copia URL**.

## Aggiungere gli URL dell’eCatalog alla pagina web {#adding-ecatalog-urls-to-your-web-page}

Il modo più comune di pubblicare un eCatalog consiste nell’inserire nella pagina Web un collegamento sotto forma di miniatura della copertina dell’eCatalog. Consultate il personale IT per fare in modo che l’eCatalog venga avviato in una finestra a comparsa centrata e senza altri contenuti, senza la barra degli strumenti né la barra degli indirizzi nel browser.

Per ulteriori dettagli ed esempi di codice, vedi [Incorpora visualizzatore eCatalog di HTML5 nella Guida di riferimento dei visualizzatori di Adobi](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Copiare il codice di incorporamento di un visualizzatore eCatalog {#copying-the-embed-code-of-an-ecatalog-viewer}

La funzione Incorpora codice permette di analizzare il codice visualizzatore dell’eCatalog selezionato. Potete anche copiare il codice negli Appunti per poi incollarlo nelle pagine Web su cui verrà distribuito il visualizzatore. La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

**Per copiare il codice di incorporamento di un visualizzatore eCatalog:**

1. Nel pannello Sfoglia risorse, nell’elenco a discesa Mostra, seleziona **[!UICONTROL Catalogo]**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene l’eCatalog di cui desiderate copiare il codice incorporato.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Vista griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL a destra, seleziona **[!UICONTROL Codice di incorporamento]**.
   * Seleziona **[!UICONTROL Vista griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi sotto l’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**.

   * Seleziona **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**.

   * Seleziona **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]**, o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**.

1. Nella finestra di dialogo Incorpora codice, seleziona **[!UICONTROL Copia negli Appunti]**.

   La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

1. Seleziona **[!UICONTROL Chiudi]**.
