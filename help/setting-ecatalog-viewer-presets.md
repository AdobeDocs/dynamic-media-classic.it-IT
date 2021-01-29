---
title: Impostazione dei predefiniti per il visualizzatore di eCatalog
description: Scoprite come impostare i predefiniti per visualizzatori di eCatalog.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 66%

---


# Impostazione dei predefiniti per il visualizzatore di eCatalog{#setting-up-ecatalog-viewer-presets}

I predefiniti per il visualizzatore di eCatalog determinano lo stile, il comportamento e l’aspetto dei visualizzatori eCatalog. Dynamic Media Classic fornisce predefiniti per visualizzatori di eCatalog e gli amministratori possono creare nuovi predefiniti per visualizzatori di eCatalog.

Per creare un nuovo predefinito, potete partire da zero o iniziare da un predefinito per visualizzatore di eCatalog fornito da Dynamic Media Classic e salvarlo con un nuovo nome. Potete creare predefiniti per visualizzatore di eCatalog personalizzati per presentare ad esempio il materiale stampato con i colori della vostra azienda.

I predefiniti per visualizzatore di eCatalog offrono diverse impostazioni per passare da una pagina all’altra, effettuare zoom e ricerche e scegliere le interfacce. L’aspetto di questi controlli e del visualizzatore dipende dalla scelta del predefinito per il visualizzatore di eCatalog.

Per creare un predefinito per visualizzatore di eCatalog, effettuate le operazioni seguenti (è necessario essere un amministratore):

1. Fate clic su **Configurazione** > **Predefiniti visualizzatore**.
1. Nella schermata Predefiniti visualizzatori, create un predefinito per visualizzatore di eCatalog iniziando da zero o da un predefinito esistente:

   * **Creazione di un**
predefinito per visualizzatore di eCatalogFate clic su Aggiungi. Nella finestra di dialogo Aggiungi predefinito per visualizzatore, scegliete una piattaforma, selezionate Visualizzatore eCatalog e fate clic su 
**Aggiungi**.

   * **Modifica di un**
predefinito per visualizzatori di eCatalogSelezionate un predefinito per visualizzatori di eCatalog, quindi fate clic su Modifica. Clic 
**Dopo aver** completato la creazione del predefinito, salvate Asas.

1. Nella schermata Configura visualizzatore, inserite un nome per il predefinito del visualizzatore eCatalog.
1. Nella schermata Configura visualizzatore, impostate le opzioni desiderate.

   Fate clic sull’icona dei suggerimenti  accanto all’opzione per visualizzarne la descrizione.

   Nella schermata di anteprima viene riportato il visualizzatore con le impostazioni aggiornate e modificate.

1. (Facoltativo) Nelle impostazioni del Pannello Info, l’opzione URL server informazioni può includere i seguenti token specifici, che vengono sostituiti dal visualizzatore:

   | Token | Sostituito da | Note |
   |--- |--- |--- |
   | `$1$` | valore rollover_key | Identificatore elemento dall&#39;elemento `<area>` della mappa. |
   | `$2$` | frame | Numero di sequenza del fotogramma attualmente visualizzato nel set di immagini. |
   | `$3$` | imageroot | Primo elemento del percorso del primo elemento specificato nel comando dell’immagine (in genere si tratta dell’ID del catalogo di immagini per la voce del catalogo che specifica il set di immagini). |

1. (Facoltativo) Nelle Impostazioni pannello Info, nella casella Modello di risposta, digitate il testo da visualizzare se Dynamic Media Classic rileva un errore nel recupero delle informazioni per una mappa immagine. Ad esempio, se il sistema riceve il nome di una società e il nome di un eCatalog, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.

>[!NOTE]
>
>per usare questo Modello di risposta invece del modello definito nell’eCatalog stesso, aggiungete“fmt=1” alla fine dell’URL server informazioni. Ad esempio: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Fate clic su **Salva**.
1. Fate clic su Impostazione predefinita se desiderate che il predefinito per visualizzatore di eCatalog creato sia quello usato per visualizzare l’eCatalog sulla pagina Web.

Per eliminare un predefinito per visualizzatori di eCatalog, selezionatelo nella schermata Predefiniti visualizzatore e fate clic su **Elimina**.

>[!MORELIKETHIS]
>
>* [Predefiniti per visualizzatori](application-setup.md#viewer_presets)

