---
title: Nitidezza di un’immagine
seo-title: Nitidezza di un’immagine
description: 'null'
seo-description: Scoprite come rendere nitida un’immagine.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/Categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
translation-type: tm+mt
source-git-commit: 917ba4469b5ef22e62c572f80008e470dccdebe4

---


# Nitidezza di un’immagine {#sharpening-an-image}

La nitidezza si ottiene con una tecnica di manipolazione dell’immagine che rende più netti i contorni di un’immagine digitale. La nitidezza aumenta il contrasto tra i pixel dei bordi ed enfatizza il passaggio dalle aree chiare a quelle scure e viceversa. La nitidezza aumenta il contrasto locale e mette in evidenza i dettagli. Non esiste una formula rigida per ottenere la giusta nitidezza per tutte le immagini. Una nitidezza troppo leggera può produrre immagini morbide mentre una nitidezza troppo accentuata può produrre immagini con artefatti, disturbo o aloni.

Dynamic Media Classic consiglia vivamente di utilizzare i predefiniti per immagini per tutte le immagini. affinché abbiano dimensioni uniformi e affinché la nitidezza venga applicata a tutte le immagini richiamate d un particolare predefinito per immagini. Inoltre, potrete modificare facilmente i parametri di nitidezza di un predefinito per immagini. Alla successiva pubblicazione i nuovi parametri verranno applicati a tutte le immagini richiamate da tale predefinito.

Dynamic Media Classic consiglia inoltre di aggiungere la nitidezza ai predefiniti per visualizzatori, quindi di richiamare un visualizzatore con tale predefinito. In questo modo tutte le immagini all’interno dei visualizzatori saranno nitide.

Tuttavia, a prescindere dall’utilizzo di predefiniti per immagini o per visualizzatori oppure di altri metodi per l’applicazione della nitidezza, è sempre necessario rendere le immagini più nitide. In caso contrario, le immagini e quindi il sito Web potrebbero avere un aspetto slavato.

>[!NOTE]
>
>il comando Più nitido sostituisce le impostazioni dei predefiniti immagine, inclusi gli effetti di nitidezza. Un predefinito per immagini regola le dimensioni e la formattazione con cui le immagini vengono trasmesse dai server di immagini per file multimediali dinamici. Dynamic Media Classic consiglia vivamente di usare i predefiniti per immagini per distribuire tutte le immagini in modo che queste vengano trasmesse con dimensioni e nitidezza uniformi. Se si cambiano le impostazioni di nitidezza di un’immagine, le impostazioni di nitidezza del predefinito per immagini non sono più applicabili. L’immagine viene quindi trasmessa senza le impostazioni di nitidezza provenienti dal predefinito per immagini.

È spesso necessario rendere le immagini più nitide. I server SPS e Image di Dynamic Media Classic offrono diverse opzioni di nitidezza. È importante comprendere l’effetto di tali opzioni sulle immagini e l’entità di nitidezza necessaria. La maggior parte delle immagini richiede l’applicazione di nitidezza, ma l’entità di tale regolazione dipende dalle singole immagini.

La nitidezza aumenta il contrasto tra i pixel dell’immagine in modo da accentuarne i bordi. Gli esseri umani percepiscono il contrasto dei bordi come nitidezza. Sebbene sia facile migliorare un’immagine tramite filtri di nitidezza, è anche facile che tale regolazione risulti eccessiva.

Nelle immagini con nitidezza eccessiva si possono osservare un effetto alone o bande nelle linee dei bordi.

Esistono procedure ottimali che potete seguire per ottimizzare la nitidezza delle immagini in Scene7 Publishing System e sul server immagini per file multimediali dinamici.

Consultate [Procedure ottimali per la nitidezza delle immagini in Scene7 Publishing System e sul server](/help/assets/s7_sharpening_images.pdf)di immagini per file multimediali dinamici.

**Per rendere più nitida un’immagine**

To sharpen an image, click its rollover **Edit** button and choose Sharpen, or open it in the Browse Panel in Detail view, then click **Sharpen**. Viene visualizzato l’Editor nitidezza con i relativi comandi. Scegliete i comandi e fate clic su **Salva**.

>[!NOTE]
>
>Prima di rendere più nitida un’immagine potete selezionare il menu Applica predefinito e scegliere un predefinito per immagini per vederne l’effetto a livello di nitidezza. Gli effetti di nitidezza di un predefinito per immagini potrebbero essere quelli giusti per la vostra immagine. Il menu Applica predefinito si trova nella parte inferiore della schermata Editor nitidezza.

