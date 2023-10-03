---
title: Migliorare la nitidezza di un’immagine
description: Scopri come rendere più nitida un’immagine in Adobe Dynamic Media Classic.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
topic: Content Management
level: Intermediate
source-git-commit: 1b90beb99b161b76da81403f5aed9755b3a92c8b
workflow-type: tm+mt
source-wordcount: '2274'
ht-degree: 39%

---

# Migliorare la nitidezza di un’immagine {#sharpening-an-image}

La nitidezza si ottiene con una tecnica di manipolazione dell’immagine che rende più netti i contorni di un’immagine digitale. La nitidezza aumenta il contrasto tra i pixel dei bordi ed enfatizza il passaggio dalle aree chiare a quelle scure e viceversa. La nitidezza aumenta il contrasto locale e mette in evidenza i dettagli. Non esiste una formula rigida per ottenere la giusta nitidezza per tutte le immagini. Una nitidezza troppo leggera può produrre immagini morbide mentre una nitidezza troppo accentuata può produrre immagini con artefatti, disturbo o aloni.

Adobe Dynamic Media Classic consiglia vivamente di utilizzare Predefiniti immagine per tutte le immagini. Assicurano dimensioni uniformi e la nitidezza viene applicata a qualsiasi immagine denominata con un predefinito immagine. Inoltre, è possibile modificare facilmente i parametri di nitidezza di un predefinito immagine. Alla successiva pubblicazione i nuovi parametri verranno applicati a tutte le immagini richiamate da tale predefinito.

Adobe Dynamic Media Classic consiglia inoltre di aggiungere nitidezza ai predefiniti visualizzatore e di chiamare un visualizzatore con tale predefinito. In questo modo, gli spettatori potranno godere di immagini nitide e accattivanti.

Tuttavia, sia che si utilizzino i predefiniti per immagini e i predefiniti per visualizzatori o si utilizzino metodi di nitidezza, la cosa più importante è che è necessario rendere più nitide le immagini. In caso contrario, le immagini (e il sito web) possono apparire morbidi e sfocati.

>[!NOTE]
>
>il comando Più nitido sostituisce le impostazioni dei predefiniti immagine, inclusi gli effetti di nitidezza. Un predefinito per immagini definisce le dimensioni e la formattazione delle immagini distribuite dai server immagini Dynamic Medie. Adobe Dynamic Media Classic consiglia vivamente di utilizzare i predefiniti immagine per fornire tutte le immagini in modo che vengano distribuite con dimensioni e nitidezza uniformi. Se si cambiano le impostazioni di nitidezza di un’immagine, le impostazioni di nitidezza del predefinito per immagini non sono più applicabili. L’immagine viene quindi trasmessa senza le impostazioni di nitidezza provenienti dal predefinito per immagini.

È spesso necessario rendere le immagini più nitide. Adobe Dynamic Media Classic e Image Server offrono diverse opzioni di nitidezza. È importante comprendere l’effetto di tali opzioni sulle immagini e l’entità di nitidezza necessaria. La maggior parte delle immagini richiede l’applicazione di nitidezza, ma l’entità di tale regolazione dipende dalle singole immagini.

La nitidezza aumenta il contrasto tra i pixel dell’immagine in modo da accentuarne i bordi. Gli esseri umani percepiscono il contrasto dei bordi come nitidezza. Sebbene sia facile migliorare un’immagine tramite filtri di nitidezza, è anche facile che tale regolazione risulti eccessiva.

L&#39;eccessiva nitidezza di un&#39;immagine crea un effetto alone o striatura delle linee del bordo.

È possibile seguire alcune best practice per ottimizzare la nitidezza delle immagini in Adobe Dynamic Media Classic e su Dynamic Medie Image Server.

Consulta [Best practice per la nitidezza delle immagini in Adobe Dynamic Media Classic e su Dynamic Medie Image Server](/help/using/assets/s7_sharpening_images.pdf).

Vedi anche [Nitidezza](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) video di formazione.

