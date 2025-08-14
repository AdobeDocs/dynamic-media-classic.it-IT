---
title: Creare i parametri per i modelli
description: Scopri come creare parametri di modello in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
topic: Development
level: Experienced
source-git-commit: 00591bdbe721035e25d3dea245a2110f978d19aa
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 45%

---

# Creare i parametri per i modelli{#creating-template-parameters}

I parametri consentono di utilizzare i modelli con la massima flessibilità; consentono di personalizzare dinamicamente un’immagine modello. Potete decidere quali livelli di testo e immagine includere nel modello e, in ciascun livello, quali parametri visualizzare. Ad esempio, per attirare l&#39;attenzione su un prodotto in vendita, è possibile creare un livello di testo In vendita. Successivamente, per rimuovere questo livello ma mantenere il resto dell’immagine modello sarà sufficiente rimuovere il parametro Offerta speciale.

Quando create dei parametri per i modelli, dichiarate quali parti del modello richiamare in una stringa URL. Un URL costruito con parametri consente di esporre tali elementi nella stringa URL. Con i parametri esposti, potete creare risultati personalizzati dal modo in cui l’immagine modello viene costruita in modo dinamico dal server immagini. In questo modo, è possibile modificare un modello in modo dinamico poiché potete richiamare alcuni o tutti i suoi parametri in un URL.

Nei parametri del livello di testo, potete anche fare sì che la stringa di testo sia un campo dinamico collegato ai valori in un database. La possibilità di collegare il testo a un database è utile, ad esempio, per gestire le promozioni. Potete personalizzare le immagini modello in modo che contengano i nomi dei clienti. È inoltre possibile collegare un parametro di livello testo a un database dei prezzi per visualizzare il prezzo di un articolo in un&#39;immagine modello.

Potete fare riferimento più volte a uno stesso parametro. Utilizzate la casella combinata per ciascun comando nella finestra di dialogo dei parametri per selezionare un parametro che corrisponda a uno specifico comando. Ad esempio, tutti i parametri di dimensione sono disponibili per il comando `size=`. Potete riassegnare il riferimento del parametro a qualsiasi parametro già presente nella casella combinata e rinominarlo in modo diverso da quanto già elencato. In quest’ultimo caso, il nome deve essere univoco. In caso contrario, viene visualizzato un errore per indicare che il parametro esiste. Quando elimini un riferimento a un parametro, questo viene rimosso dall&#39;URL se non vi è alcun riferimento in nessun altro punto. Quando modificate il valore di default di un parametro di testo, tutti i riferimenti a tale parametro vengono aggiornati. Potete vedere l&#39;aggiornamento nella tabella dei livelli, nel rendering del modello e nell&#39;URL. Quando modificate un attributo di livello modificando i quadratini di ridimensionamento o digitando i valori nel pannello delle proprietà, il valore del parametro viene aggiornato e tutti i riferimenti al parametro vengono aggiornati. Ad esempio, se avete parametrizzato la dimensione di due livelli usando uno stesso parametro e cambiate la dimensione di un livello, vengono aggiornate le dimensioni di entrambi i livelli. Quando visualizzate in anteprima un modello e cambiate un parametro, vengono aggiornati tutti i riferimenti a tale parametro.

Vedi anche il video di formazione [Nozioni di base sui modelli](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

## Parametrizzare un livello {#parameterizing-a-layer}

Per ciascun livello nel modello, attenetevi a questa procedura per creare parametri del modello:

1. Nell&#39;elenco Livelli (Layers), selezionate il pulsante Parametri (Parameters) accanto al nome del livello per il quale desiderate creare i parametri. Si apre la schermata Parametri. Elenca il nome di ciascun parametro sul livello, il relativo valore e il relativo tipo.
1. Selezionare l&#39;opzione Attivato accanto al nome di ogni parametro che si desidera includere nell&#39;immagine modello.
1. Seleziona **[!UICONTROL Chiudi]** per uscire dalla schermata Parametri.

>[!NOTE]
>
>Potete rinominare i parametri nella schermata Parametri, in mod che sia più facile individuarlo nelle stringhe URL e più semplice usarlo come valore del database. Per rinominare un parametro, selezionarne l&#39;opzione **[!UICONTROL Il]**, selezionarne il nome e immettere un nuovo nome nel campo Nome.

Per visualizzare un elenco dei parametri creati per il modello, selezionare il pulsante Riepilogo parametri nella schermata Modello. Nella schermata Riepilogo parametri, viene elencato il nome di ciascun livello e, se avete creato i parametri per un livello, i nomi e i valori dei parametri.

## Creare parametri di testo dinamici {#creating-dynamic-text-parameters}

Per i livelli di testo, potete anche rendere la stringa di testo un campo dinamico collegato a un valore di database. Effettuate le seguenti operazioni:

1. Nella schermata Modello, selezionate il pulsante Parametri accanto al nome del livello di testo per il quale desiderate creare parametri di testo dinamici. Viene visualizzata la pagina Parametri.
1. Selezionare l&#39;opzione **[!UICONTROL On]** accanto al nome dell&#39;attributo di testo (textAttr).
1. Selezionare la scheda **[!UICONTROL Testo]** nella schermata Parametri.
1. Seleziona **[!UICONTROL Aggiungi parametro]**. Viene visualizzato un nome parametro predefinito, che potete sostituire selezionandolo e digitando su di esso. La stringa di testo corrente diventa il nuovo nome del parametro.
1. Seleziona **[!UICONTROL Chiudi]** per chiudere la pagina Parametri.

Per assegnare al nome del parametro un valore del database, aggiungete la seguente stringa all’URL del modello:

```as3
?$_2(parameter name)=(database value)
```

I nomi in un campo di database o in un codice Java™ sostituiscono i nomi dei parametri. Tale funzionalità indica, ad esempio, il prezzo corrente di un articolo o il nome di un cliente.
