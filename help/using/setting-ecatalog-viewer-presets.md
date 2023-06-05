---
title: Impostazione dei predefiniti per il visualizzatore eCatalog
description: Scopri come impostare i predefiniti per visualizzatori eCatalog in Adobe Dynamic Media Classic.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 34%

---

# Impostazione dei predefiniti per il visualizzatore eCatalog{#setting-up-ecatalog-viewer-presets}

I predefiniti per il visualizzatore di eCatalog determinano lo stile, il comportamento e l’aspetto dei visualizzatori eCatalog. In Adobe Dynamic Media Classic sono disponibili i predefiniti per visualizzatori eCatalog ed è possibile creare predefiniti per visualizzatori eCatalog personalizzati anche se si è un amministratore.

Per creare un predefinito, puoi iniziare da zero o iniziare con un predefinito per visualizzatori eCatalog fornito da Adobe Dynamic Media Classic e salvarlo con un nuovo nome. Potete creare predefiniti per visualizzatore di eCatalog personalizzati per presentare ad esempio il materiale stampato con i colori della vostra azienda.

I predefiniti per visualizzatore di eCatalog offrono diverse impostazioni per passare da una pagina all’altra, effettuare zoom e ricerche e scegliere le interfacce. L&#39;aspetto di questi controlli e la modalità di visualizzazione del visualizzatore dipendono dalla scelta dei predefiniti del visualizzatore eCatalog.

Segui questi passaggi per creare un predefinito per visualizzatori eCatalog (devi essere un amministratore):

1. Sulla barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Nella schermata Predefiniti visualizzatori, create un predefinito per visualizzatore di eCatalog iniziando da zero o da un predefinito esistente:

   * **Creare un predefinito per visualizzatori eCatalog** - Seleziona **[!UICONTROL Aggiungi]**. Nella finestra di dialogo Aggiungi predefinito visualizzatore, scegli una piattaforma, scegli Visualizzatore eCatalog, quindi seleziona **[!UICONTROL Aggiungi]**.

   * **Modificare un predefinito per visualizzatori eCatalog** - Selezionate un predefinito per visualizzatori eCatalog, quindi selezionate **[!UICONTROL Modifica]**. Seleziona **[!UICONTROL Salva con nome]** dopo aver completato la creazione del predefinito.

1. Nella schermata Configura visualizzatore, inserite un nome per il predefinito del visualizzatore eCatalog.
1. Nella schermata Configura visualizzatore, impostate le opzioni desiderate.

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
1. Seleziona **[!UICONTROL Predefinito]** se desideri che il predefinito per visualizzatori eCatalog creato sia quello utilizzato per visualizzare gli eCatalog nella pagina web.

Per eliminare un predefinito visualizzatore eCatalog, selezionatelo nella schermata Predefiniti visualizzatore e selezionate **[!UICONTROL Elimina]**.

>[!MORELIKETHIS]
>
>* [Predefiniti per visualizzatori](application-setup.md#viewer_presets)