**Per rendere più nitida un’immagine:**

Per rendere più nitida un’immagine, selezionane il rollover **[!UICONTROL Modifica]** e scegliere **[!UICONTROL Nitidezza]**, o aprirlo nel pannello Sfoglia in Visualizzazione dettagli, quindi selezionare **[!UICONTROL Nitidezza]**. Viene visualizzata la pagina Editor nitidezza con i comandi di nitidezza. Scegliere i comandi, quindi selezionare **[!UICONTROL Salva]**.

>[!NOTE]
>
>Prima di rendere più nitida un’immagine potete selezionare il menu Applica predefinito e scegliere un predefinito per immagini per vederne l’effetto a livello di nitidezza. Gli effetti di nitidezza di un predefinito immagine sono adatti all&#39;immagine in uso. Il **[!UICONTROL Applica predefinito]** nella parte inferiore della pagina Editor nitidezza.

**Opzioni di nitidezza**

Nella tabella seguente sono elencate le opzioni di nitidezza del server di immagini.

| Nome | Protocollo URL | Valori | Esempio |
| --- | --- | --- | --- |
| Nitidezza semplice | `op_sharpen` | `0` Oppure `1` | `op_sharpen=1` |
| Modalità di ricampionamento | `resMode` | `bilin`, `bicub`, `sharp2`, `trilin`<br><br>`bilin`: seleziona l&#39;interpolazione bilineare standard. Metodo di ricampionamento più veloce; alcuni artefatti di aliasing sono spesso visibili.<br>`bicub`: seleziona l&#39;interpolazione bi-cubica. Richiede maggiori risorse CPU rispetto a bilin, ma produce immagini più nitide e con meno artefatti di alias.<br><br>`sharp2`: seleziona una funzione Windows® Lanczos modificata come algoritmo di interpolazione. Può produrre risultati leggermente più nitidi rispetto al bi-cubico a un costo di CPU più elevato.<br><br>`trilin`: interpolazione trilineare modificata, che utilizza risoluzioni più elevate e più basse, se disponibili. Consigliato solo in caso di problemi di alias. Riduce le dimensioni JPEG grazie alla riduzione dei dati ad alta frequenza. | `resMode=sharp2` |
| Maschera di contrasto | `op_usm` | `amount`, `radius`, `threshold`, `monochrome`<br><br>`amount`: fattore di intensità del filtro (reale 0...5)<br><br>`radius`: raggio kernel del filtro in pixel (reale 0...250) <br><br>`threshold`: livello soglia filtro (int 0...255)<br><br>`monochrome`: impostato su `0` per applicare una maschera di contrasto a ogni componente di colore separatamente, impostate `1` per mascherare la luminosità dell&#39;immagine (intensità) | `op_usm=1,1,10,0` |

Seleziona la **[!UICONTROL Nitidezza]** e scegliere un&#39;opzione:

* **Nessuno** - Disattiva la nitidezza.

* **Nitidezza** - Esegue un semplice passaggio di nitidezza sul file dopo il ridimensionamento. È simile al filtro &quot;Nitidezza&quot; in Adobe Photoshop e supporta qualsiasi parametro utente. Normalmente, si utilizza questo filtro oppure **[!UICONTROL Maschera definizione dettagli]**, ma non entrambi. Questo metodo non è consigliato come procedura abituale, ma può servire per compensare un’eventuale sfocatura delle immagini. (URL: `op_sharpen`)

* **Maschera definizione dettagli** - Consente di regolare con precisione un effetto filtro di nitidezza sull&#39;immagine ricampionata verso il basso finale. È possibile controllare l&#39;intensità dell&#39;effetto, il raggio in pixel e una soglia di contrasto ignorata. Questo effetto utilizza le stesse opzioni del filtro &quot;Maschera definizione dettagli&quot; di Photoshop. (URL: `op_usm`)

Scegliete queste opzioni per ottimizzare la nitidezza con Maschera definizione dettagli:

