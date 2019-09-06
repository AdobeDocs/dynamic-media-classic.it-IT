---
title: Configurazione dei predefiniti immagine
seo-title: Configurazione dei predefiniti immagine
description: 'null'
seo-description: Scoprite come impostare i predefiniti per immagini.
uuid: 90530948-dee 9-41 bd-b 39 e -684140446 abc
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/image_ sizing
discoiquuid: 1 ec 39 fe 5-7 b 2 a -4034-9570-6 b 5595 f 97052
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Configurazione dei predefiniti immagine{#setting-up-image-presets}

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Per comprendere l’uso dei predefiniti per immagini, supponete che nel vostro sito Web ciascuna immagine di prodotto possa essere visualizzata in due dimensioni diverse: 500 x 500 pixel e 150 x 150 pixel. In questo caso dovrete creare due predefiniti per immagini, uno denominato “Ingrandimento” e l’altro “Miniatura” per visualizzare le immagini rispettivamente a 500 x 500 e 150 x 150 pixel. Per distribuire le immagini nelle dimensioni «Ingrandimento» e «Miniatura», un server immagini Dynamic Media cerca la definizione del predefinito per immagini Ingrandimento e Miniatura. Quindi il server genera in modo dinamico un’immagine secondo le specifiche di ridimensionamento e formattazione di ciascun predefinito per immagini.

Dynamic Media Classic viene fornito con diversi predefiniti per immagini «best practice» già configurati per l'utilizzo. Tuttavia, gli amministratori possono creare nuovi predefiniti per immagini. Per creare un predefinito per immagini, potete partire da zero o iniziare da uno esistente e salvarlo con un nuovo nome.

Le immagini la cui dimensione viene ridotta quando vengono trasmesse da un server in modo dinamico possono perdere nitidezza e dettaglio. Per questa ragione, ciascun predefinito per immagini contiene controlli di formattazione per ottimizzare l’immagine quando questa viene trasmessa in una determinata dimensione. Grazie a tali controlli, le immagini trasmesse al sito Web o all’applicazione restano nitide e chiare.

## Creazione di un predefinito immagine {#creating-an-image-preset}

Se siete l’amministratore della società, potete creare dei predefiniti per immagini in base alle vostre specifiche esigenze. Potete creare nuovi predefiniti per immagini oppure iniziare con un predefinito per immagini fornito da Dynamic Media Classic, modificarlo e salvarlo con un nuovo nome.

**Per creare un predefinito per immagini**

1. Fate clic su **Configurazione** &gt; **Predefiniti immagini**.

   Per un’anteprima di un predefinito per immagini esistente, selezionatene il nome in questa schermata. Quando selezionate un nome di predefinito per immagini, l’immagine campione nella finestra Anteprima cambia di conseguenza, assumendo la dimensione e l’aspetto specificati dal predefinito.

1. Effettuate una delle seguenti operazioni:

   **Creazione di un
predefinito** per immagini.

   **Modifica di un predefinito** immagine: individuate il predefinito per immagini più simile a quello che desiderate creare, quindi fate clic su Modifica.

1. Immettete un nome per il predefinito per immagini.
1. Immettete i valori Larghezza e Altezza in pixel. Tali valori determinano la dimensione in cui verranno trasmesse le immagini.
1. Compilate la schermata Aggiungi predefinito o Modifica predefinito. Per informazioni, consultate [Opzioni dei predefiniti per immagini](application-setup.md#image_preset_options).

   Dynamic Media Classic consiglia di utilizzare queste opzioni di opzione "best practice" per iniziare:

   **Formato** Scegliete JPEG o un altro formato in base alle vostre esigenze. Il formato di immagini JPEG è supportato da tutti i browser Web; offre il giusto compromesso tra dimensioni ridotte dei file e qualità dell’immagine. Tuttavia, le immagini di formato JPEG usano uno schema di compressione con perdita di dati che introduce artefatti indesiderati se si applica una compressione eccessiva. Per tale ragione, Dynamic Media Classic consiglia di impostare la qualità di compressione (sul cursore) su 75. Questa impostazione offre il giusto compromesso tra qualità delle immagini e dimensione ridotta dei file.

   **Nitidezza** Non selezionate Nitidezza (il filtro di nitidezza offre un controllo inferiore rispetto alle impostazioni Maschera di contrasto).

   **Modalità di ricampionamento** scegliete Bicubico.

   **Opzioni Maschera di contrasto (USM)** Immettete le impostazioni seguenti:

   | Tipo predefinito | Dimensione | USM: Fattore | USM: Raggio | USM: Soglia |
   |--- |--- |--- |--- |--- |
   | Oggetti correlati (mini miniature) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniatura | 150 x 150 | 1,1 | 1 | 5 |
   | Principale | 350 x 350 | 1 | 1 | 6 |
   | Ingrandimento | 500 x 500 | 1,2 | 1,2 | 5 |

1. Fate clic su **Salva**.

Le opzioni «Best practice» di Media Media Classic per la creazione di predefiniti per immagini elencati qui sono consigli generali; La nitidezza è altamente soggettiva. Queste impostazioni si basano su un’immagine originale 2000 x 2000 e potrebbero pertanto differire per originali di dimensioni maggiori o minori. Per regolare le impostazioni Maschera di contrasto, in Media Classic Classic sono consigliati gli intervalli seguenti:

**Amount** Between .8 and 1.5.

**Raggio** tra .6 e 2.

**Soglia** da 1-6.

Per eliminare un predefinito per immagini, selezionatelo nella schermata Predefiniti immagine, quindi fate clic sul pulsante Elimina.

>[!MORELIKETHIS]
>
>* [Creare e modificare i predefiniti immagine](application-setup.md#creating_and_editing_image_presets)
>* [Opzioni dei predefiniti immagine](application-setup.md#image_preset_options)
>* [Anteprima di una risorsa immagine basata sul suo predefinito per immagini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

