---
title: Creazione di un modello
seo-title: Creazione di un modello
description: 'null'
seo-description: Scoprite come creare un modello in Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '3441'
ht-degree: 65%

---


# Creazione di un modello {#creating-a-template}

Per creare un modello, fate clic su Genera > Funzioni di base dei modelli. Selezionate Designer o Sviluppatore. In questa pagina potete aggiungere livelli di immagine e testo. Potete anche riordinare livelli, modificarne le dimensioni e la posizione e applicare effetti di ombra e bagliore alle immagini e al testo.

>[!NOTE]
>
>Se modificate un modello creato in una versione precedente di Dynamic Media Classic, potreste ricevere un messaggio di richiesta al momento del salvataggio in cui viene richiesto &quot;Vuoi aggiungere un livello quadro?&quot; Scegliete No per evitare di aggiungere un nuovo livello di base. Se accidentalmente scegliete Sì, eliminate i modificatori “&amp;allowCanvasPrompt” e “&amp;layer=0” dall’URL e premete Invio o A capo.

## Creazione di un modello iniziale {#creating-the-initial-template}

Quando create un set, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

Se necessario, potete creare un modello partendo da uno già esistente. Aprite il modello, fate clic sul pulsante **Salva con nome**, quindi immettete un nuovo nome nella finestra di dialogo Salva con nome.

**Per creare un set di modelli iniziale**

1. Per creare un proprio modello, utilizzate uno dei seguenti metodi:

   **Selezionate prima** il file PSD o le immagini Nel pannello Sfoglia, selezionate il file PSD o le immagini che desiderate per il modello, quindi fate clic su Genera > Funzioni di base dei modelli.

   **Dalla schermata** Modello fate clic su Genera > Funzioni di base dei modelli. Selezionate Designer o Sviluppatore.

1. Nella finestra di dialogo Inserisci dimensioni quadro, immettete i valori di larghezza e altezza per il modello.
1. Selezionate una cartella nella Libreria risorse e trascinate i file PSD o le immagini per il modello nella schermata Modello.
1. Al termine dell’operazione, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **Salva**.
1. Selezionate una cartella in cui memorizzare il modello, immettete un nome per il modello, quindi fate clic sul pulsante **Invia**.

   Se necessario, Dynamic Media Classic riduce le immagini per adattarle al quadro, l’area nella schermata Modello per la definizione del modello.

## Modifica di un set di modelli {#editing-a-template-set}

A seconda se modificate un set pubblicato o non pubblicato, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Il set è già pubblicato | Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio delle modifiche | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il proprio stato di pubblicazione. Tutti i nuovi membri del set aggiunti durante la modifica conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di modelli**

1. Nella visualizzazioni Griglia, individuate un set di modelli e fate clic su **Modifica** sotto l’immagine.
1. Modificate il modello nel modo desiderato.
1. Al termine dell’operazione di modifica, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **Salva**, selezionate una cartella di archiviazione, immettete un nome per il set e fate clic su **Salva**.

## Eliminazione di un modello {#deleting-a-template}

Quando eliminate un set di modelli, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un modello**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più modelli.
1. Nella barra di navigazione globale, fate clic su **File** > **Elimina** > **Elimina**.

## Comprensione della schermata Modello {#understanding-the-template-screen}

La schermata Modello offre strumenti per manipolare e impostare i parametri dei livelli.

Per creare i modelli, usate questi strumenti disponibili nella schermata Modello:

**Strumento** scorrimento Consente di selezionare i livelli, spostarli sul quadro, ridimensionarli o ruotarli.

**Strumento** Testo Consente di creare un livello di testo. Trascinate sul quadro per creare un livello di testo, quindi immettete il testo nel livello. Consultate Creare un livello di testo.

**Pulsante** Anteprima Consente di aprire la schermata Anteprima e di visualizzare il modello in un visualizzatore zoom. per vedere come si presenterà sul sito Web o sull’applicazione.

