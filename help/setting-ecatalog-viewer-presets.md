---
title: Impostazione dei predefiniti per il visualizzatore di eCatalog
description: Scopri come impostare i predefiniti per visualizzatori di eCatalog.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 65%

---


# Impostazione dei predefiniti per il visualizzatore di eCatalog{#setting-up-ecatalog-viewer-presets}

I predefiniti per il visualizzatore di eCatalog determinano lo stile, il comportamento e l’aspetto dei visualizzatori eCatalog. Dynamic Media Classic fornisce i predefiniti per visualizzatori di eCatalog ed è possibile creare i propri predefiniti per visualizzatori di eCatalog anche se si è un amministratore.

Per creare un nuovo predefinito, puoi iniziare da zero o iniziare con un predefinito per visualizzatori eCatalog fornito da Dynamic Media Classic e salvarlo con un nuovo nome. Potete creare predefiniti per visualizzatore di eCatalog personalizzati per presentare ad esempio il materiale stampato con i colori della vostra azienda.

I predefiniti per visualizzatore di eCatalog offrono diverse impostazioni per passare da una pagina all’altra, effettuare zoom e ricerche e scegliere le interfacce. L’aspetto di questi controlli e del visualizzatore dipende dalla scelta del predefinito per il visualizzatore di eCatalog.

Per creare un predefinito per visualizzatore di eCatalog, effettuate le operazioni seguenti (è necessario essere un amministratore):

1. Fate clic su **Configurazione** > **Predefiniti visualizzatore**.
1. Nella schermata Predefiniti visualizzatori, create un predefinito per visualizzatore di eCatalog iniziando da zero o da un predefinito esistente:

   * **Creazione di un visualizzatore di eCatalog**
PresetClick Aggiungi. Nella finestra di dialogo Aggiungi predefinito visualizzatore, scegli una piattaforma, scegli Visualizzatore eCatalog, quindi fai clic su 
**Aggiungi**.

   * **Modifica di un**
predefinito per visualizzatori di eCatalogSeleziona un predefinito per visualizzatori di eCatalog, quindi fai clic su Modifica. Clic 
**Salva** dopo aver completato la creazione del predefinito.

1. Nella schermata Configura visualizzatore, inserite un nome per il predefinito del visualizzatore eCatalog.
1. Nella schermata Configura visualizzatore, impostate le opzioni desiderate.

   Fate clic sull’icona dei suggerimenti  accanto all’opzione per visualizzarne la descrizione.

   Nella schermata di anteprima viene riportato il visualizzatore con le impostazioni aggiornate e modificate.

1. (Facoltativo) Nelle impostazioni del Pannello Info, l’opzione URL server informazioni può includere i seguenti token specifici, che vengono sostituiti dal visualizzatore:

   | Token | Sostituito da | Note |
   |--- |--- |--- |
   | `$1$` | valore rollover_key | Identificatore dell&#39;elemento dall&#39;elemento `<area>` della mappa. |
   | `$2$` | frame | Numero di sequenza del fotogramma attualmente visualizzato nel set di immagini. |
   | `$3$` | imageroot | Primo elemento del percorso del primo elemento specificato nel comando dell’immagine (in genere si tratta dell’ID del catalogo di immagini per la voce del catalogo che specifica il set di immagini). |

1. (Facoltativo) Nella casella Modello di risposta della casella Impostazioni pannello informazioni digitare il testo che si desidera visualizzare se Dynamic Media Classic rileva un errore nel recupero delle informazioni per una mappa immagine. Ad esempio, se il sistema riceve il nome di una società e il nome di un eCatalog, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.

>[!NOTE]
>
>per usare questo Modello di risposta invece del modello definito nell’eCatalog stesso, aggiungete“fmt=1” alla fine dell’URL server informazioni. Ad esempio: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Fate clic su **Salva**.
1. Fate clic su Impostazione predefinita se desiderate che il predefinito per visualizzatore di eCatalog creato sia quello usato per visualizzare l’eCatalog sulla pagina Web.

Per eliminare un predefinito per visualizzatori di eCatalog, selezionalo nella schermata Predefiniti visualizzatore e fai clic su **Elimina**.

>[!MORELIKETHIS]
>
>* [Predefiniti per visualizzatori](application-setup.md#viewer_presets)

