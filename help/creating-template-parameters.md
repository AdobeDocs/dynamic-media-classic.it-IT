---
title: Creazione di parametri per i modelli
description: Scopri come creare parametri modello.
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 70%

---

# Creazione di parametri per i modelli{#creating-template-parameters}

I parametri consentono di usare modelli con la massima flessibilità e di personalizzare in modo dinamico un’immagine modello. Potete decidere quali livelli di testo e immagine includere nel modello e, in ciascun livello, quali parametri visualizzare. Ad esempio, per richiamare l’attenzione su un prodotto in offerta, potete creare un livello di testo Offerta speciale. Successivamente, per rimuovere questo livello ma mantenere il resto dell’immagine modello sarà sufficiente rimuovere il parametro Offerta speciale.

Quando create dei parametri per i modelli, dichiarate quali parti del modello richiamare in una stringa URL. Un URL costruito con parametri consente di esporre tali elementi nella stringa URL. Con i parametri esposti, potete creare risultati personalizzati dal modo in cui l’immagine modello viene costruita in modo dinamico dal server immagini. In questo modo, è possibile modificare un modello in modo dinamico poiché potete richiamare alcuni o tutti i suoi parametri in un URL.

Nei parametri del livello di testo, potete anche fare sì che la stringa di testo sia un campo dinamico collegato ai valori in un database. La possibilità di collegare il testo a un database è utile, ad esempio, per gestire le promozioni. Potete personalizzare le immagini modello in modo che contengano i nomi dei clienti. È inoltre possibile collegare un parametro di livello di testo a un database dei prezzi per mostrare il prezzo di un elemento in un&#39;immagine modello.

Potete fare riferimento più volte a uno stesso parametro. Utilizzate la casella combinata per ciascun comando nella finestra di dialogo dei parametri per selezionare un parametro che corrisponda a uno specifico comando. Ad esempio, tutti i parametri di dimensione sono disponibili per il comando `size=` e così via. Potete riassegnare il riferimento del parametro a qualsiasi parametro già presente nella casella combinata e rinominarlo in modo diverso da quanto già elencato. In quest&#39;ultimo caso, il nome deve essere univoco. In caso contrario, viene visualizzato un errore che indica che il parametro esiste. Quando elimini un riferimento a un parametro, questo viene rimosso dall&#39;URL se non viene fatto riferimento in nessun altro punto. Quando modificate il valore predefinito di un parametro di testo, tutti i riferimenti a tale parametro vengono aggiornati. Puoi visualizzare l’aggiornamento nella tabella dei livelli, nel rendering del modello e nell’URL. Quando modificate un attributo di livello manipolando le maniglie di ridimensionamento o digitando valori nel pannello delle proprietà, il valore del parametro viene aggiornato e tutti i riferimenti al parametro vengono aggiornati. Ad esempio, se avete parametrizzato la dimensione di due livelli usando uno stesso parametro e cambiate la dimensione di un livello, vengono aggiornate le dimensioni di entrambi i livelli. Quando visualizzate in anteprima un modello e cambiate un parametro, vengono aggiornati tutti i riferimenti a tale parametro.

## Impostazione di parametri per un livello {#parameterizing-a-layer}

Per ciascun livello nel modello, attenetevi a questa procedura per creare parametri del modello:

1. Nell’elenco Modelli, fate clic sul pulsante Parametri  accanto al nome del livello per il quale desiderate creare dei parametri. Si apre la schermata Parametri. In essa sono elencati i nomi di ciascun parametro applicato al livello, il suo valore e il suo tipo.
1. Selezionate l’opzione Attivato accanto al nome di ciascun parametro da includere nell’immagine modello.
1. Seleziona **[!UICONTROL Chiudi]** per uscire dalla schermata Parametri.

>[!NOTE]
>
>Potete rinominare i parametri nella schermata Parametri, in mod che sia più facile individuarlo nelle stringhe URL e più semplice usarlo come valore del database. Per rinominare un parametro, selezionate la relativa opzione Attivato, fate clic sul suo nome e immettete un nuovo nome nel campo Nome.

Per visualizzare un elenco dei parametri creati per il modello, fate clic sul pulsante Riepilogo parametri nella schermata Modello. Viene visualizzata la schermata Riepilogo parametri. In essa sono elencati i nomi dei vari livelli nonché i nomi e i valori di eventuali parametri.

## Creazione di parametri di testo dinamici {#creating-dynamic-text-parameters}

Per i livelli di testo, è inoltre possibile rendere la stringa di testo un campo dinamico collegato a un valore del database. Effettuate le seguenti operazioni:

1. Nella schermata Modello, fate clic sul pulsante Parametri  accanto al nome del livello di testo per il quale desiderate creare dei parametri di testo dinamici. Viene visualizzata la pagina Parametri .
1. Fare clic sull&#39;opzione **[!UICONTROL On]** accanto al nome dell&#39;attributo di testo (textAttr).
1. Fare clic sulla scheda **[!UICONTROL Testo]** nella schermata Parametri.
1. Fai clic su **[!UICONTROL Aggiungi parametro]**. Viene visualizzato un nome parametro predefinito, che potete sostituire selezionandolo e digitando su di esso. La stringa di testo corrente diventa il nuovo nome del parametro.
1. Fare clic su **[!UICONTROL Chiudi]** per chiudere la pagina Parametri.

Per assegnare al nome del parametro un valore del database, aggiungete la seguente stringa all’URL del modello:

```as3
?$_2(parameter name)=(database value)
```

Il nome del parametro viene sostituito dai nomi in un campo di database o in un codice Java™ che indica, ad esempio, il prezzo corrente di un articolo o di un nome cliente.