**Opzioni di nitidezza**

Nella tabella seguente sono elencate le opzioni di nitidezza del server di immagini.

| Nome | Protocollo URL | Valori | Esempio |
|--- |--- |--- |--- |
| Nitidezza semplice | op_sharpen | `0 | 1` | op_sharpen=1 |
| Modalità di ricampionamento | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilin: interpolazione bilineare standard. È il metodo di ricampionamento più veloce; possono essere visibili alcuni artefatti di alias.<br>bicub: interpolazione bicubica. Richiede maggiori risorse CPU rispetto a bilin, ma produce immagini più nitide e con meno artefatti di alias.<br><br>sharp2: come algoritmo di interpolazione viene utilizzata una funzione Lanczos Window modificata. I risultati possono essere leggermente più nitidu dell’opzione bicubica, ma richiede un utilizzo maggiore della CPU.<br><br>trilin: interpolazione trilineare modificata, che utilizza risoluzioni più elevate e più basse, se disponibili. Consigliato solo in caso di problemi di alias. Riduce le dimensioni JPEG grazie alla riduzione dei dati ad alta frequenza. | resMode=sharp2 |
| Maschera di contrasto | op_usm | amount, radius, threshold,<br><br>monochromeamount: fattore di intensità del filtro (reale 0...5)<br><br>raggio: raggio kernel del filtro in pixel ( <br><br>soglia reale 0...250): livello di soglia del filtro (numero intero 0...255)<br><br>monocromatico: impostato su 0 per applicare la maschera di contrasto separatamente a ciascun componente di colore, con l’impostazione su 1 per applicare la maschera di contrasto alla luminosità dell’immagine (intensità) | op_usm=1,1,10,0 |

Selezionate il menu Nitidezza e scegliete un’opzione:

**Nessuno** Disattiva la nitidezza.

**Nitidezza** Esegue una semplice passata di nitidezza sul file ridimensionato. Questa funzione è simile al filtro Nitidezza di Photoshop e supporta tutti i parametri utente. In genere si utilizza questo filtro o Maschera di contrasto, ma non entrambi. Questo metodo non è consigliato come procedura abituale, ma può servire per compensare un’eventuale sfocatura delle immagini. (URL: op_sharpen)

**Maschera** di contrasto Consente di regolare un effetto filtro di nitidezza sull’immagine ricampionata finale. Potete controllare l’intensità dell’effetto e il raggio (in pixel) e impostare una soglia per il livello di contrasto da ignorare. Questo effetto utilizza le stesse opzioni del filtro Maschera di contrasto di Photoshop. (URL: op_usm)

Scegliete le seguenti opzioni per regolare la nitidezza con Maschera di contrasto:

**Fattore** Controlla la quantità di contrasto applicata ai pixel lungo i bordi. Il valore predefinito è 0,0. Per le immagini ad alta risoluzione, è possibile aumentare questo valore fino a 5,0. Il fattore può essere interpretato come una misura dell’intensità del filtro. L’impostazione Fattore in Dynamic Media Classic non equivale all’impostazione Fattore in Photoshop. Photoshop utilizza un valore compreso tra 1% e 500%, mentre Dynamic Media Classic viene ridimensionato da 0,0 a 5,0. dove 5,0 equivale circa a 500% in Photoshop, 0,9 a 90% e così via.

**Raggio** Determina il numero di pixel attorno ai pixel del bordo che influiscono sulla nitidezza. L’effetto viene eseguito su tutti i pixel dell’immagine, in tutte le direzioni. 

Il valore di raggio più adatto dipende dalle dimensioni dell’immagine. Un valore basso rende più nitidi solo i pixel dei bordi. Un valore alto rende più nitida una banda più ampia di pixel. 

Ad esempio, per ottenere un effetto di nitidezza simile per un’immagine di 2000x2000 pixel e una di 500x500 pixel, potete impostare un raggio di 2 pixel per l’immagine di 2000x2000 pixel. Quindi impostate un raggio di 1 pixel per l’immagine di 500x500 pixel. In altre parole, sceglierete un valore maggiore per l’immagine con più pixel. 

**Soglia** Determina l’intervallo di contrasto da ignorare quando viene applicato il filtro maschera di contrasto. Questa opzione specifica quale deve essere il grado di differenza dei pixel da rendere più nitidi rispetto all’area circostante, affinché vengano considerati pixel di un bordo e quindi resi più nitidi.

