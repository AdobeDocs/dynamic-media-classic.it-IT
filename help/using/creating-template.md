---
title: Creare un modello
description: Scopri come creare un modello in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
topic: Content Management
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '3433'
ht-degree: 36%

---

# Creare un modello

Per creare un modello, vai a **[!UICONTROL Build]** > **[!UICONTROL Nozioni di base sui modelli]**. Selezionate Designer o Sviluppatore. In questa pagina potete aggiungere livelli di immagine e testo. Potete anche riordinare livelli, modificarne le dimensioni e la posizione e applicare effetti di ombra e bagliore alle immagini e al testo.

Vedi anche il video di formazione [Nozioni di base sui modelli](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

>[!NOTE]
>
>Se si modifica un modello creato in una versione precedente di Adobe Dynamic Media Classic, viene visualizzato un messaggio che richiede di salvare &quot;Aggiungere un livello area di lavoro?&quot; Seleziona **[!UICONTROL No]** per evitare di aggiungere un livello base. Se selezioni accidentalmente **[!UICONTROL Sì]**, elimina i modificatori `&allowCanvasPrompt` e `&layer=0` nell&#39;URL e premi **[!UICONTROL Invio]** o **[!UICONTROL Ritorno]**.

## Creare il modello iniziale {#creating-the-initial-template}

Quando si crea un set di modelli, l&#39;opzione **[!UICONTROL Pubblica dopo un salvataggio]** ha effetto sui membri del set e del set nei modi seguenti:

| **[!UICONTROL Pubblicare dopo aver selezionato un&#39;opzione di salvataggio]** prima di salvare? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

Se necessario, potete creare un modello partendo da uno già esistente. Aprire il modello, selezionare **[!UICONTROL Salva con nome]** e immettere un nuovo nome nella finestra di dialogo Salva con nome.

**Per creare il modello iniziale:**

1. Per creare il modello iniziale, utilizzare uno dei metodi seguenti:

   * **Seleziona prima il PSD o le immagini**: nel pannello Sfoglia, seleziona il file PSD o le immagini che desideri per il modello, vai a **[!UICONTROL Genera]** > **[!UICONTROL Nozioni di base sul modello]**.

   * **Inizia dalla schermata Modello**: passa a **[!UICONTROL Build]** > **[!UICONTROL Nozioni di base modello]**. Selezionate Designer o Sviluppatore.

1. Nella finestra di dialogo Immetti dimensioni area di lavoro immettere le dimensioni di larghezza e altezza per il modello.
1. Selezionate una cartella nella Libreria risorse e trascinate i file PSD o le immagini per il modello nella schermata Modello.
1. Al termine, vicino all&#39;angolo inferiore destro della pagina, assicurati che sia selezionato **[!UICONTROL Pubblica dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**.
1. Seleziona una cartella per l&#39;archiviazione del modello, immetti un nome per il modello e seleziona **[!UICONTROL Invia]**.

   Adobe Dynamic Media Classic riduce le immagini se necessario per adattarle all’area di lavoro, l’area nella schermata Modello per definire il modello.

## Modificare un set di modelli {#editing-a-template-set}

Sia che si modifichi un set pubblicato o un set di modelli non pubblicato, l&#39;opzione **[!UICONTROL Pubblica dopo un salvataggio]** ha effetto sui membri del set e del set nei modi seguenti:

| Il set è già pubblicato | **[!UICONTROL Pubblicare dopo aver selezionato l&#39;opzione di salvataggio]** prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono lo stato pubblicato. I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un set di modelli:**

1. Nella visualizzazione griglia, passare a un set di modelli e quindi selezionare **[!UICONTROL Modifica]** sotto l&#39;immagine.
1. Modifica il modello in base alle esigenze.
1. Al termine della modifica, vicino all&#39;angolo inferiore destro della pagina, assicurati che sia selezionato **[!UICONTROL Pubblica dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, seleziona una cartella di archiviazione, immetti un nome per il set, quindi seleziona **[!UICONTROL Salva]**.

## Eliminare un modello

Quando si elimina un set di modelli, il set stesso viene spostato nel cestino. Tuttavia, i membri (o &quot;figli&quot;) all&#39;interno di quel set non sono interessati; invece, ciascuno di essi mantiene il proprio stato pubblicato o non pubblicato esistente.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un modello:**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più modelli.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.

## Comprendere la schermata Modello {#understanding-the-template-screen}

La schermata Modello offre strumenti per manipolare e impostare i parametri dei livelli.

Utilizza questi strumenti nella schermata Modello per creare modelli:

* **[!UICONTROL Panoramica]**: consente di selezionare i livelli, spostarli nell&#39;area di lavoro, ridimensionarli o ruotarli.

* **[!UICONTROL Testo]**: crea un livello di testo. Trascinate sul quadro per creare un livello di testo, quindi immettete il testo nel livello. Vedere [Creazione di un livello di testo](#creating-a-text-layer).

* **[!UICONTROL Anteprima]**: apre la schermata Anteprima e mostra il modello in un Visualizzatore zoom. È possibile visualizzare l&#39;aspetto del modello per gli utenti del sito Web o dell&#39;applicazione.

* **[!UICONTROL Riepilogo parametri]** Apre la schermata Riepilogo parametri. Potete visualizzare il nome di ciascun livello in un modello e per ciascun livello i nomi dei parametri che sono stati attivati.

* **[!UICONTROL Editor di testo v4.3 e Editor di testo v4.2]**: utilizza l&#39;editor di testo più recente e completo. È possibile scegliere di utilizzare Editor di testo v4.3 o l&#39;Editor di testo v4.2 precedente. Per impostazione predefinita, durante la creazione di modelli, è selezionato Editor di testo v. 4.3. Per la modifica di modelli meno recenti, per impostazione predefinita viene selezionato Editor di testo v4.2. L’editor di testo v. 4.3 non supporta attualmente il ritorno a capo automatico, pertanto quando si modificano modelli meno recenti che utilizzano il ritorno a capo automatico, utilizza l’editor di testo v. 4.2 per mantenere completamente intatta la fedeltà del modello. Se il modello meno recente non utilizza il ritorno a capo automatico, è possibile scegliere Editor di testo v. 4.3 per sfruttare le numerose nuove funzionalità offerte. Ad esempio, aumentare i margini, diminuire i margini, impostare il testo in maiuscolo e copiare il testo adattato.

  >[!NOTE]
  >
  >L’editor di testo v. 4.2 è pianificato per la rimozione come opzione in Adobe Dynamic Media Classic. Si consiglia di utilizzare Editor di testo 4.3 quando possibile. L&#39;opzione **[!UICONTROL Parola a capo]** verrà incorporata in una versione futura dell&#39;editor di testo.

* **[!UICONTROL Designer e sviluppatori]**: seleziona l&#39;opzione che descrive meglio il tuo ruolo.

* **[!UICONTROL Area di lavoro]**: definisce l&#39;area totale disponibile, in pixel, per la definizione del modello. La dimensione predefinita è 300 × 300 pixel. I livelli vengono inseriti nel quadro.

* **[!UICONTROL Elenco livelli]**: elenca il nome dei livelli nel modello. Per selezionare un livello, selezionatene il nome nell’elenco Livelli. L’elenco Livelli offre strumenti per eliminare e riordinare i livelli, per aggiungere effetti e per impostare i parametri dei livelli. Vedi [Operazioni con i livelli](#working-with-layers).

* **[!UICONTROL Area Proprietà livello]**: quest&#39;area offre gli strumenti per modificare il colore di sfondo, l&#39;opacità, le dimensioni e la posizione di un livello. È inoltre possibile modificare il colore di sfondo, l&#39;opacità e le dimensioni dell&#39;area di lavoro. Potete anche regolare gli effetti di ombra e bagliore. Vedi [Operazioni con i livelli](#working-with-layers).

## Creare livelli di immagine {#creating-image-layers}

1. Trascinate l’immagine dalla Libreria risorse al quadro.

   Il nome ID dell’immagine viene visualizzato nell’elenco Modelli.

   >[!NOTE]
   >
   >Se necessario, Adobe Dynamic Media Classic riduce le immagini per adattarle all’area di lavoro durante la creazione di un livello immagine.

## Creare un livello di testo {#creating-a-text-layer}

1. Selezionare lo strumento **[!UICONTROL Testo]**.
1. Trascinate per creare una casella di testo sul quadro o su un’immagine.
1. Nella schermata Testo visualizzata, aggiungi il testo effettuando una delle seguenti operazioni nella scheda Anteprima:

   * Digitate il testo desiderato nell’apposita casella. Scegliete Adatta testo per adattare il testo nella rispettiva casella.
   * Incollate il testo dagli Appunti alla casella di testo. 

1. Selezionare **[!UICONTROL Applica]**, quindi chiudere la schermata Testo.

### Formattare il testo {#format-text}

Per formattare il testo in un livello di testo, effettuate le seguenti operazioni:

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Nella casella di testo dell&#39;Editor di testo selezionare il testo che si desidera formattare. È possibile selezionare tutto il testo, parti di testo o singoli caratteri.
1. Specificare una delle opzioni di formattazione seguenti, quindi selezionare **[!UICONTROL Applica]**.

   * **[!UICONTROL Carattere]**: scegliere un tipo di carattere dal menu Carattere. Se il tipo di carattere desiderato non viene visualizzato nel menu, è possibile caricarlo in Adobe Dynamic Media Classic. Consulta Tipi di carattere.

   * **[!UICONTROL Dimensione font]**: scegli una dimensione font dal menu, digita una dimensione specifica nella casella oppure seleziona le frecce **[!UICONTROL Su]** o **[!UICONTROL Giù]** per aumentare o diminuire la dimensione di due punti.

   * **[!UICONTROL Colore]**: selezionare un colore per il testo.

   * **[!UICONTROL Grassetto]**, **[!UICONTROL Corsivo]** o **[!UICONTROL Sottolineato]**: selezionare il testo, quindi selezionare l&#39;icona relativa al tipo di formattazione da applicare al testo.

   * **[!UICONTROL Tutto maiuscole]**, **[!UICONTROL Apice]** o **[!UICONTROL Pedice]**: selezionare il testo, quindi selezionare l&#39;icona relativa al tipo di formattazione da applicare al testo.

   * **[!UICONTROL Allineamento]**: scegliere un pulsante Allineamento per allineare il testo a sinistra, al centro o a destra nel livello di testo.

   * **[!UICONTROL Tracciamento]**: digitare o selezionare un valore numerico in base al quale regolare la quantità di spazio tra le parole.

   * **[!UICONTROL Crenatura]**: digitare o selezionare un valore numerico in base al quale regolare lo spazio tra i caratteri.

   * **[!UICONTROL Interlinea]**: digitare o selezionare un valore numerico in base al quale regolare la quantità di spazio tra le righe.

   * **[!UICONTROL Spostamento linea di base]**: digitare o selezionare un valore numerico in base al quale spostare un carattere selezionato verso l&#39;alto o verso il basso rispetto alla linea di base del testo circostante. Questa opzione è particolarmente utile quando impostate a mano le frazioni o regolate la posizione della grafica inline.

>[!NOTE]
>
>Seleziona **[!UICONTROL Annulla]** per annullare l&#39;ultima azione. Seleziona **[!UICONTROL Ripristina]** se cambi idea sull&#39;annullamento di un&#39;azione dopo aver selezionato **[!UICONTROL Annulla]**.

### Formattare i paragrafi {#format-paragraphs}

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Selezionare il paragrafo da formattare.
1. Specificare una delle opzioni di formattazione seguenti, quindi selezionare **[!UICONTROL Applica]**.

   * **[!UICONTROL Allineamento]**: specificare il tipo di allineamento facendo clic su **[!UICONTROL Allinea a sinistra]**, **[!UICONTROL Allinea al centro]**, **[!UICONTROL Allinea a destra]** o **[!UICONTROL Giustifica]**.

   * **[!UICONTROL Giustificazione fine paragrafo]**: selezionare questa opzione per specificare il tipo di giustificazione per l&#39;ultima riga del paragrafo: l&#39;ultima riga viene allineata a sinistra, l&#39;ultima riga viene allineata al centro e l&#39;ultima riga a destra.

   * **[!UICONTROL Interlinea]**: digitare o selezionare un valore numerico in base al quale regolare lo spazio tra tutte le righe del paragrafo.

   * **[!UICONTROL Rientra tutto]**: selezionare questa opzione per aumentare il rientro del testo.

   * **[!UICONTROL Rimuovi rientro]**: selezionare questa opzione per ridurre la quantità di rientro del testo.

   * **[!UICONTROL Rientro prima riga]**: specificare la quantità di rientro della prima riga di testo.

   * **[!UICONTROL Spazio prima del paragrafo]**: specificare la quantità di spazio che si desidera visualizzare sopra la prima riga di testo del paragrafo.

   * **[!UICONTROL Spazio dopo il paragrafo]**: specificare la quantità di spazio che si desidera visualizzare sotto l&#39;ultima riga di testo del paragrafo.

   * **[!UICONTROL Allineamento verticale]**: selezionare la posizione in cui si desidera che il testo venga visualizzato verticalmente all&#39;interno della casella di testo: In alto, Al centro, In basso.

   * **[!UICONTROL Direzione testo]**: selezionare la direzione in cui si desidera visualizzare il testo: Da destra a sinistra o Da sinistra a destra.

### Regolare le proprietà del livello di testo {#adjust-text-layer-properties}

1. Nella schermata funzioni di base dei modelli, selezionate la casella di testo da regolare.
1. Nel pannello Proprietà livello, effettuate una delle seguenti operazioni:

   * **[!UICONTROL Riduci testo (solo editor di testo v. 4.2)]**: selezionare questa opzione per ridurre il testo in modo che si adatti alla casella di testo.

   * **[!UICONTROL Ritorno a capo automatico (solo editor di testo v. 4.2)]**: per specificare se o come il testo deve essere disposto, selezionare un&#39;opzione di ritorno a capo automatico:

   * **[!UICONTROL Ritorno a capo]**: adatta il testo a una casella di testo troppo piccola in orizzontale.

   * **[!UICONTROL Nessun ritorno a capo]**: non esegue il ritorno a capo del testo quando la casella di testo è troppo piccola in senso orizzontale e taglia una parte del testo.

   * **[!UICONTROL A capo automatico]**: adatta il testo a una casella di testo e non interrompe le parole.

   * **[!UICONTROL Posizione]**: specifica la posizione della casella di testo nell&#39;area di lavoro.

   * **[!UICONTROL Spaziatura interna]**: aggiunge margini o ritaglia il rettangolo del livello. Specifica il numero di pixel da aggiungere o rimuovere per Sinistra, Superiore, Inferiore e Destra. Immettere numeri positivi se si desidera aggiungere un margine o numeri negativi al ritaglio.

### Visualizzare e modificare il codice sorgente del testo {#view-and-edit-text-source-code}

Le informazioni fornite nella scheda Source dell’Editor di testo sono a tuo riferimento. Modificate il testo solo se avete esperienza nella modifica del codice sorgente.

1. Nell’elenco Livelli, fate doppio clic sul nome della casella di testo contenente il testo da modificare. Viene aperto l’editor di testo.
1. Nell&#39;editor di testo, per visualizzare il codice sorgente del testo, selezionare la scheda **[!UICONTROL Source]** nell&#39;editor di testo.
1. Visualizzate o modificate il testo come desiderate.

   Le modifiche rimangono intatte se passate dalla visualizzazione Anteprima a Sorgente e viceversa.

1. Seleziona **[!UICONTROL Applica]** per eseguire il rendering delle modifiche.

## Operazioni con i livelli {#working-with-layers}

Per effettuare operazioni con i livelli, usate l’elenco Livelli e l’area Proprietà livello. Potete riordinare livelli, modificarne le dimensioni e la posizione, ruotare i livelli e determinare il colore di sfondo, il colore di primo piano, l’opacità e il metodo di fusione di un livello.

Potete anche modificare le dimensioni di un quadro, sceglierne il colore di sfondo e modificarne le impostazioni di opacità.

### Riordinare i livelli {#reordering-layers}

La modifica dell&#39;ordine dei livelli può influire sull&#39;aspetto, in particolare quando è interessata la trasparenza o la sovrastampa. Prima di salvare le modifiche verificate quindi l’anteprima del risultato.

1. Per riordinare i livelli in un modello, effettuate una delle seguenti operazioni:

   * Selezionate un livello nel pannello Livelli. Quindi seleziona **[!UICONTROL Su]** o **[!UICONTROL Giù]** il numero di volte necessario per collocarlo nella posizione corretta nell&#39;elenco.
   * Trascinate un livello verso l’alto o il basso nell’elenco Livelli.

### Modificare le dimensioni e la posizione dei livelli e dell&#39;area di lavoro {#changing-the-size-and-position-of-layers-and-the-canvas}

I livelli devono essere di dimensioni tali da rientrare nel quadro. Potete modificare le dimensioni di un livello o del quadro manualmente o immettendo i valori desiderati. Potete modificare la posizione di un livello manualmente o immettendo i valori di scostamento desiderati. Potete anche ruotare un livello.

>[!NOTE]
>
>Adobe Dynamic Media Classic consiglia di creare un predefinito immagine delle dimensioni esatte del modello. Quando le dimensioni del predefinito per immagini corrispondono a quelle del modello, si otterranno impostazioni corrette per le dimensioni di output finali e le opzioni di nitidezza per il modello. Dopo aver creato questo predefinito immagine, potete sceglierlo dal menu Applica predefinito nella schermata Anteprima modello. Nella schermata viene visualizzato l’aspetto dell’immagine che verrà trasmessa dal server. Consulta [Configurazione predefiniti immagine](setting-image-presets.md#setting_up_image_presets).

* **Modifica delle dimensioni di un livello**: per modificare le dimensioni di un livello o dell&#39;area di lavoro, selezionare il livello o l&#39;area di lavoro nell&#39;elenco Livelli e utilizzare una delle tecniche seguenti:

* **Modifica manuale delle dimensioni**: selezionare e trascinare un angolo del livello o dell&#39;area di lavoro. Per i livelli di testo potete anche trascinare un lato del livello. Tenere premuto il tasto Maiusc mentre si trascina per modificare le dimensioni, mantenendo però le proporzioni (la forma).

* **Immissione delle dimensioni del livello**: immettere le dimensioni dei pixel nelle caselle di testo W (larghezza) e H (altezza) nell&#39;area Proprietà livello.

Oltre a modificare le dimensioni di un livello, potete aggiungervi della spaziatura. Per effettuare tale operazione, immettete un valore di spaziatura a sinistra, a destra, in alto e in basso nelle relative caselle dell’area Proprietà livello. La spaziatura consente di aggiungere un margine al livello corrente per scostarlo dal perimetro del suo livello base. La spaziatura è utile per rendere più visibile un eventuale effetto Ombra esterna o Bagliore esterno. La spaziatura consente di aumentare le dimensioni di un livello e di visualizzarne il colore di sfondo nell’area estesa. Il livello viene riposizionato rispetto alle nuove dimensioni del livello. Ad esempio, se il livello corrente è centrato su un livello base, estendendo il lato sinistro si sposta il livello verso destra rispetto al livello base.

* **Modifica della posizione di un livello**: per modificare la posizione di un livello nell&#39;area di lavoro, selezionarne il nome nell&#39;elenco Livelli e utilizzare una delle tecniche seguenti:

* **Modifica manuale della posizione**: spostare il puntatore vicino a un limite di livello, ma non su di esso, e quando viene visualizzato il cursore a freccia a quattro punte, selezionare e iniziare a trascinare.

* **Immissione delle misure di scostamento posizione**: immettere le misure di scostamento X e Y nelle caselle di testo X e Y. Questi valori rappresentano lo scostamento x, y del punto di ancoraggio in pixel.

* **Rotazione di un livello**: nella casella Ruota viene visualizzato l&#39;angolo di rotazione del livello. Per ruotare un livello, selezionatene il nome nell’elenco Livelli ed effettuate una delle seguenti operazioni:

* **Rotazione manuale**: spostare il cursore vicino a un angolo del livello, ma non sopra di esso. Quando compare il cursore di rotazione, trascinate l’angolo del livello. Per ruotare per incrementi di 15 gradi, tenete premuto il tasto Maiusc mentre trascinate.

* **Inserimento di un livello di misura**: immettere il numero di gradi per ruotare il livello. La rotazione è in senso orario; per ruotare in senso antiorario, immettete un numero negativo.

**Nascondi un livello o un effetto livello:**

Potete nascondere un livello o un effetto livello selezionando l&#39;icona dell&#39;occhio accanto al nome di un livello o di un effetto. I livelli nascosti non vengono visualizzati nelle anteprime o nell’output. Le informazioni relative al livello non vengono eliminate dall’URL. Invece, `hide=1` viene aggiunto all&#39;URL per notare che il livello è nascosto dalla vista. Ad esempio:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Determinare il colore di sfondo, l&#39;opacità e il metodo di fusione

Per scegliere un colore di sfondo, opacità e metodo di fusione per un livello o per il quadro, selezionate il livello o il quadro ed effettuate le seguenti operazioni:

* **Colore di primo piano**: selezionare **[!UICONTROL Colore di primo piano]** e scegliere un campione di colore per modificare il colore dell&#39;ombreggiatura o del bagliore. Potete anche immettere un parametro con il valore del colore nella casella. Il colore di sfondo viene applicato solo ai livelli che usano trasparenza. As esempio, viene applicato a un livello parzialmente trasparente in un etichetta con il prezzo o allo sfondo di un campo di testo. I livelli che contengono un’immagine PSD, TIFF o PNG con trasparenza attiva possono disporre di sfondi trasparenti.

* **Colore di sfondo**: selezionare **[!UICONTROL Colore di sfondo]** e scegliere un campione di colore per modificare il colore delle aree imbottite.

* **Opacità**: trascina il cursore Opacità per rendere traslucido qualsiasi livello in modo che una parte dell&#39;immagine sottostante venga visualizzata. L&#39;impostazione 100% è opaca; 0 è trasparente.

* **Metodo fusione**: per simulare uno dei metodi fusione disponibili in Photoshop, scegliere un&#39;opzione. Le opzioni sono Normale, Dissolvenza, Schiarisci, Scurisci, Moltiplica e Scolora. Queste opzioni sono disponibili per i livelli, ma non per il quadro.

## Usa effetti ombreggiatura e bagliore sui livelli {#using-shadow-and-glow-effects-on-layers}

Potete applicare un’ombra o un bagliore a un livello. L&#39;ombreggiatura o il bagliore si applica al perimetro del livello e si estende verso l&#39;interno o l&#39;esterno, a seconda dell&#39;opzione di ombreggiatura o bagliore scelta. Se il modello è stato creato con un file PSD con effetti ombreggiatura e bagliore, è possibile regolare questi effetti in Adobe Dynamic Media Classic.

Dopo aver applicato un effetto ombra o bagliore, potete regolarne le dimensioni, il colore, l’opacità e la posizione nell’area Proprietà livello della schermata Modello.

### Applicare un effetto ombra o bagliore a un livello {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Selezionate un livello nel pannello Livelli.
1. Selezionare il menu **[!UICONTROL `Add Effect`]** e scegliere un&#39;opzione:

   * **[!UICONTROL Ombra esterna]**: applica un&#39;ombreggiatura al lato inferiore e destro del livello.

   * **[!UICONTROL Ombra interna]**: applica un effetto ombreggiatura all&#39;interno di tutti i bordi del livello.

   * **[!UICONTROL Bagliore esterno]**: applica un effetto bagliore intorno a tutti i bordi del livello.

   * **[!UICONTROL Bagliore interno]**: applica un effetto alone all&#39;interno di tutti i bordi del livello.

Dopo l’applicazione di un effetto, il suo nome compare nell’elenco Livelli. Per eliminare un effetto, selezionarne il nome nell&#39;elenco Livelli, quindi selezionare **[!UICONTROL Elimina]**.

>[!NOTE]
>
>Talvolta non potete vedere l&#39;effetto di un&#39;ombra esterna o di un bagliore esterno se il livello sottostante non è abbastanza grande da visualizzarlo. Se l&#39;ombreggiatura o il bagliore non sono visibili, è consigliabile aggiungere valori di spaziatura al livello o riordinare il livello. Consultate [Modifica delle dimensioni e della posizione dei livelli e del quadro](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) e [Riordinamento dei livelli](creating-template.md#reordering_layers).

### Regolare un effetto ombra o bagliore {#adjusting-a-shadow-or-glow-effect}

Per regolare un effetto ombra o bagliore, selezionatene il nome nell’elenco Livelli. Quindi modificatene le impostazioni nell’area Proprietà livello della schermata Modello:

* **[!UICONTROL Colore]**: selezionare il pulsante Colore e scegliere un campione di colore per modificare il colore dell&#39;ombreggiatura o del bagliore. Potete anche immettere un parametro con il valore del colore nella casella.

* **[!UICONTROL Opacità]**: trascina il cursore per determinare l&#39;intensità dell&#39;effetto. Minore è l’opacità, più sono trasparenti gli effetti.

* **[!UICONTROL Metodo fusione]**: per simulare uno dei metodi fusione disponibili in Photoshop, scegliere un&#39;opzione. Le opzioni sono Normale, Dissolvenza, Schiarisci, Scurisci, Moltiplica e Scolora.

* **[!UICONTROL Dimensione]**: immettere le misure nelle caselle X e Y per ingrandire o ridurre l&#39;effetto ombreggiatura. Le opzioni Dimensione sono disponibili per le ombre interne ed esterne.

* **[!UICONTROL Ingrandisci]**: trascina il cursore per estendere l&#39;effetto verso l&#39;interno o l&#39;esterno.

* **[!UICONTROL Sfocatura]**: trascina il cursore per controllare la sfumatura ai bordi dell&#39;effetto. Con una sfocatura maggiore si ottengono bordi più sfumati.

## Mascherare i livelli {#masking-layers}

L’elenco Modelli offre un pulsante Maschera che consente di specificare come viene usata la maschera o il canale alfa di un livello. Tramite il pulsante Maschera, potete applicare l’effetto di un livello di sfondo a un particolare livello o all’intero livello principale nel modello. Selezionare un livello nell&#39;elenco Livelli e selezionare **[!UICONTROL Maschera]** per passare da uno stato all&#39;altro:

* Lo sfondo del livello è opaco.
* Il contenuto del livello viene invertito e lo sfondo del livello viene riempito con nero in tinta unita.
* Lo sfondo del livello viene riempito con nero in tinta unita.
