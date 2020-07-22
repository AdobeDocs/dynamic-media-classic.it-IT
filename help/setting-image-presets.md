---
title: Configurazione dei predefiniti immagine
seo-title: Configurazione dei predefiniti immagine
description: 'null'
seo-description: Scoprite come impostare i predefiniti per immagini.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 66%

---


# Configurazione dei predefiniti immagine{#setting-up-image-presets}

Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. Per comprendere l’uso dei predefiniti per immagini, supponete che nel vostro sito Web ciascuna immagine di prodotto possa essere visualizzata in due dimensioni diverse: 500 x 500 pixel e 150 x 150 pixel. In questo caso dovrete creare due predefiniti per immagini, uno denominato “Ingrandimento” e l’altro “Miniatura” per visualizzare le immagini rispettivamente a 500 x 500 e 150 x 150 pixel. Per trasmettere le immagini nelle dimensioni &quot;Ingrandimento&quot; e &quot;Miniatura&quot;, un server immagini Dynamic Media cerca la definizione di Ingrandimento predefinito per immagini e Miniatura. Quindi il server genera in modo dinamico un’immagine secondo le specifiche di ridimensionamento e formattazione di ciascun predefinito per immagini.

Dynamic Media Classic viene fornito con diversi predefiniti per immagini &quot;best practice&quot; già configurati per l’utilizzo. Tuttavia, gli amministratori possono creare nuovi predefiniti per immagini. Per creare un predefinito per immagini, potete partire da zero o iniziare da uno esistente e salvarlo con un nuovo nome.

Le immagini la cui dimensione viene ridotta quando vengono trasmesse da un server in modo dinamico possono perdere nitidezza e dettaglio. Per questa ragione, ciascun predefinito per immagini contiene controlli di formattazione per ottimizzare l’immagine quando questa viene trasmessa in una determinata dimensione. Grazie a tali controlli, le immagini trasmesse al sito Web o all’applicazione restano nitide e chiare.

## Creazione di un predefinito immagine {#creating-an-image-preset}

Se siete l’amministratore della società, potete creare dei predefiniti per immagini in base alle vostre specifiche esigenze. Potete creare nuovi predefiniti per immagini o iniziare con un predefinito per immagini predefinito fornito da Dynamic Media Classic, modificarlo e salvarlo con un nuovo nome.

**Per creare un predefinito per immagini**

1. Fate clic su **Configurazione** > **Predefiniti immagini**.

   Per un’anteprima di un predefinito per immagini esistente, selezionatene il nome in questa schermata. Quando selezionate un nome di predefinito per immagini, l’immagine campione nella finestra Anteprima cambia di conseguenza, assumendo la dimensione e l’aspetto specificati dal predefinito.

1. Effettuate una delle seguenti operazioni:

   * **Per creare un predefinito** per immagini, fate clic su Aggiungi.

   * **Modifica di un predefinito** per immagini Individuate il predefinito per immagini più simile a quello che desiderate creare e fate clic su Modifica.

1. Immettete un nome per il predefinito per immagini.
1. Immettete i valori Larghezza e Altezza in pixel. Tali valori determinano la dimensione in cui verranno trasmesse le immagini.
1. Compilate la schermata Aggiungi predefinito o Modifica predefinito. Per informazioni, consultate [Opzioni dei predefiniti per immagini](application-setup.md#image_preset_options).

   Dynamic Media Classic consiglia di iniziare con le seguenti opzioni &quot;best practice&quot;:

   * **Formato** Scegliere JPEG o un altro formato conforme alle proprie esigenze. Tutti i browser web supportano il formato immagine JPEG, in quanto offre un buon compromesso tra dimensioni ridotte dei file e qualità delle immagini. Tuttavia, le immagini in formato JPEG usano uno schema di compressione che causa la perdita di dati, con possibile introduzione di artefatti di immagine indesiderati, qualora l’impostazione di compressione sia troppo bassa. Per questo motivo, Dynamic Media Classic consiglia di impostare la qualità di compressione (sul cursore) su 75. Questa impostazione offre un buon compromesso tra la qualità delle immagini e le dimensioni ridotte dei file.

   * **Nitidezza** Non selezionate Nitidezza (il filtro di nitidezza offre un controllo inferiore rispetto alle impostazioni Maschera di contrasto).

   * **Modalità** Di Ricampionamento Scegliete Bicubico.

   * **Opzioni** Maschera di contrasto (USM) Immettere le impostazioni mostrate di seguito:
   | Tipo predefinito | Dimensione | USM: Fattore | USM: Raggio | USM: Soglia |
   |--- |--- |--- |--- |--- |
   | Oggetti correlati (mini miniature) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniatura | 150 x 150 | 1,1 | 1 | 5 |
   | Principale | 350 x 350 | 1 | 1 | 6 |
   | Ingrandimento | 500 x 500 | 1,2 | 1,2 | 5 |

1. Fate clic su **Salva**.

Le opzioni &quot;best practice&quot; di Dynamic Media Classic per la creazione di predefiniti per immagini elencate di seguito offrono consigli generali; la nitidezza è molto soggettiva. Queste impostazioni si basano su un’immagine originale 2000 x 2000 e potrebbero pertanto differire per originali di dimensioni maggiori o minori. Per regolare le impostazioni Maschera di contrasto, Dynamic Media Classic consiglia i seguenti intervalli:

* **Importo** compreso tra 0,8 e 1,5.

* **Raggio** compreso tra 0,6 e 2.

* **Soglia** Da 1 A 6.

Per eliminare un predefinito per immagini, selezionatelo nella schermata Predefiniti immagine, quindi fate clic sul pulsante Elimina.

>[!MORELIKETHIS]
>
>* [Creare e modificare i predefiniti immagine](application-setup.md#creating_and_editing_image_presets)
>* [Opzioni dei predefiniti immagine](application-setup.md#image_preset_options)
>* [Anteprima di una risorsa immagine basata sul suo predefinito per immagini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