Soglia utilizza un valore da 0-255, che corrisponde al numero di incrementi di luminosità di un’immagine in scala di grigio. 0=nero, 128=grigio al 50% e 255=bianco. Ad esempio, con un valore di soglia pari a 12 vengono ignorate le variazioni lievi di luminosità nell’incarnato, in modo da non introdurre disturbo, mentre viene aumentato il contrasto lungo i bordi delle aree con maggior contrasto, ad esempio tra ciglia e incarnato. 

Ad esempio, per una foto di un volto, Maschera di contrasto agisce sulle parti dell’immagine con maggior contrasto, ma anche sulle aree di incarnato uniforme. Anche l’incarnato più omogeneo presenta lievi variazioni nei valori di luminosità. Se non si utilizza un valore di soglia, il filtro accentuerebbe tali lievi variazioni nei pixel dell’incarnato rendendolo meno uniforme (creando un effetto indesiderato), mentre aumenterebbe il contrasto per le ciglia rendendole più nitide (creando un effetto gradevole). Per evitare questo problema, utilizzate un valore di soglia che indichi al filtro di ignorare i pixel con modifiche lievi a livello di contrasto, come appunto nel caso della pelle. Per evitare di introdurre disturbo o posterizzazione, ad esempio nelle immagini con toni di carne, provate a sperimentare con valori di soglia compresi tra 2 e 20. Il valore predefinito di Soglia pari a 0 rende più nitidi tutti i pixel dell’immagine.

**Applica a** scegliere ogni colore per applicare la nitidezza separatamente a ciascun componente di colore; scegliete Luminosità per rendere più nitide le aree di luminosità delle immagini.

**Ricampionamento**

Selezionate il menu Ricampionamento e scegliete un’opzione. Queste opzioni aumentano la nitidezza quando si esegue il downsampling dell’immagine:

**Nessuno** Disattiva il ricampionamento.

**Bilineare** Il metodo di ricampionamento più veloce; alcuni artefatti di alias sono visibili.

**Bicubica** Aumenta l’utilizzo della CPU sul server immagini, ma produce immagini più nitide con meno artefatti di alias.

**Sharpen2** Può produrre risultati leggermente più nitidi rispetto all’opzione Bicubica, ma con un utilizzo maggiore della CPU sul server immagini.

**Trilineare** utilizza risoluzioni più elevate e più basse, se disponibili; consigliato solo quando l'aliasing è un problema. Questo metodo riduce le dimensioni JPEG grazie a una minore quantità di dati ad alta frequenza.

**Nitidezza e predefiniti per immagini**

Per ottenere risultati ottimali è possibile applicare tutti e tre gli effetti di nitidezza. Tuttavia, questo è sconsigliato. Dynamic Media Classic consiglia di salvare gli effetti di nitidezza come parte di un predefinito per immagini. I predefiniti per immagini consentono di creare pacchetti di modificatori di immagini usati più di frequente per creare un’immagine ridimensionata in modo dinamico in una piccola stringa di testo. Un predefinito per immagini contiene valori per il formato file (in genere JPEG per il Web), il numero di pixel e la nitidezza dell’immagine. Invece di aggiungere all’URL un modificatore immagine per ogni tipo di dimensioni immagine, potete creare un predefinito per immagini, ad esempio “miniatura”, e configurarlo con le dimensioni, il formato file e le opzioni di nitidezza desiderati. Successivamente potete richiamare l’immagine utilizzando il nome di tale predefinito per immagini. L’utilizzo di predefiniti per immagini produce URL più brevi, come illustrato dai due esempi di seguito, entrambi per la stessa immagine JPEG con nitidezza. 

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

I predefiniti per immagini possono essere modificati e aggiornati in qualsiasi momento. I risultati delle modifiche apportate a un predefinito per immagini sono visibili dopo la pubblicazione e dopo la cancellazione della cache per l’URL.

Se utilizzate un predefinito per ciascuna immagine di una categoria di dimensioni, l’amministratore società può aggiornare la definizione del predefinito per immagini e pubblicare nuovamente i contenuti: tutte le immagini che utilizzano tale formato verranno regolate di conseguenza, senza che sia stato necessario modificare il codice Web. Si consiglia di utilizzare un predefinito per immagini per ciascuna dimensione di immagini utilizzata nel sito. Per aggiungere un predefinito per immagini, passate a Configurazione &gt; Impostazioni applicazione &gt; Predefiniti immagini. Quindi, scegliete Aggiungi per crearne uno nuovo predefinito o Modifica per modificarne uno esistente. L’unico campo obbligatorio è il nome del predefinito. Tuttavia, è utile includere nel predefinito la regolazione della nitidezza.

**Qualità JPG**

