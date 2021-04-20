---
title: Creazione di un modello
description: Scopri come creare un modello in Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '3442'
ht-degree: 65%

---


# Creazione di un modello {#creating-a-template}

Per creare un modello, fate clic su Genera > Funzioni di base dei modelli. Selezionate Designer o Sviluppatore. In questa pagina potete aggiungere livelli di immagine e testo. Potete anche riordinare livelli, modificarne le dimensioni e la posizione e applicare effetti di ombra e bagliore alle immagini e al testo.

>[!NOTE]
>
>Se modifichi un modello creato in una versione precedente di Dynamic Media Classic, potresti ricevere una richiesta al salvataggio chiedendo &quot;Vuoi aggiungere un livello di quadro?&quot; Scegliete No per evitare di aggiungere un nuovo livello di base. Se accidentalmente scegliete Sì, eliminate i modificatori “&amp;allowCanvasPrompt” e “&amp;layer=0” dall’URL e premete Invio o A capo.

## Creazione di un modello iniziale  {#creating-the-initial-template}

Quando create un set, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

Se necessario, potete creare un modello partendo da uno già esistente. Aprite il modello, fate clic sul pulsante **Salva con nome**, quindi immettete un nuovo nome nella finestra di dialogo Salva con nome.

**Per creare un set di modelli iniziale**

1. Per creare un proprio modello, utilizzate uno dei seguenti metodi:

   **Selezionare** prima la PSD o le immaginiNel pannello Sfoglia, selezionare il file PSD o le immagini che si desidera per il modello, fare clic su Genera > Nozioni di base sui modelli.

   **Inizia dalla** schermata ModelloFai clic su Genera > Nozioni di base sui modelli. Selezionate Designer o Sviluppatore.

1. Nella finestra di dialogo Inserisci dimensioni quadro, immettete i valori di larghezza e altezza per il modello.
1. Selezionate una cartella nella Libreria risorse e trascinate i file PSD o le immagini per il modello nella schermata Modello.
1. Al termine dell’operazione, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **Salva**.
1. Selezionate una cartella in cui memorizzare il modello, immettete un nome per il modello, quindi fate clic sul pulsante **Invia**.

   Se necessario, Dynamic Media Classic restringe le immagini per adattarle all’area di lavoro, l’area nella schermata Modello per la definizione del modello.

## Modifica di un set di modelli {#editing-a-template-set}

A seconda se modificate un set pubblicato o non pubblicato, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Il set è già pubblicato | Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio delle modifiche | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono il proprio stato di pubblicazione.Tutti i nuovi membri del set aggiunti durante la modifica conservano il proprio stato di pubblicazione o di annullamento della pubblicazione. |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di modelli**

1. Nella visualizzazioni Griglia, individuate un set di modelli e fate clic su **Modifica** sotto l’immagine.
1. Modificate il modello nel modo desiderato.
1. Al termine dell’operazione di modifica, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **Salva**, selezionate una cartella di archiviazione, immettete un nome per il set e fate clic su **Salva**.

## Eliminazione di un modello  {#deleting-a-template}

Quando eliminate un set di modelli, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un modello**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più modelli.
1. Nella barra di navigazione globale, fate clic su **File** > **Elimina** > **Elimina**.

## Comprensione della schermata Modello {#understanding-the-template-screen}

La schermata Modello offre strumenti per manipolare e impostare i parametri dei livelli.

Per creare i modelli, usate questi strumenti disponibili nella schermata Modello:

**Strumento** PanningConsente di selezionare i livelli, spostarli nell’area di lavoro, ridimensionarli o ruotarli.

**Strumento** TestoCrea un livello di testo. Trascinate sul quadro per creare un livello di testo, quindi immettete il testo nel livello. Consultate Creare un livello di testo.

**Pulsante AnteprimaApre la schermata Anteprima e mostra il modello in un visualizzatore zoom.** per vedere come si presenterà sul sito Web o sull’applicazione.

