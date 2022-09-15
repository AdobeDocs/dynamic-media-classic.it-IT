---
title: Creare un modello
description: Scopri come creare un modello in Adobe Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '3469'
ht-degree: 44%

---

# Creare un modello {#creating-a-template}

Per creare un modello, vai a **[!UICONTROL Crea]** > **[!UICONTROL Nozioni di base sui modelli]**. Selezionate Designer o Sviluppatore. In questa pagina potete aggiungere livelli di immagine e testo. Potete anche riordinare livelli, modificarne le dimensioni e la posizione e applicare effetti di ombra e bagliore alle immagini e al testo.

Vedi anche [Nozioni di base sui modelli](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) video di formazione.

>[!NOTE]
>
>Se modifichi un modello creato in una versione precedente di Adobe Dynamic Media Classic, al momento del salvataggio viene richiesto &quot;Aggiungere un livello di quadro?&quot;. Seleziona **[!UICONTROL No]** per evitare di aggiungere un livello base. Se selezioni accidentalmente **[!UICONTROL Sì]**, elimina `&allowCanvasPrompt` e `&layer=0` nell&#39;URL e premi **[!UICONTROL Invio]** o **[!UICONTROL Ritorno]**.

## Crea il modello iniziale {#creating-the-initial-template}

Quando create un set, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** incide su set e relativi membri nei seguenti modi:

| **[!UICONTROL Pubblica dopo il salvataggio]** opzione selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

Se necessario, potete creare un modello partendo da uno già esistente. Apri il modello, seleziona **[!UICONTROL Salva con nome]**, quindi immettete un nuovo nome nella finestra di dialogo Salva con nome.

**Per creare il modello iniziale:**

1. Per creare il modello iniziale, utilizza uno dei metodi seguenti:

   * **Seleziona prima il PSD o le immagini** - Nel pannello Sfoglia, seleziona il file PSD o le immagini che desideri per il modello, vai a **[!UICONTROL Crea]** > **[!UICONTROL Nozioni di base sui modelli]**.

   * **Inizia dalla schermata Modello** - Vai a **[!UICONTROL Crea]** > **[!UICONTROL Nozioni di base sui modelli]**. Selezionate Designer o Sviluppatore.

1. Nella finestra di dialogo Inserisci dimensioni quadro, immettete i valori di larghezza e altezza per il modello.
1. Selezionate una cartella nella Libreria risorse e trascinate i file PSD o le immagini per il modello nella schermata Modello.
1. Al termine dell’operazione, verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**.
1. Selezionare una cartella in cui memorizzare il modello, immettere un nome per il modello e selezionare **[!UICONTROL Invia]**.

   Se necessario, Adobe Dynamic Media Classic restringe le immagini per adattarle all’area di lavoro, l’area nella schermata Modello per la definizione del modello.

## Modificare un set di modelli {#editing-a-template-set}

Se modifichi un set pubblicato o un set di modelli non pubblicato, la variabile **[!UICONTROL Pubblica dopo il salvataggio]** influenza i membri set e set nei seguenti modi:

| Il set è già pubblicato | **[!UICONTROL Pubblica dopo il salvataggio]** opzione selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di modelli:**

1. In Vista a griglia, individuare un set di modelli, quindi selezionare sotto l&#39;immagine **[!UICONTROL Modifica]**.
1. Modificate il modello in base alle necessità.
1. Al termine dell’operazione di modifica, verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, seleziona una cartella di archiviazione, immetti un nome per il set, quindi seleziona **[!UICONTROL Salva]**.

## Eliminare un modello {#deleting-a-template}

Quando eliminate un set di modelli, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un modello:**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più modelli.
1. Nella barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.

## Comprendere la schermata Modello {#understanding-the-template-screen}

La schermata Modello offre strumenti per manipolare e impostare i parametri dei livelli.

Utilizza questi strumenti nella schermata Modello per creare i modelli:

* **[!UICONTROL Pan]** - Consente di selezionare i livelli, spostarli sull&#39;area di lavoro, ridimensionarli o ruotarli.