* **Quantità** - Controlla il contrasto applicato ai pixel del bordo. Il valore predefinito è 0,0. Per le immagini ad alta risoluzione, è possibile aumentare questo valore fino a 5,0. Il fattore può essere interpretato come una misura dell’intensità del filtro. Il **[!UICONTROL Quantità]** in Adobe Dynamic Media Classic è diversa dall’impostazione Importo in Adobe Photoshop. Adobe Photoshop utilizza una quantità compresa tra l’1% e il 500%, mentre Adobe Dynamic Media Classic viene scalato da 0,0 a 5,0. dove 5,0 equivale circa a 500% in Photoshop, 0,9 a 90% e così via.

* **Raggio** - Determina il numero di pixel attorno al bordo che influiscono sulla nitidezza. L’effetto viene eseguito su tutti i pixel dell’immagine, in tutte le direzioni. 

Il valore di raggio più adatto dipende dalle dimensioni dell’immagine. Un valore basso rende più nitidi solo i pixel dei bordi. Un valore alto rende più nitida una banda più ampia di pixel. 

Ad esempio, per ottenere un effetto di nitidezza simile per un&#39;immagine da 2000 x 2000 pixel e per un&#39;immagine da 500 x 500 pixel, potete impostare un valore di raggio di due pixel sull&#39;immagine da 2000 x 2000 pixel. Quindi impostate un raggio di 1 pixel per l’immagine di 500x500 pixel. In altre parole, sceglierete un valore maggiore per l’immagine con più pixel. 

* **Soglia** - Determina l&#39;intervallo di contrasto da ignorare quando si applica il filtro Maschera di contrasto. Questa opzione specifica quale deve essere il grado di differenza dei pixel da rendere più nitidi rispetto all’area circostante, affinché vengano considerati pixel di un bordo e quindi resi più nitidi.

La soglia utilizza un valore compreso tra 0 e 255, che rappresenta il numero di livelli di luminosità in un&#39;immagine in scala di grigio. 0=nero, 128=grigio al 50% e 255=bianco. Ad esempio, con un valore di soglia pari a 12 vengono ignorate le variazioni lievi di luminosità nell’incarnato, in modo da non introdurre disturbo, mentre viene aumentato il contrasto lungo i bordi delle aree con maggior contrasto, ad esempio tra ciglia e incarnato. 

Ad esempio, supponiamo di avere una foto del volto di qualcuno. Maschera di contrasto agisce sulle parti dell’immagine con maggior contrasto, ma anche sulle aree di incarnato uniforme. Anche l’incarnato più omogeneo presenta lievi variazioni nei valori di luminosità. Se non si utilizza un valore di soglia, il filtro accentuerebbe tali lievi variazioni nei pixel dell’incarnato rendendolo meno uniforme (creando un effetto indesiderato), mentre aumenterebbe il contrasto per le ciglia rendendole più nitide (creando un effetto gradevole). Per evitare questo problema, utilizzate un valore di soglia che indichi al filtro di ignorare i pixel con modifiche lievi a livello di contrasto, come appunto nel caso della pelle. Per evitare l&#39;introduzione di rumore o di immagini di posterizzazione con toni di carne, ad esempio provare a sperimentare con **[!UICONTROL Soglia]** da due a 20. Il valore predefinito **[!UICONTROL Soglia]** il valore 0 applica la nitidezza a tutti i pixel dell&#39;immagine.

* **Applica a** - Scegli **[!UICONTROL Ogni colore]** se desiderate applicare la nitidezza separatamente a ciascun componente di colore, scegliete **[!UICONTROL Luminosità]** se desiderate applicare la nitidezza alle aree di luminosità dell&#39;immagine.

**Ricampionamento**

Seleziona la **[!UICONTROL Ricampionamento]** e scegliere un&#39;opzione. Queste opzioni aumentano la nitidezza quando si esegue il downsampling dell’immagine:

* **[!UICONTROL Nessuno]** - Disattiva il ricampionamento.

* **[!UICONTROL Bilineare]** - Il metodo di ricampionamento più veloce; alcuni artefatti di aliasing sono evidenti.

* **[!UICONTROL Bicubica]** - Aumenta l&#39;utilizzo della CPU sul server immagini, ma produce immagini più nitide con artefatti di aliasing meno evidenti.

* **[!UICONTROL Nitidezza2]** - Produce risultati leggermente più nitidi rispetto a **[!UICONTROL Bicubica]**, ma a un costo della CPU ancora più elevato sul server immagini.

* **[!UICONTROL Trilineare]** : utilizza risoluzioni più alte e più basse se disponibili; consigliato solo quando l’aliasing è un problema. Questo metodo riduce le dimensioni JPEG grazie a una minore quantità di dati ad alta frequenza.

**Predefiniti per nitidezza e immagini**

Potete incorporare tutti e tre gli effetti di nitidezza per ottenere il risultato finale. Tuttavia, questo metodo non è consigliato. Adobe Dynamic Media Classic consiglia di salvare gli effetti di nitidezza come parte di un predefinito immagine. I predefiniti per immagini consentono di creare un pacchetto dei modificatori di immagini più utilizzati per creare un&#39;immagine ridimensionata dinamicamente in una piccola stringa di testo. Un predefinito immagine contiene valori per il formato file (in genere JPEG per il web), il conteggio dei pixel e la nitidezza delle immagini. Invece di aggiungere l’URL a ogni modificatore di immagine da utilizzare per creare un tipo specifico di dimensione dell’immagine, crea un predefinito immagine denominato, ad esempio &quot;miniatura&quot;. Quindi, configura il predefinito per immagini miniatura con le dimensioni, il formato di file e le opzioni di nitidezza appropriati. Chiama l’immagine utilizzando il nome del predefinito immagine. I predefiniti per immagini riducono la lunghezza dell’URL complessivo. Questi due URL producono la stessa immagine 350x350 JPEG con nitidezza:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

I predefiniti per immagini possono essere modificati e aggiornati in qualsiasi momento. Dopo la pubblicazione e la cancellazione della cache per l’URL, vengono visualizzati i risultati di una modifica a un predefinito immagine.

Se utilizzate un predefinito per ciascuna immagine di una categoria di dimensioni, l’amministratore società può aggiornare la definizione del predefinito per immagini e pubblicare nuovamente i contenuti: tutte le immagini che utilizzano tale formato verranno regolate di conseguenza, senza che sia stato necessario modificare il codice Web. Si consiglia di utilizzare un predefinito per immagini per ciascuna dimensione di immagini utilizzata nel sito. Per aggiungere un predefinito immagine, nella barra di navigazione globale vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazioni applicazione]** > **[!UICONTROL Predefiniti immagine]**. Quindi seleziona **[!UICONTROL Aggiungi]** o seleziona **[!UICONTROL Modifica]** per modificare un predefinito esistente. L’unico campo obbligatorio è il nome del predefinito. Tuttavia, è meglio includere un certo livello di nitidezza in ogni predefinito.

**Qualità JPG**

Le opzioni di Qualità JPG controllano il livello di compressione JPG:

* **Qualità JPG** - Selezionare questa opzione per controllare i livelli di compressione e il downsampling della crominanza.

* **Cursore** - Determina il livello di compressione JPG. Questa impostazione interessa sia le dimensioni del file che la qualità dell’immagine. La scala di qualità JPG è 1-100.

* **Abilita downsampling crominanza JPG** - Poiché l&#39;occhio è meno sensibile alle informazioni cromatiche ad alta frequenza rispetto alla luminanza ad alta frequenza, le immagini JPEG dividono le informazioni in luminanza e componenti di colore. Quando un’immagine JPEG viene compressa, il componente della luminanza viene lasciato alla massima risoluzione, mentre per i componenti colore viene eseguito il downsampling calcolando la media di gruppi di pixel. Il downsampling riduce il volume dei dati della metà o di un terzo senza alcun impatto sulla qualità percepita. Non è possibile eseguire il downsampling sulle immagini in scala di grigio. Questa tecnica riduce il fattore di compressione ed è utile per le immagini ad alto contrasto (ad esempio, immagini con testo sovrapposto).