**Pulsante Riepilogo parametriApre** la schermata Riepilogo parametri. Potete visualizzare il nome di ciascun livello in un modello e per ciascun livello i nomi dei parametri che sono stati attivati.

**Editor di testo v4.3 e Editor di testo v4.2** È possibile scegliere di utilizzare l’editor di testo più recente e completo, Editor di testo v4.3 o l’editor di testo precedente, Editor di testo v4.2. Quando si creano nuovi modelli, Editor di testo v4.3 è selezionato per impostazione predefinita. Per la modifica di modelli meno recenti, per impostazione predefinita viene selezionato Editor di testo v4.2. Editor di testo v4.3 attualmente non supporta il ritorno a capo automatico, quindi per modificare i modelli meno recenti con la funzione di ritorno a capo automatico, usate Editor di testo v4.2. Se il modello meno recente non usa la funzione di ritorno a capo automatico, potete scegliere Editor di testo v4.3 per usare le numerose funzioni che offre, quali Aumenta margini, Riduci margini, Imposta il testo tutto maiuscolo e Adatta testo.

***nota **: L’editor di testo v4.2 verrà infine rimosso come opzione in Dynamic Media Classic, pertanto si consiglia di utilizzare l’editor di testo 4.3 quando possibile. L’opzione Parola a-capo verrà incorporata in una versione futura dell’Editor di testo.*

**Designer e** DeveloperSeleziona l’opzione che descrive meglio il tuo ruolo.

**** Area di lavoroDefinisce l’area totale disponibile, in pixel, per la definizione del modello. Le dimensioni predefinite sono 300 x 300 pixel. I livelli vengono inseriti nel quadro.

**Elenco livelli** Elenca il nome dei livelli nel modello. Per selezionare un livello, selezionatene il nome nell’elenco Livelli. L’elenco Livelli offre strumenti per eliminare e riordinare i livelli, per aggiungere effetti e per impostare i parametri dei livelli. Consultate Utilizzo dei livelli.

**Area Proprietà livello** Offre strumenti per modificare il colore di sfondo, l&#39;opacità, le dimensioni e la posizione di un livello, nonché il colore di sfondo, l&#39;opacità e le dimensioni dell&#39;area di lavoro. Potete anche regolare gli effetti di ombra e bagliore. Consultate Utilizzo dei livelli.

## Creazione di livelli di immagine {#creating-image-layers}

1. Trascinate l’immagine dalla Libreria risorse al quadro.

   Il nome ID dell’immagine viene visualizzato nell’elenco Modelli.

>[!NOTE]
>
>Se necessario, Dynamic Media Classic restringe le immagini per adattarle all&#39;area di lavoro quando create un livello immagine.

## Creazione di un livello di testo {#creating-a-text-layer}

1. Fare clic sullo strumento Testo.
1. Trascinate per creare una casella di testo sul quadro o su un’immagine.
1. Nella schermata Testo visualizzata, aggiungete il testo effettuando una delle seguenti operazioni nella scheda Anteprima:

   * Digitate il testo desiderato nell’apposita casella. Scegliete Adatta testo per adattare il testo nella rispettiva casella.
   * Incollate il testo dagli Appunti alla casella di testo. 

1. Fate clic su Applica, quindi chiudete la schermata Testo.

### Formattare il testo  {#format-text}

