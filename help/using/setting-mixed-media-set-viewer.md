---
title: Impostare un predefinito visualizzatore set di file multimediali diversi
description: Scopri come impostare un predefinito visualizzatore set di file multimediali diversi in Adobe Dynamic Media Classic.
uuid: d5bf1840-e453-445d-bebc-84889b29f3c8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 8029aad8-d696-4d7c-99e2-3b08edb68181
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: d41b30e7-994a-43f3-8698-7dbfc36305ae
topic: Content Management
level: Intermediate
source-git-commit: faa1784e1d19b1167cad5749dc04227e3ff388e5
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 40%

---

# Impostare un predefinito visualizzatore set di file multimediali diversi{#setting-up-a-mixed-media-set-viewer-preset}

I predefiniti per visualizzatori di set di file multimediali diversi determinano lo stile, il comportamento e l’aspetto del visualizzatore principale. Quando configurate un predefinito, specificate quali altri visualizzatori devono apparire nel visualizzatore di set di file multimediali diversi. Ad esempio, se nel set di file multimediali diversi avete incluso un set di immagini, specificate anche un predefinito per visualizzatori di set di immagini.

Potete scegliere di includere nel visualizzatore di set di file multimediali diversi tutte le funzioni per le community Internet o solo alcune di esse. La funzione Incorpora aggiunge al visualizzatore un collegamento che permette agli utenti di copiare il codice richiesto per aprire il visualizzatore in una pagina esterna (ad esempio un blog, un sito Web o un sito di social networking). La funzione Collegamento fornisce l’URL del visualizzatore, in modo che gli utenti possano usare un collegamento al visualizzatore. La funzione Visita fornisce un collegamento al sito Web specificato.

1. Sulla barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**.
1. Nella pagina Predefiniti visualizzatore effettuare una delle seguenti operazioni:

   * Per creare un predefinito, seleziona **[!UICONTROL Aggiungi]**. Nella finestra di dialogo Aggiungi predefinito visualizzatore, scegli una piattaforma, scegli **[!UICONTROL Visualizzatore set di file multimediali diversi]**, quindi seleziona **[!UICONTROL Aggiungi]**.
   * Per modificare un predefinito per visualizzatore set di file multimediali diversi, selezionalo, quindi seleziona **[!UICONTROL Modifica]**.

1. Nella pagina Visualizzatore configurazione, digita un nome nella casella Nome predefinito per il predefinito Visualizzatore set di file multimediali diversi.
1. Specifica **[!UICONTROL Schede]** o **[!UICONTROL Nessuna scheda]**. Le schede separano gli elementi in base al tipo, ad esempio set di video, di campioni o set 360 gradi. Se non specificate alcuna scheda, tutti gli elementi vengono visualizzati in una riga sotto la finestra Anteprima.
1. In **[!UICONTROL Nome]** digitare un nome per il visualizzatore da aggiungere.

   Ad esempio, se stai aggiungendo un set di campioni al set di file multimediali diversi, digita `Swatch Set A`.

1. Nel menu Visualizzatore, scegliete il tipo di risorsa da visualizzare, ad esempio Set campioni.
1. Nel menu Predefinito, scegliete un predefinito per il tipo di risorsa scelta.

   Ad esempio, se state aggiungendo un set di campioni, scegliete **[!UICONTROL ColoriSetCampioni1]**.

1. Seleziona **[!UICONTROL Aggiungi]**.

   Il nuovo predefinito per visualizzatori viene riportato nell’elenco.

1. Ripetete i passaggi da 6 a 9 per tutti i predefiniti da aggiungere.
1. Per modificare l’elenco dei predefiniti, effettuate una delle seguenti operazioni:

   * Per eliminare un predefinito dall&#39;elenco, selezionatelo, quindi selezionate **[!UICONTROL Elimina]**.
   * Per riordinare i predefiniti nell’elenco, seleziona un predefinito, quindi seleziona il **[!UICONTROL Su]** o **[!UICONTROL Giù]** freccia.

1. Per aggiungere al visualizzatore funzioni per la community Internet (Incorpora, Collegamento, Visita), specificate le opzioni per una delle seguenti operazioni:

   * **E-mail** - Seleziona **[!UICONTROL On]** per attivare un pulsante E-mail nel visualizzatore. Quando gli utenti selezionano il pulsante E-mail durante la visualizzazione del set, viene visualizzato un messaggio e-mail contenente il collegamento al set.

   * **Incorpora** - Seleziona **[!UICONTROL Live]**. Nella casella Etichetta pulsante incorpora, digitate il nome che sarà visibile nel visualizzatore per il pulsante Incorpora. Se lo desideri, seleziona **[!UICONTROL Sfoglia]** per individuare e selezionare uno skin personalizzato per il pulsante.

   * **Collegamento** - Seleziona **[!UICONTROL Live]**. Nella casella Etichetta pulsante collegamento digitare il nome che si desidera visualizzare nel visualizzatore per il pulsante Collegamento. Se lo desideri, seleziona **[!UICONTROL Sfoglia]** per individuare e selezionare uno skin personalizzato per il pulsante.

   * **Visita** - Seleziona **[!UICONTROL Live]**. Nella casella Etichetta pulsante visita digitare il nome che si desidera visualizzare nel visualizzatore del pulsante Visita. Nella casella URL visita digitare l&#39;URL del sito Web che si desidera aprire quando si seleziona il collegamento.

1. Specificate le altre opzioni desiderate. Per visualizzare una descrizione di un&#39;opzione, selezionare l&#39;icona Suggerimento informazioni accanto all&#39;opzione.

   Nella pagina Anteprima viene visualizzato il visualizzatore durante l&#39;aggiornamento e la modifica delle impostazioni.

1. Seleziona **[!UICONTROL Salva]**.

>[!MORELIKETHIS]
>
>* [Creare e modificare i predefiniti per visualizzatori](application-setup.md#adding_and_editing_viewer_presets)
