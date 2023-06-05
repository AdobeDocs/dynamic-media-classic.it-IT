---
title: Collegare un set 360 gradi a una pagina web
description: Scopri come collegare un set 360 gradi a una pagina web in Adobe Dynamic Media Classic.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 40%

---

# Collegare un set 360 gradi a una pagina web{#linking-a-spin-set-to-a-web-page}

I siti Web e le applicazioni accedono al contenuto di Dynamic Media Image Server, inclusi i set 360 gradi, tramite stringhe URL o codice incorporato. Queste stringhe URL vengono attivate durante il processo di pubblicazione. Per inserire la stringa dell’URL o il codice da incorporare per il set 360 gradi nelle pagine web e nelle applicazioni, copialo da Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

## Copiare un URL del set 360 gradi {#copying-a-spin-set-url}

1. Nel pannello Sfoglia risorse, nell’elenco a discesa Mostra, seleziona **[!UICONTROL Set 360 gradi]**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il set 360 gradi di cui desiderate copiare il codice incorporato.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Vista griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e Codice di incorporamento a destra, seleziona **[!UICONTROL Copia URL]** a destra del visualizzatore desiderato.
   * Seleziona **[!UICONTROL Vista griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi sotto l’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Copia URL]**.

   * Seleziona **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Copia URL]**.

   * Seleziona **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]**, o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Copia URL]**.

## Aggiungere gli URL del set 360 gradi alla pagina web {#adding-spin-set-urls-to-your-web-page}

I set 360 gradi vengono distribuiti come tutti i visualizzatori di zoom, tramite una pagina dinamica (ASP o JSP) che visualizza il set 360 gradi in una finestra di zoom. La chiamata URL alla piattaforma Adobe Dynamic Media Classic segue lo stesso protocollo sul visualizzatore zoom. Tuttavia, il nome del predefinito per visualizzatori dipende dal l’impostazione predefinita specificata dall’amministratore per i visualizzatori di set 360 gradi. Ad esempio, la sintassi dell’URL di prova riportato di seguito include un predefinito denominato `viewer.jsp` e il parametro SKU è il nome del set 360 gradi:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

In questo esempio di sintassi URL (il collegamento non è attivo), è riportato un numero SKU ( `sku=backpack_spin`). La stringa dopo `sku=` è il nome del set 360 gradi ( `backpack spin`).

## Copiare il codice di incorporamento di un visualizzatore di set 360 gradi {#copying-the-embed-code-of-a-spin-set-viewer}

La funzione Incorpora codice permette di analizzare il codice visualizzatore del set 360 gradi selezionato. Potete anche copiare il codice negli Appunti per poi incollarlo nelle pagine Web su cui verrà distribuito il visualizzatore. La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

**Per copiare il codice da incorporare di un visualizzatore set 360 gradi:**

1. Nel pannello Sfoglia risorse, nell’elenco a discesa Mostra, seleziona **[!UICONTROL Set 360 gradi]**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il set 360 gradi di cui desiderate copiare il codice incorporato.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Seleziona **[!UICONTROL Vista griglia]**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e Codice di incorporamento a destra, seleziona **[!UICONTROL Codice di incorporamento]** a destra del visualizzatore desiderato.
   * Seleziona **[!UICONTROL Vista griglia]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi sotto l’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**.

   * Seleziona **[!UICONTROL Vista a elenco]**. Nel pannello Sfoglia risorse, seleziona una singola risorsa, quindi a destra dell’immagine di miniatura vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**.

   * Seleziona **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista a elenco]**, o **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]**.

1. Nella finestra di dialogo Incorpora codice, seleziona **[!UICONTROL Copia negli Appunti]**.

   La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

1. Seleziona **[!UICONTROL Chiudi]**.
