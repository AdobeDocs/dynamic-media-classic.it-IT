---
title: Caricamento di file PDF
description: Scopri come caricare i file PDF associati a un eCatalog.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Visualizzatori,eCatalog
role: Business Practitioner
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 56%

---

# Caricamento di file PDF{#uploading-the-pdf-files}

In genere, i file Adobe PDF sono l’origine di un eCatalog. Questi file contengono tutte le informazioni sulle immagini, i font e la grafica vettoriale. Potete anche creare un eCatalog a partire da immagini. Dopo aver preparato i file PDF per il caricamento, fate clic sul pulsante Carica nella barra di navigazione globale per avviarne il caricamento.

## Preparazione dei file PDF  {#preparing-your-pdf-files}

Prepara i file PDF prima di caricarli in Dynamic Media Classic:

* Per semplificare il caricamento dei file, inserisci tutti i file nella stessa cartella sul computer o sulla rete.
* Denominate i file in ordine alfanumerico per pagina in modo da facilitare il posizionamento delle pagine nell’ordine corretto dopo che i file sono stati caricati.
* Per verificare se le pagine PDF contengono indicatori di ritaglio, destinazioni di registrazione o barre dei colori, esaminare le pagine. Questi indicatori determinano come tagliare la carta quando i documenti vengono stampati e devono essere rimossi prima di pubblicare l’eCatalog in rete. Dynamic Media Classic fornisce opzioni per gli indicatori di ritaglio quando si caricano i file PDF.
* Per consentire agli utenti di effettuare ricerche nell’eCatalog mediante parole chiave, verificate che i file PDF non siano “appiattiti” (convertiti in immagini). Non è possibile estrarre parole di ricerca da file PDF appiattiti. Per verificare se un PDF è stato appiattito, provate a selezionare il testo al suo interno. Se non potete selezionare il testo, il PDF è appiattito e gli utenti non possono effettuare ricerche per parole chiave nell’eCatalog.
* Poiché sono destinati alla stampa, i file PDF contengono generalmente immagini CMYK. Per impostazione predefinita, Dynamic Media Classic può rilevare in modo intelligente queste immagini CMYK e convertirle utilizzando un profilo colore CMYK interno. Se necessario potete anche utilizzare un profilo colore personalizzato per convertire le immagini CMYK. 

   Consultate [Profili ICC](icc-profiles.md#icc_profiles).

## Opzioni di caricamento dei PDF “best practice”  {#best-practice-pdf-upload-options}

Per informazioni dettagliate sui diversi metodi di caricamento, consultate [Caricamento dei file](uploading-files.md#uploading_your_files).

Selezionate i file da caricare, quindi selezionate le opzioni PDF *best practice*:

* ****
RitaglioSelezionate il menu Ritaglio e scegliete Manuale se le pagine contengono indicatori di ritaglio, indicatori di registrazione o altri indicatori. Specificate quanti pixel ritagliare dalla parte superiore, destra, inferiore e sinistra delle pagine. I segni di ritaglio sono spesso impostati su un margine di mezzo pollice. Si supponga di scegliere 150 (consigliato) come risoluzione pixel per pollice e di immettere 75, 75, 75, 75, 75 nelle caselle di testo In alto, A destra, In basso e A sinistra. In tal caso, ritaglia un pollice e mezzo dai margini (a 150 ppi, metà di 1 è uguale a 75 pixel).

* ****
ElaborazioneSelezionare il menu Elaborazione e scegliere Rasterizza. Il file PDF deve essere rasterizzato affinché tutte le pagine e le immagini possano essere visualizzate nell’eCatalog.

* **Estrai parole di ricerca (facoltativo)**
Seleziona questa opzione se vuoi che i tuoi visualizzatori siano in grado di cercare per parola chiave nel tuo eCatalog.

* **Genera automaticamente eCatalog da più pagine PDF (facoltativo)**
Seleziona questa opzione per creare automaticamente un eCatalog al momento del caricamento. Potete accedere direttamente alla schermata eCatalog e iniziare a lavorarci senza dover prima selezionare i file PDF e il comando Genera. L’eCatalog viene denominato in base al file PDF.

* ****
RisoluzioneDynamic Media Classic consiglia 150 pixel per pollice.

* ****
ColorspaceDynamic Media Classic consiglia di scegliere Rileva automaticamente. Generalmente, i PDF creati per la stampa sono in CMYK; i PDF per la visualizzazione online sono in RGB. Se un PDF utilizza entrambi gli spazi colore, potete selezionarne uno specifico scegliendo Forza come RGB oppure Forza come CMYK. Nei PDF possono essere utilizzati entrambi gli spazi colore se, ad esempio, la grafica utilizza uno spazio colore CMYK mentre le immagini utilizzano RGB. Se avete caricato un profilo ICC, il relativo nome viene visualizzato nel menu Spazio colore e lo potete scegliere. 

   Consultate [Profili ICC](icc-profiles.md#icc_profiles).

* **Colore**
ProfiloScegliere un&#39;opzione Profilo colore:

* **Converti in**
SRGBConverts in SRGB (Standard Rosso Verde Blu). sRGB è lo spazio colore consigliato per la visualizzazione delle immagini sulle pagine Web.

* **Mantieni**
spazio colore originaleConserva lo spazio colore originale.

* **Personalizzato da >**
A aperture menu in modo da poter scegliere uno spazio colore Converti da e Converti in. Puoi scegliere uno spazio colore Photoshop standard o uno spazio colore caricato in Dynamic Media Classic.

Consultate [Profili ICC](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>per i dettagli su tutte le opzioni PDF, consultate [Opzioni di caricamento PDF](pdfs.md#pdf_upload_options).
