---
title: Collegare gli URL all’applicazione web
description: Scopri come collegare gli URL all’applicazione web da Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
autotag-review: '2026-05-13T20:03:48.579Z'
TQID: 'https://experienceleague.adobe.com/c8e722KVmasJVtoVl8k7-5vGjvs4Lm-GZavm-TF9fk0'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1960799e4144942d4d9443196e6db425f87c7686
workflow-type: tm+mt
source-wordcount: 821
ht-degree: 16%

---

# Collegare gli URL all’applicazione web{#linking-urls-to-your-web-application}

I siti Web e le applicazioni accedono al contenuto del server immagini Dynamic Media utilizzando stringhe URL. Dopo aver pubblicato un’immagine, Adobe Dynamic Media Classic attiva una stringa URL che fa riferimento al predefinito immagine nei server immagini Dynamic Media. Puoi utilizzare questi URL in un browser web per eseguire test.

Per inserire queste stringhe URL nelle pagine Web e nelle applicazioni, copiarle da Adobe Dynamic Media Classic. Per ottenere una stringa URL generata con un predefinito immagine, passa alla schermata Anteprima o al pannello Sfoglia (in Vista dettagli).

## Ottenere un URL per un predefinito immagine {#obtaining-an-image-preset-url}

Potete ottenere una stringa URL generata da un predefinito per immagini dalla schermata Anteprima o dalla visualizzazione Dettagli. Dopo aver copiato l’URL, questo viene salvato negli Appunti in modo da poterlo incollare in base alle esigenze.

>[!NOTE]
>
>l’URL diventa attivo solo dopo che la risorsa è stata pubblicata.

### Ottieni un URL per predefinito immagine da Anteprima {#obtaining-an-image-preset-url-from-preview}

1. Nel pannello Libreria risorse, a sinistra, passa alla cartella Risorse che contiene la risorsa immagine da visualizzare in anteprima.
1. Effettuate una delle seguenti operazioni:

   * Sopra la finestra di Assets, sul lato destro della barra degli strumenti, selezionare **[!UICONTROL Vista griglia]**. Nella finestra Risorsa, seleziona una singola risorsa immagine, quindi, sotto l&#39;immagine di anteprima, passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco predefiniti immagine]**.
   * Sopra la finestra di Assets, sul lato destro della barra degli strumenti, seleziona **[!UICONTROL Vista a elenco]**. Nella finestra Risorsa, seleziona una singola risorsa immagine, quindi a destra dell&#39;immagine miniatura passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco predefiniti immagine]**.
   * Sopra la finestra di Assets, sul lato destro della barra degli strumenti, selezionare **[!UICONTROL Vista dettagli]**. Sulla stessa barra degli strumenti, passa a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco predefiniti immagine]**.

1. (Facoltativo) Nell’elenco Predefiniti immagine, seleziona l’URL Encoding da applicare all’URL della risorsa immagine copiata nell’elenco a discesa Codifica URL per Copia generazione URL.
1. Nella finestra Elenco predefiniti immagine, nell&#39;area superiore destra del riquadro di anteprima, selezionare **[!UICONTROL Copia URL]** per il tipo di predefinito selezionato.
1. Nell&#39;angolo inferiore destro della finestra Elenco predefiniti immagine, seleziona **[!UICONTROL Chiudi]** per tornare alla schermata di Assets.

### Ottenere un URL per un predefinito immagine dal pannello Sfoglia {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Nel pannello Libreria risorse, a sinistra, passa alla cartella Risorse contenente la risorsa immagine da visualizzare in anteprima.
1. Sopra la finestra di Assets, sul lato destro della barra degli strumenti, selezionare **[!UICONTROL Vista griglia]**. Nella finestra Risorse, selezionate una singola risorsa di immagine.
1. Sopra la finestra di Assets, sul lato destro della barra degli strumenti, selezionare **[!UICONTROL Vista dettagli]**.
1. Seleziona **[!UICONTROL URL]** nel pannello di destra per visualizzare l&#39;elenco dei predefiniti immagine.
1. Seleziona il collegamento **[!UICONTROL Copia URL]** accanto al nome del predefinito immagine con l&#39;URL da copiare negli Appunti.

## Panoramica delle stringhe URL del predefinito immagine {#about-image-preset-url-strings}

Una chiamata URL per il dimensionamento delle immagini sui server immagini Dynamic Media ha la seguente sintassi di base:

*percorso*/*nome del server immagini*/*nome account*/*nome immagine*?*modificatore1*&amp;*modificatore2*&amp;...

In un URL di Dynamic Media Image Server, le istruzioni per la visualizzazione dell&#39;immagine seguono il punto interrogativo (?). Ad esempio, questa chiamata URL fornisce un’immagine denominata &quot;zaino&quot; con una larghezza di 250 pixel:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

L’URL di un predefinito per immagini contiene tutte le istruzioni sui modificatori necessarie per presentare l’immagine secondo le specifiche di formattazione e ridimensionamento corrette. Senza un predefinito immagine, annota tutte le istruzioni del modificatore dopo il punto interrogativo (?) come in questa stringa URL:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

Tuttavia, in una stringa URL generata con un predefinito immagine, il nome del predefinito immagine sostituisce le istruzioni definite dal predefinito immagine. Ad esempio, per l’URL lungo di cui sopra, la stringa URL è:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

I nomi dei predefiniti immagine negli URL utilizzano i simboli del dollaro ($). Quando un server immagini Dynamic Media elabora la porzione dell&#39;URL relativa al predefinito immagine (in questo caso `Large`), utilizza le istruzioni di dimensione e formattazione definite dal predefinito immagine &quot;Large&quot;.

## Aggiungere immagini dinamiche alla pagina Web {#adding-dynamic-images-to-your-web-page}

Quando si aggiungono immagini dinamiche alle pagine Web, il tag `<IMG>` viene in genere modificato utilizzando la stringa URL di Adobe Dynamic Media Classic per richiedere immagini dai server di immagini Dynamic Media. La stringa produce l’immagine secondo le specifiche di formattazione e ridimensionamento definite dal predefinito per immagini.

Ad esempio, al posto della tipica richiesta di apertura di un’immagine statica, ovvero

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Il tag `<IMG>` viene ora utilizzato per sostituire il riferimento a un&#39;immagine statica con una chiamata di predefinito immagine alla piattaforma Adobe Dynamic Media Classic. Esempio di richiesta:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

In questo esempio, un server immagini Dynamic Media recupera la definizione di `$thumbnail$` e genera dinamicamente l&#39;immagine appropriata con le specifiche di ridimensionamento e formattazione definite dal predefinito immagine `thumbnail`. In una stringa URL, tutti gli elementi ad eccezione del nome file dell&#39;immagine del prodotto ( `backpack_trns` in questo caso) sono in genere configurati per il modello della pagina. L’unico elemento che viene inserito automaticamente nel modello di pagina dal vostro server commerciale è l’ID IPS o il nome dell’immagine.
