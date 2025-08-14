---
title: 'Guida introduttiva: Integrazione con Adobe Target Standard/Premium'
description: Introduzione e Guida rapida ad Adobe Target Standard/Premium per aiutarti a iniziare rapidamente a utilizzare le tecniche di integrazione di Adobe Target Standard/Premium in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Guida introduttiva: Integrazione con Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium lascia il controllo direttamente nelle mani degli addetti al marketing. In questo modo è possibile eseguire in modo rapido e continuo più test A/B e multivariati e misurare l’efficacia. Inoltre, può aumentare la rilevanza dei contenuti online tramite segmentazione, targeting e Automated Personalization.

Adobe Dynamic Media Classic consente di creare offerte e set di offerte per le campagne Adobe Target Standard/Premium. Ad esempio, puoi creare un set di offerte con tre varianti della stessa risorsa rich media. Quindi puoi avere Adobe Target Standard o Premium per determinare quale risorsa fornisce un incremento di conversione migliore. Puoi creare offerte e set di offerte da un modello base o da singole immagini. Dopo che il set di offerte è stato inviato o salvato in Adobe Target Standard/Premium, dove le offerte sono associate a mbox ed esperienze, Adobe Target Standard/Premium può eseguire campagne. Queste campagne determinano la variante di un sito web che probabilmente offre le prestazioni migliori per i click-through e la conversione.

Per una maggiore personalizzazione dei contenuti Adobe Dynamic Media Classic dinamici, utilizza le offerte HTML di Adobe Target Standard/Premium. Per ulteriori informazioni, consulta la [documentazione di Adobe Target Standard/Premium](https://experienceleague.adobe.com/en/docs/target).

>[!NOTE]
>
>Per utilizzare Adobe Target Standard/Premium con Adobe Dynamic Media Classic è necessario un account Adobe Target Standard/Premium valido.

Questa Guida introduttiva è stata progettata per aiutarti a iniziare rapidamente a lavorare con i set di offerte HTML di Adobe Target Standard/Premium. Seguite i passaggi da 1 a 3. Dopo ogni passaggio, viene inserito un riferimento incrociato a un titolo di argomento in cui è possibile trovare ulteriori informazioni.

## &#x200B;1. Immetti l&#39;URL di Adobe Target Standard/Premium nella pagina Impostazioni generali applicazione

Adobe Dynamic Media Classic ha bisogno del tuo URL di Adobe Target Standard/Premium per integrarsi con Adobe Target Standard/Premium. Copiare la parte dell&#39;URL di Adobe Target Standard/Premium fino a `.com` incluso e immetterla nella pagina **[!UICONTROL Impostazioni generali applicazione]** di Adobe Dynamic Media Classic, nel campo di testo **[!UICONTROL Nome server Test&amp;Target]** del gruppo **[!UICONTROL Server]**. Consulta [Integrare Adobe Dynamic Media Classic con Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## &#x200B;2. Creare la serie di offerte

Utilizza un modello con parametri o immagini per creare un set di offerte. Puoi creare i set di offerte HTML nella pagina Set di offerte Test&amp;Target. Per aprire questa pagina, seleziona il modello o le immagini, quindi sulla barra di navigazione globale vai a **[!UICONTROL Build]** > **[!UICONTROL Set di offerte Test&amp;Target]**.

Per creare un&#39;offerta con un modello, selezionare **[!UICONTROL Aggiungi e visualizza anteprima]**. Nella pagina Aggiungi e visualizza anteprima, modifica i valori dei parametri.

Per creare un&#39;offerta con immagini, trascina le immagini nella pagina Set di offerte Test&amp;Target. Seleziona **[!UICONTROL Anteprima]** e scegli un predefinito immagine per un&#39;immagine o tutte le immagini nel set di offerte.

Salva il set di offerte dopo averlo creato.

Vedi [Creare un set di offerte](creating-offer-set.md#creating_an_offer_set).

## &#x200B;3. Invia il set di offerte ad Adobe Target Standard/Premium

Nella pagina Set di offerte Test&amp;Target, seleziona **[!UICONTROL Offerte push]** e immetti le credenziali di accesso nella finestra di dialogo Accesso Test&amp;Target. Consulta [Invia set di offerte ad Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
