---
title: Impostazione dei predefiniti per il visualizzatore di eCatalog
description: Scopri come impostare i predefiniti per visualizzatori di eCatalog.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 42%

---

# Impostazione dei predefiniti per il visualizzatore di eCatalog{#setting-up-ecatalog-viewer-presets}

I predefiniti per il visualizzatore di eCatalog determinano lo stile, il comportamento e l’aspetto dei visualizzatori eCatalog. Ad Adobe, Dynamic Media Classic fornisce i predefiniti per visualizzatori di eCatalog ed è possibile creare i propri predefiniti per visualizzatori di eCatalog anche se si è un amministratore.

Per creare un predefinito, puoi iniziare da zero o iniziare con un predefinito per visualizzatori eCatalog fornito da Dynamic Media Classic e salvarlo con un nuovo nome. Potete creare predefiniti per visualizzatore di eCatalog personalizzati per presentare ad esempio il materiale stampato con i colori della vostra azienda.

I predefiniti per visualizzatore di eCatalog offrono diverse impostazioni per passare da una pagina all’altra, effettuare zoom e ricerche e scegliere le interfacce. L’aspetto di questi controlli e l’aspetto del visualizzatore dipendono dalla scelta dei predefiniti per visualizzatori di eCatalog.

Segui questi passaggi per creare un predefinito per visualizzatori di eCatalog (devi essere un amministratore):

1. Nella barra di navigazione globale, fai clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Nella schermata Predefiniti visualizzatori, create un predefinito per visualizzatore di eCatalog iniziando da zero o da un predefinito esistente:

   * **Creazione di un predefinito per visualizzatori di eCatalog**  - Fai clic su  **[!UICONTROL Aggiungi]**. Nella finestra di dialogo Aggiungi predefinito visualizzatore, scegli una piattaforma, scegli Visualizzatore eCatalog, quindi fai clic su **[!UICONTROL Aggiungi]**.

   * **Modifica di un predefinito per visualizzatori di eCatalog** : seleziona un predefinito per visualizzatori di eCatalog, quindi fai clic su  **[!UICONTROL Modifica]**. Fai clic su **[!UICONTROL Salva con nome]** al termine della creazione del predefinito.

1. Nella schermata Configura visualizzatore, inserite un nome per il predefinito del visualizzatore eCatalog.
1. Nella schermata Configura visualizzatore, impostate le opzioni desiderate.

   Fai clic sull&#39;icona **[!UICONTROL Suggerimento]** accanto all&#39;opzione per leggerne la descrizione.

   Nella pagina Anteprima viene visualizzato il visualizzatore durante l’aggiornamento e la modifica delle impostazioni.

1. (Facoltativo) In **[!UICONTROL Impostazioni pannello informazioni]**, l&#39;opzione **[!UICONTROL URL server informazioni]** può includere i seguenti token speciali, che il visualizzatore sostituisce:

   | Token | Sostituito da | Note |
   |--- |--- |--- |
   | `$1$` | valore rollover_key | Identificatore dell&#39;elemento dall&#39;elemento `<area>` della mappa. |
   | `$2$` | frame | Numero di sequenza del fotogramma attualmente visualizzato nel set di immagini. |
   | `$3$` | imageroot | Primo elemento del percorso del primo elemento specificato nel comando dell’immagine (in genere si tratta dell’ID del catalogo di immagini per la voce del catalogo che specifica il set di immagini). |

1. (Facoltativo) Nella casella **[!UICONTROL Impostazioni pannello informazioni]**, digitare il testo che si desidera visualizzare se, ad Adobe, Dynamic Media Classic rileva un errore nel recupero delle informazioni relative a una mappa immagine. **** Ad esempio, se il sistema riceve il nome di una società e il nome di un eCatalog, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.

>[!NOTE]
>
>Per utilizzare questo modello di risposta invece del modello definito nell&#39;eCatalog stesso, aggiungi `fmt=1` alla fine dell&#39;URL del server informazioni. Ad esempio: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Fate clic su **Salva**.
1. Fate clic su Impostazione predefinita se desiderate che il predefinito per visualizzatore di eCatalog creato sia quello usato per visualizzare l’eCatalog sulla pagina Web.

Per eliminare un predefinito per visualizzatori di eCatalog, selezionalo nella schermata Predefiniti visualizzatore e fai clic su **[!UICONTROL Elimina]**.

>[!MORELIKETHIS]
>
>* [Predefiniti per visualizzatori](application-setup.md#viewer_presets)

