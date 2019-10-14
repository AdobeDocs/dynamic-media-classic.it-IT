---
title: '"Avvio rapido: funzioni di base dei modelli"'
seo-title: '"Avvio rapido: funzioni di base dei modelli"'
description: 'null'
seo-description: Introduzione e Introduzione rapida ai modelli di base per imparare a usare rapidamente i modelli.
uuid: 16 d 78 cbb-f 762-4263-aea 9-5712 eb 933693
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/template_ basics
discoiquuid: dd 0 fbb 39-3 f 6 a -496 b-a 9 b 6-63 b 11 dcb 823 a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Avvio rapido: funzioni di base dei modelli{#quick-start-template-basics}

Le funzioni di base dei modelli sono file di immagini con più livelli creati in modo dinamico e indirizzabili come file con più livelli nelle applicazioni di elaborazione delle immagini come Adobe Photoshop. Diversamente dai file statici contenenti livelli, come ad esempio un file PSD, un modello può includere dei parametri che consentono di agire su diversi aspetti dell’immagine e personalizzarli.

>[!NOTE]
>
>Potete anche creare modelli da layout con Pubblicazione modelli e file da Adobe Illustrator e Adobe indesign. Consultate [Pubblicazione modelli ](quick-start-template-publishing.md).

Un modello può contenere un qualsiasi numero di livelli di immagine e di testo. Potete convertire un file statico contenente livelli, ad esempio un file PSD con più livelli, in un modello, nonché creare modelli in Dynamic Media Classic. Per creare dei livelli di testo nei modelli vengono usati i font caricati in SPS. Dopo aver aggiunto del testo a un modello, potete formattarlo modificandone giustificazione, font, dimensioni font e colore.

Tramite la schermata Parametri, potete convertire qualsiasi aspetto di un modello in un parametro indirizzabile. Questo consente di scegliere l’immagine a livelli o il valore di testo da usare nel modello. I parametri vengono trasmessi con la stringa URL e possono essere modificati per personalizzare in modo dinamico l’immagine di risposta generata dal server immagini.

**Avvio rapido**

Questa sezione è stata progettata per imparare a usare rapidamente i modelli di tipo Funzioni di base dei modelli.

**1. Caricare i file**

Per iniziare, caricate il file PSD o il file immagine per il modello. Dynamic Media Classic supporta molti formati di file immagine oltre a PSD, ma per i modelli si consiglia di usare immagini senza perdita di dati TIFF e PNG, poiché consentono la trasparenza.

Se generate il modello a partire da un file PSD, quando caricate il file PSD selezionate l’opzione Crea modello nella finestra di dialogo Opzioni processo di caricamento. Scegliete anche un'opzione Denominazione livelli per indicare a Dynamic Media Classic come denominare i livelli PSD quando questi vengono caricati in Scene 7 Publishing System.

Se utilizzate dei file immagine, al momento del caricamento potete ritagliare le immagini e creare una maschera dai tracciati di ritaglio presenti nelle immagini.

Per caricare un file PSD o un altro file immagine dal computer a una cartella di SPS, fate clic sul pulsante Carica nella Barra di navigazione globale. Consultate [Caricamento dei file modello](uploading-template-files.md#uploading_template_files)

**2. Creare un modello**

Per creare un modello da un file PSD, quando caricate il file selezionate l’opzione Crea modello. Per creare un modello da immagini, scegliete Genera &gt; Funzioni di base dei modelli, immettete le misure di larghezza e altezza per il quadro, selezionate Designer o Sviluppatore e trascinate le immagini nella schermata Modello. Potete anche selezionare le immagini prima di scegliere Genera &gt; Funzioni di base dei modelli. La schermata Modello offre gli strumenti per effettuare le seguenti operazioni:

* Aggiungere dei livelli di immagine. Per aggiungere un livello, trascinate un’immagine nella schermata Modello.
* Aggiungere dei livelli di testo. Selezionate lo strumento testo  e trascinate per disegnare una casella per il livello di testo; quindi formattate il testo con gli strumenti nella schermata Testo.
* Modificare le dimensioni e la posizione dei livelli
* Modificare l’ordine dei livelli
* Applicare un effetto ombra o bagliore ai livelli di immagine e testo

Consultate [Creazione di un modello](creating-template.md#creating_a_template).

**3. Creare i parametri per i modelli**

La fase successiva comporta l’impostazione dei parametri per le proprietà dei livelli per determinare quali proprietà includere nella stringa URL. I parametri consentono di usare i modelli con la massima flessibilità. Dopo aver impostato un parametro per una proprietà del livello, potete modificarlo in modo dinamico.

Per impostare parametri per un livello, aprite il modello nella schermata Modello e fate clic sul pulsante Parametri accanto al nome del livello. Nella schermata Parametri, selezionate l’opzione accanto a ciascun parametro da aggiungere. Consultate [Creazione di parametri per i modelli](creating-template-parameters.md#creating_template_parameters).

**4. Pubblicare i modelli**

Quando un modello viene pubblicato, viene inserito sui server immagini contenuti multimediali dinamici in modo che possa essere trasmesso in modo dinamico al sito Web o all'applicazione in cui deve essere visualizzato. La pubblicazione attiva inoltre l'URL per richiamare il modello dai server immagini Dynamic Media al sito Web o all'applicazione.

Assicuratevi di pubblicare tutte le immagini associate al modello.

Per pubblicare un modello, contrassegnatelo per la pubblicazione e fate clic sul pulsante Pubblica sulla barra Navigazione globale. Quindi fate clic sul pulsante Avvia pubblicazione. Consultate [Pubblicazione dei modelli](publishing-templates.md#publishing_templates).

**5. Collegare un modello a una pagina Web**

Dynamic Media Classic crea URL per i modelli e attiva gli URL quando pubblicate modelli su server immagini Dynamic Media. Potete copiare le stringhe URL dalla schermata Anteprima modello.

Selezionate il modello nel pannello Sfoglia e fate clic sul pulsante Anteprima per aprire la schermata Anteprima modello. Quindi scegliete un Predefinito immagine per la trasmissione del modello e fate clic sul pulsante Copia URL. Dopo aver copiato l’URL dalla schermata Anteprima, potete usarlo nel sito Web o nell’applicazione. Consultate [Collegamento di un modello a una pagina Web](linking-template-web-page.md#linking_a_template_to_a_web_page).