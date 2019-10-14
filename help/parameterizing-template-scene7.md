---
title: Parametrizzazione di un modello in Dynamic Media Classic
seo-title: Parametrizzazione di un modello in Dynamic Media Classic
description: 'null'
seo-description: Come parametrizzare un modello in Dynamic Media Classic
uuid: 27c8c8b4-47f3-4270-a6db-d304648ba357
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/Categories/template-publishing
discoiquuid: df1a9ff5-a5ba-4480-ba0d-a19bc665f907
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Parametrizzazione di un modello in Dynamic Media Classic{#parameterizing-a-template-in-scene}

Dopo aver caricato in Scene7 Publishing System un modello Illustrator salvato come Dynamic Media Classic FXG, potete definirne gli elementi variabili. A questo scopo, potete usare le schermate Genera e Anteprima di Pubblicazione modelli. Dynamic Media Classic offre strumenti per definire i parametri di testo e oggetti sui livelli e le rispettive proprietà. Potete anche creare versioni differenti di un modello.

La parametrizzazione di un modello FXG consente di personalizzare la variabilità di testo, immagini ed elementi grafici nel modello. È ad esempio possibile parametrizzare una riga di testo in modo che gli utenti finali possano modificare il testo mediante un’interfaccia utente Web. Potete definire campi di testo vuoti come variabili in modo che gli utenti finali possano compilarli con testo personalizzato. Potete inoltre parametrizzare gli attributi e le proprietà degli elementi di progettazione nella schermata Genera di Pubblicazione modelli di Dynamic Media Classic.

>[!NOTE]
>
>La parametrizzazione del modello in Dynamic Media Classic non è necessaria se intendete utilizzare la modifica DOM.

## Definizione dei parametri nei modelli FXG {#defining-parameters-in-fxg-templates}

Per definire i parametri per un modello FXG, effettuate le seguenti operazioni in Dynamic Media Classic:

1. Nella finestra Sfoglia selezionate il file FXG.
1. Click **Build** and choose **Template Publishing**, or click the file’s **Edit** button.

   Viene visualizzata la schermata Pubblicazione modelli.

1. Selezionate LRCo\FXG\Welcome_Summit_10 (file FXG) e fate clic su **Genera** &gt; Pubblicazione **** modelli.</p>

   ![](assets/wp_fxg_edit.png)

1. Nel pannello Livelli della schermata Pubblicazione modelli selezionate il livello contenente gli elementi da parametrizzare. 

   >[!NOTE]
   >
   >Fate clic saltuariamente sull’icona occhio per assicurarvi di avere selezionato l’oggetto desiderato.

1. Nel pannello Proprietà fate clic su un parametro nella colonna Nome (per parametrizzare il testo) o nella colonna Parametro (per parametrizzare gli oggetti).

   * **Testo** Fare clic nel campo di testo (per trovare il campo, scorrete fino in fondo all’elenco Proprietà). Viene visualizzata la finestra di dialogo Parametri. Select the text that you want to parameterize and click **Add**. Potete creare più parametri con la stessa proprietà di testo selezionando diverse porzioni del testo e aggiungendo parametri a ciascuna di esse. To change the name of the parameter, click it, enter a new name, and click **Close**.

   * **Oggetti** Fare clic su una casella nella colonna Parametro. Viene visualizzata la finestra di dialogo Modifica parametro. Enter a name and click **OK**.
   Per personalizzare più attributi contemporaneamente con lo stesso valore, usate lo stesso nome di parametro per ogni attributo. Se ad esempio il modello presenta un rettangolo e una stella, digitate il nome di parametro `newcolor` per specificare l’attributo del colore SolidColor per entrambi. Ogni volta che modificate il valore `newcolor`, sia il rettangolo sia la stella assumono il nuovo colore.

1. Specificate un valore predefinito per l’attributo nel campo Valore o Dati. Impostate tutte le proprietà per l’oggetto selezionato in modo da specificare l’aspetto desiderato.
1. (Facoltativo) Ripetete i passaggi da 3 a 5 per tutti gli oggetti o i livelli che desiderate parametrizzare.
1. Fate clic su **Salva** o **Salva con nome**.
1. Click **Preview** to open the FXG Preview window and see the parameters you created with their default values.

## Mostrare o nascondere un oggetto o un livello nel modello FXG {#show-or-hide-an-object-or-layer-in-the-fxg-template}

Gli oggetti e i livelli nascosti non sono visibili nell’anteprima o nell’output, ma non vengono eliminati dal file. Potete renderli nuovamente visibili se lo desiderate. La visibilità è un attributo che potete rendere variabile. Facendo clic sull’icona con l’occhio per attivarla o disattivarla, impostate il valore predefinito per la visibilità di un oggetto o un livello.

1. Nel pannello Oggetti fate clic sull’icona con l’occhio accanto al nome di un oggetto o livello per nasconderlo nel file.
1. Fate di nuovo clic per rendere l’oggetto visibile.

## Creare versioni differenti di un modello {#create-different-versions-of-a-template}

Potete modificare gli attributi per creare versioni del modello per usi differenti.

Nella schermata Pubblicazione modelli, fate clic su Salva con nome per salvare il file come nuovo modello FXG senza sovrascrivere il modello FXG originale.

## Utilizzo di testo con traccia {#using-stroked-text}

Il testo con traccia rappresenta un esempio di come si possono parametrizzare gli attributi. Dynamic Media Classic supporta le seguenti funzioni per il testo con traccia:

* Larghezza della traccia
* Motivo tratteggiato della traccia
* Diversi stili di giunzione
* Diversi stili di estremità
* Sovrastampa della traccia
* Gestione separata del colore per la traccia, con supporto delle tinte piatte

In questa tabella sono descritti gli attributi supportati per il testo con traccia.

| Attributo | Descrizione |
|--- |--- |
| s7:fill `<Boolean>`(S7FXG Only) | Specifica se il riempimento è abilitato per il testo. Il valore predefinito è true. |
| s7:stroke `<Boolean>` (S7FXG Only) | Specifica se la traccia è abilitata per il testo. Il valore predefinito è false. |
| s7:weight `<number>` (S7FXG Only) | Specifica lo spessore della traccia da applicare al testo, in punti. Il valore predefinito è 1 punto. |
| s7:joints `<string>` (miter, round, bevel) (S7FXG Only) | Specifica il tipo di giunzione da applicare alla traccia. Il valore predefinito è round. |
| s7:caps `<string>` (none, round, square) (S7FXG Only) | Specifica il tipo di estremità da applicare alla traccia. Il valore predefinito è round. |
| s7:miterLimit `<number>` (S7FXG Only) | Specifica il limite quando la giunzione per la traccia è impostata su miter (appuntita). Il valore predefinito è 4. |
| s7:strokeOverprint `<Boolean>` (S7FXG Only) | Specifica se la sovrastampa è abilitata per la traccia. Il valore predefinito è false. |
| s7:strokeColorName (solo per S7FXG) | Come s7:colorName, ma definisce il nome del colore della traccia. |
| s7:strokeColorValue (solo per S7FXG) | Come s7:colorValue, ma definisce il valore del colore usato per la traccia. |
| s7:strokeColorspace (solo per S7FXG) | Come s7:colorspace, ma definisce lo spazio colore per la traccia. |
| flm:dashPattern `<array>` (S7FXG Only) | Per impostazione predefinita non è applicato alcun motivo di trattini e spazi. Questo attributo definisce il motivo di trattini e spazi da applicare alla traccia. Il primo valore corrisponde al trattino del motivo tratteggiato. Il secondo corrisponde allo spazio tra trattini nel motivo tratteggiato. Potete estendere la matrice per più valori, alternando valori per trattini e spazi. |

## Utilizzo di testo alterato {#using-warped-text}

Per testo alterato si intende testo dall’aspetto modificato mediante effetti onda, bandiera, dilatazione e così via.

Il testo alterato è supportato per gli oggetti di tipo Rich Text. Il testo può essere verticale o orizzontale e può essere testo indipendente, in area e su un tracciato. Per applicare l’alterazione al testo, è necessario selezionare l’intero oggetto di testo.

Il testo alterato può essere creato in Adobe Illustrator.

Quando si applica l’alterazione al testo, è possibile impostare i seguenti attributi:

* Stile
* Direzione
* Piega
* Distorsione orizzontale
* Distorsione verticale

Per ogni attributo è disponibile un set di valori.

| Attributo | Valori | Predefinito |
|--- |--- |--- |
| Styles7:warpStyle | nonearcarcLowerarcUpperarchbulgeshellLowershellUpperflagwavefishrisefishEyeinflatesqueezetwist | none |
| Indicazioni7:warpDirection | horizontalvertical | horizontal |
| Piega7:warpBend | Da -1 a 1 | 0,5 |
| Distorsioni orizzontali7:warpHorizontalDistortion | Da -1 a 1 | 0 |
| Distorsione verticale7:warpVerticalDistortion | Da -1 a 1 | 0 |

>[!NOTE]
>
>For `inflate` and `fishEye`, changing the `s7:warpDirection` flag between horizontal and vertical does not have any effect on the output.

Per ulteriori informazioni su come creare e utilizzare il testo alterato, consultate la documentazione di Adobe Illustrator.

>[!MORELIKETHIS]
>
>* [Creare il modello iniziale in Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)
>* [Caricare i file per Pubblicazione modelli](upload-files-template-publishing.md#upload_files_for_template-publishing)