Per formattare il testo in un livello di testo, effettuate le seguenti operazioni:

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Nella casella di testo, selezionate il testo che desiderate formattare. Potete selezionare tutto il testo, parti di esso o singoli caratteri.
1. Specificate una delle seguenti opzioni di formattazione, quindi fate clic su Applica.

   **** FontScegli un font dal menu Font. Se un font desiderato non viene visualizzato nel menu, puoi caricarlo in Dynamic Media Classic. Consultate Font.

   **Font** SizeScegliere una dimensione del carattere dal menu, digitare una dimensione specifica nella casella oppure fare clic sulle frecce verso l&#39;alto o verso il basso per aumentare o diminuire la dimensione di due punti.

   **** ColoreFai clic per scegliere un colore per il testo.

   **Grassetto, Corsivo o** SottolineatoSelezionare il testo, quindi fare clic sull&#39;icona relativa al tipo di formattazione che si desidera applicare al testo.

   **Tutto maiuscole, apice o** pediceSelezionare il testo, quindi fare clic sull&#39;icona relativa al tipo di formattazione che si desidera applicare al testo.

   **** AllineamentoScegliere un pulsante Allineamento per allineare a sinistra, al centro o a destra il testo nel livello di testo.

   **** TrackingType o seleziona un valore numerico in base al quale regolare la quantità di spazio tra le parole.

   **** KerningType o seleziona un valore numerico in base al quale regolare la quantità di spazio tra i caratteri.

   **Line** SpacingType o selezionare un valore numerico in base al quale regolare la quantità di spazio tra le righe.

   **Linea di base** ShiftType o selezionare un valore numerico in base al quale spostare un carattere selezionato verso l&#39;alto o verso il basso rispetto alla linea di base del testo circostante. Questa opzione è utile per impostare manualmente le frazioni o per posizionare gli elementi grafici agganciati al testo.

>[!NOTE]
>
>Fate clic su Annulla per annullare l’ultima azione. Fate clic su Ripristina se cambiate idea dopo aver fatto clic su Annulla.

### Formattare i paragrafi  {#format-paragraphs}

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Selezionate il paragrafo che desiderate formattare.
1. Specificate una delle seguenti opzioni di formattazione, quindi fate clic su Applica.

   **** AllineamentoFare clic per specificare il tipo di allineamento: allinea a sinistra, allinea al centro, allinea a destra o giustifica.

   **Fine** giustificazione paragrafoFare clic per specificare il tipo di giustificazione per l&#39;ultima riga del paragrafo: l&#39;ultima linea si allinea a sinistra; l&#39;ultima linea allinea il centro; e l&#39;ultima riga è allineata a destra.

   **Tipo di** spaziatura linea o selezionare un valore numerico in base al quale regolare la quantità di spazio tra tutte le righe del paragrafo.

   **Rientra** tuttoFare clic per aumentare il rientro del testo.

   **Rimuovi** rientroFare clic per ridurre il rientro del testo.

   **Rientro prima** rigaSpecifica la quantità di rientro della prima riga di testo.

   **Spazio prima del** paragrafoConsente di specificare la quantità di spazio che si desidera visualizzare sopra la prima riga di testo del paragrafo.

   **Spazio dopo** paragrafoConsente di specificare la quantità di spazio che si desidera visualizzare sotto l’ultima riga di testo del paragrafo.

   **Allinea** in verticaleSelezionare la posizione in cui il testo deve essere visualizzato in verticale all’interno della casella di testo: In alto, In mezzo, In basso.

   **Direzione** testoSelezionare la direzione in cui si desidera visualizzare il testo: Da destra a sinistra o da sinistra a destra.

### Regolare le proprietà del livello di testo {#adjust-text-layer-properties}

1. Nella schermata funzioni di base dei modelli, selezionate la casella di testo da regolare.
1. Nel pannello Proprietà livello, effettuate una delle seguenti operazioni:

   **Testo ridotto (solo Editor di testo v4.2)** Selezionare questa opzione per ridurre il testo e adattarlo alla casella di testo.

   **A capo automatico (solo nell’Editor di testo v4.2)** Selezionate un’opzione a capo automatico per specificare se o come applicare al testo il ritorno a capo:

   **** WrapRacchiude il testo in una casella di testo troppo piccola in orizzontale.

   **Nessun** ritorno a capoNon esegue il ritorno a capo automatico del testo quando la casella di testo è troppo piccola in orizzontale e, invece, taglia una parte del testo.

   **NB Wrap**  (ritorno a capo non interrotto) Racchiude il testo per inserirlo in una casella di testo e non interrompe le parole.

   **** PosizioneSpecifica la posizione della casella di testo sull&#39;area di lavoro.

   **** PaddingAggiunge margini o ritaglia il rettangolo di livello. Specificate il numero di pixel da aggiungere o rimuovere a sinistra, in alto, in basso e a destra. Immettete numeri positivi per aggiungere un margine; immettete numeri negativi per ritagliare.

