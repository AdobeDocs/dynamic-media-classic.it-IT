---
title: '"Avvio rapido: funzioni di base dei modelli"'
description: Introduzione e nozioni di base sui modelli per un rapido utilizzo.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 34%

---

# Avvio rapido: funzioni di base dei modelli{#quick-start-template-basics}

I modelli di base vengono creati in modo dinamico e indirizzabili file di immagini a più livelli, come file a più livelli in applicazioni di modifica delle immagini come Adobe Photoshop. Diversamente dai file statici contenenti livelli, come ad esempio un file PSD, un modello può includere dei parametri che consentono di agire su diversi aspetti dell’immagine e personalizzarli.

Un modello può contenere un qualsiasi numero di livelli di immagine e di testo. È possibile convertire un file statico contenente livelli, ad esempio un file PSD a livelli, in un modello e creare modelli in Dynamic Media Classic. È possibile creare livelli di testo nei modelli utilizzando i font caricati in Dynamic Media Classic. Dopo aver aggiunto del testo a un modello, potete formattarlo modificandone giustificazione, font, dimensioni font e colore.

La pagina Parametri consente di convertire qualsiasi aspetto di un modello in un parametro indirizzabile. Questo consente di scegliere l’immagine a livelli o il valore di testo da usare nel modello. I parametri vengono trasmessi con la stringa URL e possono essere modificati per personalizzare in modo dinamico l’immagine di risposta generata dal server immagini.

Questa sezione è stata progettata per imparare a usare rapidamente i modelli di tipo Funzioni di base dei modelli.

## 1. Carica i file

Per iniziare, caricate il file PSD o il file immagine per il modello. Dynamic Media Classic supporta molti formati di file immagine oltre a PSD, ma le immagini TIFF e PNG senza perdita sono consigliate per i modelli perché consentono la trasparenza.

Se utilizzi un file PSD per generare il modello, seleziona **[!UICONTROL Crea modello]** nella finestra di dialogo **[!UICONTROL Opzioni processo di caricamento]** quando carichi il file PSD. Scegli anche un&#39;opzione **[!UICONTROL Denominazione livello]** in modo che Dynamic Media Classic sappia come denominare i livelli PSD quando vengono caricati in Dynamic Media Classic.

Se utilizzate dei file immagine, al momento del caricamento potete ritagliare le immagini e creare una maschera dai tracciati di ritaglio presenti nelle immagini.

Nella barra di navigazione globale, fai clic su **[!UICONTROL Carica]** per caricare un file PSD o altri file di immagine dal computer in una cartella in Dynamic Media Classic. Consultate [Caricamento dei file modello](uploading-template-files.md#uploading_template_files)

## 2. Creare un modello

Per creare un modello da un file PSD, seleziona **[!UICONTROL Crea modello]** quando carichi il file. Per creare un modello dalle immagini, nella barra di navigazione globale fai clic su **[!UICONTROL Genera]** > **[!UICONTROL Nozioni di base sui modelli]**, immetti una misura di larghezza e altezza per l’area di lavoro. Nell’angolo in alto a destra della pagina, seleziona **[!UICONTROL Designer]** o **[!UICONTROL Sviluppatore]** e trascina le immagini nella pagina Modello. È inoltre possibile selezionare le immagini *prima* facendo clic su **[!UICONTROL Genera]** > **[!UICONTROL Nozioni di base sui modelli]**. La pagina Modello offre gli strumenti per:

* Aggiungere dei livelli di immagine. Per aggiungere un livello, trascinate un’immagine nella pagina Modello.
* Aggiungere dei livelli di testo. Fare clic sull&#39;icona **[!UICONTROL Strumento testo]**. Trascinare il puntatore per creare una casella per il livello di testo; quindi formattare il testo con gli strumenti nella pagina Testo .
* Modificare le dimensioni e la posizione dei livelli
* Modificare l’ordine dei livelli
* Applicare un effetto ombra o bagliore ai livelli di immagine e testo

Consultate [Creazione di un modello](creating-template.md#creating_a_template).

## 3. Creare parametri modello

La fase successiva comporta l’impostazione dei parametri per le proprietà dei livelli per determinare quali proprietà includere nella stringa URL. I parametri consentono di usare i modelli con la massima flessibilità. Dopo aver impostato un parametro per una proprietà del livello, potete modificarlo in modo dinamico.

Per parametrizzare un livello, apri il modello nella pagina Modello, quindi fai clic su **[!UICONTROL Parametri]** accanto al nome di un livello. Nella pagina Parametri , seleziona l’opzione accanto a ciascun parametro da aggiungere. Consultate [Creazione di parametri per i modelli](creating-template-parameters.md#creating_template_parameters).

## 4. Pubblicare modelli

Quando si pubblica un modello, questo viene inserito sui server di immagini Dynamic Media in modo che possa essere distribuito in modo dinamico al sito Web o all’applicazione. La pubblicazione attiva anche l’URL per chiamare il modello dai server immagini Dynamic Media al sito Web o all’applicazione.

Assicuratevi di pubblicare tutte le immagini associate al modello.

Per pubblicare un modello, contrassegnalo per la pubblicazione e nella barra di navigazione globale fai clic su **[!UICONTROL Pubblica]**. Quindi fai clic su **[!UICONTROL Invia pubblicazione]**. Consultate [Pubblicazione dei modelli](publishing-templates.md#publishing_templates).

## 5. Collegare un modello a una pagina web

Dynamic Media Classic crea gli URL per i modelli e li attiva quando i modelli vengono pubblicati sui server di immagini Dynamic Media. Puoi copiare queste stringhe URL dalla pagina Anteprima modello.

Seleziona il modello nel pannello Sfoglia, quindi fai clic su **[!UICONTROL Anteprima]** per aprire la pagina Anteprima modello. Scegli un predefinito per immagini per la consegna del modello, quindi fai clic su **[!UICONTROL Copia URL]**. Dopo aver copiato l’URL dalla pagina Anteprima, puoi utilizzarlo nel sito Web o nell’applicazione. Consultate [Collegamento di un modello a una pagina Web](linking-template-web-page.md#linking_a_template_to_a_web_page).
