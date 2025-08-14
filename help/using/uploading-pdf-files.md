---
title: Carica i file PDF
description: Scopri come caricare i file PDF associati a un eCatalog in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 30%

---

# Carica i file PDF{#uploading-the-pdf-files}

In genere, i file Adobe PDF sono l’origine di un eCatalog. Questi file contengono tutte le informazioni sull&#39;immagine, i font e gli elementi grafici vettoriali. Potete anche creare un eCatalog a partire da immagini. Dopo aver preparato i file PDF per il caricamento, sulla barra di navigazione globale, seleziona **[!UICONTROL Carica]** per iniziare a caricare i PDF.

Quando carichi un PDF per l’estrazione della pagina, Adobe applica il seguente limite:

| Tipo limite PDF | Limite imposto | Modifica del limite del 31 dicembre 2022 |
| --- | --- | --- |
| Numero massimo di pagine per un PDF da considerare per l’estrazione | 5000 (per nuovi caricamenti) | 100 (per tutti i PDF) |

Vedi anche [Limitazioni di Dynamic Media](/help/using/limitations.md).

## Preparare i file PDF

Prepara i file PDF prima di caricarli in Adobe Dynamic Media Classic:

* Per semplificare il caricamento dei file, inserire tutti i file nella stessa cartella sul computer o in rete.
* Denominate i file in ordine alfanumerico per pagina in modo da facilitare il posizionamento delle pagine nell’ordine corretto dopo che i file sono stati caricati.
* Esaminare le pagine per verificare se le pagine di PDF contengono indicatori di ritaglio, destinazioni di registrazione o barre dei colori. Questi indicatori determinano come tagliare la carta quando i documenti vengono stampati e devono essere rimossi prima di pubblicare l’eCatalog in rete. In Adobe Dynamic Media Classic sono disponibili opzioni per i segni di ritaglio durante il caricamento di file PDF.
* Se si desidera che i visualizzatori effettuino ricerche nell&#39;eCatalog per parola chiave, verificare se i file PDF sono &quot;appiattiti&quot;. Non è possibile estrarre parole di ricerca da file PDF appiattiti. Per verificare se un PDF è appiattito, provare a selezionare il testo al suo interno. Se non è possibile selezionare il testo, il PDF viene appiattito e i visualizzatori non possono eseguire ricerche per parola chiave nell&#39;eCatalog.
* Poiché sono destinati alla stampa, i file PDF contengono generalmente immagini CMYK. Per impostazione predefinita, Adobe Dynamic Media Classic è in grado di rilevare in modo intelligente queste immagini CMYK e convertirle utilizzando un profilo colore CMYK interno. Se necessario potete anche utilizzare un profilo colore personalizzato per convertire le immagini CMYK. 

  Consulta [Profili ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

## Opzioni di caricamento dei PDF “best practice” {#best-practice-pdf-upload-options}

Per informazioni dettagliate sui diversi metodi di caricamento, consultate [Caricamento dei file](uploading-files.md#uploading_your_files).

Seleziona i file da caricare, quindi seleziona le *opzioni consigliate* per PDF:

* **Opzioni ritaglio**: nella finestra di dialogo Opzioni processo di caricamento selezionare **[!UICONTROL Opzioni ritaglio]**. Se le pagine PDF contengono indicatori di ritaglio, indicatori di registrazione o altri indicatori, nell&#39;elenco a discesa **[!UICONTROL Ritaglio]** scegliere **[!UICONTROL Manuale]**. Immetti il numero di pixel da ritagliare dai lati superiore, destro, inferiore e sinistro delle pagine. Gli indicatori di ritaglio vengono spesso impostati su un margine di mezzo pollice. Si supponga di scegliere **[!UICONTROL 150]** (scelta consigliata) come risoluzione pixel per pollice. Immettere 75, 75, 75, 75 nelle caselle di testo Superiore, Destra, Inferiore e Sinistra. In questo caso, ritaglia mezzo pollice dai margini (a 150 ppi, metà di 1 equivale a 75 pixel).

* **Elaborazione**: nella finestra di dialogo Opzioni processo di caricamento selezionare **[!UICONTROL Opzioni PDF]**. Nell&#39;elenco a discesa **[!UICONTROL Elaborazione]**, scegliere **[!UICONTROL Rasterizza]**. Il file PDF deve essere rasterizzato affinché tutte le pagine e le immagini possano essere visualizzate nell’eCatalog.

* **Estrai parole da cercare (facoltativo)**: nella finestra di dialogo Opzioni processo di caricamento selezionare **[!UICONTROL Opzioni PDF]**. Nell&#39;elenco a discesa Estrai, scegli **[!UICONTROL Cerca parole]** se vuoi che i tuoi visualizzatori siano in grado di effettuare ricerche per parola chiave nell&#39;eCatalog.

* **Generazione automatica eCatalog da PDF a più pagine (facoltativo)**: nella finestra di dialogo Opzioni processo di caricamento selezionare **[!UICONTROL Opzioni PDF]**. Fai clic su **[!UICONTROL Genera automaticamente eCatalog da più pagine di PDF]** per creare automaticamente un eCatalog al momento del caricamento. Potete accedere direttamente alla schermata eCatalog e iniziare a lavorarci senza dover prima selezionare i file PDF e il comando Genera. L’eCatalog viene denominato in base al file PDF.

* **Risoluzione**: nella finestra di dialogo Opzioni processo di caricamento selezionare **[!UICONTROL Opzioni PDF]**. Nel campo di testo **[!UICONTROL Risoluzione]** immettere un valore. Adobe Dynamic Media Classic consiglia 150 pixel per pollice.

* **Spazio colore**: nella finestra di dialogo Opzioni processo di caricamento selezionare **[!UICONTROL Opzioni PDF]**. Nell&#39;elenco a discesa Spazio colore scegliere **[!UICONTROL Rileva automaticamente]**. Generalmente, i PDF creati per la stampa sono in CMYK; i PDF per la visualizzazione online sono in RGB. Se un PDF utilizza entrambi gli spazi colore, potete selezionarne uno specifico scegliendo Forza come RGB oppure Forza come CMYK. Nei PDF possono essere utilizzati entrambi gli spazi colore se, ad esempio, la grafica utilizza uno spazio colore CMYK mentre le immagini utilizzano RGB. Se avete caricato un profilo ICC, il relativo nome viene visualizzato nel menu Spazio colore e lo potete scegliere. 

  Consulta [Profili ICC (International Color Consortium)](/help/using/icc-profiles.md).

* **Opzioni profilo colore**: nella finestra di dialogo Opzioni processo di caricamento selezionare **[!UICONTROL Opzioni profilo colore]**, quindi scegliere un&#39;opzione Profilo colore:

   * **Mantieni spazio colore originale**: mantiene lo spazio colore originale.

   * **Personalizza da > A**: apre i sottomenu per scegliere uno spazio colore **[!UICONTROL Converti da]** e **[!UICONTROL Converti in]**. Puoi scegliere uno spazio colore standard di Photoshop o uno spazio colore caricato in Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

Consulta [Profili ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>per i dettagli su tutte le opzioni PDF, consultate [Opzioni di caricamento PDF](pdfs.md#pdf_upload_options).
