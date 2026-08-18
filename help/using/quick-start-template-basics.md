---
title: 'Avvio rapido: funzioni di base dei modelli'
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
autotag-review: '2026-05-13T20:10:57.394Z'
TQID: 'https://experienceleague.adobe.com/2DaWdJsCz9f5iXEkMi6N1L7s3eFdvpBc1ECrgbVAueo'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 604d547f6867b1a7683f6489555bd5932270d873
workflow-type: tm+mt
source-wordcount: 840
ht-degree: 18%

---

# Avvio rapido: funzioni di base dei modelli{#quick-start-template-basics}

I modelli vengono creati in modo dinamico e possono essere indirizzati come file immagine a più livelli, in modo analogo ai file a più livelli utilizzati nelle applicazioni di modifica delle immagini come Adobe Photoshop. Diversamente dai file statici contenenti livelli, come ad esempio un file PSD, un modello può includere dei parametri che consentono di agire su diversi aspetti dell’immagine e personalizzarli.

Un modello può contenere un qualsiasi numero di livelli di immagine e di testo. Potete convertire un file statico contenente livelli, ad esempio un file PSD con livelli, in un modello e creare modelli in Adobe Dynamic Media Classic. Potete creare livelli di testo nei modelli utilizzando i font caricati in Adobe Dynamic Media Classic. Dopo aver aggiunto il testo a un modello, è possibile formattarlo modificandone la giustificazione, il tipo di carattere, la dimensione e il colore.

La pagina Parametri consente di convertire qualsiasi aspetto di un modello in un parametro indirizzabile. È possibile modificare il valore di testo o immagine a livelli da utilizzare nel modello. I parametri vengono passati con la stringa URL. Questo consente di modificare qualsiasi parametro in modo da personalizzare dinamicamente l&#39;immagine risultante generata dal server immagini.

Vedi anche il video di formazione [Nozioni di base sui modelli](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

Questa Guida introduttiva è stata progettata per aiutarti a iniziare a utilizzare le nozioni di base sui modelli.

## &#x200B;1. Caricare i file

Carica il file PSD o il file immagine per il modello. Adobe Dynamic Media Classic supporta molti formati di file immagine oltre a PSD, ma per i modelli sono consigliate immagini TIFF e PNG senza perdita di dati, in quanto consentono la trasparenza.

Se si utilizza un file PSD per generare il modello, selezionare **[!UICONTROL Crea modello]** nella finestra di dialogo **[!UICONTROL Opzioni processo di caricamento]** al momento del caricamento del file PSD. Scegli anche un&#39;opzione **[!UICONTROL Denominazione livelli]** in modo che Adobe Dynamic Media Classic sappia come denominare i livelli PSD quando vengono caricati in Adobe Dynamic Media Classic.

Se si utilizzano file di immagine, è possibile ritagliare le immagini e creare una maschera dai tracciati di ritaglio nelle immagini durante il caricamento.

Sulla barra di spostamento globale, selezionare **[!UICONTROL Carica]** per caricare un file PSD o altri file immagine dal computer in una cartella in Adobe Dynamic Media Classic. Consulta [Caricare file modello](uploading-template-files.md#uploading_template_files).

## &#x200B;2. Creare un modello

Per creare un modello da un file PSD, selezionare **[!UICONTROL Crea modello]** quando si carica il file. Per creare un modello dalle immagini, sulla barra di navigazione globale vai a **[!UICONTROL Build]** > **[!UICONTROL Nozioni di base sui modelli]**. Immettere la larghezza e l&#39;altezza dell&#39;area di lavoro. Nell&#39;angolo superiore destro della pagina selezionare **[!UICONTROL Designer]** o **[!UICONTROL Sviluppatore]** e trascinare le immagini nella pagina Modello. Puoi anche selezionare le immagini *prima* di passare a **[!UICONTROL Build]** > **[!UICONTROL Nozioni di base sui modelli]**. La pagina Modello offre strumenti per:

* Aggiungere dei livelli di immagine. Per aggiungere un livello, trascinate un&#39;immagine nella pagina Modello.
* Aggiungere dei livelli di testo. Seleziona l&#39;icona **[!UICONTROL Strumento di testo]**. Trascinare il puntatore per creare una casella per il livello di testo, quindi formattare il testo con gli strumenti nella pagina Testo.
* Modificare le dimensioni e la posizione dei livelli
* Modificare l’ordine dei livelli
* Applicare un effetto ombra o bagliore ai livelli di immagine e testo

Vedi [Creare un modello](creating-template.md#creating_a_template).

## &#x200B;3. Creare i parametri per i modelli

La fase successiva comporta l’impostazione dei parametri per le proprietà dei livelli per determinare quali proprietà includere nella stringa URL. I parametri consentono di utilizzare i modelli con maggiore flessibilità. Dopo aver impostato un parametro per una proprietà del livello, potete modificarlo in modo dinamico.

Per parametrizzare un livello, aprire il modello nella pagina Modello, quindi selezionare **[!UICONTROL Parametri]** accanto al nome di un livello. Nella pagina Parametri selezionare l&#39;opzione accanto a ogni parametro che si desidera aggiungere. Consulta [Creare parametri modello](creating-template-parameters.md#creating_template_parameters).

## &#x200B;4. Pubblicare i modelli

Quando si pubblica un modello, questo viene inserito nei server di immagini Dynamic Media e può quindi essere distribuito dinamicamente al sito web o all’applicazione. La pubblicazione attiva anche l’URL per chiamare il modello dai server immagini Dynamic Media al sito web o all’applicazione.

Assicuratevi di pubblicare tutte le immagini associate al modello.

Per pubblicare un modello, contrassegnalo per la pubblicazione e sulla barra di navigazione globale seleziona **[!UICONTROL Pubblica]**. Quindi selezionare **[!UICONTROL Invia pubblicazione]**. Consulta [Modelli di pubblicazione](publishing-templates.md#publishing_templates).

## &#x200B;5. Collegare un modello a una pagina Web

Dynamic Media Classic crea gli URL per i modelli e li attiva quando pubblichi i modelli in Dynamic Media Image Server. Puoi copiare queste stringhe URL dalla pagina Anteprima modello.

Seleziona il modello nel pannello Sfoglia, quindi seleziona **[!UICONTROL Anteprima]** per aprire la pagina Anteprima modello. Scegli un predefinito immagine per la distribuzione del modello, quindi fai clic sul pulsante **[!UICONTROL Copia URL]**. Dopo aver copiato l’URL dalla pagina di anteprima, puoi utilizzarlo nel sito web o nell’applicazione. Consultate [Collegare un modello a una pagina Web](linking-template-web-page.md#linking_a_template_to_a_web_page).