**Pulsante** Riepilogo parametri Consente di aprire la schermata Riepilogo parametri. Potete visualizzare il nome di ciascun livello in un modello e per ciascun livello i nomi dei parametri che sono stati attivati.

**Editor di testo v4.3 e Editor di testo v4.2** È possibile scegliere di utilizzare l&#39;editor di testo più recente e completo, Editor di testo v4.3 o l&#39;editor di testo precedente, Editor di testo v4.2. Per la creazione di nuovi modelli, per impostazione predefinita viene selezionato Editor di testo v4.3. Per la modifica di modelli meno recenti, per impostazione predefinita viene selezionato Editor di testo v4.2. Editor di testo v4.3 attualmente non supporta il ritorno a capo automatico, quindi per modificare i modelli meno recenti con la funzione di ritorno a capo automatico, usate Editor di testo v4.2. Se il modello meno recente non usa la funzione di ritorno a capo automatico, potete scegliere Editor di testo v4.3 per usare le numerose funzioni che offre, quali Aumenta margini, Riduci margini, Imposta il testo tutto maiuscolo e Adatta testo.

***nota **: Editor di testo v4.2 verrà alla fine rimosso come opzione in Dynamic Media Classic, pertanto si consiglia di utilizzare Editor di testo 4.3 quando possibile. L’opzione Parola a-capo verrà incorporata in una versione futura dell’Editor di testo.*

**Designer e Sviluppatore** Selezionate l&#39;opzione che descrive meglio il vostro ruolo.

**Area di lavoro** Definisce l’area totale disponibile, in pixel, per la definizione del modello. Le dimensioni predefinite sono 300 x 300 pixel. I livelli vengono inseriti nel quadro.

**Elenco** Livelli Elenca il nome dei livelli nel modello. Per selezionare un livello, selezionatene il nome nell’elenco Livelli. L’elenco Livelli offre strumenti per eliminare e riordinare i livelli, per aggiungere effetti e per impostare i parametri dei livelli. Consultate Utilizzo dei livelli.

**Area** Proprietà livello Offre strumenti per modificare il colore di sfondo, l’opacità, le dimensioni e la posizione di un livello, nonché il colore di sfondo, l’opacità e le dimensioni del quadro. Potete anche regolare gli effetti di ombra e bagliore. Consultate Utilizzo dei livelli.

## Creazione di livelli di immagine {#creating-image-layers}

1. Trascinate l’immagine dalla Libreria risorse al quadro.

   Il nome ID dell’immagine viene visualizzato nell’elenco Modelli.

>[!NOTE]
>
>Se necessario, Dynamic Media Classic restringe le immagini per adattarle al quadro quando create un livello immagine.

## Creazione di un livello di testo {#creating-a-text-layer}

1. Fate clic sullo strumento testo.
1. Trascinate per creare una casella di testo sul quadro o su un’immagine.
1. Nella schermata Testo visualizzata, aggiungete il testo effettuando una delle seguenti operazioni nella scheda Anteprima:

   * Digitate il testo desiderato nell’apposita casella. Scegliete Adatta testo per adattare il testo nella rispettiva casella.
   * Incollate il testo dagli Appunti alla casella di testo. 

1. Fate clic su Applica, quindi chiudete la schermata Testo.

### Formattare il testo {#format-text}

