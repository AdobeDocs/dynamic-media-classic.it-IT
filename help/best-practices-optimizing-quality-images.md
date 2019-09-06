---
title: Procedure ottimali per ottimizzare la qualità delle immagini
seo-title: Procedure ottimali per ottimizzare la qualità delle immagini
description: 'null'
seo-description: Scopri le best practice per ottimizzare la qualità delle immagini.
uuid: 102 e 83 fe-ee 2 a -443 b-ba 92-6 ad 5 cc 3 daef 0
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 8164466 e -2520-482 a -88 ec -6191 fdc 77 ea 3
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Procedure ottimali per ottimizzare la qualità delle immagini{#best-practices-for-optimizing-the-quality-of-your-images}

L’ottimizzazione della qualità delle immagini può richiedere del tempo, poiché molti fattori incidono sui risultati. Inoltre il risultato ottenuto è in parte soggettivo in quanto persone diverse percepiscono in modo differente la qualità dell’immagine. È indispensabile procedere mediante sperimentazione strutturata.

Dynamic Media Classic include più di 100 comandi per la gestione delle immagini che consentono di ottimizzare le immagini e i risultati di rendering. Le seguenti indicazioni vi possono aiutare a semplificare il processo e ottenere rapidamente buoni risultati utilizzando alcuni comandi e procedure ottimali essenziali.

Consultate anche [Imaging avanzato](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html).

## Procedure ottimali per il formato delle immagini (&amp;fmt=) {#best-practices-for-image-format-fmt}

* I formati JPG e PNG rappresentano la scelta migliore per la distribuzione di immagini di buona qualità e di dimensioni gestibili.
* Se nell'URL non viene fornito alcun comando di formato, per impostazione predefinita viene utilizzato Dynamic Media Image Server.
* Con il formato JPG si ottiene un rapporto di compressione di 10:1 e si ottengono in genere file di dimensioni ridotte. Con il formato PNG si ottiene un rapporto di compressione di 2:1 ad eccezione di alcuni casi, ad esempio per le immagini con sfondo bianco. In genere, tuttavia, i file PNG sono di dimensioni maggiori rispetto ai file JPG.
* Il formato JPG utilizza la compressione con perdita di dati, ossia durante la compressione vengono omessi degli elementi grafici (pixel). Il formato PNG utilizza invece la compressione senza perdita di dati.
* Il formato JPG spesso comprime le immagini fotografiche con fedeltà migliore rispetto alle immagini sintetiche contenenti bordi netti e contrasto ben definito.
* Se le immagini contengono trasparenze, utilizzate il formato PNG perché il JPG non supporta la trasparenza.

As a best practice for image format, start with the most common setting `&fmt=JPG`.

## Procedure ottimali per le dimensioni delle immagini {#best-practices-for-image-size}

La riduzione dinamica delle dimensioni dell'immagine è una delle attività più comuni eseguite da Dynamic Media Image Server. Occorre specificare le dimensioni e, facoltativamente, la modalità di downsampling da usare per la riduzione dell’immagine.

* For image sizing, the best and most straightforward approach is to use `&wid=<value>` and `&hei=<value>` or just `&hei=<value>`. Questi parametri impostano automaticamente la larghezza dell’immagine in base alle proporzioni.
* `&resMode=<value>` controlla l'algoritmo utilizzato per il downsampling. Inizia con `&resMode=sharp2`. Questo valore offre la qualità immagine migliore. While using the downsampling value `=bilin` is faster, it often results in the aliasing of artifacts.

Come procedura ottimale per il ridimensionamento delle immagini, l'utilizzo `&wid=<value>&hei=<value>&resMode=sharp2` o `&hei=<value>&resMode=sharp2`

## Procedure ottimali per la nitidezza delle immagini {#best-practices-for-image-sharpening}

La nitidezza delle immagini è l’aspetto più complesso e suscettibile ad errori per la gestione delle immagini di un sito Web. Dedicate il tempo necessario per migliorare la nitidezza e la maschera di contrasto in Dynamic Media Classic, facendo riferimento alle seguenti risorse utili:

Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

On Adobe TV, watch [Sharpening an image with unsharp mask](https://tv.adobe.com/watch/visual-design-cs6/sharpening-an-image-with-unsharp-mask/).

Con Dynamic Media Classic potete rendere le immagini più nitide durante l'assimilazione, la distribuzione o entrambi. In molti casi, tuttavia, è necessario rendere le immagini più nitide utilizzando un solo metodo e non entrambi. In genere si ottengono i risultati migliori applicando la nitidezza in fase di distribuzione, agendo sull’URL.

Esistono due metodi per rendere le immagini più nitide:

* Simple sharpening ( `&op_sharpen`) - Similar to the sharpen filter used in Photoshop, simple sharpening applies basic sharpening to the final view of the image following dynamic resizing. Tuttavia, questo metodo non può essere configurato dall’utente. The best practice is to not use `&op_sharpen` unless required.
* Unsharp masking ( `&op_USM`) - Unsharp masking is an industry standard sharpening filter. Come procedura ottimale si consiglia di rendere le immagini più nitide con la maschera di contrasto in base alle linee guida riportate di seguito. La mascheratura di contrasto consente di controllare tre parametri:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, quantità o intensità dell’effetto)
      * `radius` (0-250, raggio o larghezza in pixel delle “linee di nitidezza” tracciate attorno all’oggetto).

         Tenete presente che i parametri `radius` e `amount` funzionano in contrapposizione l’uno con l’altro. Reducing `radius` can be compensated by increasing `amount`. Il parametro `Radius` consente di agire con precisione: con un valore ridotto si agisce infatti solo sui pixel del bordo, mentre con un valore più elevato si agisce su una fascia più ampia di pixel.

      * `threshold` (0-255, sensibilità dell'effetto).

         Questo parametro specifica quale deve essere il grado di differenza dei pixel da rendere più nitidi rispetto all’area circostante, affinché vengano considerati pixel di un bordo e quindi resi più nitidi. Con questo valore di soglia è possibile evitare che venga applicata eccessiva nitidezza alle aree con colori simili, ad esempio nelle aree di incarnato. Ad esempio, con un valore di soglia pari a 12 vengono ignorate le variazioni lievi di luminosità nell’incarnato, in modo da non introdurre disturbo, mentre viene aumentato il contrasto lungo i bordi delle aree con maggior contrasto, ad esempio tra ciglia e pelle.
      Per ulteriori informazioni su come impostare questi tre parametri, incluse le procedure ottimali per l’utilizzi del filtro, consultate le risorse seguenti:

      Argomento della Guida Dynamic Media Classic sull' [applicazione della nitidezza a un'immagine](https://help.adobe.com/en_US/scene7/using/WS389B162D-2981-41e5-9253-15D22D2ECBC8.html).

      Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

   * Dynamic Media Classic consente anche di controllare un quarto parametro: monocromatico ( `0,1`). Questo parametro determina se la maschera di contrasto viene applicata separatamente a ciascun componente di colore mediante il valore `0` oppure alla luminosità/intensità dell’immagine mediante il valore `1`.


Come procedura ottimale, iniziate con il parametro di maschera di contrasto “radius”. Potete iniziare con le seguenti impostazioni del raggio:

* Per sito Web: 0.2-0.3 pixel
* Stampa fotografica (250-300 ppi): 0.3-0.5 pixel
* Stampa offset (266-300 ppi): 0.7-1.0 pixel
* Stampa su tela (150 ppi): 1.5-2.0 pixel

Potete aumentare quindi gradualmente il valore di intensità “amount” da 1.75 a 4. Se il risultato di nitidezza non è ancora quello desiderato, aumentate il raggio di un decimo e provate nuovamente con un valore “amount” da 1,75 a 4. Ripetete fino a ottenere il risultato desiderato.

Lasciate il parametro “monochrome” su 0.

## Procedure ottimali per la compressione JPEG (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* Questo parametro controlla la qualità della codifica JPG. A un valore più elevato corrisponde un’immagine di qualità migliore ma anche un file di dimensioni maggiori, e viceversa. I valori ammessi per questo parametro sono 0-100.
* Per ottimizzare la qualità, non impostate il valore del parametro su 100. La differenza tra un’impostazione di 90 o 95 e 100 è quasi impercettibile, ma con un valore pari a 100 le dimensioni del file immagini aumentano inutilmente. Therefore, to optimize for quality but avoid image files becoming too large, set the `qlt=` value to 90 or 95.
* To optimize for a small image file size but keep image quality at an acceptable level, set the `qlt=` value to 80. Con valori inferiori a 70-75 si verifica invece un notevole degrado della qualità dell’immagine.
* As a best practice, to stay in the middle, set the `qlt=` value to 85 to stay in the middle.
* Utilizzo del flag chroma in `qlt=`

   * The `qlt=` parameter has a second setting that lets you turn on RGB chromaticity downsampling using the normal value `,0` (default), or turn it off using the value `,1`.
   * Per semplificare le cose, iniziate con il downsampling della cromaticità RGB disattivato ( `,1`). Questa impostazione offre in genere una migliore qualità immagine, in particolare per le immagini sintetiche con bordi netti e forte contrasto.

Come procedura ottimale, per la compressione JPG si consiglia di utilizzare `&qlt=85,0`.

## Procedure ottimali per il ridimensionamento JPEG (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

`jpegSize` è un parametro utile affinché l’immagine non superi determinate dimensioni per la distribuzione su dispositivi con memoria limitata.

* Questo parametro è impostato in kilobyte ( `jpegSize=<size_in_kilobytes>`). Definisce la dimensione file massima consentita per la distribuzione dell’immagine.
* `&jpegSize=` interagisce con il parametro `&qlt=`di compressione JPG. If the JPG response with the specified JPG compression parameter ( `&qlt=`) does not exceed the `jpegSize` value, the image is returned with `&qlt=` as defined. Otherwise, `&qlt=` is gradually decreased until the image fits in the maximum allowed size, or until the system determines it cannot fit and returns an error.

As a best practice, set `&jpegSize=` and add the parameter `&qlt=` if you are delivering JPG images to devices with limited memory.

## Riepilogo delle procedure ottimali {#best-practices-summary}

Per ottenere immagini di alta qualità e file di dimensioni ridotte, utilizzate la seguente combinazione di parametri:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Questa combinazione di impostazioni consente di ottenere risultati ottimali nella maggior parte dei casi.

Se l’immagine richiede ulteriore ottimizzazione, regolate gradualmente i parametri di nitidezza (maschera di contrasto): iniziate a regolare il raggio su 0.2 o 0.3, quindi aumentate il valore di intensità “amount” da 1.75 fino a un massimo di 4 (equivalente a 400% in Photoshop). Verificate il risultato ottenuto.

Se i risultati non sono ancora soddisfacenti, aumentate il raggio per incrementi decimali. Per ogni incremento decimale, impostate di nuovo il valore “amount” su 1.75 e aumentatelo gradualmente fino a 4. Ripetete questa procedura fino a ottenere l’effetto desiderato. I valori riportati qui sopra rappresentano un approccio convalidato dagli studi creativi. Tuttavia, potete anche iniziare con altri valori e seguire altre strategie. La qualità dei risultati ottenuti è soggettiva e si consiglia pertanto di procedere mediante un approccio di sperimentazione strutturata.

Per ottimizzare il flusso di lavoro, può essere utile seguire anche i consigli generali riportati di seguito:

* Provate e testate i diversi parametri in tempo reale, direttamente con un URL Dynamic Media Classic oppure utilizzando la funzionalità di regolazione delle immagini di Scene 7 Publishing System che fornisce anteprime in tempo reale per le operazioni di regolazione.
* Come procedura ottimale, potete raggruppare i comandi Dynamic Media Image Serving in un predefinito per immagini. An image preset is basically URL command macros with custom preset names such as `$thumb_low$` and `&product_high$`. Il nome del predefinito personalizzato in un percorso URL richiama il predefinito corrispondente. Tale funzionalità facilita la gestione dei comandi e delle impostazioni di qualità per vari pattern di utilizzo delle immagini nel sito Web e genera URL più brevi.
* Dynamic Media Classic offre inoltre metodi più avanzati per ottimizzare la qualità delle immagini, ad esempio l'applicazione di nitidezza alle immagini durante l'assimilazione. Per le situazioni d’uso avanzate in cui questa può rappresentare un’opzione per ottimizzare ulteriormente i risultati di rendering, il team Adobe Professional Services può aiutarvi con approfondimenti mirati e procedure ottimali.

