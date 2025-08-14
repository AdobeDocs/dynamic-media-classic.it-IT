---
title: Opzioni di ottimizzazione immagine al caricamento
description: Scopri le opzioni di ottimizzazione delle immagini disponibili al momento del caricamento in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
topic: Administration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 28%

---

# Opzioni di ottimizzazione immagine al caricamento{#image-editing-options-at-upload}

Durante il caricamento di file di immagine, inclusi i file AI, EPS e PSD, nella finestra di dialogo Opzioni processo di caricamento potete effettuare le seguenti operazioni di modifica:

* Ritaglia lo spazio vuoto dal bordo delle immagini.
* Ritagliare manualmente dai lati delle immagini.
* Scegliere un profilo colore.
* Creare una maschera da un tracciato di ritaglio.
* Rendere le immagini più nitide con opzioni di maschera di contrasto.
* Foratura sfondo

Queste opzioni si trovano nella pagina di caricamento sotto l&#39;intestazione **[!UICONTROL Opzioni di modifica immagini]**.

## Ritaglia spazio vuoto dalle immagini

È possibile ritagliare automaticamente i pixel dello spazio vuoto da un&#39;immagine. Nella finestra di dialogo Opzioni processo di caricamento selezionare **[!UICONTROL Opzioni ritaglio]**. Nell&#39;elenco a discesa **[!UICONTROL Ritaglia]** scegliere **[!UICONTROL Ritaglia]**. A questo punto, scegliete le seguenti opzioni:

* **[!UICONTROL Rifila in base a]**: da questo elenco a discesa, scegli se ritagliare in base al colore o alla trasparenza:

   * **[!UICONTROL Colore]**: scegli l&#39;opzione **[!UICONTROL Colore]**. Quindi, dall&#39;elenco a discesa **[!UICONTROL Angolo]**, selezionare l&#39;angolo dell&#39;immagine con il colore che meglio rappresenta il colore dello spazio bianco da ritagliare.

   * **[!UICONTROL Trasparenza]**: scegliere l&#39;opzione Trasparenza.

* **[!UICONTROL Tolleranza]**: trascina il cursore per specificare una tolleranza da 0 a 1:

   * **Rifilatura in base al colore**: specificare 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell&#39;angolo dell&#39;immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

   * **Taglio basato sulla trasparenza**: specificare 0 per ritagliare i pixel solo se sono trasparenti; i numeri più vicini a 1 consentono una maggiore trasparenza.

## Ritaglio manuale dai lati delle immagini

Per ritagliare manualmente dai lati di un’immagine, scegliete Manuale dal menu Ritaglio. Immettete quindi il numero di pixel da ritagliare da ogni lato o da uno dei lati dell’immagine. La quantità di immagine che viene ritagliata dipende dall’impostazione ppi (pixel per pollice) nel file immagine. Si supponga, ad esempio, che l&#39;immagine visualizzi 150 ppi. Immettere 75 nelle caselle di testo Superiore, Destra, Inferiore e Sinistra. A questo punto, ciascun lato viene ritagliato di 0,5 pollici.

## Scegli un profilo colore

Per selezionare uno spazio colore per l&#39;immagine, scegliete un&#39;opzione Profilo colore:

* **[!UICONTROL Converti in sRGB]**: viene convertito in sRGB (blu rosso verde standard). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini nelle pagine Web.

* **[!UICONTROL Mantieni spazio colore originale]**: mantiene lo spazio colore originale.

* **[!UICONTROL Personalizza da]** > **[!UICONTROL A]**: apre i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore standard di Photoshop o uno spazio colore caricato in Adobe Dynamic Media Classic.