Per formattare il testo in un livello di testo, effettuate le seguenti operazioni:

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Nella casella di testo, selezionate il testo che desiderate formattare. Potete selezionare tutto il testo, parti di esso o singoli caratteri.
1. Specificate una delle seguenti opzioni di formattazione, quindi fate clic su Applica.

   **Font** Scegliere un font dal menu Font. Se il font che desiderate usare non viene visualizzato nel menu, potete caricarlo in Dynamic Media Classic. Consultate Font.

   **Dimensione** font Scegliete una dimensione font dal menu, digitate una dimensione specifica nella casella oppure fate clic sulle frecce verso l’alto o il basso per aumentare o diminuire la dimensione di due punti.

   **Colore** Fare clic per scegliere un colore per il testo.

   **Grassetto, Corsivo o Sottolineato** Selezionare il testo, quindi fare clic sull&#39;icona relativa al tipo di formattazione da applicare al testo.

   **Tutte maiuscole, Apice o Pedice** Selezionare il testo, quindi fare clic sull&#39;icona relativa al tipo di formattazione da applicare al testo.

   **Allineamento** Scegliere un pulsante di allineamento per allineare a sinistra, centrare o allineare a destra il testo nel livello di testo.

   **Tipo di tracciamento** o selezionate un valore numerico tramite il quale regolare la quantità di spazio tra le parole.

   **Tipo crenatura** o selezionate un valore numerico tramite il quale regolare la quantità di spazio tra i caratteri.

   **Interlinea** Tipo o selezionare un valore numerico tramite il quale regolare la quantità di spazio tra le righe.

   **Spostamento** linea di base Digitare o selezionare un valore numerico tramite il quale spostare il carattere selezionato verso l&#39;alto o verso il basso rispetto alla linea di base del testo circostante. Questa opzione è utile per impostare manualmente le frazioni o per posizionare gli elementi grafici agganciati al testo.

>[!NOTE]
>
>Fate clic su Annulla per annullare l’ultima azione. Fate clic su Ripristina se cambiate idea dopo aver fatto clic su Annulla.

### Formattare i paragrafi {#format-paragraphs}

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Selezionate il paragrafo che desiderate formattare.
1. Specificate una delle seguenti opzioni di formattazione, quindi fate clic su Applica.

   **Allineamento** Fare clic per specificare il tipo di allineamento: allinea a sinistra, allinea al centro, allinea a destra o giustifica.

   **Fine giustificazione** paragrafo Fare clic per specificare il tipo di giustificazione per l&#39;ultima riga del paragrafo: l&#39;ultima riga allinea a sinistra; l&#39;ultima linea allinea il centro; e l&#39;ultima riga è allineata a destra.

   **Interlinea** Tipo o selezionare un valore numerico tramite il quale regolare la quantità di spazio tra tutte le righe del paragrafo.

   **Rientra tutto** Fare clic per aumentare il rientro del testo.

   **Rimuovi rientro** Fare clic per diminuire il rientro del testo.

   **Rientro prima riga** Consente di specificare il rientro della prima riga del testo.

   **Spazio prima del paragrafo** Specificate la quantità di spazio da inserire sopra la prima riga del testo del paragrafo.

   **Spazio dopo il paragrafo** Specificate la quantità di spazio da inserire sotto l’ultima riga del testo del paragrafo.

   **Allineamento** verticale Consente di selezionare il punto in cui il testo deve essere visualizzato in verticale all’interno della casella di testo: In alto, In mezzo, In basso.

   **Direzione** testo Selezionare la direzione in cui visualizzare il testo: Da destra a sinistra o da sinistra a destra.

### Regolare le proprietà del livello di testo {#adjust-text-layer-properties}

1. Nella schermata funzioni di base dei modelli, selezionate la casella di testo da regolare.
1. Nel pannello Proprietà livello, effettuate una delle seguenti operazioni:

   **Riduci testo (solo Editor di testo v4.2)** Consente di ridurre il testo per adattarlo alla casella di testo.

   **Parola a capo (solo Editor di testo v4.2)** Selezionate un’opzione di ritorno a capo automatico per specificare se o come il testo va a capo:

   **Racchiudi** il testo per adattarlo a una casella di testo troppo piccola in orizzontale.

   **Nessuna a capo** Il testo non va a capo se la casella di testo è troppo piccola in orizzontale e viene tagliata una parte del testo.

   **NB A capo** (a capo automatico) Consente di racchiudere il testo per adattarlo a una casella di testo e non interrompe le parole.

   **Posizione** Specifica la posizione della casella di testo sul quadro.

   **Spaziatura** Consente di aggiungere margini o ritagliare il rettangolo del livello. Specificate il numero di pixel da aggiungere o rimuovere a sinistra, in alto, in basso e a destra. Immettete numeri positivi per aggiungere un margine; immettete numeri negativi per ritagliare.