* **[!UICONTROL Testo]** - Crea un livello di testo. Trascinate sul quadro per creare un livello di testo, quindi immettete il testo nel livello. Vedi [Creazione di un livello di testo](#creating-a-text-layer).

* **[!UICONTROL Anteprima]** - Apre la schermata Anteprima e mostra il modello in un visualizzatore zoom. per vedere come si presenterà sul sito Web o sull’applicazione.

* **[!UICONTROL Riepilogo parametri]** Apre la schermata Riepilogo parametri. Potete visualizzare il nome di ciascun livello in un modello e per ciascun livello i nomi dei parametri che sono stati attivati.

* **[!UICONTROL Editor di testo v4.3 e Editor di testo v4.2]** - È possibile scegliere di utilizzare l’editor di testo più recente e completo, Editor di testo v4.3 o l’editor di testo precedente, Editor di testo v4.2. Quando si creano modelli, Editor di testo v4.3 è selezionato per impostazione predefinita. Per la modifica di modelli meno recenti, per impostazione predefinita viene selezionato Editor di testo v4.2. Editor di testo v4.3 attualmente non supporta il ritorno a capo automatico, quindi per modificare i modelli meno recenti con la funzione di ritorno a capo automatico, usate Editor di testo v4.2. Se il modello precedente non utilizza il ritorno a capo automatico, puoi scegliere Editor di testo v4.3 per sfruttare le numerose nuove funzioni offerte. Ad esempio, Aumenta margini, Diminuisci margini, Imposta testo in tutte le maiuscole e Copia testo adatto.

   >[!NOTE]
   >
   >L’editor di testo v4.2 è pianificato per la rimozione come opzione in Adobe Dynamic Media Classic, pertanto si consiglia di utilizzare l’editor di testo 4.3 quando possibile. La **[!UICONTROL Parola a capo]** Questa opzione verrà incorporata in una versione futura dell’Editor di testo.

* **[!UICONTROL Designer e sviluppatore]** - Seleziona l’opzione che meglio descrive il tuo ruolo.

* **[!UICONTROL Canvas]** - Definisce l’area totale disponibile, in pixel, per la definizione del modello. Le dimensioni predefinite sono 300 x 300 pixel. I livelli vengono inseriti nel quadro.

* **[!UICONTROL Elenco Livelli]** - Elenca il nome dei livelli nel modello. Per selezionare un livello, selezionatene il nome nell’elenco Livelli. L’elenco Livelli offre strumenti per eliminare e riordinare i livelli, per aggiungere effetti e per impostare i parametri dei livelli. Vedi [Operazioni con i livelli](#working-with-layers).

* **[!UICONTROL Area Proprietà livello]** - Offre strumenti per modificare il colore di sfondo, l&#39;opacità, le dimensioni e la posizione di un livello, nonché il colore di sfondo, l&#39;opacità e le dimensioni del quadro. Potete anche regolare gli effetti di ombra e bagliore. Vedi [Operazioni con i livelli](#working-with-layers).

## Creare livelli di immagine {#creating-image-layers}

1. Trascinate l’immagine dalla Libreria risorse al quadro.

   Il nome ID dell’immagine viene visualizzato nell’elenco Modelli.

   >[!NOTE]
   >
   >Se necessario, Adobe Dynamic Media Classic restringe le immagini per adattarle all&#39;area di lavoro quando si crea un livello immagine.

## Creare un livello di testo {#creating-a-text-layer}

1. Seleziona la **[!UICONTROL Testo]** strumento.
1. Trascinate per creare una casella di testo sul quadro o su un’immagine.
1. Nella schermata Testo visualizzata, aggiungete il testo effettuando una delle seguenti operazioni nella scheda Anteprima:

   * Digitate il testo desiderato nell’apposita casella. Scegliete Adatta testo per adattare il testo nella rispettiva casella.
   * Incollate il testo dagli Appunti alla casella di testo. 

1. Seleziona **[!UICONTROL Applica]**, quindi chiudere la schermata Testo .

### Formattare il testo {#format-text}

Per formattare il testo in un livello di testo, procedi come segue:

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Nella casella di testo dell’Editor di testo, selezionare il testo che si desidera formattare. È possibile selezionare tutto il testo, parti del testo o singoli caratteri.
1. Specificare una delle seguenti opzioni di formattazione, quindi selezionare **[!UICONTROL Applica]**.

   * **[!UICONTROL Font]** - Scegliere un font dal menu Font. Se un font desiderato non viene visualizzato nel menu, puoi caricarlo in Adobe Dynamic Media Classic. Consultate Font.

   * **[!UICONTROL Dimensione font]** - Scegliere una dimensione del font dal menu, digitare una dimensione specifica nella casella o selezionare la **[!UICONTROL Su]** o **[!UICONTROL Giù]** frecce per aumentare o diminuire la dimensione di due punti.

   * **[!UICONTROL Colore]** - Selezionare per scegliere un colore per il testo.

   * **[!UICONTROL Grassetto]**, **[!UICONTROL Corsivo]** oppure **[!UICONTROL Sottolineato]** - Selezionare il testo, quindi selezionare l&#39;icona relativa al tipo di formattazione che si desidera applicare al testo.

   * **[!UICONTROL Tutte maiuscole]**, **[!UICONTROL Apice]** oppure **[!UICONTROL Pedice]** - Selezionare il testo, quindi selezionare l&#39;icona relativa al tipo di formattazione che si desidera applicare al testo.

   * **[!UICONTROL Allineamento]** - Scegliere un pulsante Allineamento per allineare il testo a sinistra, al centro o a destra nel livello di testo.

   * **[!UICONTROL Tracking]** - Digitare o selezionare un valore numerico in base al quale regolare la quantità di spazio tra le parole.

   * **[!UICONTROL Crenatura]** - Digitare o selezionare un valore numerico in base al quale regolare la quantità di spazio tra i caratteri.

   * **[!UICONTROL Interlinea]** - Digitare o selezionare un valore numerico in base al quale regolare la quantità di spazio tra le righe.

   * **[!UICONTROL Spostamento linea di base]** - Digitare o selezionare un valore numerico in base al quale spostare un carattere selezionato in alto o in basso rispetto alla linea di base del testo circostante. Questa opzione è utile per impostare manualmente le frazioni o per posizionare gli elementi grafici agganciati al testo.

>[!NOTE]
>
>Seleziona **[!UICONTROL Annulla]** per annullare l’ultima azione. Seleziona **[!UICONTROL Ripeti]** se cambi idea sull&#39;inversione di un&#39;azione dopo aver selezionato **[!UICONTROL Annulla]**.

### Formattare i paragrafi {#format-paragraphs}

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Selezionare il paragrafo da formattare.
1. Specificare una delle seguenti opzioni di formattazione, quindi selezionare **[!UICONTROL Applica]**.

   * **[!UICONTROL Allineamento]** - Selezionare per specificare il tipo di allineamento: allinea a sinistra, allinea al centro, allinea a destra o giustifica.

   * **[!UICONTROL Giustificazione della fine del paragrafo]** - Selezionare per specificare il tipo di giustificazione per l&#39;ultima riga del paragrafo: l&#39;ultima linea si allinea a sinistra; l&#39;ultima linea allinea il centro; e l&#39;ultima riga è allineata a destra.

   * **[!UICONTROL Interlinea]** - Digitare o selezionare un valore numerico in base al quale regolare la quantità di spazio tra tutte le righe del paragrafo.

   * **[!UICONTROL Rientro tutto]** - Selezionare questa opzione per aumentare il rientro del testo.

   * **[!UICONTROL Rimuovi rientro]** - Selezionare questa opzione per ridurre il rientro del testo.

   * **[!UICONTROL Rientro prima riga]** - Specificare la quantità in base alla quale si desidera applicare un rientro alla prima riga di testo.

   * **[!UICONTROL Spazio prima del paragrafo]** - Consente di specificare la quantità di spazio che si desidera visualizzare sopra la prima riga di testo del paragrafo.

   * **[!UICONTROL Spazio dopo il paragrafo]** - Specificare la quantità di spazio che si desidera visualizzare sotto l&#39;ultima riga di testo del paragrafo.

   * **[!UICONTROL Allineamento verticale]** - Selezionare il punto in cui si desidera visualizzare il testo in verticale all’interno della casella di testo: In alto, In mezzo, In basso.

   * **[!UICONTROL Direzione testo]** - Selezionare la direzione in cui visualizzare il testo: Da destra a sinistra o da sinistra a destra.

### Regolare le proprietà del livello di testo {#adjust-text-layer-properties}

1. Nella schermata funzioni di base dei modelli, selezionate la casella di testo da regolare.
1. Nel pannello Proprietà livello, effettuate una delle seguenti operazioni:

   * **[!UICONTROL Testo ridotto (solo Editor di testo v4.2)]** - Per adattarsi alla casella di testo, selezionare per ridurre il testo.

   * **[!UICONTROL Parola a capo (solo Editor di testo v4.2)]** - Per specificare se o come applicare il ritorno a capo al testo, selezionare un’opzione di ritorno a capo automatico:

   * **[!UICONTROL Involucro]** - Racchiude il testo in una casella di testo troppo piccola in orizzontale.

   * **[!UICONTROL Nessun impedimento]** - Non esegue il ritorno a capo automatico del testo quando la casella di testo è troppo piccola in orizzontale, ma taglia una parte del testo.

   * **[!UICONTROL Involucro a tracolla]** - Racchiude il testo in una casella di testo e non interrompe le parole.

   * **[!UICONTROL Posizione]** - Specifica la posizione della casella di testo sull&#39;area di lavoro.

   * **[!UICONTROL Spaziatura]** - Aggiunge margini o ritaglia il rettangolo del livello. Specifica il numero di pixel che desideri aggiungere o rimuovere per Sinistra, Superiore, Inferiore e Destra. Immettere numeri positivi se si desidera aggiungere un margine o numeri negativi da ritagliare.

### Visualizzare e modificare il codice sorgente del testo {#view-and-edit-text-source-code}

Le informazioni fornite nella scheda Sorgente dell’editor di testo fungono da riferimento. Modificate il testo solo se avete esperienza nella modifica del codice sorgente.

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Nell’Editor di testo, per visualizzare il codice sorgente del testo, seleziona la **[!UICONTROL Origine]** nell’Editor di testo.
1. Visualizzate o modificate il testo come desiderate.

   Le modifiche rimangono intatte se passate dalla visualizzazione Anteprima a Sorgente e viceversa.

1. Seleziona **[!UICONTROL Applica]** per eseguire il rendering delle modifiche.

## Operazioni con i livelli {#working-with-layers}

Per effettuare operazioni con i livelli, usate l’elenco Livelli e l’area Proprietà livello. Potete riordinare livelli, modificarne le dimensioni e la posizione, ruotare i livelli e determinare il colore di sfondo, il colore di primo piano, l’opacità e il metodo di fusione di un livello.

Potete anche modificare le dimensioni di un quadro, sceglierne il colore di sfondo e modificarne le impostazioni di opacità.

### Riordina livelli {#reordering-layers}

La modifica dell’ordine dei livelli può influire sull’aspetto, in particolare quando si tratta di trasparenza o sovrastampa. Prima di salvare le modifiche verificate quindi l’anteprima del risultato.

1. Per riordinare i livelli in un modello, effettuate una delle seguenti operazioni:

   * Selezionate un livello nel pannello Livelli. Quindi seleziona **[!UICONTROL Su]** o **[!UICONTROL Giù]** il numero di volte necessario per posizionarlo nella posizione corretta nell’elenco.
   * Trascinate un livello verso l’alto o il basso nell’elenco Livelli.

### Modificare le dimensioni e la posizione dei livelli e del quadro {#changing-the-size-and-position-of-layers-and-the-canvas}

I livelli devono essere di dimensioni tali da rientrare nel quadro. Potete modificare le dimensioni di un livello o del quadro manualmente o immettendo i valori desiderati. Potete modificare la posizione di un livello manualmente o immettendo i valori di scostamento desiderati. Potete anche ruotare un livello.

>[!NOTE]
>
>Adobe Dynamic Media Classic consiglia di creare un predefinito per immagini con le stesse dimensioni del modello. Quando le dimensioni del predefinito per immagini corrispondono a quelle del modello, si otterranno impostazioni corrette per le dimensioni di output finali e le opzioni di nitidezza per il modello. Dopo aver creato il predefinito per immagini, potete sceglierlo dal menu Applica predefinito sulla schermata Anteprima modello. Nella schermata viene visualizzato l’aspetto dell’immagine che verrà trasmessa dal server. Vedi [Impostazione dei predefiniti per immagini](setting-image-presets.md#setting_up_image_presets).

* **Modifica delle dimensioni di un livello** - Per modificare le dimensioni di un livello o dell’area di lavoro, selezionare il livello o l’area di lavoro nell’elenco Livelli e utilizzare una delle seguenti tecniche:

* **Modifica manuale delle dimensioni** - Selezionate e trascinate un angolo del livello o dell&#39;area di lavoro. Per i livelli di testo potete anche trascinare un lato del livello. Tenete premuto il tasto Maiusc mentre trascinate per cambiare le dimensioni ma mantenere le stesse proporzioni (forma).

* **Immissione delle misurazioni delle dimensioni dello strato** - Immettere le misure dei pixel nelle caselle di testo W (Larghezza) e H (Altezza) nell&#39;area Proprietà livello.

Oltre a modificare le dimensioni di un livello, potete aggiungervi della spaziatura. Per effettuare tale operazione, immettete un valore di spaziatura a sinistra, a destra, in alto e in basso nelle relative caselle dell’area Proprietà livello. La spaziatura consente di aggiungere un margine al livello corrente per scostarlo dal perimetro del suo livello base. La spaziatura è utile per rendere più visibile un eventuale effetto Ombra esterna o Bagliore esterno. La spaziatura consente di aumentare le dimensioni di un livello e di visualizzarne il colore di sfondo nell’area estesa. Il livello viene riposizionato rispetto alle nuove dimensioni del livello. Ad esempio, se il livello corrente è centrato su un livello base, estendendo il lato sinistro si sposta il livello verso destra rispetto al livello base.

* **Modifica della posizione di un livello** - Per modificare la posizione di un livello nell&#39;area di lavoro, selezionarne il nome nell&#39;elenco Livelli e utilizzare una delle seguenti tecniche:

* **Modifica manuale della posizione** - Spostare il puntatore vicino a un limite di livello ma non sopra di esso e, quando viene visualizzato il cursore a freccia a quattro punte, selezionare e iniziare a trascinare.

* **Inserimento delle misure di offset della posizione** - Immettere le misure di offset X e Y nelle caselle di testo X e Y. Questi valori rappresentano lo scostamento x, y del punto di ancoraggio in pixel.

* **Rotazione di un livello** - La casella Ruota elenca l&#39;angolo in cui il livello è stato ruotato. Per ruotare un livello, selezionatene il nome nell’elenco Livelli ed effettuate una delle seguenti operazioni:

* **Rotazione manuale** - Spostare il cursore vicino a un angolo del livello ma non sopra di esso. Quando compare il cursore di rotazione, trascinate l’angolo del livello. Per ruotare per incrementi di 15 gradi, tenete premuto il tasto Maiusc mentre trascinate.

* **Inserimento di una misura del grado** - Immettere il numero di gradi per ruotare il livello. La rotazione è in senso orario; per ruotare in senso antiorario, immettete un numero negativo.

**Nascondere un livello o un effetto livello:**

Potete nascondere un livello o un effetto livello selezionando l&#39;icona occhio accanto al nome di un livello o di un effetto. I livelli nascosti non vengono visualizzati nelle anteprime o nell’output. Le informazioni relative al livello non vengono eliminate dall’URL. Invece, `hide=1` viene aggiunto all’URL per notare che il livello è nascosto dalla visualizzazione. Ad esempio:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Determinare il colore di sfondo, l&#39;opacità e il metodo di fusione {#determining-the-background-color-opacity-and-blend-mode}

Per scegliere un colore di sfondo, opacità e metodo di fusione per un livello o per il quadro, selezionate il livello o il quadro ed effettuate le seguenti operazioni:

* **Colore di primo piano** - Seleziona **[!UICONTROL Colore di primo piano]** e scegliete un campione di colore per modificare il colore dell&#39;ombra o del bagliore. Potete anche immettere un parametro con il valore del colore nella casella. Il colore di sfondo viene applicato solo ai livelli che usano trasparenza. As esempio, viene applicato a un livello parzialmente trasparente in un etichetta con il prezzo o allo sfondo di un campo di testo. I livelli che contengono un’immagine PSD, TIFF o PNG con trasparenza attiva possono disporre di sfondi trasparenti.

* **Colore di sfondo** - Seleziona **[!UICONTROL Colore di sfondo]** e scegliete un campione di colore per modificare il colore delle aree imbottite.

* **Opacità** - Trascinate il cursore Opacità per rendere traslucido qualsiasi livello in modo che parte dell&#39;immagine sottostante appaia attraverso. L&#39;impostazione 100% è opaca; 0 è trasparente.

* **Metodo fusione** - Per simulare uno dei metodi di fusione disponibili in Photoshop, scegliete un&#39;opzione. Le opzioni sono Normale, Dissolvenza, Schiarisci, Scurisci, Moltiplica e Scolora. Queste opzioni sono disponibili per i livelli, ma non per il quadro.

## Usa effetti di ombra e bagliore sui livelli {#using-shadow-and-glow-effects-on-layers}

Potete applicare un’ombra o un bagliore a un livello. L’ombra o il bagliore viene applicato al perimetro del livello e si estende verso l’interno o l’esterno, a seconda dell’opzione scelta. Se il modello è stato creato con un file PSD con effetti di ombra e bagliore, è possibile regolare questi effetti in Adobe Dynamic Media Classic.

Dopo aver applicato un effetto ombra o bagliore, potete regolarne le dimensioni, il colore, l’opacità e la posizione nell’area Proprietà livello della schermata Modello.

### Applicare un effetto ombra o bagliore a un livello {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Selezionate un livello nel pannello Livelli.
1. Selezionate il menu Aggiungi effetto e scegliete un’opzione:

   * **[!UICONTROL Ombra esterna]** - Applica un&#39;ombreggiatura al lato inferiore e destro del livello.

   * **[!UICONTROL Ombra interna]** - Applica un effetto ombreggiatura all&#39;interno di tutti i bordi del livello.

   * **[!UICONTROL Bagliore esterno]** - Applica un effetto di bagliore intorno a tutti i bordi del livello.

   * **[!UICONTROL Bagliore interno]** - Applica un effetto di bagliore all&#39;interno di tutti i bordi del livello.

Dopo l’applicazione di un effetto, il suo nome compare nell’elenco Livelli. Per eliminare un effetto, selezionarne il nome nell’elenco Livelli, quindi selezionare **[!UICONTROL Elimina]**.

>[!NOTE]
>
>Talvolta non è possibile vedere l&#39;effetto di un&#39;ombra esterna o di un bagliore esterno se il livello sottostante non è sufficientemente grande per visualizzarlo. Se non è possibile visualizzare l’ombra o il bagliore, è consigliabile aggiungere valori di spaziatura al livello o riordinare il livello. Consultate [Modifica delle dimensioni e della posizione dei livelli e del quadro](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) e [Riordinamento dei livelli](creating-template.md#reordering_layers).

### Regolare un effetto ombra o bagliore {#adjusting-a-shadow-or-glow-effect}

Per regolare un effetto ombra o bagliore, selezionatene il nome nell’elenco Livelli. Quindi modificatene le impostazioni nell’area Proprietà livello della schermata Modello:

* **[!UICONTROL Colore]** - Selezionare il pulsante Colore e scegliere un campione di colore per modificare il colore dell&#39;ombra o del bagliore. Potete anche immettere un parametro con il valore del colore nella casella.

* **[!UICONTROL Opacità]** - Trascinare il cursore per determinare l&#39;intensità dell&#39;effetto. Minore è l’opacità, più sono trasparenti gli effetti.

* **[!UICONTROL Metodo fusione]** - Per simulare uno dei metodi di fusione disponibili in Photoshop, scegliete un&#39;opzione. Le opzioni sono Normale, Dissolvenza, Schiarisci, Scurisci, Moltiplica e Scolora.

* **[!UICONTROL Dimensione]** - Inserire le misure nella casella X e Y per ingrandire o ridurre l&#39;effetto ombra. Le opzioni Dimensione sono disponibili per le ombre interne ed esterne.

* **[!UICONTROL Crescita]** - Trascinare il cursore per estendere l&#39;effetto verso l&#39;interno o verso l&#39;esterno.

* **[!UICONTROL Sfoca]** - Trascinate il cursore per controllare la sfumatura ai bordi dell&#39;effetto. Con una sfocatura maggiore si ottengono bordi più sfumati.

## Livelli maschera {#masking-layers}

L’elenco Modelli offre un pulsante Maschera che consente di specificare come viene usata la maschera o il canale alfa di un livello. Tramite il pulsante Maschera, potete applicare l’effetto di un livello di sfondo a un particolare livello o all’intero livello principale nel modello. Seleziona un livello nell’elenco Livelli e seleziona **[!UICONTROL Maschera]** per scorrere tra questi stati:

* Lo sfondo del livello è opaco.
* Il contenuto del livello viene invertito e lo sfondo del livello viene riempito con nero in tinta unita.
* Lo sfondo del livello viene riempito con nero in tinta unita.
