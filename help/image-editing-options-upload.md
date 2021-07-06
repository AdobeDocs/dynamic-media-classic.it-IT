---
title: Opzioni di modifica delle immagini al caricamento
description: Scopri le opzioni di modifica delle immagini disponibili al momento del caricamento.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
feature: Dynamic Media Classic,Gestione risorse
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 59%

---

# Opzioni di modifica delle immagini al caricamento{#image-editing-options-at-upload}

Durante il caricamento di file di immagine, inclusi i file AI, EPS e PSD, nella finestra di dialogo Opzioni processo di caricamento potete effettuare le seguenti operazioni di modifica:

* Ritagliare lo spazio bianco dal bordo delle immagini.
* Ritagliare manualmente dai lati delle immagini.
* Scegliere un profilo colore.
* Creare una maschera da un tracciato di ritaglio.
* Rendere le immagini più nitide con opzioni di maschera di contrasto.
* Foratura sfondo

Queste opzioni si trovano nella pagina Carica in Opzioni di modifica delle immagini.

## Ritaglio di spazi bianchi dalle immagini

Per ritagliare automaticamente i pixel dello spazio bianco da un&#39;immagine, nella finestra di dialogo Opzioni processo di caricamento fai clic su **[!UICONTROL Opzioni di ritaglio]**. Nell&#39;elenco a discesa **[!UICONTROL Ritaglia]**, scegli **[!UICONTROL Taglia]**. A questo punto, scegliete le seguenti opzioni:

* **Rifila in base a** : da questo elenco a discesa, scegli se ritagliare in base al colore o alla trasparenza:

   * **Colore** : scegli l’opzione  **** Colore. Dall’elenco a discesa **[!UICONTROL Angolo]** , seleziona quindi l’angolo dell’immagine con il colore che rappresenta meglio lo spazio bianco da ritagliare.

   * **Trasparenza** : scegli l’opzione Trasparenza.

* **Tolleranza** : trascina il cursore per specificare una tolleranza da 0 a 1:

   * **Rifilatura in base al colore**  - Consente di specificare 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell’angolo dell’immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

   * **Rifilatura in base alla trasparenza**  - Consente di specificare 0 per ritagliare i pixel solo se sono trasparenti; numeri più vicini a 1 assicurano una maggiore trasparenza.

## Ritaglio manuale dai lati delle immagini

Per ritagliare manualmente dai lati di un’immagine, scegliete Manuale dal menu Ritaglio. Immettete quindi il numero di pixel da ritagliare da ogni lato o da uno dei lati dell’immagine. La quantità di immagine che viene ritagliata dipende dall’impostazione ppi (pixel per pollice) nel file immagine. Ad esempio, se l’immagine viene visualizzata a 150 ppi e immettete 75 nelle caselle di testo, viene ritagliato mezzo pollice da ogni lato.

## Scelta di un profilo colore

Per selezionare uno spazio colore per l’immagine, scegli un’opzione Profilo colore:

* **Converti in sRGB**  - Converte in sRGB (Standard Rosso Verde Blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

* **Mantieni spazio colore originale** : mantiene lo spazio colore originale.

* **Personalizzato da > A** : apre i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore Photoshop standard o uno spazio colore caricato in Dynamic Media Classic.

Consultate [Profili ICC](icc-profiles.md#icc_profiles).

## Creazione di una maschera da un tracciato di ritaglio

Per creare una maschera per l&#39;immagine in base alle informazioni del relativo tracciato di ritaglio, fare clic su **[!UICONTROL Crea maschera dal percorso di ritaglio]**. Questa opzione può essere applicata alle immagini create con applicazioni di elaborazione immagini in cui è stato creato un tracciato di ritaglio.

## Rendere un’immagine più nitida con Maschera di contrasto

Questo filtro consente di regolare con precisione un effetto filtro di nitidezza sull’immagine ricampionata verso il basso finale. Consente di controllare l’intensità dell’effetto, il raggio dell’effetto (misurato in pixel) e una soglia di contrasto da ignorare.

Questo effetto utilizza le stesse opzioni del filtro Maschera di contrasto di Photoshop. Nonostante il nome possa fare pensare altrimenti, Maschera di contrasto è un filtro di nitidezza.

In Maschera di contrasto, impostate le opzioni desiderate come descritto nella seguente tabella:

| Opzioni di Maschera di contrasto | Descrizione |
|--- |--- |
| Fattore | Controlla il fattore di contrasto applicato ai pixel lungo i bordi.<br><br>Corrisponde all’intensità dell’effetto. La differenza principale tra i valori di quantità di Maschera definizione dettagli in Dynamic Media Classic e i valori di quantità in Adobe Photoshop, è che Photoshop ha un intervallo di quantità compreso tra l’1% e il 500%. considerando che in Dynamic Media Classic l&#39;intervallo di valori è compreso tra 0,0 e 5,0. Un valore di 5,0 in Dynamic Media Classic corrisponde approssimativamente al 500% in Photoshop; il valore 0,9 equivale al 90% e così via. |
| Raggio | Controlla il raggio dell’effetto. <br><br>I valori consentiti sono compresi tra 0 e 250. L’effetto viene eseguito su tutti i pixel dell’immagine e si irradia da tutti i pixel in tutte le direzioni. Il raggio è espresso in pixel. Ad esempio, per ottenere un effetto di nitidezza simile per un&#39;immagine da 2000 x 2000 pixel e un&#39;immagine da 500 x 500 pixel, è necessario impostare un raggio di due pixel sull&#39;immagine da 2000 x 2000 pixel. Quindi imposta un valore di raggio di un pixel sull&#39;immagine da 500 x 500 pixel. In altre parole, sceglierete un valore maggiore per l’immagine con più pixel.  |
| Soglia | Specifica l’intervallo di contrasto da ignorare quando viene applicato il filtro Maschera di contrasto. Questo effetto è importante in modo che non venga introdotto alcun &quot;rumore&quot; a un&#39;immagine quando si utilizza questo filtro. Il valore di soglia deve essere compreso tra 0 e 255 e corrisponde al numero di incrementi di luminosità di un’immagine in scala di grigio. 0=nero, 128=grigio al 50% e 255=bianco. <br><br>Ad esempio, con un valore di soglia pari a 12 vengono ignorate le variazioni lievi di luminosità nell’incarnato, in modo da non introdurre disturbo, mentre viene aumentato il contrasto lungo i bordi delle aree con maggior contrasto, ad esempio tra ciglia e palpebre.<br><br>Ad esempio, se scegli una foto del volto di un utente, la Maschera definizione dettagli influisce sulle parti a contrasto dell’immagine. Ad esempio, dove ciglia e pelle si incontrano per creare un&#39;area ovvia di contrasto, e la pelle liscia stessa. Anche l’incarnato più omogeneo presenta lievi variazioni nei valori di luminosità. Se non si utilizza un valore di soglia, il filtro accentua le lievi differenze di tonalità nelle aree di pelle. Questo genera un effetto sgradevole mentre il maggior contrasto delle ciglia migliora la nitidezza dell’immagine.<br><br>Per evitare questo problema, utilizzate un valore di soglia che indichi al filtro di ignorare i pixel con modifiche lievi a livello di contrasto, come appunto nel caso dell’incarnato uniforme. <br><br>Nella precedente grafica delle zip, osservate la texture accanto alle zip. Si verifica del disturbo perché i valori di soglia sono troppo bassi per evitarlo. |
| Monocromatico | Seleziona la luminosità dell’immagine con maschera di contrasto (intensità).<br><br>Deselezionate questa opzione per applicare la maschera di contrasto separatamente a ciascun componente di colore. |

Consultate anche [Nitidezza di un’immagine](sharpening-image.md#sharpening_an_image).

Vedere anche [Nitidezza delle immagini in Scene7 Publishing System e su Image Server](/help/assets/s7_sharpening_images.pdf).

## Foratura sfondo

Potete utilizzare Foratura sfondo per rimuovere automaticamente lo sfondo di un’immagine durante il caricamento. Questa tecnica è utile per attirare l’attenzione su un particolare oggetto e farlo risaltare su uno sfondo complesso.

| Opzioni di Foratura sfondo | Descrizione |
|:--- |:--- |
| Foratura sfondo | Selezionare per attivare o &quot;attivare&quot; la funzione e le opzioni Sfondo di blocco. |
| Angolo | Obbligatorio.<br><br>Angolo dell’immagine utilizzato per definire il colore di sfondo da forare.<br><br>Potete scegliere tra <b>In alto a sinistra, In basso a sinistra, In alto a destra o In basso a destra</b>. |
| Metodo di riempimento | Obbligatorio. <br><br>Controlla la trasparenza dei pixel dalla posizione Angolo impostata.<br><br>Potete scegliere tra le seguenti opzioni: <ul><li><b>Riempimento completo</b>: rende trasparenti tutti i pixel che corrispondono all’angolo specificato e che sono uniti a esso.</li><li><b>Corrispondenza pixel</b>: rende trasparenti tutti i pixel corrispondenti, ovunque si trovino nell’immagine.</li></ul> |
| Tolleranza | Facoltativo.<br><br>Controlla la quantità ammessa di variazione nella corrispondenza del colore dei pixel in base alla posizione Angolo impostata.<br><br>Con un valore pari a 0.0 verranno presi in considerazione solo i pixel di colore identico, mentre un valore pari a 1.0 consente la massima variazione. |

>[!MORELIKETHIS]
>
>* [Ritaglio di un’immagine](cropping-image.md#cropping_an_image)

