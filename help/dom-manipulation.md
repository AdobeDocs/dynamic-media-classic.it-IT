---
title: Modifica DOM
seo-title: Modifica DOM
description: 'null'
seo-description: Informazioni sulla modifica DOM.
uuid: 275 cd 49 d -2 a 55-41 f 9-80 b 0-e 147 d 0 cd 2907
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/template-publishing
discoiquuid: 890 ca 93 e -3146-4347-864 b-bd 5 e 94037038
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Modifica DOM{#dom-manipulation}

La modifica DOM (document object model) è una tecnica per modificare un file di progetto elaborando direttamente il relativo codice XML. La modifica DOM consente di controllare meglio gli elementi di progettazione variabili, inclusi la modifica del contenuto e dell’aspetto. Potete anche creare elementi nuovi in base alle esigenze.

Dynamic Media Classic consente di manipolare il DOM di un modello FXG dinamico in base ai comandi URL dopo la pubblicazione del modello. Gli elementi di progettazione nel modello FXG vengono modificati trasferendo i comandi mediante l’URL. In questo modo, potete modificare e aggiungere dinamicamente gli attributi agli elementi grafici.

Per usare la modifica DOM, create s 7: Gli ID del file Illustrator prima di convertirlo in un file FXG Dynamic Media Classic e caricarlo su SPS.

>[!NOTE]
>
>quando usate i comandi di manipolazione DOM, tutti i valori passati devono essere codificati nell’URL.

>[!NOTE]
>
>Illustrator Plug-in for Web-to-Print (for converting Illustrator files) converts to FXG 2.0. For information about this specification, see [www.adobe.com/go/learn_s7_fxg2_en](https://www.adobe.com/go/learn_s7_fxg2_en).

## Creazione di ID di elementi s7 nei file Illustrator {#creating-s-elementids-in-illustrator-files}

Per usare la modifica DOM con un progetto creato in Illustrator, create gli ID di elementi s7 nel progetto Illustrator. La creazione di ID di elementi s7 consente di modificare gli elementi di progettazione con i comandi URL dopo che il modello è stato pubblicato.

### Creazione di ID di elementi s7 per la modifica DOM del testo {#creating-s-elementids-for-dom-manipulation-of-text}

Per creare un ID di elemento s7 per la modifica DOM di un oggetto di testo, aprite il pannello Livelli in Illustrator. Quindi, nel livello di testo che contiene il testo variabile, assegnate al livello un nome con un ID di elemento s7. To do so, enter the letters `id` (for identification), a colon ( `:`), and a name. Di seguito sono riportati alcuni esempi di nomi per un livello di testo con ID di elementi s7: 

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### Creazione di ID di elementi s7 per la modifica DOM di oggetti {#creating-s-elementids-for-dom-manipulation-of-objects}

Gli ID di elementi s7 devono essere creati quando desiderate consentire agli utenti finali di modificare gli attributi degli oggetti. Gli oggetti possono essere intere cornici di testo, elementi grafici e immagini. Un colore di sfondo è un esempio di ID di elemento oggetto. Gli utenti possono ad esempio cambiare il colore di sfondo di un poster per riflettere la stagione appropriata in base al cambiamento delle stagioni. 

Prima di creare un ID di elemento s7 per un oggetto in Illustrator, create un livello separato per l’oggetto.

Per creare un ID di elemento s7 per un oggetto in Illustrator, eseguite i seguenti passaggi:

1. Selezionate l’oggetto.
1. Fate clic **su Finestre** &gt; **Livelli**.
1. Nel pannello Livelli, denominate il livello dell'oggetto con un elemento s 7: ID. To do so, enter the letters `id` (for identification), a colon ( `:`), and description to identify the element. Di seguito sono riportati alcuni esempi di nomi per un livello oggetto con ID di elemento s7: 

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## Pubblicare modelli FXG {#publish-fxg-templates}

Quando un modello FXG viene pubblicato, viene inserito nei server Dynamic Media Classic, dove è disponibile per il sito Web e l'applicazione. Durante il processo di pubblicazione, Scene7 Publishing System attiva gli URL necessari per il sito Web e l’applicazione.

>[!NOTE]
>
>per usare il modello FXG, pubblicate tutti i contenuti usati crearlo, inclusi i font e le immagini. Se non includete tutti i file necessari, al momento della pubblicazione verrà visualizzato un messaggio di errore.

### Contrassegnare modelli FXG per la pubblicazione {#mark-fxg-templates-for-publish}

I modelli e tutti i relativi file di supporto devono essere contrassegnati per la pubblicazione in modo da essere inseriti nei server immagini Dynamic Media.

1. Nel pannello Sfoglia selezionate il modello FXG insieme agli elementi grafici, alle immagini e ai font usati.
1. Fate clic **su Contrassegna per pubblicazione**.

### Pubblicare il modello FXG {#publish-your-fxg-template}

1. Nella barra di navigazione globale, fate clic su **Pubblica**.
1. Selezionate un’opzione di Quando e facoltativamente immettete un nome per il processo di pubblicazione.
1. Click **Start Publish**.

### Visualizzazione dell’indicatore del testo in eccesso {#text-overflow-indicator-display}

Un *indicatore di testo in eccesso* mostra quando il testo eccede lo spazio allocato al testo in una cornice di testo (o nell’ultima cornice di testo nel caso di testo in più cornici concatenate). Questo indicatori è una casella rossa contenente un segno più (+). Gli indicatori di testo in eccesso in SPS sono sempre attivati.

Text overflow indicators are controlled with the `markOverflowingTextFrame` modifier. Potete usare questo modificatore come segue:

| Modificatore/Valori | Descrizione |
|--- |--- |
| Markoverflowingtextframe = 0,1 | Il valore 1 rende visibile l’indicatore dello scorrimento del testo. Il valore predefinito è 0. Nonostante il valore predefinito sia 0, gli indicatori di testo in eccesso in SPS sono sempre attivati. Tenete presente che il modificatore markOverflowingTextFrame fa distinzione tra maiuscole e minuscole. |

>[!MORELIKETHIS]
>
>* [Definizione di variabilità: parametrizzazione e modifica DOM](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [Pubblicazione](publishing-files.md#publishing_files)

