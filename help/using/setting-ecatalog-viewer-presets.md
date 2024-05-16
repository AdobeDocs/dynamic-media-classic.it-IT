---
title: Impostazione dei predefiniti per il visualizzatore eCatalog
description: Scopri come impostare i predefiniti per visualizzatori eCatalog in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 25%

---

# Impostazione dei predefiniti per il visualizzatore eCatalog{#setting-up-ecatalog-viewer-presets}

I predefiniti per il visualizzatore di eCatalog determinano lo stile, il comportamento e l’aspetto dei visualizzatori eCatalog. In Adobe Dynamic Media Classic sono disponibili i predefiniti per visualizzatori eCatalog ed è possibile creare predefiniti per visualizzatori eCatalog personalizzati anche se si è un amministratore.

Per creare un predefinito, puoi iniziare da zero o iniziare con un predefinito per visualizzatori eCatalog fornito da Adobe Dynamic Media Classic e salvarlo con un nuovo nome. Potete creare predefiniti per visualizzatore di eCatalog personalizzati per presentare ad esempio il materiale stampato con i colori della vostra azienda.

I predefiniti per visualizzatori eCatalog offrono molte impostazioni per passare da una pagina all&#39;altra, ingrandire, cercare e scegliere gli skin. L&#39;aspetto di questi controlli e la modalità di visualizzazione del visualizzatore dipendono dalla scelta dei predefiniti del visualizzatore eCatalog.

Segui questi passaggi per creare un predefinito per visualizzatori eCatalog (devi essere un amministratore):

1. Sulla barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Nella schermata Predefiniti visualizzatori, create un predefinito per visualizzatore di eCatalog iniziando da zero o da un predefinito esistente:

   * **Creare un predefinito per visualizzatori eCatalog**: Seleziona **[!UICONTROL Aggiungi]**. Nella finestra di dialogo Aggiungi predefinito visualizzatore, scegli una piattaforma, scegli Visualizzatore eCatalog, quindi seleziona **[!UICONTROL Aggiungi]**.

   * **Modificare un predefinito per visualizzatori eCatalog**: seleziona un predefinito per visualizzatori eCatalog, quindi fai clic su **[!UICONTROL Modifica]**. Seleziona **[!UICONTROL Salva con nome]** dopo aver completato la creazione del predefinito.

1. Il giorno `Configure Viewer` , immetti un nome per il predefinito visualizzatore eCatalog.
1. Il giorno `Configure Viewer` , impostare le opzioni desiderate.

   seleziona la **[!UICONTROL Suggerimento]** accanto all’opzione se desideri leggerne la descrizione.

   Nella pagina Anteprima viene visualizzato il visualizzatore durante l&#39;aggiornamento e la modifica delle impostazioni.

1. (Facoltativo) In **[!UICONTROL Impostazioni pannello Info]**, il **[!UICONTROL URL server informazioni]** L&#39;opzione può includere i seguenti token speciali, che il visualizzatore sostituisce:

   | Token | Sostituito da | Note |
   | --- | --- | --- |
   | `$1$` | valore rollover_key | L’identificatore dell’elemento da `<area>` elemento della mappa. |
   | `$2$` | frame | Numero di sequenza del fotogramma attualmente visualizzato nel set di immagini. |
   | `$3$` | root immagine | Primo elemento del percorso del primo elemento specificato nel comando dell’immagine (in genere si tratta dell’ID del catalogo di immagini per la voce del catalogo che specifica il set di immagini). |

1. (Facoltativo) In **[!UICONTROL Impostazioni pannello Info]**, nella **[!UICONTROL Modello di risposta]** digitare il testo che si desidera visualizzare se in Adobe Dynamic Media Classic viene rilevato un errore durante il recupero delle informazioni per una mappa immagine. Ad esempio, se il sistema riceve il nome di una società e il nome di un eCatalog, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.

>[!NOTE]
>
>Per utilizzare questo modello di risposta invece del modello definito nell&#39;eCatalog stesso, aggiungere `fmt=1` alla fine dell’URL del server informazioni. Ad esempio: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Seleziona **[!UICONTROL Salva]**.
1. Seleziona **[!UICONTROL Predefinito]** in modo che il predefinito visualizzatore eCatalog creato sia quello utilizzato per visualizzare gli eCatalog nella pagina Web.

Per eliminare un predefinito visualizzatore eCatalog, selezionatelo nella schermata Predefiniti visualizzatore e selezionate **[!UICONTROL Elimina]**.

>[!MORELIKETHIS]
>
>* [Predefiniti per visualizzatori](application-setup.md#viewer_presets)
