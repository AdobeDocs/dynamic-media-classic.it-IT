---
title: "Guida introduttiva: nozioni di base sui modelli"
description: Introduzione e Guida rapida alle nozioni di base sui modelli per aiutarti a iniziare rapidamente a utilizzare Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 17%

---

# Avvio rapido: funzioni di base dei modelli{#quick-start-template-basics}

Le nozioni di base sui modelli sono file immagine a livelli dinamici e indirizzabili, come i file a livelli, nelle applicazioni di modifica delle immagini come Adobe Photoshop. Diversamente dai file statici contenenti livelli, come ad esempio un file PSD, un modello può includere dei parametri che consentono di agire su diversi aspetti dell’immagine e personalizzarli.

Un modello può contenere un qualsiasi numero di livelli di immagine e di testo. Potete convertire un file statico contenente livelli, ad esempio un file di PSD con livelli, in un modello e creare modelli in Adobe Dynamic Media Classic. Potete creare livelli di testo nei modelli utilizzando i font caricati in Adobe Dynamic Media Classic. Dopo aver aggiunto il testo a un modello, è possibile formattarlo modificandone la giustificazione, il tipo di carattere, la dimensione e il colore.

La pagina Parametri consente di convertire qualsiasi aspetto di un modello in un parametro indirizzabile. In questo modo, puoi modificare l’immagine a livelli da utilizzare o il valore di testo da utilizzare nel modello. I parametri vengono passati con la stringa URL, consentendo di modificare qualsiasi parametro in modo da personalizzare dinamicamente l’immagine di risposta generata dal server immagini.

Vedi anche il video di formazione [Nozioni di base sui modelli](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

Questa Guida introduttiva è stata progettata per consentirti di iniziare subito a lavorare con le nozioni di base sui modelli.

## 1. Caricare i file

Per iniziare, caricate il file PSD o il file immagine per il modello. Adobe Dynamic Media Classic supporta molti formati di file immagine oltre a PSD, ma per i modelli sono consigliate immagini TIFF e PNG senza perdita di dati, in quanto consentono la trasparenza.

Se si utilizza un file PSD per generare il modello, selezionare **[!UICONTROL Crea modello]** nella finestra di dialogo **[!UICONTROL Opzioni processo di caricamento]** al momento del caricamento del file PSD. Scegli anche un&#39;opzione **[!UICONTROL Denominazione livelli]** in modo che Adobe Dynamic Media Classic sappia come denominare i livelli PSD quando vengono caricati in Adobe Dynamic Media Classic.

Se si utilizzano file di immagine, è possibile ritagliare le immagini e creare una maschera dai tracciati di ritaglio nelle immagini durante il caricamento.

Sulla barra di spostamento globale, selezionare **[!UICONTROL Carica]** per caricare un file PSD o altri file immagine dal computer in una cartella in Adobe Dynamic Media Classic. Consulta [Caricare file modello](uploading-template-files.md#uploading_template_files).

## 2. Creare un modello

Per creare un modello da un file PSD, selezionare **[!UICONTROL Crea modello]** al momento del caricamento del file. Per creare un modello dalle immagini, sulla barra di navigazione globale, vai a **[!UICONTROL Build]** > **[!UICONTROL Nozioni di base sui modelli]**, immetti una misurazione di larghezza e altezza per l&#39;area di lavoro. Nell&#39;angolo superiore destro della pagina selezionare **[!UICONTROL Designer]** o **[!UICONTROL Sviluppatore]** e trascinare le immagini nella pagina Modello. Puoi anche selezionare le immagini *prima* di passare a **[!UICONTROL Build]** > **[!UICONTROL Nozioni di base sui modelli]**. La pagina Modello offre strumenti per:

* Aggiungere dei livelli di immagine. Per aggiungere un livello, trascinate un&#39;immagine nella pagina Modello.
* Aggiungere dei livelli di testo. Seleziona l&#39;icona **[!UICONTROL Strumento di testo]**. Trascinare il puntatore per creare una casella per il livello di testo, quindi formattare il testo con gli strumenti nella pagina Testo.
* Modificare le dimensioni e la posizione dei livelli
* Modificare l’ordine dei livelli
* Applicare un effetto ombra o bagliore ai livelli di immagine e testo

Vedi [Creare un modello](creating-template.md#creating_a_template).

## 3. Creare i parametri del modello

La fase successiva comporta l’impostazione dei parametri per le proprietà dei livelli per determinare quali proprietà includere nella stringa URL. I parametri consentono di usare i modelli con la massima flessibilità. Dopo aver impostato un parametro per una proprietà del livello, potete modificarlo in modo dinamico.

Per parametrizzare un livello, aprire il modello nella pagina Modello, quindi selezionare **[!UICONTROL Parametri]** accanto al nome di un livello. Nella pagina Parametri selezionare l&#39;opzione accanto a ogni parametro che si desidera aggiungere. Consulta [Creare parametri modello](creating-template-parameters.md#creating_template_parameters).

## 4. Modelli Publish

Quando si pubblica un modello, questo viene posizionato su server immagini Dynamic Medie in modo che possa essere distribuito dinamicamente al sito Web o all&#39;applicazione. La pubblicazione attiva inoltre l&#39;URL per chiamare il modello dai server immagini di Dynamic Medie al sito Web o all&#39;applicazione.

Assicuratevi di pubblicare tutte le immagini associate al modello.

Per pubblicare un modello, contrassegnalo per la pubblicazione e sulla barra di navigazione globale, seleziona **[!UICONTROL Publish]**. Quindi selezionare **[!UICONTROL Invia Publish]**. Consulta [Modelli Publish](publishing-templates.md#publishing_templates).

## 5. Collegare un modello a una pagina web

Dynamic Media Classic crea gli URL per i modelli e li attiva quando pubblichi i modelli sui server immagini Dynamic Medie. Puoi copiare queste stringhe URL dalla pagina Anteprima modello.

Seleziona il modello nel pannello Sfoglia, quindi seleziona **[!UICONTROL Anteprima]** per aprire la pagina Anteprima modello. Scegli un predefinito immagine per la distribuzione del modello, quindi fai clic sul pulsante **[!UICONTROL Copia URL]**. Dopo aver copiato l&#39;URL dalla pagina Anteprima, è possibile utilizzarlo nel sito Web o nell&#39;applicazione. Vedere [Collegare un modello a una pagina Web](linking-template-web-page.md#linking_a_template_to_a_web_page).
