---
title: Opzioni di modifica delle immagini al caricamento
seo-title: Opzioni di modifica delle immagini al caricamento
description: 'null'
seo-description: Scoprite le opzioni di modifica delle immagini disponibili al momento del caricamento.
uuid: 0912 ae 6 f -41 c 9-41 b 5-94 d 1-e 266 face 782 e
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: d 3 f 21 cdf -2 cb 3-46 e 8-955 a-b 8 daf 0 b 233 bc
translation-type: tm+mt
source-git-commit: 0f6c8e6ac69e29aab7a48425aab76c10170d9ddf

---


# Opzioni di modifica delle immagini al caricamento{#image-editing-options-at-upload}

Durante il caricamento di file di immagine, inclusi i file AI, EPS e PSD, nella finestra di dialogo Opzioni processo di caricamento potete effettuare le seguenti operazioni di modifica:

* Ritagliare lo spazio bianco dal bordo delle immagini.
* Ritagliare manualmente dai lati delle immagini.
* Scegliere un profilo colore.
* Creare una maschera da un tracciato di ritaglio.
* Rendere le immagini più nitide con opzioni di maschera di contrasto.
* Foratura sfondo

Queste opzioni si trovano nella sezione Opzioni modifica immagini della schermata Carica.

**Ritaglio di spazi bianchi dalle immagini**

Per ritagliare automaticamente i pixel degli spazi bianchi da un’immagine, selezionate il menu Ritaglio e scegliete Rifila. A questo punto, scegliete le seguenti opzioni:

**Rifila
in base alla** scelta Se ritagliare in base al colore o alla trasparenza:

**Colore** Scegliete l'opzione Colore. Dall’elenco a discesa Angolo scegliete quindi l’angolo dell’immagine con il colore che rappresenta meglio quello dello spazio bianco da ritagliare.

**Trasparenza** Scegliete l'opzione Trasparenza.

**Tolleranza** Consente di trascinare il cursore per specificare un valore di tolleranza da 0 a 1.

**Per ritagliare in base al colore** , specificate 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell'angolo dell'immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

**Ritaglio basato sulla trasparenza** Specificate 0 per ritagliare i pixel solo se sono completamente trasparenti; numeri più vicini a 1 consentono una minore trasparenza.

**Ritaglio manuale dai lati delle immagini**

Per ritagliare manualmente dai lati di un’immagine, scegliete Manuale dal menu Ritaglio. Immettete quindi il numero di pixel da ritagliare da ogni lato o da uno dei lati dell’immagine. La quantità di immagine che viene ritagliata dipende dall’impostazione ppi (pixel per pollice) nel file immagine. Ad esempio, se l’immagine viene visualizzata a 150 ppi e immettete 75 nelle caselle di testo, viene ritagliato mezzo pollice da ogni lato.

**Scelta di un profilo colore**

Scegliete un’opzione Profilo colore per selezionare uno spazio colore per l’immagine:

