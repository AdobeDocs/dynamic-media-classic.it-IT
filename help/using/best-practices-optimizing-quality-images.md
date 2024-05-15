---
title: Procedure ottimali per ottimizzare la qualità delle immagini
description: Scopri le best practice per ottimizzare la qualità delle immagini.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
topic: Content Management
level: Intermediate
source-git-commit: 163eb32112ec6fbefd1dacf48212353ff3053d54
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 40%

---

# Procedure ottimali per ottimizzare la qualità delle immagini{#best-practices-for-optimizing-the-quality-of-your-images}

L&#39;ottimizzazione della qualità delle immagini può richiedere molto tempo. Molti fattori contribuiscono a rendere accettabili i risultati. Inoltre il risultato ottenuto è in parte soggettivo in quanto persone diverse percepiscono in modo differente la qualità dell’immagine. È indispensabile procedere mediante sperimentazione strutturata.

Adobe Dynamic Media Classic include più di 100 comandi per la gestione delle immagini che consentono di ottimizzare e ottimizzare le immagini e i risultati del rendering. Le seguenti indicazioni vi possono aiutare a semplificare il processo e ottenere rapidamente buoni risultati utilizzando alcuni comandi e procedure ottimali essenziali.

Vedi anche [Imaging avanzato](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

>[!TIP]
>
>Provate e scoprite i vantaggi dei modificatori di immagini Dynamic Medie e dell&#39;imaging avanzato con Dynamic Medie [_Snapshot_](https://snapshot.scene7.com/).
>
> Snapshot è uno strumento di dimostrazione visiva, progettato per illustrare la potenza di Dynamic Medie per la distribuzione di immagini ottimizzate e dinamiche. Sperimenta immagini di test o URL Dynamic Medie per osservare visivamente l’output di vari modificatori di immagini Dynamic Medie e ottimizzazioni Smart Imaging per i seguenti elementi:
>
>* Dimensione del file (con consegna WebP e AVIF)
>* Larghezza di banda di rete
>* DPR (Device Pixel Ratio, rapporto pixel dispositivo)
>
>Per scoprire quanto è facile utilizzare Snapshot, riprodurre il [Video di formazione sulle istantanee](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot) (3 minuti e 17 secondi)


## Procedure ottimali per il formato delle immagini (&amp;fmt=) {#best-practices-for-image-format-fmt}

* I formati JPG e PNG rappresentano la scelta migliore per la distribuzione di immagini di buona qualità e di dimensioni gestibili.
* Se nell’URL non viene fornito alcun comando di formato, Dynamic Medie Image Server utilizza per impostazione predefinita JPG per la consegna.
* Con il formato JPG si ottiene un rapporto di compressione di 10:1 e si ottengono in genere file di dimensioni ridotte. Il PNG viene compresso con un rapporto di circa 2:1, tranne che a volte quando le immagini contengono uno sfondo vuoto. In genere, tuttavia, i file PNG sono di dimensioni maggiori rispetto ai file JPG.
* Il formato JPG utilizza la compressione con perdita di dati, ossia durante la compressione vengono omessi degli elementi grafici (pixel). Il formato PNG utilizza invece la compressione senza perdita di dati.
* Il formato JPG spesso comprime le immagini fotografiche con fedeltà migliore rispetto alle immagini sintetiche contenenti bordi netti e contrasto ben definito.
* Se le immagini contengono trasparenze, utilizzate il formato PNG perché il JPG non supporta la trasparenza.

Come best practice per il formato immagine, inizia con l’impostazione più comune `&fmt=JPG`.

## Procedure ottimali per le dimensioni delle immagini {#best-practices-for-image-size}

La riduzione dinamica delle dimensioni delle immagini è una delle attività più comuni eseguite da Dynamic Medie Image Server. Occorre specificare le dimensioni e, facoltativamente, la modalità di downsampling da usare per la riduzione dell’immagine.

* Per il dimensionamento delle immagini, l&#39;approccio migliore e più semplice consiste nell&#39;utilizzare `&wid=<value>` e `&hei=<value>` o semplicemente `&hei=<value>`. Questi parametri impostano automaticamente la larghezza dell’immagine in base alle proporzioni.
* `&resMode=<value>` controlla l&#39;algoritmo utilizzato per il downsampling. Inizia con `&resMode=sharp2`. Questo valore offre la qualità immagine migliore. Durante l’utilizzo del valore di downsampling `=bilin` è più veloce, spesso determina l’aliasing degli artefatti.

Come best practice per il dimensionamento delle immagini, utilizza `&wid=<value>&hei=<value>&resMode=sharp2` o `&hei=<value>&resMode=sharp2`

## Procedure ottimali per la nitidezza delle immagini {#best-practices-for-image-sharpening}

La nitidezza delle immagini è l’aspetto più complesso e suscettibile ad errori per la gestione delle immagini di un sito Web. Per ulteriori informazioni su come funziona la nitidezza e la maschera di contrasto in Adobe Dynamic Media Classic, consulta le seguenti risorse utili:

White paper sulle best practice [Nitidezza delle immagini in Adobe Dynamic Media Classic e su Image Server](/help/using/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

Con Adobe Dynamic Media Classic, puoi rendere più nitide le immagini al momento dell’acquisizione, della consegna o di entrambe. In genere, tuttavia, le immagini vengono rese più nitide utilizzando un solo metodo o l&#39;altro, ma non entrambi. In genere si ottengono i risultati migliori applicando la nitidezza in fase di distribuzione, agendo sull’URL.

Esistono due metodi per la nitidezza delle immagini:

* Nitidezza semplice ( `&op_sharpen`) - Simile al filtro di nitidezza utilizzato in Photoshop, la nitidezza semplice applica la nitidezza di base alla visualizzazione finale dell&#39;immagine dopo il ridimensionamento dinamico. Tuttavia, questo metodo non può essere configurato dall’utente. La best practice consiste nell’evitare l’utilizzo di `&op_sharpen` a meno che non sia richiesto.
* Maschera di contrasto ( `&op_USM`) - Maschera di contrasto è un filtro standard di settore per la nitidezza. Come procedura ottimale si consiglia di rendere le immagini più nitide con la maschera di contrasto in base alle linee guida riportate di seguito. La mascheratura di contrasto consente di controllare tre parametri:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, intensità dell&#39;effetto).
      * `radius` (0-250, larghezza delle &quot;linee di nitidezza&quot; disegnate attorno all&#39;oggetto nitidezza, misurata in pixel).

        I parametri `radius` e `amount` lavorare l&#39;uno contro l&#39;altro. Riduzione `radius` può essere compensato aumentando `amount`. `Radius` consente un controllo più preciso, poiché un valore inferiore agisce solo sui pixel del bordo, mentre un valore più elevato agisce su una banda di pixel più ampia.

      * `threshold` (0-255, sensibilità dell&#39;effetto).

        Questo parametro specifica quale deve essere il grado di differenza dei pixel da rendere più nitidi rispetto all’area circostante, affinché vengano considerati pixel di un bordo e quindi resi più nitidi. Con questo valore di soglia è possibile evitare che venga applicata eccessiva nitidezza alle aree con colori simili, ad esempio nelle aree di incarnato. Ad esempio, con un valore di soglia pari a 12 vengono ignorate le variazioni lievi di luminosità nell&#39;incarnato per evitare di aggiungere &quot;disturbo&quot;, mentre viene aumentato il contrasto lungo i bordi delle aree dove è più presente, ad esempio tra ciglia e pelle.

        Per ulteriori informazioni su come impostare questi tre parametri, incluse le best practice da utilizzare con il filtro, consulta [Nitidezza delle immagini in Adobe Dynamic Media Classic e su Image Server](/help/using/assets/s7_sharpening_images.pdf).

      * Adobe Dynamic Media Classic consente inoltre di controllare un quarto parametro: monocromatico ( `0,1`). Questo parametro determina se la maschera di contrasto viene applicata separatamente a ciascun componente di colore utilizzando il valore `0` o alla luminosità/intensità dell&#39;immagine utilizzando il valore `1`.

Come procedura ottimale, iniziate con il parametro di maschera di contrasto “radius”. Potete iniziare con le seguenti impostazioni del raggio:

* Per sito Web: 0.2-0.3 pixel
* Stampa fotografica (250-300 ppi): 0.3-0.5 pixel
* Stampa offset (266-300 ppi): 0.7-1.0 pixel
* Stampa su tela (150 ppi): 1.5-2.0 pixel

Potete aumentare quindi gradualmente il valore di intensità “amount” da 1.75 a 4. Se il risultato di nitidezza non è ancora quello desiderato, aumentate il raggio di un decimo e provate nuovamente con un valore “amount” da 1,75 a 4. Ripetete fino a ottenere il risultato desiderato.

Lasciate il parametro “monochrome” su 0.

## Best practice per la compressione JPEG (`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* Questo parametro controlla la qualità della codifica JPG. A un valore più elevato corrisponde un’immagine di qualità migliore ma anche un file di dimensioni maggiori, e viceversa. I valori ammessi per questo parametro sono 0-100.
* Per ottimizzare la qualità, non impostate il valore del parametro su 100. La differenza tra un&#39;impostazione di 90 o 95 e 100 è quasi impercettibile. Tuttavia, 100 aumenta inutilmente la dimensione del file di immagine. Pertanto, per ottimizzare la qualità, ma evitare che i file di immagine diventino troppo grandi, impostare `qlt=` a 90 o 95.
* Per ottimizzare un file immagine di dimensioni ridotte mantenendo la qualità a un livello accettabile, impostare `qlt=` a 80. Con valori inferiori a 70-75 si verifica invece un notevole degrado della qualità dell’immagine.
* Come best practice, per rimanere al centro, imposta il `qlt=` valore 85 per rimanere al centro.
* Utilizzo del flag chroma in `qlt=`

   * Il `qlt=` Il parametro dispone di una seconda impostazione che consente di attivare il downsampling della cromaticità RGB utilizzando il valore normale `,0` (impostazione predefinita) o disattivala utilizzando il valore `,1`.
   * Per semplificare la procedura, iniziare con il downsampling della cromaticità RGB disattivato ( `,1`). Questa impostazione offre in genere una migliore qualità immagine, in particolare per le immagini sintetiche con bordi netti e forte contrasto.

Come best practice per la compressione JPG `&qlt=85,0`.

## Procedure ottimali per il ridimensionamento JPEG (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

Il parametro `jpegSize` è utile se si desidera garantire che un&#39;immagine non superi una determinata dimensione per la distribuzione a dispositivi con memoria limitata.

* Questo parametro è impostato in kilobyte ( `jpegSize=<size_in_kilobytes>`). Definisce la dimensione file massima consentita per la distribuzione dell’immagine.
* `&jpegSize=` interagisce direttamente con il parametro di compressione JPG `&qlt=`. Se la risposta del JPG con il parametro di compressione JPG specificato ( `&qlt=`) non supera il valore `jpegSize` , l’immagine viene restituita con `&qlt=` come definito. Altrimenti, `&qlt=` viene gradualmente ridotta fino a quando l’immagine non rientra nelle dimensioni massime consentite. Oppure, finché il sistema non determina che non può rientrare e restituisce un errore.

Come best practice, imposta `&jpegSize=` e aggiungi il parametro `&qlt=` se si consegnano immagini JPG a dispositivi con memoria limitata.

## Riepilogo delle procedure ottimali {#best-practices-summary}

Come best practice, per ottenere una qualità immagine elevata e dimensioni file ridotte, inizia con la seguente combinazione di parametri:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Nella maggior parte dei casi, questa combinazione di impostazioni produce risultati eccellenti.

Se l’immagine richiede ulteriore ottimizzazione, regolate gradualmente i parametri di nitidezza (maschera di contrasto): iniziate a regolare il raggio su 0.2 o 0.3, quindi aumentate il valore di intensità “amount” da 1.75 fino a un massimo di 4 (equivalente a 400% in Photoshop). Verificate il risultato ottenuto.

Se i risultati non sono ancora soddisfacenti, aumentate il raggio per incrementi decimali. Per ogni incremento decimale, impostate di nuovo il valore “amount” su 1.75 e aumentatelo gradualmente fino a 4. Ripetete questa procedura fino a ottenere l’effetto desiderato. I valori riportati qui sopra rappresentano un approccio convalidato dagli studi creativi. Tuttavia, potete anche iniziare con altri valori e seguire altre strategie. La qualità dei risultati ottenuti è soggettiva e si consiglia pertanto di procedere mediante un approccio di sperimentazione strutturata.

Durante la sperimentazione, i seguenti suggerimenti generali sono utili per ottimizzare il flusso di lavoro:

* Prova e testa diversi parametri in tempo reale, direttamente su un URL o utilizzando la funzionalità di regolazione delle immagini di Adobe Dynamic Media Classic. Quest&#39;ultimo fornisce anteprime in tempo reale per le operazioni di regolazione.
* Come best practice, ricorda che puoi raggruppare i comandi di Dynamic Medie Image Server in un predefinito per immagini. Un predefinito immagine è fondamentalmente una macro di comando URL con nomi predefiniti personalizzati, ad esempio `$thumb_low$` e `&product_high$`. Il nome del predefinito personalizzato in un percorso URL chiama questi predefiniti. Tale funzionalità facilita la gestione dei comandi e delle impostazioni di qualità per vari pattern di utilizzo delle immagini nel sito Web e genera URL più brevi.
* Adobe Dynamic Media Classic offre inoltre metodi più avanzati per regolare la qualità delle immagini, ad esempio applica la nitidezza delle immagini al momento dell’acquisizione. Per casi d’uso avanzati in cui è possibile ottimizzare ulteriormente i risultati riprodotti, Adobe Professional Services può aiutarti con informazioni approfondite e best practice personalizzate.