### Visualizzare e modificare il codice sorgente del testo {#view-and-edit-text-source-code}

Le informazioni fornite nella scheda Sorgente dell’editor di testo fungono da riferimento. Modificate il testo solo se avete esperienza nella modifica del codice sorgente.

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Fate clic sulla scheda Sorgente nell’editor di testo per visualizzare il codice sorgente per il testo.
1. Visualizzate o modificate il testo come desiderate.

   Le modifiche rimangono intatte se passate dalla visualizzazione Anteprima a Sorgente e viceversa.

1. Fate clic su Applica per rendere le modifiche effettive.

## Utilizzo dei livelli {#working-with-layers}

Per effettuare operazioni con i livelli, usate l’elenco Livelli e l’area Proprietà livello. Potete riordinare livelli, modificarne le dimensioni e la posizione, ruotare i livelli e determinare il colore di sfondo, il colore di primo piano, l’opacità e il metodo di fusione di un livello.

Potete anche modificare le dimensioni di un quadro, sceglierne il colore di sfondo e modificarne le impostazioni di opacità.

### Riordinamento dei livelli {#reordering-layers}

Quando si cambia l’ordine dei livelli si possono verificare dei cambiamenti nell’aspetto, in particolare in presenza di trasparenza o sovrastampa. Prima di salvare le modifiche verificate quindi l’anteprima del risultato.

1. Per riordinare i livelli in un modello, effettuate una delle seguenti operazioni:

   * Selezionate un livello nel pannello Livelli. Quindi fate clic sui pulsanti Su o Giù il numero di volte necessario per portarlo nella posizione corretta nell’elenco.
   * Trascinate un livello verso l’alto o il basso nell’elenco Livelli.

### Modifica delle dimensioni e della posizione dei livelli e del quadro {#changing-the-size-and-position-of-layers-and-the-canvas}

I livelli devono essere di dimensioni tali da rientrare nel quadro. Potete modificare le dimensioni di un livello o del quadro manualmente o immettendo i valori desiderati. Potete modificare la posizione di un livello manualmente o immettendo i valori di scostamento desiderati. Potete anche ruotare un livello.