### Visualizzare e modificare il codice sorgente del testo {#view-and-edit-text-source-code}

Le informazioni fornite nella scheda Sorgente dell’editor di testo fungono da riferimento. Modificate il testo solo se avete esperienza nella modifica del codice sorgente.

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Fate clic sulla scheda Sorgente nell’editor di testo per visualizzare il codice sorgente per il testo.
1. Visualizzate o modificate il testo come desiderate.

   Le modifiche rimangono intatte se passate dalla visualizzazione Anteprima a Sorgente e viceversa.

1. Fate clic su Applica per rendere le modifiche effettive.

## Utilizzo dei livelli  {#working-with-layers}

Per effettuare operazioni con i livelli, usate l’elenco Livelli e l’area Proprietà livello. Potete riordinare livelli, modificarne le dimensioni e la posizione, ruotare i livelli e determinare il colore di sfondo, il colore di primo piano, l’opacità e il metodo di fusione di un livello.

Potete anche modificare le dimensioni di un quadro, sceglierne il colore di sfondo e modificarne le impostazioni di opacità.

### Riordinamento dei livelli  {#reordering-layers}

Quando si cambia l’ordine dei livelli si possono verificare dei cambiamenti nell’aspetto, in particolare in presenza di trasparenza o sovrastampa. Prima di salvare le modifiche verificate quindi l’anteprima del risultato.

1. Per riordinare i livelli in un modello, effettuate una delle seguenti operazioni:

   * Selezionate un livello nel pannello Livelli. Quindi fate clic sui pulsanti Su o Giù il numero di volte necessario per portarlo nella posizione corretta nell’elenco.
   * Trascinate un livello verso l’alto o il basso nell’elenco Livelli.

### Modifica delle dimensioni e della posizione dei livelli e del quadro  {#changing-the-size-and-position-of-layers-and-the-canvas}

I livelli devono essere di dimensioni tali da rientrare nel quadro. Potete modificare le dimensioni di un livello o del quadro manualmente o immettendo i valori desiderati. Potete modificare la posizione di un livello manualmente o immettendo i valori di scostamento desiderati. Potete anche ruotare un livello.