**Imposta opzioni di nitidezza a livello aziendale**

Se non usate un predefinito per immagini o non passate specifici protocolli di nitidezza per il server immagine tramite la stringa URL, l’immagine ricampionata non verrà resa più nitida. Tuttavia, se si verifica questa mancanza di nitidezza, potete impostare i valori di nitidezza predefiniti, in modo che qualsiasi immagine abbia sempre una certa nitidezza.

Per impostare le opzioni di nitidezza predefinite della tua azienda, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazione pubblicazione]** > **[!UICONTROL Server immagini]**. Se impostate la modalità di ricampionamento predefinita su **[!UICONTROL Nitido2]**, aumenta sempre la nitidezza dell&#39;immagine durante il downsampling.

**Aggiungi nitidezza ai predefiniti visualizzatore**

Se non aggiungete al predefinito i modificatori immagine per la nitidezza, la piccola immagine di caricamento iniziale può apparire sfocata: questo accade perché viene ricampionata per rientrare nella finestra del visualizzatore, ma non viene applicata alcuna regolazione a livello di nitidezza.

I predefiniti visualizzatore (come i predefiniti immagine) consentono di centralizzare molte opzioni in un&#39;unica posizione, inclusa la scelta dell&#39;interfaccia e delle opzioni visualizzatore (ad esempio l&#39;inclusione di un pulsante Stampa o il controllo della velocità dell&#39;animazione di zoom). I predefiniti per visualizzatori si trovano nella stessa sezione dei predefiniti immagine, in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazioni applicazione]** > **[!UICONTROL Predefiniti visualizzatore]**.

Consulta [Predefiniti visualizzatore](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) video di formazione.

L’opzione Modificatori si trova nella sezione Impostazioni principali di tutti i predefiniti per visualizzatori eCatalog, 360 gradi e Zoom personalizzati. Aggiungendo i comandi URL di nitidezza alla casella Modificatori, potete applicare la nitidezza ogni volta che il visualizzatore viene richiamato con quel predefinito per visualizzatori.

Per chiamare il predefinito visualizzatore, usa `config=` nell&#39;URL del visualizzatore. Esempio di chiamata di set di immagini (Shoes) con un predefinito per visualizzatori (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

In questo caso il predefinito applica la nitidezza e cambia l’interfaccia predefinita del visualizzatore.

**Creare sostituzioni specifiche per l’immagine**

L’ultimo metodo per l’applicazione della nitidezza, e il meno consigliato, consiste nel creare impostazioni locali di nitidezza a livello delle singole immagini. Questo metodo sostituisce la nitidezza in un predefinito immagine con valori specifici. Tuttavia, questo metodo ignora anche tutti gli altri metodi di nitidezza di qualsiasi dimensione. Questo metodo può risultare utile, ad esempio, se alcune delle immagini non sono ad alta risoluzione e i valori nei predefiniti per immagini sono quindi troppo elevati. In questo caso, potrebbe essere necessario un po’ di nitidezza per immagine.

In Adobe Dynamic Media Classic, selezionare un&#39;immagine qualsiasi, passare alla visualizzazione dei dettagli (facendo doppio clic o premendo **[!UICONTROL Vista dettagli]** ) e selezionare **[!UICONTROL Nitidezza]**. Modifica un parametro, quindi seleziona **[!UICONTROL Salva]**. Questo processo indica al server immagini di utilizzare questi parametri di nitidezza anziché qualsiasi comando chiamato nell’URL, ad esempio un modificatore di nitidezza o un predefinito immagine. Assicurati di pubblicare per vedere che le modifiche diventano effettive.