>[!NOTE]
>
>Dynamic Media Classic consiglia di creare un predefinito per immagini delle stesse dimensioni del modello. Quando le dimensioni del predefinito per immagini corrispondono a quelle del modello, si otterranno impostazioni corrette per le dimensioni di output finali e le opzioni di nitidezza per il modello. Dopo aver creato il predefinito per immagini, potete sceglierlo dal menu Applica predefinito sulla schermata Anteprima modello. Nella schermata viene visualizzato l’aspetto dell’immagine che verrà trasmessa dal server. Consultate [Configurazione dei predefiniti per immagini](setting-image-presets.md#setting_up_image_presets).

**Modifica delle dimensioni di un livello**

Per modificare le dimensioni di un livello o del quadro, selezionate il livello o il quadro nell’elenco Livelli ed effettuate una delle seguenti operazioni:

**Modifica manuale delle dimensioni** Selezionate e trascinate un angolo del livello o del quadro. Per i livelli di testo potete anche trascinare un lato del livello. Tenete premuto il tasto Maiusc mentre trascinate per cambiare le dimensioni ma mantenere le stesse proporzioni (forma).

**Immissione delle misure** delle dimensioni del livello Immettete le misure in pixel nelle caselle di testo L (Larghezza) e A (Altezza) nell’area Proprietà livello.

Oltre a modificare le dimensioni di un livello, potete aggiungervi della spaziatura. Per effettuare tale operazione, immettete un valore di spaziatura a sinistra, a destra, in alto e in basso nelle relative caselle dell’area Proprietà livello. La spaziatura consente di aggiungere un margine al livello corrente per scostarlo dal perimetro del suo livello base. La spaziatura è utile per rendere più visibile un eventuale effetto Ombra esterna o Bagliore esterno. La spaziatura consente di aumentare le dimensioni di un livello e di visualizzarne il colore di sfondo nell’area estesa. Il livello viene riposizionato rispetto alle nuove dimensioni del livello. Ad esempio, se il livello corrente è centrato su un livello base, estendendo il lato sinistro si sposta il livello verso destra rispetto al livello base.

**Modifica della posizione di un livello**

Per modificare la posizione di un livello sul quadro, selezionatene il nome nell’elenco Modelli ed effettuate una delle seguenti operazioni:

**Modifica manuale della posizione** Spostare il puntatore vicino ma non sopra il limite di un livello; quando compare il cursore freccia a quattro punte, fare clic e iniziare a trascinare.

**Immissione dei valori** di scostamento della posizione Immettere i valori di scostamento X e Y nelle caselle di testo X e Y. Questi valori rappresentano lo scostamento x, y del punto di ancoraggio in pixel.

**Rotazione di un livello**

La casella Ruota riporta l’angolazione in cui viene ruotato il livello. Per ruotare un livello, selezionatene il nome nell’elenco Livelli ed effettuate una delle seguenti operazioni:

**Rotazione** manuale Consente di spostare il cursore accanto a un angolo del livello, ma non sopra di esso. Quando compare il cursore di rotazione, trascinate l’angolo del livello. Per ruotare per incrementi di 15 gradi, tenete premuto il tasto Maiusc mentre trascinate.

**Immissione di una misura** in gradi Immettere il numero di gradi per ruotare il livello. La rotazione è in senso orario; per ruotare in senso antiorario, immettete un numero negativo.

**Nascondere un livello o un effetto livello**

Potete nascondere un livello o un effetto livello facendo clic sull’icona occhio  accanto al nome del livello o dell’effetto livello. I livelli nascosti non vengono visualizzati nelle anteprime o nell’output. Le informazioni relative al livello non vengono eliminate dall’URL. Al contrario, “hide=1” viene aggiunto all’URL per indicare che il livello è attualmente nascosto. Ad esempio:

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;hide=1&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

### Determinazione del colore di sfondo, dell’opacità e metodo di fusione {#determining-the-background-color-opacity-and-blend-mode}

Per scegliere un colore di sfondo, opacità e metodo di fusione per un livello o per il quadro, selezionate il livello o il quadro ed effettuate le seguenti operazioni:

**Colore** di primo piano Fate clic sul pulsante Colore di primo piano e scegliete un campione colore per modificare il colore dell’ombra o del bagliore. Potete anche immettere un parametro con il valore del colore nella casella. Il colore di sfondo viene applicato solo ai livelli che usano trasparenza. As esempio, viene applicato a un livello parzialmente trasparente in un etichetta con il prezzo o allo sfondo di un campo di testo. I livelli che contengono un’immagine PSD, TIFF o PNG con trasparenza attiva possono disporre di sfondi trasparenti.

**Colore** di sfondo Fare clic sul pulsante Colore di sfondo e scegliere un campione colore per modificare il colore delle aree imbottite.

**Opacità** Trascinate il cursore Opacità per rendere traslucido qualsiasi livello in modo che parte dell’immagine sottostante sia visibile. L’impostazione 100% significa completamente opaco; l’impostazione 0% significa trasparente.

**Metodo** fusione Scegliete un’opzione per simulare uno dei metodi di fusione disponibili in Photoshop. Le opzioni sono Normale, Dissolvenza, Schiarisci, Scurisci, Moltiplica e Scolora. Queste opzioni sono disponibili per i livelli, ma non per il quadro.

## Utilizzo degli effetti ombra e bagliore sui livelli {#using-shadow-and-glow-effects-on-layers}

Potete applicare un’ombra o un bagliore a un livello. L’ombra o il bagliore viene applicato al perimetro del livello e si estende verso l’interno o l’esterno, a seconda dell’opzione scelta. Se il modello è stato creato con un file PSD con effetti ombra e bagliore, potete regolare questi effetti in Dynamic Media Classic.

Dopo aver applicato un effetto ombra o bagliore, potete regolarne le dimensioni, il colore, l’opacità e la posizione nell’area Proprietà livello della schermata Modello.

### Applicazione di un effetto ombra o bagliore a un livello {#applying-a-shadow-or-glow-effect-to-a-layer}

Per applicare un effetto ombra o bagliore:

1. Selezionate un livello nel pannello Livelli.
1. Selezionate il menu Aggiungi effetto e scegliete un’opzione:

   **Ombra** esterna Consente di applicare un’ombra sul lato inferiore e destro del livello.

   **Ombra** interna Consente di applicare un effetto ombra all’interno di tutti i bordi del livello.

   **Bagliore** esterno Applica un effetto bagliore intorno a tutti i bordi del livello.

   **Bagliore** interno Applica un effetto bagliore all’interno di tutti i bordi del livello.

Dopo l’applicazione di un effetto, il suo nome compare nell’elenco Livelli. Per eliminare un effetto, selezionatene il nome nell’elenco Livelli e fate clic sul pulsante Elimina.

>[!NOTE]
>
>a volte non è possibile visualizzare l’effetto di un’ombra esterna o di un bagliore esterno se il livello sottostante non è abbastanza grande per contenerlo. Se non potete visualizzare ombra o bagliore, provate ad aggiungere dei valori di spaziatura al livello o a riordinarlo. Consultate [Modifica delle dimensioni e della posizione dei livelli e del quadro](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) e [Riordinamento dei livelli](creating-template.md#reordering_layers).

### Regolazione di un effetto ombra o bagliore {#adjusting-a-shadow-or-glow-effect}

Per regolare un effetto ombra o bagliore, selezionatene il nome nell’elenco Livelli. Quindi modificatene le impostazioni nell’area Proprietà livello della schermata Modello:

**Colore** Selezionate il pulsante Colore e scegliete un campione colore per modificare il colore dell’ombra o del bagliore. Potete anche immettere un parametro con il valore del colore nella casella.

**Opacità** Trascinate il cursore per determinare l’intensità dell’effetto. Minore è l’opacità, più sono trasparenti gli effetti.

**Metodo** fusione Scegliete un’opzione per simulare uno dei metodi di fusione disponibili in Photoshop. Le opzioni sono Normale, Dissolvenza, Schiarisci, Scurisci, Moltiplica e Scolora.

**Dimensioni** Immettete i valori desiderati nelle caselle X e Y per ingrandire o ridurre l’effetto ombra. Le opzioni Dimensione sono disponibili per le ombre interne ed esterne.

**Aumenta** Trascinate il cursore per estendere l’effetto verso l’interno o l’esterno.

**Sfocatura** Trascinate il cursore per controllare la sfumatura ai bordi dell’effetto. Con una sfocatura maggiore si ottengono bordi più sfumati.

## Maschere di livello {#masking-layers}

L’elenco Modelli offre un pulsante Maschera che consente di specificare come viene usata la maschera o il canale alfa di un livello. Tramite il pulsante Maschera, potete applicare l’effetto di un livello di sfondo a un particolare livello o all’intero livello principale nel modello. Selezionate un livello nell’elenco Livelli e fate clic sul pulsante Maschera  per scorrere tra i seguenti stati:

* Lo sfondo del livello è opaco.
* Il contenuto del livello viene invertito e lo sfondo del livello viene riempito con nero in tinta unita.
* Lo sfondo del livello viene riempito con nero in tinta unita.