>[!NOTE]
>
>Dynamic Media Classic consiglia di creare un predefinito per immagini con le stesse dimensioni del modello. Quando le dimensioni del predefinito per immagini corrispondono a quelle del modello, si otterranno impostazioni corrette per le dimensioni di output finali e le opzioni di nitidezza per il modello. Dopo aver creato il predefinito per immagini, potete sceglierlo dal menu Applica predefinito sulla schermata Anteprima modello. Nella schermata viene visualizzato l’aspetto dell’immagine che verrà trasmessa dal server. Consultate [Configurazione dei predefiniti per immagini](setting-image-presets.md#setting_up_image_presets).

**Modifica delle dimensioni di un livello**

Per modificare le dimensioni di un livello o del quadro, selezionate il livello o il quadro nell’elenco Livelli ed effettuate una delle seguenti operazioni:

**Modifica manuale delle** dimensioniSeleziona e trascina un angolo del livello o dell’area di lavoro. Per i livelli di testo potete anche trascinare un lato del livello. Tenete premuto il tasto Maiusc mentre trascinate per cambiare le dimensioni ma mantenere le stesse proporzioni (forma).

**Inserimento di** misure di dimensione del livelloImmettere le misure dei pixel nelle caselle di testo W (Larghezza) e H (Altezza) nell&#39;area Proprietà livello.

Oltre a modificare le dimensioni di un livello, potete aggiungervi della spaziatura. Per effettuare tale operazione, immettete un valore di spaziatura a sinistra, a destra, in alto e in basso nelle relative caselle dell’area Proprietà livello. La spaziatura consente di aggiungere un margine al livello corrente per scostarlo dal perimetro del suo livello base. La spaziatura è utile per rendere più visibile un eventuale effetto Ombra esterna o Bagliore esterno. La spaziatura consente di aumentare le dimensioni di un livello e di visualizzarne il colore di sfondo nell’area estesa. Il livello viene riposizionato rispetto alle nuove dimensioni del livello. Ad esempio, se il livello corrente è centrato su un livello base, estendendo il lato sinistro si sposta il livello verso destra rispetto al livello base.

**Modifica della posizione di un livello**

Per modificare la posizione di un livello sul quadro, selezionatene il nome nell’elenco Modelli ed effettuate una delle seguenti operazioni:

**Modifica manuale della** posizioneSpostare il puntatore vicino a un limite di livello ma non sopra di esso e, quando viene visualizzato il cursore a freccia a quattro punte, fare clic su e iniziare a trascinare.

**Inserimento delle** misure di offset della posizioneImmettere le misure di offset X e Y nelle caselle di testo X e Y. Questi valori rappresentano lo scostamento x, y del punto di ancoraggio in pixel.

**Rotazione di un livello**

La casella Ruota riporta l’angolazione in cui viene ruotato il livello. Per ruotare un livello, selezionatene il nome nell’elenco Livelli ed effettuate una delle seguenti operazioni:

**Rotazione manualeSpostare il cursore accanto a un angolo del livello ma non sopra di esso.** Quando compare il cursore di rotazione, trascinate l’angolo del livello. Per ruotare per incrementi di 15 gradi, tenete premuto il tasto Maiusc mentre trascinate.

**Immissione di una** misura del gradoImmettere il numero di gradi per ruotare il livello. La rotazione è in senso orario; per ruotare in senso antiorario, immettete un numero negativo.

**Nascondere un livello o un effetto livello**

Potete nascondere un livello o un effetto livello facendo clic sull’icona occhio  accanto al nome del livello o dell’effetto livello. I livelli nascosti non vengono visualizzati nelle anteprime o nell’output. Le informazioni relative al livello non vengono eliminate dall’URL. Al contrario, “hide=1” viene aggiunto all’URL per indicare che il livello è attualmente nascosto. Ad esempio:

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;hide=1&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

### Determinazione del colore di sfondo, dell’opacità e metodo di fusione  {#determining-the-background-color-opacity-and-blend-mode}

Per scegliere un colore di sfondo, opacità e metodo di fusione per un livello o per il quadro, selezionate il livello o il quadro ed effettuate le seguenti operazioni:

**Colore** di primo pianoFare clic sul pulsante Colore di primo piano e scegliere un campione di colore per modificare il colore dell&#39;ombra o del bagliore. Potete anche immettere un parametro con il valore del colore nella casella. Il colore di sfondo viene applicato solo ai livelli che usano trasparenza. As esempio, viene applicato a un livello parzialmente trasparente in un etichetta con il prezzo o allo sfondo di un campo di testo. I livelli che contengono un’immagine PSD, TIFF o PNG con trasparenza attiva possono disporre di sfondi trasparenti.

**Colore di sfondoFare clic sul pulsante Colore di sfondo e scegliere un campione di colore per modificare il colore delle aree imbottite.** 

**** OpacitàTrascinate il cursore Opacità per rendere traslucido qualsiasi livello in modo che parte dell&#39;immagine sottostante sia visibile attraverso. L’impostazione 100% significa completamente opaco; l’impostazione 0% significa trasparente.

**Metodo fusioneScegliere un&#39;opzione per simulare uno dei metodi di fusione disponibili in Photoshop.** Le opzioni sono Normale, Dissolvenza, Schiarisci, Scurisci, Moltiplica e Scolora. Queste opzioni sono disponibili per i livelli, ma non per il quadro.

## Utilizzo degli effetti ombra e bagliore sui livelli  {#using-shadow-and-glow-effects-on-layers}

Potete applicare un’ombra o un bagliore a un livello. L’ombra o il bagliore viene applicato al perimetro del livello e si estende verso l’interno o l’esterno, a seconda dell’opzione scelta. Se il modello è stato creato con un file PSD con effetti di ombra e bagliore, è possibile regolare questi effetti in Dynamic Media Classic.

Dopo aver applicato un effetto ombra o bagliore, potete regolarne le dimensioni, il colore, l’opacità e la posizione nell’area Proprietà livello della schermata Modello.

### Applicazione di un effetto ombra o bagliore a un livello  {#applying-a-shadow-or-glow-effect-to-a-layer}

Per applicare un effetto ombra o bagliore:

1. Selezionate un livello nel pannello Livelli.
1. Selezionate il menu Aggiungi effetto e scegliete un’opzione:

   **Ombreggiatura esternaApplica un&#39;ombreggiatura al lato inferiore e destro del livello.** 

   **Ombreggiatura internaApplica un effetto ombra all&#39;interno di tutti i bordi del livello.** 

   **Bagliore esternoApplica un effetto di bagliore intorno a tutti i bordi del livello.** 

   **Inner** GlowApplica un effetto di bagliore all&#39;interno di tutti i bordi del livello.

Dopo l’applicazione di un effetto, il suo nome compare nell’elenco Livelli. Per eliminare un effetto, selezionatene il nome nell’elenco Livelli e fate clic sul pulsante Elimina.

>[!NOTE]
>
>a volte non è possibile visualizzare l’effetto di un’ombra esterna o di un bagliore esterno se il livello sottostante non è abbastanza grande per contenerlo. Se non potete visualizzare ombra o bagliore, provate ad aggiungere dei valori di spaziatura al livello o a riordinarlo. Consultate [Modifica delle dimensioni e della posizione dei livelli e del quadro](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) e [Riordinamento dei livelli](creating-template.md#reordering_layers).

### Regolazione di un effetto ombra o bagliore  {#adjusting-a-shadow-or-glow-effect}

Per regolare un effetto ombra o bagliore, selezionatene il nome nell’elenco Livelli. Quindi modificatene le impostazioni nell’area Proprietà livello della schermata Modello:

**** ColoreSeleziona il pulsante Colore e scegli un campione di colore per modificare il colore dell’ombra o del bagliore. Potete anche immettere un parametro con il valore del colore nella casella.

**** OpacitàTrascina il cursore per determinare l&#39;intensità dell&#39;effetto. Minore è l’opacità, più sono trasparenti gli effetti.

**Metodo fusioneScegliere un&#39;opzione per simulare uno dei metodi di fusione disponibili in Photoshop.** Le opzioni sono Normale, Dissolvenza, Schiarisci, Scurisci, Moltiplica e Scolora.

**** DimensioniImmettere le misure nella casella X e Y per ingrandire o ridurre l&#39;effetto ombra. Le opzioni Dimensione sono disponibili per le ombre interne ed esterne.

**** AumentaTrascina il cursore per estendere l’effetto verso l’interno o verso l’esterno.

**** BlurTrascina il cursore per controllare la sfumatura ai bordi dell&#39;effetto. Con una sfocatura maggiore si ottengono bordi più sfumati.

## Maschere di livello  {#masking-layers}

L’elenco Modelli offre un pulsante Maschera che consente di specificare come viene usata la maschera o il canale alfa di un livello. Tramite il pulsante Maschera, potete applicare l’effetto di un livello di sfondo a un particolare livello o all’intero livello principale nel modello. Selezionate un livello nell’elenco Livelli e fate clic sul pulsante Maschera  per scorrere tra i seguenti stati:

* Lo sfondo del livello è opaco.
* Il contenuto del livello viene invertito e lo sfondo del livello viene riempito con nero in tinta unita.
* Lo sfondo del livello viene riempito con nero in tinta unita.

