---
title: Creare i parametri per i modelli
description: Scopri come creare parametri di modello in Adobe Dynamic Media Classic.
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
topic: Development
level: Experienced
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 54%

---

# Creare i parametri per i modelli{#creating-template-parameters}

I parametri consentono di usare modelli con la massima flessibilità e di personalizzare in modo dinamico un’immagine modello. Potete decidere quali livelli di testo e immagine includere nel modello e, in ciascun livello, quali parametri visualizzare. Ad esempio, per attirare l&#39;attenzione su un prodotto in vendita, è possibile creare un livello di testo In vendita. Successivamente, per rimuovere questo livello ma mantenere il resto dell’immagine modello sarà sufficiente rimuovere il parametro Offerta speciale.

Quando create dei parametri per i modelli, dichiarate quali parti del modello richiamare in una stringa URL. Un URL costruito con parametri consente di esporre tali elementi nella stringa URL. Con i parametri esposti, potete creare risultati personalizzati dal modo in cui l’immagine modello viene costruita in modo dinamico dal server immagini. In questo modo, è possibile modificare un modello in modo dinamico poiché potete richiamare alcuni o tutti i suoi parametri in un URL.

Nei parametri del livello di testo, potete anche fare sì che la stringa di testo sia un campo dinamico collegato ai valori in un database. La possibilità di collegare il testo a un database è utile, ad esempio, per gestire le promozioni. Potete personalizzare le immagini modello in modo che contengano i nomi dei clienti. È inoltre possibile collegare un parametro di livello testo a un database dei prezzi per visualizzare il prezzo di un articolo in un&#39;immagine modello.

Potete fare riferimento più volte a uno stesso parametro. Utilizzate la casella combinata per ciascun comando nella finestra di dialogo dei parametri per selezionare un parametro che corrisponda a uno specifico comando. Ad esempio, tutti i parametri di dimensione sono disponibili per `size=` comando. Potete riassegnare il riferimento del parametro a qualsiasi parametro già presente nella casella combinata e rinominarlo in modo diverso da quanto già elencato. In quest’ultimo caso, il nome deve essere univoco. In caso contrario, viene visualizzato un errore per indicare che il parametro esiste. Quando elimini un riferimento a un parametro, questo viene rimosso dall&#39;URL se non vi è alcun riferimento in nessun altro punto. Quando modificate il valore di default di un parametro di testo, tutti i riferimenti a tale parametro vengono aggiornati. Potete vedere l&#39;aggiornamento nella tabella dei livelli, nel rendering del modello e nell&#39;URL. Quando modificate un attributo di livello modificando i quadratini di ridimensionamento o digitando i valori nel pannello delle proprietà, il valore del parametro viene aggiornato e tutti i riferimenti al parametro vengono aggiornati. Ad esempio, se avete parametrizzato la dimensione di due livelli usando uno stesso parametro e cambiate la dimensione di un livello, vengono aggiornate le dimensioni di entrambi i livelli. Quando visualizzate in anteprima un modello e cambiate un parametro, vengono aggiornati tutti i riferimenti a tale parametro.

Vedi anche [Nozioni di base sui modelli](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) video di formazione.

## Parametrizzare un livello {#parameterizing-a-layer}

Per ciascun livello nel modello, attenetevi a questa procedura per creare parametri del modello:

1. Nell’elenco Modelli, fate clic sul pulsante Parametri  accanto al nome del livello per il quale desiderate creare dei parametri. Si apre la schermata Parametri. In essa sono elencati i nomi di ciascun parametro applicato al livello, il suo valore e il suo tipo.
1. Selezionare l&#39;opzione Attivato accanto al nome di ogni parametro che si desidera includere nell&#39;immagine modello.
1. Seleziona **[!UICONTROL Chiudi]** per uscire dalla schermata Parametri.

>[!NOTE]
>
>Potete rinominare i parametri nella schermata Parametri, in mod che sia più facile individuarlo nelle stringhe URL e più semplice usarlo come valore del database. Per rinominare un parametro, selezionatene uno **[!UICONTROL On]** , selezionarne il nome e immettere un nuovo nome nel campo Nome.

Per visualizzare un elenco dei parametri creati per il modello, selezionare il pulsante Riepilogo parametri nella schermata Modello. Viene visualizzata la schermata Riepilogo parametri. In essa sono elencati i nomi dei vari livelli nonché i nomi e i valori di eventuali parametri.

## Creare parametri di testo dinamici {#creating-dynamic-text-parameters}

Per i livelli di testo, è inoltre possibile rendere la stringa di testo un campo dinamico collegato a un valore di database. Effettuate le seguenti operazioni:

1. Nella schermata Modello, fate clic sul pulsante Parametri  accanto al nome del livello di testo per il quale desiderate creare dei parametri di testo dinamici. Viene visualizzata la pagina Parametri.
1. Seleziona la **[!UICONTROL On]** accanto al nome dell&#39;attributo di testo (textAttr).
1. Seleziona la **[!UICONTROL Testo]** nella schermata Parameters.
1. Seleziona **[!UICONTROL Aggiungi parametro]**. Viene visualizzato un nome parametro predefinito, che potete sostituire selezionandolo e digitando su di esso. La stringa di testo corrente diventa il nuovo nome del parametro.
1. Seleziona **[!UICONTROL Chiudi]** per chiudere la pagina Parametri.

Per assegnare al nome del parametro un valore del database, aggiungete la seguente stringa all’URL del modello:

```as3
?$_2(parameter name)=(database value)
```

Il nome del parametro viene sostituito dai nomi in un campo del database o da un codice Java™ che indica, ad esempio, il prezzo corrente di un articolo o il nome di un cliente.