**Converti in srgb** converte in srgb (Standard Rosso Verde Blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

**Mantieni spazio colore originale** conserva lo spazio colore originale.

**Personale Da &gt; Ad** aprire i menu per scegliere uno spazio colore Conversione da e Converti in. Potete scegliere uno spazio colore standard di Photoshop o uno caricato in SPS. 

Consultate [Profili ICC](icc-profiles.md#icc_profiles).

**Creazione di una maschera da un tracciato di ritaglio**

Selezionate l’opzione **Crea maschera dal tracciato di ritaglio** per creare una maschera per l’immagine in base alle informazioni del suo tracciato di ritaglio. Questa opzione può essere applicata alle immagini create con applicazioni di elaborazione immagini in cui è stato creato un tracciato di ritaglio.

**Rendere un’immagine più nitida con Maschera di contrasto**

Questo filtro consente di regolare un effetto di nitidezza applicato all’immagine ricampionata finale, controllando l’intensità e il raggio (in pixel) dell’effetto e una soglia di contrasto che determina quando l’effetto debba essere ignorato.

Questo effetto utilizza le stesse opzioni del filtro Maschera di contrasto di Photoshop. Nonostante il nome possa fare pensare altrimenti, Maschera di contrasto è un filtro di nitidezza.

In Maschera di contrasto, impostate le opzioni desiderate come descritto nella seguente tabella:

| Opzioni di Maschera di contrasto | Descrizione |
|--- |--- |
| Fattore | Controlla il fattore di contrasto applicato ai pixel lungo i bordi.<br><br>Corrisponde all’intensità dell’effetto. La differenza principale tra questo valore in SPS e in Adobe Photoshop, è che Photoshop supporta valori compresi tra 1% e 500%. In SPS i valori ammessi sono compresi tra 0.0 e 5.0 dove 5.0 equivale circa al valore 500% in Photoshop, 0.9 equivale a 90% e così via. |
| Raggio | Controlla il raggio dell’effetto. <br><br>L'intervallo di valori è 0-250. L'effetto viene eseguito su tutti i pixel di un'immagine e si irradia da tutti i pixel in tutte le direzioni. Il raggio è espresso in pixel. Ad esempio, per ottenere un effetto di nitidezza simile per un’immagine di 2000x 2000 pixel e una di 500x 500 pixel, potete impostare un raggio di 2 pixel per l’immagine di 2000x2000 pixel e raggio di 1 pixel per l’immagine di 500x500 pixel. In altre parole, sceglierete un valore maggiore per l’immagine con più pixel.  |
| Soglia | Specifica l’intervallo di contrasto da ignorare quando viene applicato il filtro Maschera di contrasto. È importante per evitare di introdurre “disturbo” quando questo filtro viene applicato a un’immagine. Il valore di soglia deve essere compreso tra 0 e 255 e corrisponde al numero di incrementi di luminosità di un’immagine in scala di grigio. 0=nero, 128=grigio al 50% e 255=bianco. <br><br>Ad esempio, con un valore di soglia pari a 12 vengono ignorate le variazioni lievi di luminosità nell’incarnato, in modo da non introdurre disturbo, mentre viene aumentato il contrasto lungo i bordi delle aree con maggior contrasto, ad esempio tra ciglia e palpebre.<br><br>Ad esempio, per una foto di un volto, Maschera di contrasto agisce sulle parti dell’immagine con maggior contrasto (come tra ciglia e palpebre) e sull’incarnato uniforme. Anche l’incarnato più omogeneo presenta lievi variazioni nei valori di luminosità. Se non si utilizza un valore di soglia, il filtro accentua le lievi differenze di tonalità nelle aree di pelle. Questo genera un effetto sgradevole mentre il maggior contrasto delle ciglia migliora la nitidezza dell’immagine.<br><br>Per evitare questo problema, utilizzate un valore di soglia che indichi al filtro di ignorare i pixel con modifiche lievi a livello di contrasto, come appunto nel caso dell’incarnato uniforme. <br><br>Nella precedente grafica delle zip, osservate la texture accanto alle zip. Si verifica del disturbo perché i valori di soglia sono troppo bassi per evitarlo. |
| Monocromatico | Seleziona la luminosità dell’immagine con maschera di contrasto (intensità).<br><br>Deselezionate questa opzione per applicare la maschera di contrasto separatamente a ciascun componente di colore. |

Consultate anche [Nitidezza di un’immagine](sharpening-image.md#sharpening_an_image).

See also [Sharpening images in Scene7 Publishing System and on Image Server](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

**Foratura sfondo**

Potete utilizzare Foratura sfondo per rimuovere automaticamente lo sfondo di un’immagine durante il caricamento. Questa tecnica è utile per attirare l’attenzione su un particolare oggetto e farlo risaltare su uno sfondo complesso.

| Opzioni di Foratura sfondo | Descrizione |
|:--- |:--- |
| Foratura sfondo | Selezionate questa opzione per attivare la foratura dello sfondo e le relative opzioni. |
| Angolo | Obbligatorio.<br><br>Angolo dell’immagine utilizzato per definire il colore di sfondo da forare.<br><br>Potete scegliere tra <b>In alto a sinistra, In basso a sinistra, In alto a destra o In basso a destra</b>. |
| Metodo di riempimento | Obbligatorio. <br><br>Controlla la trasparenza dei pixel dalla posizione Angolo impostata.<br><br>Potete scegliere tra le seguenti opzioni: <ul><li><b>Riempimento completo</b>: rende trasparenti tutti i pixel che corrispondono all’angolo specificato e che sono uniti a esso.</li><li><b>Corrispondenza pixel</b>: rende trasparenti tutti i pixel corrispondenti, ovunque si trovino nell’immagine.</li></ul> |
| Tolleranza | Facoltativo.<br><br>Controlla la quantità ammessa di variazione nella corrispondenza del colore dei pixel in base alla posizione Angolo impostata.<br><br>Con un valore pari a 0.0 verranno presi in considerazione solo i pixel di colore identico, mentre un valore pari a 1.0 consente la massima variazione. |

>[!MORELIKETHIS]
>
>* [Ritaglio di un’immagine](cropping-image.md#cropping_an_image)

