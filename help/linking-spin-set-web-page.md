---
title: Collegamento di un set 360 gradi a una pagina Web
seo-title: Collegamento di un set 360 gradi a una pagina Web
description: 'null'
seo-description: Come collegare un set 360 gradi a una pagina Web.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 88%

---


# Collegamento di un set 360 gradi a una pagina Web{#linking-a-spin-set-to-a-web-page}

I siti Web e le applicazioni accedono al contenuto di Dynamic Media Image Server, compresi i set 360 gradi, mediante stringhe URL o codice incorporato. Queste stringhe URL vengono attivate durante il processo di pubblicazione. Per inserire la stringa URL o il codice da incorporare per il set 360 gradi nelle pagine Web e nelle applicazioni, copiate la stringa o il codice da Dynamic Media Classic.

>[!NOTE]
>
>l’URL non è attivo finché non pubblicate la risorsa.

## Copia dell’URL di un set 360 gradi  {#copying-a-spin-set-url}

1. Nel pannello delle risorse, nell’elenco a discesa Mostra, fate clic su **Set 360 gradi**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il set 360 gradi di cui desiderate copiare il codice incorporato.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, fate clic su **Copia URL** a destra del visualizzatore desiderato.
   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, sotto la miniatura, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**.

   * Fate clic su **Visualizzazione elenco**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, a destra della miniatura, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**.

   * Fate clic su **Visualizzazione griglia**, **Visualizzazione elenco** o **Visualizzazione dettagli**. Nella stessa barra degli strumenti, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Copia URL**.

## Aggiunta di URL di set 360 gradi alla pagina Web  {#adding-spin-set-urls-to-your-web-page}

I set 360 gradi vengono distribuiti come tutti i visualizzatori di zoom, tramite una pagina dinamica (ASP o JSP) che visualizza il set 360 gradi in una finestra di zoom. La richiesta URL alla piattaforma Dynamic Media Classic segue lo stesso protocollo sul visualizzatore zoom. Tuttavia, il nome del predefinito per visualizzatori dipende dal l’impostazione predefinita specificata dall’amministratore per i visualizzatori di set 360 gradi. Ad esempio, la sintassi dell’URL di prova riportato di seguito include un predefinito denominato `viewer.jsp` e il parametro SKU è il nome del set 360 gradi:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

In questo esempio di sintassi URL (il collegamento non è attivo), è riportato un numero SKU ( `sku=backpack_spin`). La stringa dopo `sku=` è il nome del set 360 gradi ( `backpack spin`).

## Copia del codice da incorporare di un visualizzatore set 360 gradi {#copying-the-embed-code-of-a-spin-set-viewer}

La funzione Incorpora codice permette di analizzare il codice visualizzatore del set 360 gradi selezionato. Potete anche copiare il codice negli Appunti per poi incollarlo nelle pagine Web su cui verrà distribuito il visualizzatore. La modifica del codice non è consentita nella finestra di dialogo Incorpora codice.

**Per copiare il codice da incorporare di un visualizzatore set 360 gradi**

1. Nel pannello delle risorse, nell’elenco a discesa Mostra, fate clic su **Set 360 gradi**.
1. Nel pannello Libreria risorse a sinistra, individuate la cartella di risorse che contiene il set 360 gradi di cui desiderate copiare il codice incorporato.
1. Sopra il pannello delle risorse, sul lato destro della barra degli strumenti, effettuate una delle seguenti operazioni:

   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, fate doppio clic su una singola risorsa per aprirla in visualizzazione Dettagli. Nel pannello URL e codice da incorporare a destra, fate clic su **Incorpora codice** a destra del visualizzatore desiderato.
   * Fate clic su **Visualizzazione griglia**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, sotto la miniatura, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**.

   * Fate clic su **Visualizzazione elenco**. Nel pannello delle risorse, selezionate una singola risorsa, quindi, a destra della miniatura, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**.

   * Fate clic su **Visualizzazione griglia**, **Visualizzazione elenco** o **Visualizzazione dettagli**. Nella stessa barra degli strumenti, fate clic su **Anteprima** > **Elenco visualizzatori**.

      Nella pagina Elenco visualizzatori, nella colonna Azioni della tabella, fate clic su **Incorpora codice**.

1. Nella finestra di dialogo Codice da incorporare, fate clic su **Copia negli Appunti**.

   La modifica del codice non è consentita nella finestra di dialogo Codice da incorporare.

1. Fai clic su Chiudi.

