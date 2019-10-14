---
title: Caricamento di file PDF
seo-title: Caricamento di file PDF
description: 'null'
seo-description: Scoprite come caricare i file PDF associati a un eCatalog.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Caricamento di file PDF{#uploading-the-pdf-files}

Di solito, un eCatalog viene generato a partire da file Adobe PDF contenenti tutti i dati sulle immagini, sui font e sulla grafica vettoriale. Potete anche creare un eCatalog a partire da immagini. Dopo aver preparato i file PDF per il caricamento, fate clic sul pulsante Carica nella barra di navigazione globale per avviarne il caricamento.

## Preparazione dei file PDF {#preparing-your-pdf-files}

Preparate i file PDF prima di caricarli su Scene7 Publishing System:

* Per facilitare il caricamento dei file, posizionateli tutti nella stessa cartella sul computer locale o sulla rete.
* Denominate i file in ordine alfanumerico per pagina in modo da facilitare il posizionamento delle pagine nell’ordine corretto dopo che i file sono stati caricati.
* Esaminate le pagine PDF per verificare se contengono indicatori di ritaglio, crocini di registro o barre di colore. Questi indicatori determinano come tagliare la carta quando i documenti vengono stampati e devono essere rimossi prima di pubblicare l’eCatalog in rete. Dynamic Media Classic offre opzioni per gli indicatori di taglio al momento del caricamento dei file PDF.
* Per consentire agli utenti di effettuare ricerche nell’eCatalog mediante parole chiave, verificate che i file PDF non siano “appiattiti” (convertiti in immagini). Non è possibile estrarre parole di ricerca da file PDF appiattiti. Per verificare se un PDF è stato appiattito, provate a selezionare il testo al suo interno. Se non potete selezionare il testo, il PDF è appiattito e gli utenti non possono effettuare ricerche per parole chiave nell’eCatalog.
* Poiché sono destinati alla stampa, i file PDF contengono generalmente immagini CMYK. Per impostazione predefinita, SPS è in grado di rilevare in modo intelligente tali immagini CMYK e convertirle utilizzando un profilo colore CMYK interno. Se necessario potete anche utilizzare un profilo colore personalizzato per convertire le immagini CMYK. 

   Consultate [Profili ICC](icc-profiles.md#icc_profiles).

## Opzioni di caricamento dei PDF “best practice” {#best-practice-pdf-upload-options}

Per informazioni dettagliate sui diversi metodi di caricamento, consultate [Caricamento dei file](uploading-files.md#uploading_your_files).

Selezionate i file da caricare, quindi selezionate le opzioni PDF *best practice*:

* **Ritaglia** Selezionate il menu Ritaglio e scegliete Manuale se le pagine contengono indicatori di taglio, crocini di registro o altri indicatori. Specificate quanti pixel ritagliare dalla parte superiore, destra, inferiore e sinistra delle pagine. Gli indicatori di taglio vengono impostati generalmente in un margine di mezzo pollice. Supponiamo che scegliate 150 come risoluzione di pixel per pollice (impostazione consigliata): inserendo 75, 75, 75, 75 nelle caselle di testo In alto, A destra, In basso e A sinistra, il ritaglio applicato è di mezzo pollice dai margini (a 150 ppi, mezzo pollice corrisponde a 75 pixel).

* **Elaborazione** Selezionate il menu Elaborazione e scegliete Rasterizza. Il file PDF deve essere rasterizzato affinché tutte le pagine e le immagini possano essere visualizzate nell’eCatalog.

* **Estrai termini di ricerca (facoltativo)** Selezionate questa opzione se desiderate che gli utenti possano effettuare ricerche per parole chiave nell’eCatalog.

* **Genera automaticamente eCatalog da PDF con più pagine (facoltativo)** Selezionate questa opzione per creare automaticamente un eCatalog al momento del caricamento. Potete accedere direttamente alla schermata eCatalog e iniziare a lavorarci senza dover prima selezionare i file PDF e il comando Genera. L’eCatalog viene denominato in base al file PDF.

* **Risoluzione** Dynamic Media Classic consiglia 150 pixel per pollice.

* **Colorspace** Dynamic Media Classic consiglia di scegliere Rileva automaticamente. Generalmente, i PDF creati per la stampa sono in CMYK; i PDF per la visualizzazione online sono in RGB. Se un PDF utilizza entrambi gli spazi colore, potete selezionarne uno specifico scegliendo Forza come RGB oppure Forza come CMYK. Nei PDF possono essere utilizzati entrambi gli spazi colore se, ad esempio, la grafica utilizza uno spazio colore CMYK mentre le immagini utilizzano RGB. Se avete caricato un profilo ICC, il relativo nome viene visualizzato nel menu Spazio colore e lo potete scegliere. 

   Consultate [Profili ICC](icc-profiles.md#icc_profiles).

* **Profilo** colore Scegliete un’opzione Profilo colore:

* **ConvertTo SRGB** Converte in SRGB (Standard Rosso Verde Blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

* **Mantieni spazio** colore originale Conserva lo spazio colore originale.

* **Personalizzato da &gt;** Apre i menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Potete scegliere uno spazio colore standard di Photoshop o uno caricato in SPS. 

Consultate [Profili ICC](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>per i dettagli su tutte le opzioni PDF, consultate [Opzioni di caricamento PDF](pdfs.md#pdf_upload_options).

