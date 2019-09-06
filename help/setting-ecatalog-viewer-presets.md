---
title: Impostazione dei predefiniti per il visualizzatore di eCatalog
seo-title: Impostazione dei predefiniti per il visualizzatore di eCatalog
description: 'null'
seo-description: Scoprite come impostare predefiniti per visualizzatore di ecatalog.
uuid: aca 66 bc 5-8491-4 d 81-9 a 06-1 d 3531860 a 14
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 6 c 123 f 85-3 bc 4-4392-a 7 fb -55618127 c 65 e
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Impostazione dei predefiniti per il visualizzatore di eCatalog{#setting-up-ecatalog-viewer-presets}

I predefiniti per il visualizzatore di eCatalog determinano lo stile, il comportamento e l’aspetto dei visualizzatori eCatalog. Dynamic Media Classic fornisce predefiniti per visualizzatore ecatalog e potete creare anche i predefiniti per visualizzatore di ecatalog.

Per creare un nuovo predefinito, potete partire da zero o iniziare con un predefinito per visualizzatore di ecatalog fornito da Dynamic Media Classic e salvarlo con un nuovo nome. Potete creare predefiniti per visualizzatore di eCatalog personalizzati per presentare ad esempio il materiale stampato con i colori della vostra azienda.

I predefiniti per visualizzatore di eCatalog offrono diverse impostazioni per passare da una pagina all’altra, effettuare zoom e ricerche e scegliere le interfacce. L’aspetto di questi controlli e del visualizzatore dipende dalla scelta del predefinito per il visualizzatore di eCatalog.

Per creare un predefinito per visualizzatore di eCatalog, effettuate le operazioni seguenti (è necessario essere un amministratore):

1. Fate clic su **Configurazione** &gt; **Predefiniti visualizzatore**.
1. Nella schermata Predefiniti visualizzatori, create un predefinito per visualizzatore di eCatalog iniziando da zero o da un predefinito esistente:

   **Creazione di un predefinito** per visualizzatore di ecatalog. In the Add Viewer Preset dialog box, choose a platform, choose eCatalog Viewer, then click **Add**.

   **Modifica di un predefinito per visualizzatore di ecatalog** Selezionate un predefinito per visualizzatore ecatalog, quindi fate clic su Modifica. Click **Save As** after you finish creating the preset.

1. Nella schermata Configura visualizzatore, inserite un nome per il predefinito del visualizzatore eCatalog.
1. Nella schermata Configura visualizzatore, impostate le opzioni desiderate.

   Fate clic sull’icona dei suggerimenti  accanto all’opzione per visualizzarne la descrizione.

   Nella schermata di anteprima viene riportato il visualizzatore con le impostazioni aggiornate e modificate.

1. (Facoltativo) Nelle impostazioni del Pannello Info, l’opzione URL server informazioni può includere i seguenti token specifici, che vengono sostituiti dal visualizzatore:

   | Token | Sostituito da | Note |
   |--- |--- |--- |
   | `$1$` | valore rollover_key | The item identifier from the `<area>` element of the map. |
   | `$2$` | frame | Numero di sequenza del fotogramma attualmente visualizzato nel set di immagini. |
   | `$3$` | imageroot | Primo elemento del percorso del primo elemento specificato nel comando dell’immagine (in genere si tratta dell’ID del catalogo di immagini per la voce del catalogo che specifica il set di immagini). |

1. (Facoltativo) Nella casella Impostazioni pannello Info, digitate il testo da visualizzare se Dynamic Media Classic restituisce un errore durante il recupero delle informazioni per una mappa immagine. Ad esempio, se il sistema riceve il nome di una società e il nome di un eCatalog, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.

>[!NOTE]
>
>per usare questo Modello di risposta invece del modello definito nell’eCatalog stesso, aggiungete“fmt=1” alla fine dell’URL server informazioni. Ad esempio: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Fate clic su **Salva**.
1. Fate clic su Impostazione predefinita se desiderate che il predefinito per visualizzatore di eCatalog creato sia quello usato per visualizzare l’eCatalog sulla pagina Web.

To delete an eCatalog Viewer Preset, select it on the Viewer Presets screen and click **Delete**.

>[!MORELIKETHIS]
>
>* [Predefiniti per visualizzatori](application-setup.md#viewer_presets)