Consultate [Profili ICC](icc-profiles.md#icc_profiles).

## Creare una maschera da un tracciato di ritaglio

Per creare una maschera per l&#39;immagine in base alle informazioni sul relativo percorso di ritaglio, selezionare **[!UICONTROL Crea maschera da percorso di ritaglio]**. Questa opzione può essere applicata alle immagini create con applicazioni di elaborazione immagini in cui è stato creato un tracciato di ritaglio.

## Nitidezza di un&#39;immagine utilizzando Maschera di contrasto

Questo filtro consente di regolare con precisione un effetto filtro di nitidezza sull’immagine ricampionata verso il basso finale. Consente di controllare l&#39;intensità dell&#39;effetto, il raggio dell&#39;effetto (misurato in pixel) e una soglia di contrasto che viene ignorata.

Questo effetto utilizza le stesse opzioni del filtro Maschera di contrasto di Photoshop. Nonostante il nome possa fare pensare altrimenti, Maschera di contrasto è un filtro di nitidezza.

In Maschera di contrasto, impostate le opzioni desiderate come descritto nella seguente tabella:

| Opzioni di Maschera di contrasto | Descrizione |
| --- | --- |
| Fattore | Importo controlla il contrasto applicato ai pixel del bordo.<br><br>Consideralo come l&#39;intensità dell&#39;effetto. Esiste una differenza tra la quantità di valori di Maschera di contrasto in Dynamic Media Classic e in Adobe Photoshop. La differenza principale è che Photoshop ha un intervallo di quantità compreso tra 1% e 500%. In Adobe Dynamic Media Classic, invece, l’intervallo di valori è compreso tra 0,0 e 5,0. Un valore di 5,0 in Adobe Dynamic Media Classic è l’equivalente approssimativo del 500% in Photoshop; un valore di 0,9 è l’equivalente del 90% e così via. |
| Raggio | Controlla il raggio dell’effetto. <br><br>L&#39;intervallo di valori è compreso tra 0 e 250. L’effetto viene eseguito su tutti i pixel dell’immagine e si irradia da tutti i pixel in tutte le direzioni. Il raggio è espresso in pixel. Ad esempio, per ottenere un effetto di nitidezza simile per un&#39;immagine da 2000 × 2000 pixel e per un&#39;immagine da 500 × 500 pixel, è necessario impostare un raggio di due pixel sull&#39;immagine da 2000 × 2000 pixel. Quindi impostate un valore di raggio di un pixel sull&#39;immagine da 500 × 500 pixel. In altre parole, sceglierete un valore maggiore per l’immagine con più pixel.  |
| Soglia | Specifica l’intervallo di contrasto da ignorare quando viene applicato il filtro Maschera di contrasto. Questo effetto è importante in modo che non venga introdotto alcun &quot;disturbo&quot; in un&#39;immagine quando si utilizza questo filtro. Il valore di soglia deve essere compreso tra 0 e 255 e corrisponde al numero di incrementi di luminosità di un’immagine in scala di grigio. 0=nero, 128=grigio al 50% e 255=bianco. <br><br>Ad esempio, con un valore di soglia pari a 12 vengono ignorate le variazioni lievi della luminosità della tonalità della pelle per evitare di aggiungere rumore, ma viene comunque aggiunto contrasto ai bordi delle aree in cui le ciglia si incontrano con la pelle.<br><br>Ad esempio, se si dispone di una foto del volto di un utente, la maschera di contrasto influisce sulle parti di contrasto dell&#39;immagine. Ad esempio, dove ciglia e pelle si incontrano per creare un’area di contrasto evidente e la pelle liscia stessa. Anche l’incarnato più omogeneo presenta lievi variazioni nei valori di luminosità. Se non si utilizza un valore di soglia, il filtro accentua le lievi differenze di tonalità nelle aree di pelle. Questo genera un effetto sgradevole mentre il maggior contrasto delle ciglia migliora la nitidezza dell’immagine.<br><br>Per evitare questo problema, viene introdotto un valore di soglia che indica al filtro di ignorare i pixel che non cambiano in modo significativo il contrasto, come lo skin uniforme. <br><br>Nell&#39;immagine della cerniera mostrata in precedenza, notare la trama accanto alle cerniere. Viene visualizzato disturbo dell&#39;immagine perché i valori di soglia sono troppo bassi per sopprimere il disturbo. |
| Monocromatico | Seleziona la luminosità dell’immagine con maschera di contrasto (intensità).<br><br>Deselezionate questa opzione per applicare una maschera di contrasto a ogni componente di colore separatamente. |

Vedi anche [Contrassegnare un&#39;immagine](sharpening-image.md#sharpening_an_image).

Vedi anche [Immagini più nitide in Adobe Dynamic Media e sul server immagini](/help/using/assets/s7_sharpening_images.pdf).

## Foratura sfondo

Utilizza Foratura sfondo per rimuovere automaticamente lo sfondo di un&#39;immagine quando la carichi. Questa tecnica è utile per attirare l’attenzione su un particolare oggetto e farlo risaltare su uno sfondo complesso.

| Opzioni di Foratura sfondo | Descrizione |
| --- | --- |
| Foratura sfondo | Selezionare per attivare o &quot;attivare&quot; la funzione e le opzioni di Foratura sfondo. |
| Angolo | Obbligatorio.<br>Angolo dell&#39;immagine utilizzato per definire il colore di sfondo da ritagliare.<br>È possibile scegliere tra <b>Superiore sinistro, Inferiore sinistro, Superiore destro o Inferiore destro</b>. |
| Metodo di riempimento | Obbligatorio. <br>Controlla la trasparenza dei pixel dalla posizione dell&#39;angolo impostata.<br>È possibile scegliere uno dei seguenti metodi di riempimento:<br>· <b>Riempimento completo</b>: rende trasparenti tutti i pixel che corrispondono all&#39;angolo specificato e a esso sono connessi.<br>· <b>Corrispondenza pixel</b>: rende trasparenti tutti i pixel corrispondenti, indipendentemente dalla loro posizione sull&#39;immagine. |
| Tolleranza | Facoltativo.<br>Controlla la quantità di variazione consentita nella corrispondenza dei colori dei pixel in base alla posizione dell&#39;angolo impostata.<br>Utilizzare un valore di 0,0 per far corrispondere esattamente i colori dei pixel. In alternativa, utilizza il valore 1.0 per consentire la variazione più grande. |

>[!MORELIKETHIS]
>
>* [Ritagliare un&#39;immagine](cropping-image.md#cropping_an_image)
