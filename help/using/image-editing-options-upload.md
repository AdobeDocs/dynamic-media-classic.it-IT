---
title: Opzioni di ottimizzazione immagine al caricamento
description: Scopri le opzioni di ottimizzazione delle immagini disponibili al momento del caricamento in Adobe Dynamic Media Classic.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
topic: Administration, Content Management
level: Intermediate
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 52%

---

# Opzioni di ottimizzazione immagine al caricamento{#image-editing-options-at-upload}

Durante il caricamento di file di immagine, inclusi i file AI, EPS e PSD, nella finestra di dialogo Opzioni processo di caricamento potete effettuare le seguenti operazioni di modifica:

* Ritagliare lo spazio bianco dal bordo delle immagini.
* Ritagliare manualmente dai lati delle immagini.
* Scegliere un profilo colore.
* Creare una maschera da un tracciato di ritaglio.
* Rendere le immagini più nitide con opzioni di maschera di contrasto.
* Foratura sfondo

Queste opzioni si trovano nella pagina Carica di **[!UICONTROL Opzioni di modifica immagini]** intestazione.

## Ritaglia spazio vuoto dalle immagini

Per ritagliare automaticamente i pixel dello spazio vuoto da un&#39;immagine, nella finestra di dialogo Opzioni processo di caricamento selezionare **[!UICONTROL Opzioni di ritaglio]**. In **[!UICONTROL Ritaglio]** elenco a discesa, scegliere **[!UICONTROL Rifila]**. A questo punto, scegliete le seguenti opzioni:

* **[!UICONTROL Rifila in base a]** - Da questo elenco a discesa, scegliere se ritagliare in base al colore o alla trasparenza:

   * **[!UICONTROL Colore]** - Scegli la **[!UICONTROL Colore]** opzione. Quindi, dalla sezione **[!UICONTROL Angolo]** dall&#39;elenco a discesa, selezionare l&#39;angolo dell&#39;immagine con il colore che meglio rappresenta lo spazio bianco che si desidera ritagliare.

   * **[!UICONTROL Trasparenza]** - Scegliere l&#39;opzione Trasparenza.

* **[!UICONTROL Tolleranza]** - Trascinate il dispositivo di scorrimento per specificare una tolleranza da 0 a 1:

   * **Rifilatura in base al colore** - Specificate 0 per ritagliare i pixel solo se corrispondono esattamente al colore selezionato nell&#39;angolo dell&#39;immagine. Con valori più vicini a 1 viene invece tollerata una maggiore differenza di colore. 

   * **Rifilatura basata sulla trasparenza** - Specificate 0 per ritagliare i pixel solo se sono trasparenti; i numeri più vicini a 1 consentono una maggiore trasparenza.

## Ritagliare manualmente dai lati delle immagini

Per ritagliare manualmente dai lati di un’immagine, scegliete Manuale dal menu Ritaglio. Immettete quindi il numero di pixel da ritagliare da ogni lato o da uno dei lati dell’immagine. La quantità di immagine che viene ritagliata dipende dall’impostazione ppi (pixel per pollice) nel file immagine. Ad esempio, se l&#39;immagine visualizza 150 ppi e si immette 75 nelle caselle di testo Superiore, Destra, Inferiore e Sinistra, 0,5 pollici. viene ritagliato da ogni lato.

## Scegliere un profilo colore

Per selezionare uno spazio colore per l&#39;immagine, scegliete un&#39;opzione Profilo colore:

* **[!UICONTROL Converti in sRGB]** - Converte in sRGB (rosso standard, verde, blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

* **[!UICONTROL Mantieni spazio colore originale]** - Mantiene lo spazio colore originale.

* **[!UICONTROL Personalizza da]** > **[!UICONTROL A]** - Apre i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore standard di Photoshop o uno spazio colore caricato in Adobe Dynamic Media Classic.

Consultate [Profili ICC](icc-profiles.md#icc_profiles).

## Creare una maschera da un tracciato di ritaglio

Per creare una maschera per l&#39;immagine in base alle informazioni sul tracciato di ritaglio, selezionate **[!UICONTROL Crea maschera da tracciato di ritaglio]**. Questa opzione può essere applicata alle immagini create con applicazioni di elaborazione immagini in cui è stato creato un tracciato di ritaglio.

## Nitidezza di un&#39;immagine utilizzando Maschera di contrasto

Questo filtro consente di regolare con precisione un effetto filtro di nitidezza sull’immagine ricampionata verso il basso finale. Consente di controllare l&#39;intensità dell&#39;effetto, il raggio dell&#39;effetto (misurato in pixel) e una soglia di contrasto che viene ignorata.

Questo effetto utilizza le stesse opzioni del filtro Maschera di contrasto di Photoshop. Nonostante il nome possa fare pensare altrimenti, Maschera di contrasto è un filtro di nitidezza.

In Maschera di contrasto, impostate le opzioni desiderate come descritto nella seguente tabella:

| Opzioni di Maschera di contrasto | Descrizione |
| --- | --- |
| Fattore | Controlla il fattore di contrasto applicato ai pixel lungo i bordi.<br><br>Corrisponde all’intensità dell’effetto. La differenza principale tra i valori di quantità di Maschera di contrasto in Adobe Dynamic Media Classic e i valori di quantità in Adobe Photoshop è che Photoshop ha un intervallo di quantità compreso tra 1% e 500%. In Adobe Dynamic Media Classic, invece, l’intervallo di valori è compreso tra 0,0 e 5,0. Un valore di 5,0 in Adobe Dynamic Media Classic è l’equivalente approssimativo del 500% in Photoshop; un valore di 0,9 è l’equivalente del 90% e così via. |
| Raggio | Controlla il raggio dell’effetto. <br><br>I valori consentiti sono compresi tra 0 e 250. L’effetto viene eseguito su tutti i pixel dell’immagine e si irradia da tutti i pixel in tutte le direzioni. Il raggio è espresso in pixel. Ad esempio, per ottenere un effetto di nitidezza simile per un&#39;immagine da 2000 x 2000 pixel e per un&#39;immagine da 500 x 500 pixel, è necessario impostare un raggio di due pixel sull&#39;immagine da 2000 x 2000 pixel. Quindi impostate un valore di raggio di un pixel sull&#39;immagine da 500 x 500 pixel. In altre parole, sceglierete un valore maggiore per l’immagine con più pixel.  |
| Soglia | Specifica l’intervallo di contrasto da ignorare quando viene applicato il filtro Maschera di contrasto. Questo effetto è importante in modo che non venga introdotto alcun &quot;disturbo&quot; in un&#39;immagine quando si utilizza questo filtro. Il valore di soglia deve essere compreso tra 0 e 255 e corrisponde al numero di incrementi di luminosità di un’immagine in scala di grigio. 0=nero, 128=grigio al 50% e 255=bianco. <br><br>Ad esempio, con un valore di soglia pari a 12 vengono ignorate le variazioni lievi di luminosità nell’incarnato, in modo da non introdurre disturbo, mentre viene aumentato il contrasto lungo i bordi delle aree con maggior contrasto, ad esempio tra ciglia e palpebre.<br><br>Ad esempio, se avete una foto del volto di qualcuno, la Maschera definizione dettagli influisce sulle parti in contrasto dell&#39;immagine. Ad esempio, dove ciglia e pelle si incontrano per creare un’area di contrasto evidente e la pelle liscia stessa. Anche l’incarnato più omogeneo presenta lievi variazioni nei valori di luminosità. Se non si utilizza un valore di soglia, il filtro accentua le lievi differenze di tonalità nelle aree di pelle. Questo genera un effetto sgradevole mentre il maggior contrasto delle ciglia migliora la nitidezza dell’immagine.<br><br>Per evitare questo problema, utilizzate un valore di soglia che indichi al filtro di ignorare i pixel con modifiche lievi a livello di contrasto, come appunto nel caso dell’incarnato uniforme. <br><br>Nella precedente grafica delle zip, osservate la texture accanto alle zip. Si verifica del disturbo perché i valori di soglia sono troppo bassi per evitarlo. |
| Monocromatico | Seleziona la luminosità dell’immagine con maschera di contrasto (intensità).<br><br>Deselezionate questa opzione per applicare la maschera di contrasto separatamente a ciascun componente di colore. |

Vedi anche [Nitidezza di un&#39;immagine](sharpening-image.md#sharpening_an_image).

Vedi anche [Immagini più nitide in Adobe Dynamic Media e sul server immagini](/help/using/assets/s7_sharpening_images.pdf).

## Foratura sfondo

Potete utilizzare Foratura sfondo per rimuovere automaticamente lo sfondo di un’immagine durante il caricamento. Questa tecnica è utile per attirare l’attenzione su un particolare oggetto e farlo risaltare su uno sfondo complesso.

| Opzioni di Foratura sfondo | Descrizione |
| --- | --- |
| Foratura sfondo | Selezionare per attivare o &quot;attivare&quot; la funzione e le opzioni di Foratura sfondo. |
| Angolo | Obbligatorio.<br>Angolo dell’immagine utilizzato per definire il colore di sfondo da forare.<br>Potete scegliere tra <b>In alto a sinistra, In basso a sinistra, In alto a destra o In basso a destra</b>. |
| Metodo di riempimento | Obbligatorio. <br>Controlla la trasparenza dei pixel dalla posizione Angolo impostata.<br>È possibile scegliere uno dei seguenti metodi di riempimento:<br>· <b>Riempimento Flood</b> - rende trasparenti tutti i pixel che corrispondono all&#39;angolo specificato e ad esso sono collegati.<br>• <b>Corrispondenza pixel</b>: rende trasparenti tutti i pixel corrispondenti, ovunque si trovino nell’immagine. |
| Tolleranza | Facoltativo.<br>Controlla la quantità ammessa di variazione nella corrispondenza del colore dei pixel in base alla posizione Angolo impostata.<br>Con un valore pari a 0.0 verranno presi in considerazione solo i pixel di colore identico, mentre un valore pari a 1.0 consente la massima variazione. |

>[!MORELIKETHIS]
>
>* [Ritagliare un’immagine](cropping-image.md#cropping_an_image)
