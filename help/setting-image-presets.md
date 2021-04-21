---
title: Configurazione dei predefiniti immagine
description: Scopri come impostare i predefiniti per immagini.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Predefiniti immagine
role: Business Practitioner
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 66%

---

# Configurazione dei predefiniti immagine{#setting-up-image-presets}

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Per comprendere l’uso dei predefiniti per immagini, supponete che nel vostro sito Web ciascuna immagine di prodotto possa essere visualizzata in due dimensioni diverse: 500 x 500 pixel e 150 x 150 pixel. In questo caso dovrete creare due predefiniti per immagini, uno denominato “Ingrandimento” e l’altro “Miniatura” per visualizzare le immagini rispettivamente a 500 x 500 e 150 x 150 pixel. Per fornire immagini con le dimensioni &quot;Ingrandisci&quot; e &quot;Miniature&quot;, un server di immagini Dynamic Media cerca la definizione di Ingrandisci predefinito immagine e Predefinito immagine miniatura. Quindi il server genera in modo dinamico un’immagine secondo le specifiche di ridimensionamento e formattazione di ciascun predefinito per immagini.

Dynamic Media Classic include diversi predefiniti immagine &quot;best practice&quot; già configurati per l’utilizzo. Tuttavia, gli amministratori possono creare nuovi predefiniti per immagini. Per creare un predefinito per immagini, potete partire da zero o iniziare da uno esistente e salvarlo con un nuovo nome.

Le immagini la cui dimensione viene ridotta quando vengono trasmesse da un server in modo dinamico possono perdere nitidezza e dettaglio. Per questa ragione, ciascun predefinito per immagini contiene controlli di formattazione per ottimizzare l’immagine quando questa viene trasmessa in una determinata dimensione. Grazie a tali controlli, le immagini trasmesse al sito Web o all’applicazione restano nitide e chiare.

## Creazione di un predefinito immagine  {#creating-an-image-preset}

Se siete l’amministratore della società, potete creare dei predefiniti per immagini in base alle vostre specifiche esigenze. È possibile creare nuovi predefiniti per immagini o iniziare con un predefinito per immagini predefinito fornito da Dynamic Media Classic, modificarlo e salvarlo con un nuovo nome.

**Per creare un predefinito per immagini:**

1. Fate clic su **Configurazione** > **Predefiniti immagini**.

   Per un’anteprima di un predefinito per immagini esistente, selezionatene il nome in questa schermata. Quando selezionate un nome di predefinito per immagini, l’immagine campione nella finestra Anteprima cambia di conseguenza, assumendo la dimensione e l’aspetto specificati dal predefinito.

1. Effettuate una delle seguenti operazioni:

   * **Creazione di un**
predefinito immagineClic su Aggiungi.

   * **Modifica di un**
predefinito per immaginiIndividua il predefinito per immagini più simile a quello che desideri creare, quindi fai clic su Modifica.

1. Immettete un nome per il predefinito per immagini.
1. Immettete i valori Larghezza e Altezza in pixel. Tali valori determinano la dimensione in cui verranno trasmesse le immagini.
1. Compilate la schermata Aggiungi predefinito o Modifica predefinito. Per informazioni, consultate [Opzioni dei predefiniti per immagini](application-setup.md#image_preset_options).

   Dynamic Media Classic consiglia di iniziare con le seguenti opzioni di &quot;best practice&quot;:

   * ****
FormatoScegli JPEG o un altro formato che soddisfi le tue esigenze. Tutti i browser web supportano il formato immagine JPEG, in quanto offre un buon compromesso tra dimensioni ridotte dei file e qualità delle immagini. Tuttavia, le immagini in formato JPEG usano uno schema di compressione che causa la perdita di dati, con possibile introduzione di artefatti di immagine indesiderati, qualora l’impostazione di compressione sia troppo bassa. Per questo motivo, Dynamic Media Classic consiglia di impostare la qualità di compressione (sul cursore) su 75. Questa impostazione offre un buon compromesso tra la qualità delle immagini e le dimensioni ridotte dei file.

   * ****
NitidezzaNon selezionare Nitidezza (il filtro di nitidezza offre un controllo inferiore rispetto alle impostazioni Maschera definizione dettagli).

   * ****
Modalità di ricampionamentoScegliere Bi-Cubic.

   * **Opzioni Maschera definizione dettagli (USM)**
Immetti le impostazioni mostrate qui:
   | Tipo predefinito | Dimensione | USM: Fattore | USM: Raggio | USM: Soglia |
   |--- |--- |--- |--- |--- |
   | Oggetti correlati (mini miniature) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniatura | 150 x 150 | 1,1 | 1 | 5 |
   | Principale | 350 x 350 | 3 | 3 | 6 |
   | Ingrandimento | 500 x 500 | 1,2 | 1,2 | 5 |

1. Fate clic su **Salva**.

Le opzioni di &quot;best practice&quot; di Dynamic Media Classic per la creazione di predefiniti per immagini elencate di seguito sono raccomandazioni generali; la nitidezza è molto soggettiva. Queste impostazioni si basano su un’immagine originale 2000 x 2000 e potrebbero pertanto differire per originali di dimensioni maggiori o minori. Per regolare le impostazioni Maschera definizione dettagli, Dynamic Media Classic consiglia gli intervalli seguenti:

* ****
AmountBetween .8 e 1.5.

* ****
RaggioTra .6 e 2.

* ****
ThresholdFrom 1-6.

Per eliminare un predefinito per immagini, selezionatelo nella schermata Predefiniti immagine, quindi fate clic sul pulsante Elimina.

>[!MORELIKETHIS]
>
>* [Creare e modificare i predefiniti immagine](application-setup.md#creating_and_editing_image_presets)
>* [Opzioni dei predefiniti immagine](application-setup.md#image_preset_options)
>* [Anteprima di una risorsa immagine basata sul suo predefinito per immagini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

