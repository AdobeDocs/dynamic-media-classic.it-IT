---
title: Procedure ottimali per ottimizzare la qualità delle immagini
description: Scopri le best practice per ottimizzare la qualità delle immagini.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Gestione risorse
role: Business Practitioner
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
translation-type: tm+mt
source-git-commit: 31ac96e6fd11c47284d58540f5ec0135f0e6223b
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 56%

---

# Procedure ottimali per ottimizzare la qualità delle immagini{#best-practices-for-optimizing-the-quality-of-your-images}

L’ottimizzazione della qualità delle immagini può richiedere del tempo, poiché molti fattori incidono sui risultati. Inoltre il risultato ottenuto è in parte soggettivo in quanto persone diverse percepiscono in modo differente la qualità dell’immagine. È indispensabile procedere mediante sperimentazione strutturata.

Dynamic Media Classic include più di 100 comandi di gestione delle immagini per ottimizzare e ottimizzare le immagini e i risultati di rendering. Le seguenti indicazioni vi possono aiutare a semplificare il processo e ottenere rapidamente buoni risultati utilizzando alcuni comandi e procedure ottimali essenziali.

Vedere anche [Smart imaging](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

## Procedure ottimali per il formato delle immagini (&amp;fmt=) {#best-practices-for-image-format-fmt}

* I formati JPG e PNG rappresentano la scelta migliore per la distribuzione di immagini di buona qualità e di dimensioni gestibili.
* Se nell’URL non viene fornito alcun comando di formato, per impostazione predefinita Dynamic Media Image Serving utilizza JPG per la consegna.
* Con il formato JPG si ottiene un rapporto di compressione di 10:1 e si ottengono in genere file di dimensioni ridotte. PNG si comprime a un rapporto di circa 2:1, a meno che talvolta le immagini contengano uno sfondo vuoto. In genere, tuttavia, i file PNG sono di dimensioni maggiori rispetto ai file JPG.
* Il formato JPG utilizza la compressione con perdita di dati, ossia durante la compressione vengono omessi degli elementi grafici (pixel). Il formato PNG utilizza invece la compressione senza perdita di dati.
* Il formato JPG spesso comprime le immagini fotografiche con fedeltà migliore rispetto alle immagini sintetiche contenenti bordi netti e contrasto ben definito.
* Se le immagini contengono trasparenze, utilizzate il formato PNG perché il JPG non supporta la trasparenza.

Come best practice per il formato immagine, inizia con l’impostazione più comune `&fmt=JPG`.

## Procedure ottimali per le dimensioni delle immagini {#best-practices-for-image-size}

La riduzione dinamica delle dimensioni dell&#39;immagine è una delle attività più comuni che Dynamic Media Image Serving esegue. Occorre specificare le dimensioni e, facoltativamente, la modalità di downsampling da usare per la riduzione dell’immagine.

* Per il dimensionamento delle immagini, l&#39;approccio migliore e più semplice consiste nell&#39;utilizzare `&wid=<value>` e `&hei=<value>` o semplicemente `&hei=<value>`. Questi parametri impostano automaticamente la larghezza dell’immagine in base alle proporzioni.
* `&resMode=<value>` controlla l’algoritmo utilizzato per il downsampling. Inizia con `&resMode=sharp2`. Questo valore offre la qualità immagine migliore. L’utilizzo del valore di downsampling `=bilin` è più veloce, ma spesso comporta l’aliasing degli artefatti.

Come best practice per il dimensionamento delle immagini, utilizza `&wid=<value>&hei=<value>&resMode=sharp2` o `&hei=<value>&resMode=sharp2`

## Procedure ottimali per la nitidezza delle immagini {#best-practices-for-image-sharpening}

La nitidezza delle immagini è l’aspetto più complesso e suscettibile ad errori per la gestione delle immagini di un sito Web. Dedica del tempo a scoprire come funziona la nitidezza e la Mascheratura definizione dettagli in Dynamic Media Classic facendo riferimento alle seguenti risorse utili:

White paper sulle best practice [Nitidezza delle immagini in Adobe Dynamic Media Classic e su Image Server](/help/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

Con Dynamic Media Classic è possibile rendere più nitide le immagini in fase di acquisizione, consegna o entrambe. Di solito, tuttavia, le immagini vengono rese più nitide utilizzando un solo metodo o l’altro, ma non entrambi. In genere si ottengono i risultati migliori applicando la nitidezza in fase di distribuzione, agendo sull’URL.

Esistono due metodi per rendere le immagini più nitide:

* Nitidezza semplice ( `&op_sharpen`) : simile al filtro di nitidezza utilizzato in Photoshop, la nitidezza semplice applica una nitidezza di base alla visualizzazione finale dell’immagine dopo il ridimensionamento dinamico. Tuttavia, questo metodo non può essere configurato dall’utente. La best practice consigliata consiste nell’utilizzare `&op_sharpen` solo se necessario.
* Maschera definizione dettagli ( `&op_USM`) - Il mascheramento definizione dettagli è un filtro di nitidezza standard del settore. Come procedura ottimale si consiglia di rendere le immagini più nitide con la maschera di contrasto in base alle linee guida riportate di seguito. La mascheratura di contrasto consente di controllare tre parametri:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, quantità o intensità dell’effetto)
      * `radius` (0-250, raggio o larghezza in pixel delle “linee di nitidezza” tracciate attorno all’oggetto).

         Tenete presente che i parametri `radius` e `amount` funzionano in contrapposizione l’uno con l’altro. La riduzione di `radius` può essere compensata aumentando `amount`. Il parametro `Radius` consente di agire con precisione: con un valore ridotto si agisce infatti solo sui pixel del bordo, mentre con un valore più elevato si agisce su una fascia più ampia di pixel.

      * `threshold` (0-255, sensibilità dell&#39;effetto.)

         Questo parametro determina la differenza tra i pixel da rendere più nitidi rispetto all’area circostante, prima che vengano considerati pixel del bordo e che il filtro li renda più nitidi. Con questo valore di soglia è possibile evitare che venga applicata eccessiva nitidezza alle aree con colori simili, ad esempio nelle aree di incarnato. Ad esempio, con un valore di soglia pari a 12 vengono ignorate le variazioni lievi di luminosità nell’incarnato per evitare di aggiungere “disturbo”, mentre viene aumentato il contrasto lungo i bordi delle aree dove è più presente, ad esempio tra ciglia e pelle.

         Per ulteriori informazioni su come impostare questi tre parametri, incluse le best practice da utilizzare con il filtro, consulta [Nitidezza delle immagini in Adobe Scene7 Publishing System e su Image Server](/help/assets/s7_sharpening_images.pdf).

      * Dynamic Media Classic consente inoltre di controllare un quarto parametro: monocromatico ( `0,1`). Questo parametro determina se la maschera di contrasto viene applicata separatamente a ciascun componente di colore mediante il valore `0` oppure alla luminosità/intensità dell’immagine mediante il valore `1`.

Come procedura ottimale, iniziate con il parametro di maschera di contrasto “radius”. Potete iniziare con le seguenti impostazioni del raggio:

* Per sito Web: 0.2-0.3 pixel
* Stampa fotografica (250-300 ppi): 0.3-0.5 pixel
* Stampa offset (266-300 ppi): 0.7-1.0 pixel
* Stampa su tela (150 ppi): 1.5-2.0 pixel

Potete aumentare quindi gradualmente il valore di intensità “amount” da 1.75 a 4. Se il risultato di nitidezza non è ancora quello desiderato, aumentate il raggio di un decimo e provate nuovamente con un valore “amount” da 1,75 a 4. Ripetete fino a ottenere il risultato desiderato.

Lasciate il parametro “monochrome” su 0.

## Procedure ottimali per la compressione JPEG (&amp;qlt=)  {#best-practices-for-jpeg-compression-qlt}

* Questo parametro controlla la qualità della codifica JPG. A un valore più elevato corrisponde un’immagine di qualità migliore ma anche un file di dimensioni maggiori, e viceversa. I valori ammessi per questo parametro sono 0-100.
* Per ottimizzare la qualità, non impostate il valore del parametro su 100. La differenza tra un’impostazione di 90 o 95 e 100 è quasi impercettibile, ma con un valore pari a 100 le dimensioni del file immagini aumentano inutilmente. Pertanto, per ottimizzare la qualità ma evitare che i file di immagine diventino troppo grandi, imposta il valore `qlt=` su 90 o 95.
* Per ottimizzare le dimensioni di un file immagine di piccole dimensioni ma mantenere la qualità dell&#39;immagine a un livello accettabile, imposta il valore `qlt=` su 80. Con valori inferiori a 70-75 si verifica invece un notevole degrado della qualità dell’immagine.
* Come best practice, per rimanere al centro, imposta il valore `qlt=` su 85 per rimanere al centro.
* Utilizzo del flag chroma in `qlt=`

   * Il parametro `qlt=` dispone di una seconda impostazione che consente di attivare il sottocampionamento della cromaticità RGB utilizzando il valore normale `,0` (impostazione predefinita) o di disattivarlo utilizzando il valore `,1`.
   * Per semplificare le cose, iniziate con il downsampling della cromaticità RGB disattivato ( `,1`). Questa impostazione offre in genere una migliore qualità immagine, in particolare per le immagini sintetiche con bordi netti e forte contrasto.

Come procedura ottimale, per la compressione JPG si consiglia di utilizzare `&qlt=85,0`.

## Procedure ottimali per il ridimensionamento JPEG (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

Il parametro `jpegSize` è utile se si desidera garantire che un&#39;immagine non superi una certa dimensione per la consegna a dispositivi con memoria limitata.

* Questo parametro è impostato in kilobyte ( `jpegSize=<size_in_kilobytes>`). Definisce la dimensione file massima consentita per la distribuzione dell’immagine.
* `&jpegSize=` interagisce con il parametro di compressione JPG  `&qlt=`. Se la risposta JPG con il parametro di compressione JPG specificato ( `&qlt=`) non supera il valore `jpegSize`, l&#39;immagine viene restituita con `&qlt=` come definito. In caso contrario, `&qlt=` viene gradualmente ridotto finché l&#39;immagine non rientra nelle dimensioni massime consentite, o finché il sistema non lo determina e restituisce un errore.

Come best practice, imposta `&jpegSize=` e aggiungi il parametro `&qlt=` se distribuisci immagini JPG a dispositivi con memoria limitata.

## Riepilogo delle procedure ottimali {#best-practices-summary}

Per ottenere immagini di alta qualità e file di dimensioni ridotte, utilizzate la seguente combinazione di parametri:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Questa combinazione di impostazioni consente di ottenere risultati ottimali nella maggior parte dei casi.

Se l’immagine richiede ulteriore ottimizzazione, regolate gradualmente i parametri di nitidezza (maschera di contrasto): iniziate a regolare il raggio su 0.2 o 0.3, quindi aumentate il valore di intensità “amount” da 1.75 fino a un massimo di 4 (equivalente a 400% in Photoshop). Verificate il risultato ottenuto.

Se i risultati non sono ancora soddisfacenti, aumentate il raggio per incrementi decimali. Per ogni incremento decimale, impostate di nuovo il valore “amount” su 1.75 e aumentatelo gradualmente fino a 4. Ripetete questa procedura fino a ottenere l’effetto desiderato. I valori riportati qui sopra rappresentano un approccio convalidato dagli studi creativi. Tuttavia, potete anche iniziare con altri valori e seguire altre strategie. La qualità dei risultati ottenuti è soggettiva e si consiglia pertanto di procedere mediante un approccio di sperimentazione strutturata.

Durante l’esperimento, i seguenti suggerimenti generali sono utili per ottimizzare il flusso di lavoro:

* Prova e verifica diversi parametri in tempo reale, direttamente su un URL Dynamic Media Classic o utilizzando la funzionalità di regolazione delle immagini di Dynamic Media Classic. Quest&#39;ultima fornisce anteprime in tempo reale per le operazioni di regolazione.
* Come best practice, ricorda che puoi raggruppare i comandi di Dynamic Media Image Serving in un predefinito per immagini. Un predefinito per immagini è fondamentalmente macro di comando URL con nomi predefiniti personalizzati come `$thumb_low$` e `&product_high$`. Il nome predefinito personalizzato in un percorso URL chiama questi predefiniti. Tale funzionalità facilita la gestione dei comandi e delle impostazioni di qualità per vari pattern di utilizzo delle immagini nel sito Web e genera URL più brevi.
* Dynamic Media Classic offre anche modi più avanzati per ottimizzare la qualità delle immagini, ad esempio applicando la nitidezza delle immagini durante l’acquisizione. Per i casi d’uso avanzati in cui l’ulteriore ottimizzazione e ottimizzazione dei risultati di rendering è un’opzione, Adobe Professional Services può aiutarti con informazioni personalizzate e best practice.
