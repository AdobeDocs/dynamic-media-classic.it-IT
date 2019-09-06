---
title: '" Avvio rapido: Pubblicazione modelli "'
seo-title: '" Avvio rapido: Pubblicazione modelli "'
description: 'null'
seo-description: Introduzione e Avvio rapido al publishing dei modelli per iniziare a usare rapidamente.
uuid: 101 b 6211-2421-4565-8635-944315 a 5 c 512
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/template-publishing
discoiquuid: 03671 fc 1-ce 3 b -4 fae-ad 1 f -53 c 99 abcabde
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Quick Start: Template publishing{#quick-start-template-publishing}

La funzione Web-stampa di Adobe Dynamic Media Classic consente di creare contenuti per la stampa professionali che i vostri clienti e il vostro staff potranno personalizzare con facilità. Per l’intero processo di pubblicazione potete gestire i contenuti aziendali e l’identità del marchio. Gli utenti finali possono personalizzare il contenuto per la stampa, ma solo la sezione stabilita da voi. Carta da lettere, biglietti da visita, poster, biglietti d’auguri, etichette, scontrini, regali, vestiti, calendari, album e album fotografici sono alcuni esempi di prodotti per la stampa personalizzati che potete distribuire. Le grandi aziende possono rispettare l’identità del loro marchio in tutte le indicazioni, personalizzandole in base alle regioni, alle filiali, ai magazzini e alle succursali.

Potete iniziare a progettare un modello in Adobe Illustrator. Nel modello vengono definiti accuratamente i contenuti costanti e quelli variabili: i componenti variabili sono quelli che è possibile personalizzare. Ad esempio, dopo aver impostato i parametri del testo in un file Illustrator, gli utenti finali possono immettere il testo desiderato. In modo simile, un colore di sfondo dopo essere stato impostato come componente variabile, può essere sostituito con un colore di sfondo differente.

Dynamic Media Classic offre due flussi di lavoro Pubblicazione modelli, uno per casi d'uso di base e uno per scenari avanzati. Gli scenari di base includono la creazione di un progetto in Adobe Illustrator, il caricamento di quest'ultimo in Dynamic Media Classic e la definizione degli elementi variabili con i parametri in SPS. Gli scenari avanzati richiedono una definizione più completa delle variabili. Gli scenari avanzati includono la creazione di elementi variabili in Adobe Illustrator, il caricamento del file in Dynamic Media Classic e la manipolazione direttamente di tali elementi a livello XML con le chiamate URL. Questo scenario viene chiamato *`*DOM manipulation*`*.

>[!NOTE]
>
>For more information about Dynamic Media Classic web-to-print workflows, template creation, parameterization, DOM manipulation, and more, see the Web-to-Print Workflow Guide here: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . Scaricate il file Zip sul disco rigido locale ed estraetene il contenuto (il documento per l'esercitazione Web-stampa Dynamic-To-printworkflow e le risorse per l'esercitazione).

**Avvio rapido**

In questa sezione viene illustrato il flusso di lavoro di base per l’utilizzo dei file Illustrator per creare prodotti per la stampa personalizzabili e di alta qualità.

**1. Progettare un file Illustrator per Pubblicazione modelli**

In Illustrator, progettate il modello. Per usare un metodo di modifica DOM avanzato per la personalizzazione del modello, definite gli ID di elementi s7 per gli elementi variabili in Illustrator.

Consultate [Creare il modello iniziale in Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator) e [Modifica DOM](dom-manipulation.md#dom_manipulation).

**2. Convert your template to Dynamic Media Classic FXG and upload it to Scene7 Publishing System**

Per utilizzare la funzione Web-stampa, gli utenti di Adobe Creative Cloud possono usare il plug-in per Adobe Illustrator. Questo plug-in converte i modelli in FXG Dynamic Media Classic. Se un modello contiene font, i file dei font corrispondenti devono essere caricati in Scene7 Publishing System prima di caricare il file FXG.

Consultate [Caricare i file per Pubblicazione modelli](upload-files-template-publishing.md#upload_files_for_template_publishing).

**3. Visualizzare, definire o perfezionare i parametri in Dynamic Media Classic**

Nelle schermate Anteprima e Genera di Pubblicazione modelli potete definire e perfezionare gli elementi variabili mediante i parametri, la visualizzazione in anteprima e la verifica dei risultati. In queste schermate potete effettuare le seguenti operazioni:

* Creare e modificare i parametri
* Specificare i valori predefiniti per le proprietà e gli attributi dei parametri
* Fare clic su Copia URL per copiare l’URL di anteprima negli Appunti e visualizzare il risultato in anteprima nella finestra Sfoglia

Consultate [Parametrizzazione di un modello in Dynamic Media Classic](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7).

**4. Pubblicare il modello FXG**

Dopo aver definito e verificato i parametri e gli attributi, pubblicate il file. Quando un modello FXG viene pubblicato, viene inserito nei server immagini Dynamic Media e viene attivato l'URL.

Assicuratevi di pubblicare tutte le immagini e i font associati al modello FXG.

Consultate [Pubblicare i modelli FXG](dom-manipulation.md#publish_fxg_templates).

**5. Ottenere l’URL**

Il modello è ora pronto per essere incorporato nel sito Web, mediante il relativo URL, per consentire agli utenti finali di personalizzare il contenuto variabile.

Consultate [Collegamento di un modello FXG a una pagina Web](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page).
