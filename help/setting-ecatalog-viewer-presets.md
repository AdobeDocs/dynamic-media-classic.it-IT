---
title: Configurare i predefiniti per visualizzatori di eCatalog
description: Scopri come configurare i predefiniti per visualizzatori di eCatalog in Adobe Dynamic Media Classic.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 34%

---

# Configurare i predefiniti per visualizzatori di eCatalog{#setting-up-ecatalog-viewer-presets}

I predefiniti per il visualizzatore di eCatalog determinano lo stile, il comportamento e l’aspetto dei visualizzatori eCatalog. Adobe Dynamic Media Classic fornisce predefiniti per visualizzatori di eCatalog ed è possibile creare predefiniti per visualizzatori di eCatalog personalizzati anche se si è un amministratore.

Per creare un predefinito, puoi iniziare da zero o iniziare con un predefinito per visualizzatori eCatalog fornito da Adobe Dynamic Media Classic e salvarlo con un nuovo nome. Potete creare predefiniti per visualizzatore di eCatalog personalizzati per presentare ad esempio il materiale stampato con i colori della vostra azienda.

I predefiniti per visualizzatore di eCatalog offrono diverse impostazioni per passare da una pagina all’altra, effettuare zoom e ricerche e scegliere le interfacce. L’aspetto di questi controlli e l’aspetto del visualizzatore dipendono dalla scelta dei predefiniti per visualizzatori di eCatalog.

Segui questi passaggi per creare un predefinito per visualizzatori di eCatalog (devi essere un amministratore):

1. Nella barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Nella schermata Predefiniti visualizzatori, create un predefinito per visualizzatore di eCatalog iniziando da zero o da un predefinito esistente:

   * **Creare un predefinito per visualizzatori di eCatalog** - Seleziona **[!UICONTROL Aggiungi]**. Nella finestra di dialogo Aggiungi predefinito visualizzatore, scegli una piattaforma, scegli Visualizzatore eCatalog, quindi seleziona **[!UICONTROL Aggiungi]**.

   * **Modificare un predefinito per visualizzatori di eCatalog** - Seleziona un predefinito per visualizzatori di eCatalog, quindi seleziona **[!UICONTROL Modifica]**. Seleziona **[!UICONTROL Salva con nome]** al termine della creazione del predefinito.

1. Nella schermata Configura visualizzatore, inserite un nome per il predefinito del visualizzatore eCatalog.
1. Nella schermata Configura visualizzatore, impostate le opzioni desiderate.

   seleziona la **[!UICONTROL Suggerimento]** icona accanto all’opzione per leggerne la descrizione.

   Nella pagina Anteprima viene visualizzato il visualizzatore durante l’aggiornamento e la modifica delle impostazioni.

1. (Facoltativo) In **[!UICONTROL Impostazioni del pannello Info]**, **[!UICONTROL URL del server informazioni]** possono includere i seguenti token speciali, che il visualizzatore sostituisce:

   | Token | Sostituito da | Note |
   | --- | --- | --- |
   | `$1$` | valore rollover_key | L&#39;identificatore dell&#39;elemento dal `<area>` elemento della mappa. |
   | `$2$` | frame | Numero di sequenza del fotogramma attualmente visualizzato nel set di immagini. |
   | `$3$` | radice immagine | Primo elemento del percorso del primo elemento specificato nel comando dell’immagine (in genere si tratta dell’ID del catalogo di immagini per la voce del catalogo che specifica il set di immagini). |

1. (Facoltativo) In **[!UICONTROL Impostazioni del pannello Info]**, nella **[!UICONTROL Modello di risposta]** digitare il testo che si desidera visualizzare se Adobe Dynamic Media Classic rileva un errore nel recupero delle informazioni per una mappa immagine. Ad esempio, se il sistema riceve il nome di una società e il nome di un eCatalog, ma nessun identificatore di rollover, l’utente riceve il messaggio di errore qui configurato.

>[!NOTE]
>
>Per utilizzare questo modello di risposta invece del modello definito nell&#39;eCatalog stesso, aggiungi `fmt=1` alla fine dell&#39;URL del server informazioni. Ad esempio: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Seleziona **[!UICONTROL Salva]**.
1. Seleziona **[!UICONTROL Predefinito]** se desideri che il predefinito per visualizzatori di eCatalog creato sia quello utilizzato per visualizzare gli eCatalog sulla pagina web.

Per eliminare un predefinito per visualizzatori di eCatalog, selezionalo nella schermata Predefiniti visualizzatore e seleziona **[!UICONTROL Elimina]**.

>[!MORELIKETHIS]
>
>* [Predefiniti per visualizzatori](application-setup.md#viewer_presets)