Le opzioni di Qualità JPG controllano il livello di compressione JPG:

**Qualità** JPG Selezionate questa opzione se desiderate controllare i livelli di compressione e il downsampling della crominanza.

**Slider** Determina il livello di compressione JPG. Questa impostazione interessa sia le dimensioni del file che la qualità dell’immagine. La scala di qualità JPG va da 1 a 100.

**Attiva il downsampling della crominanza** JPG Poiché l’occhio è meno sensibile alle informazioni sui colori ad alta frequenza rispetto alla luminanza ad alta frequenza, le immagini JPEG dividono le informazioni sulle immagini in componenti luminanza e colore. Quando un’immagine JPEG viene compressa, il componente della luminanza viene lasciato alla massima risoluzione, mentre per i componenti colore viene eseguito il downsampling calcolando la media di gruppi di pixel. Il downsampling riduce di metà o un terzo il volume di dati, con impatto trascurabile sulla qualità percepita. Non è possibile eseguire il downsampling sulle immagini in scala di grigio. Questa tecnica riduce il fattore di compressione ed è utile per le immagini ad alto contrasto (ad esempio, immagini con testo sovrapposto).

**Impostazione delle opzioni di nitidezza a livello di società**

Se non usate un predefinito per immagini o non passate specifici protocolli di nitidezza per il server immagine tramite la stringa URL, l’immagine ricampionata non verrà resa più nitida. Tuttavia, potete impostare dei valori di nitidezza predefiniti da applicare a tutte le immagini.

Per impostare le opzioni di nitidezza predefinite per la società, passate a Configurazione &gt; Impostazione applicazione &gt; Configurazione pubblicazione &gt; Server immagini. Se impostate la modalità di ricampionamento predefinito su Sharp2, le immagini verranno sempre rese più nitide al momento del ricampionamento.

**Aggiunta di nitidezza ai predefiniti per visualizzatori**

Se non aggiungete al predefinito i modificatori immagine per la nitidezza, la piccola immagine di caricamento iniziale può apparire sfocata: questo accade perché viene ricampionata per rientrare nella finestra del visualizzatore, ma non viene applicata alcuna regolazione a livello di nitidezza.

In SPS, i predefiniti per visualizzatori (come i predefiniti per immagini) consentono di centralizzare molte opzioni in una singola posizione, compresa la scelta delle opzioni per l’interfaccia e per il visualizzatore (ad esempio, l’inserimento di un pulsante Stampa o di un controllo per variare la velocità di animazione dello zoom). I predefiniti per visualizzatori sono disponibili nella stessa sezione dei predefiniti per immagini, in Configurazione &gt; Impostazioni applicazione &gt; Predefiniti visualizzatore.

L’opzione Modificatori si trova nella sezione Impostazioni principali di tutti i predefiniti per visualizzatori eCatalog, 360 gradi e Zoom personalizzati. Aggiungendo i comandi URL di nitidezza alla casella Modificatori, potete applicare la nitidezza ogni volta che il visualizzatore viene richiamato con quel predefinito per visualizzatori.

Per richiamare il predefinito per visualizzatori, usate il comando di config= nell’URL del visualizzatore. Esempio di chiamata di set di immagini (Shoes) con un predefinito per visualizzatori (FantasticoZoom2009):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

In questo caso il predefinito applica la nitidezza e cambia l’interfaccia predefinita del visualizzatore.

**Creazione di impostazioni locali per specifiche immagini**

L’ultimo metodo per l’applicazione della nitidezza, e il meno consigliato, consiste nel creare impostazioni locali di nitidezza a livello delle singole immagini. In questo modo si ignorano le impostazioni di nitidezza specificate nel predefinito per immagini e si usano invece valori specifici. Tuttavia, questo sostituisce anche tutti gli altri metodi di nitidezza per qualsiasi dimensione. Questo metodo può risultare utile, ad esempio, se alcune delle immagini non sono ad alta risoluzione e i valori nei predefiniti per immagini sono quindi troppo elevati. In questo caso può essere utile applicare la nitidezza alle singole immagini.

In SPS, selezionate un’immagine, passate alla visualizzazione Dettagli (facendo doppio clic su di essa o facendo clic sul pulsante Visualizzazione dettagli) e fate clic su Nitidezza. Modificate i parametri e fate clic su Salva. Il server di immagini utilizzerà quindi tali parametri di nitidezza anziché il comando chiamato dall’URL mediante un modificatore di nitidezza di immagine o un predefinito per immagini. La modifica ha effetto dopo la pubblicazione.
