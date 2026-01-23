---
title: Collegare un set 360 gradi a una pagina web
description: Scopri come collegare un set 360 gradi a una pagina web in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 21%

---

# Collegare un set 360 gradi a una pagina web{#linking-a-spin-set-to-a-web-page}

I siti Web e le applicazioni accedono al contenuto del server immagini Dynamic Media, inclusi i set 360 gradi, tramite stringhe URL o codice incorporato. Queste stringhe URL vengono attivate durante il processo di pubblicazione. Per inserire la stringa URL o il codice di incorporamento per il set 360 gradi nelle pagine web e nelle applicazioni, copialo da Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Copiare un URL del set 360 gradi {#copying-a-spin-set-url}

1. Nel pannello Sfoglia risorse, nell&#39;elenco a discesa Mostra, selezionare **[!UICONTROL Set 360 gradi]**.
1. nel pannello Libreria risorse, a sinistra, accedi alla cartella delle risorse contenente il set 360 gradi di cui desideri copiare il codice da incorporare.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e Codice di incorporamento a destra, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato.
   * Selezionare **[!UICONTROL Visualizzazione griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]** sotto l&#39;immagine di anteprima.

     Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

   * Selezionare **[!UICONTROL Vista elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell&#39;immagine di anteprima passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

   * Selezionare **[!UICONTROL Visualizzazione griglia]**, **[!UICONTROL Visualizzazione elenco]** o **[!UICONTROL Visualizzazione dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

     Nella pagina Elenco visualizzatori selezionare **[!UICONTROL Copia URL]** nella colonna Azioni della tabella.

## Aggiungere gli URL del set 360 gradi alla pagina web {#adding-spin-set-urls-to-your-web-page}

I set 360 gradi vengono distribuiti come tutti i visualizzatori di zoom, tramite una pagina dinamica (ASP o JSP) che visualizza il set 360 gradi in una finestra di zoom. La chiamata URL alla piattaforma Adobe Dynamic Media Classic segue lo stesso protocollo sul visualizzatore zoom. Tuttavia, il nome del predefinito per visualizzatori dipende dal l’impostazione predefinita specificata dall’amministratore per i visualizzatori di set 360 gradi. Ad esempio, il seguente esempio di sintassi URL non live include un nome di predefinito denominato `viewer.jsp` e il parametro SKU è ora il nome del set 360 gradi:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

In questo esempio di sintassi URL (il collegamento non è attivo), noterai un numero SKU ( `sku=backpack_spin`). La stringa dopo `sku=` è il nome del set 360 gradi ( `backpack spin`).

## Copiare il codice incorporato di un visualizzatore di set 360 gradi {#copying-the-embed-code-of-a-spin-set-viewer}

L’utilizzo della funzione del codice incorporato consente di rivedere il codice visualizzatore per il set 360 gradi selezionato. È inoltre possibile copiare il codice negli Appunti in modo da poterlo incollare nelle pagine Web per la distribuzione del visualizzatore. La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

**Per copiare il codice incorporato di un visualizzatore di set 360 gradi:**

1. Nel pannello Sfoglia risorse, nell&#39;elenco a discesa Mostra, selezionare **[!UICONTROL Set 360 gradi]**.
1. nel pannello Libreria risorse, a sinistra, accedi alla cartella delle risorse contenente il set 360 gradi di cui desideri copiare il codice da incorporare.
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
