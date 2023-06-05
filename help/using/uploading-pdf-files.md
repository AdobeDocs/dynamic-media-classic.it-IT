---
title: Carica i file PDF
description: Scopri come caricare i file PDF associati a un eCatalog in Adobe Dynamic Media Classic.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 36%

---

# Carica i file PDF{#uploading-the-pdf-files}

In genere, i file Adobe PDF sono l’origine di un eCatalog. Questi file contengono tutte le informazioni sull&#39;immagine, i font e gli elementi grafici vettoriali. Potete anche creare un eCatalog a partire da immagini. Dopo aver preparato i file PDF per il caricamento, nella barra di navigazione globale seleziona **[!UICONTROL Carica]** per iniziare a caricare i PDF.

Quando carichi un PDF per l’estrazione della pagina, Adobe applica il seguente limite:

| Tipo di limite PDF | Limite imposto | Modifica del limite del 31 dicembre 2022 |
| --- | --- | --- |
| Numero massimo di pagine per un PDF da considerare per l’estrazione | 5000 (per nuovi caricamenti) | 100 (per tutti i PDF) |

Vedi anche [Limitazioni di Dynamic Media](/help/using/limitations.md).

## Preparare i file PDF {#preparing-your-pdf-files}

Prepara i file PDF prima di caricarli in Adobe Dynamic Media Classic:

* Per semplificare il caricamento dei file, inserire tutti i file nella stessa cartella sul computer o in rete.
* Denominate i file in ordine alfanumerico per pagina in modo da facilitare il posizionamento delle pagine nell’ordine corretto dopo che i file sono stati caricati.
* Esaminare le pagine per verificare se le pagine PDF contengono indicatori di ritaglio, destinazioni di registrazione o barre dei colori. Questi indicatori determinano come tagliare la carta quando i documenti vengono stampati e devono essere rimossi prima di pubblicare l’eCatalog in rete. In Adobe Dynamic Media Classic sono disponibili opzioni per i segni di ritaglio durante il caricamento di file PDF.
* Per consentire agli utenti di effettuare ricerche nell’eCatalog mediante parole chiave, verificate che i file PDF non siano “appiattiti” (convertiti in immagini). Non è possibile estrarre parole di ricerca da file PDF appiattiti. Per verificare se un PDF è stato appiattito, provate a selezionare il testo al suo interno. Se non è possibile selezionare il testo, il PDF viene appiattito e gli utenti non possono eseguire ricerche per parola chiave nell&#39;eCatalog.
* Poiché sono destinati alla stampa, i file PDF contengono generalmente immagini CMYK. Per impostazione predefinita, Adobe Dynamic Media Classic è in grado di rilevare in modo intelligente queste immagini CMYK e convertirle utilizzando un profilo colore CMYK interno. Se necessario potete anche utilizzare un profilo colore personalizzato per convertire le immagini CMYK. 

   Consulta [Profili ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

## Opzioni di caricamento dei PDF “best practice” {#best-practice-pdf-upload-options}

Per informazioni dettagliate sui diversi metodi di caricamento, consultate [Caricamento dei file](uploading-files.md#uploading_your_files).

Seleziona i file da caricare, quindi fai clic su *best practice* Opzioni PDF:

* **Opzioni di ritaglio** - Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Opzioni di ritaglio]**. Se le pagine PDF contengono segni di ritaglio, segni di registrazione o altri segni, nel **[!UICONTROL Ritaglio]** elenco a discesa, scegliere **[!UICONTROL Manuale]**. Specificate quanti pixel ritagliare dalla parte superiore, destra, inferiore e sinistra delle pagine. Gli indicatori di ritaglio vengono spesso impostati su un margine di mezzo pollice. Supponiamo di scegliere **[!UICONTROL 150]** (opzione consigliata) come risoluzione pixel per pollice e immettete 75, 75, 75, 75 nelle caselle di testo Superiore, Destra, Inferiore e Sinistra. In tal caso, ritaglia un mezzo pollice dai margini (a 150 ppi, metà di 1 equivale a 75 pixel).

* **Elaborazione** - Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Opzioni PDF]**. In **[!UICONTROL Elaborazione]** elenco a discesa, scegliere **[!UICONTROL Rasterizza]**. Il file PDF deve essere rasterizzato affinché tutte le pagine e le immagini possano essere visualizzate nell’eCatalog.

* **Estrai parole di ricerca (facoltativo)** - Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Opzioni PDF]**. Nell&#39;elenco a discesa Estrai, scegliere **[!UICONTROL Parole di ricerca]** se desideri che gli utenti possano effettuare ricerche per parola chiave nell’eCatalog.

* **Genera automaticamente eCatalog da più pagine PDF (facoltativo)** - Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Opzioni PDF]**. Seleziona **[!UICONTROL Genera automaticamente eCatalog da più PDF di pagine]** per creare automaticamente un eCatalog durante il caricamento. Potete accedere direttamente alla schermata eCatalog e iniziare a lavorarci senza dover prima selezionare i file PDF e il comando Genera. L’eCatalog viene denominato in base al file PDF.

* **Risoluzione** - Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Opzioni PDF]**. In **[!UICONTROL Risoluzione]** immetti un valore. Adobe Dynamic Media Classic consiglia 150 pixel per pollice.

* **Spazio colore** - Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Opzioni PDF]**. Nell&#39;elenco a discesa Spazio colore, selezionate **[!UICONTROL Rileva automaticamente]**. Generalmente, i PDF creati per la stampa sono in CMYK; i PDF per la visualizzazione online sono in RGB. Se un PDF utilizza entrambi gli spazi colore, potete selezionarne uno specifico scegliendo Forza come RGB oppure Forza come CMYK. Nei PDF possono essere utilizzati entrambi gli spazi colore se, ad esempio, la grafica utilizza uno spazio colore CMYK mentre le immagini utilizzano RGB. Se avete caricato un profilo ICC, il relativo nome viene visualizzato nel menu Spazio colore e lo potete scegliere. 

   Consulta [Profili ICC (International Color Consortium)](/help/using/icc-profiles.md).

* **Opzioni profilo colore** - Nella finestra di dialogo Opzioni processo di caricamento, seleziona **[!UICONTROL Opzioni profilo colore]**, quindi scegliere un&#39;opzione Profilo colore:

   * **Mantieni spazio colore originale** - Mantiene lo spazio colore originale.

   * **Personalizza Da > A** - Apre i sottomenu in modo da poter scegliere **[!UICONTROL Converti da]** e **[!UICONTROL Converti in]** spazio colore. Puoi scegliere uno spazio colore standard di Photoshop o uno spazio colore caricato in Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Consulta [Profili ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>per i dettagli su tutte le opzioni PDF, consultate [Opzioni di caricamento PDF](pdfs.md#pdf_upload_options).
