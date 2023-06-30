---
title: "Guida introduttiva: Integrazione di Adobe Target Standard/Premium"
description: Introduzione e Guida rapida ad Adobe Target Standard/Premium per aiutarti a iniziare rapidamente a utilizzare le tecniche di integrazione di Adobe Target Standard/Premium in Adobe Dynamic Media Classic.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 7%

---

# Guida introduttiva: Integrazione con Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium consente agli addetti al marketing di eseguire in modo rapido e continuo più test A/B e multivariati, misurare l’efficacia e aumentare la rilevanza dei contenuti online tramite segmentazione, targeting e Automated Personalization.

Adobe Dynamic Media Classic consente di creare offerte e set di offerte per le campagne Adobe Target Standard/Premium. Ad esempio, puoi creare un set di offerte con tre varianti della stessa risorsa rich media. Quindi puoi chiedere ad Adobe Target Standard/Premium di determinare quale risorsa fornisce un incremento di conversione migliore. Potete creare offerte e set di offerte da un modello base o da immagini singole. Dopo che il set di offerte è stato inviato o salvato in Adobe Target Standard/Premium, dove le offerte sono associate a mbox ed esperienze, Adobe Target Standard/Premium può eseguire campagne. Queste campagne determinano la variante di un sito web che probabilmente offre le prestazioni migliori per i click-through e la conversione.

Per una maggiore personalizzazione dei contenuti Adobe Dynamic Media Classic dinamici, utilizza le offerte Adobe Target Standard/Premium HTML. Consulta la [Documentazione di Adobe Target Standard/Premium](https://experienceleague.adobe.com/docs/target.html) per ulteriori informazioni.

>[!NOTE]
>
>Per utilizzare Adobe Target Standard/Premium con Adobe Dynamic Media Classic è necessario un account Adobe Target Standard/Premium valido.

Questa Guida rapida è stata progettata per aiutarti a iniziare rapidamente a lavorare con i set di offerte di Adobe Target Standard/Premium HTML. Seguite i passaggi da 1 a 3. Dopo ogni passaggio, viene inserito un riferimento incrociato a un titolo di argomento in cui è possibile trovare ulteriori informazioni.

## 1. Immetti l&#39;URL di Adobe Target Standard/Premium nella pagina Impostazioni generali applicazione

Adobe Dynamic Media Classic ha bisogno del tuo URL di Adobe Target Standard/Premium per integrarsi con Adobe Target Standard/Premium. Copia la porzione dell’URL di Adobe Target Standard/Premium fino a e incluso `.com`e immetterlo in Adobe Dynamic Media Classic **[!UICONTROL Impostazioni generali applicazione]** pagina, nella **[!UICONTROL Server]** gruppo, **[!UICONTROL Nome server Test&amp;Target]** campo di testo. Consulta [Integrare Adobe Dynamic Media Classic con Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Creare il set di offerte

Usate un modello o immagini con parametri per creare un set di offerte. I set di offerte HTML vengono creati nella pagina Set di offerte Test&amp;Target. Per aprire questa pagina, seleziona il modello o le immagini, quindi sulla barra di navigazione globale vai a **[!UICONTROL Genera]** > **[!UICONTROL Set di offerte Test&amp;Target]**.

Per creare un’offerta con un modello, seleziona **[!UICONTROL Aggiungi e visualizza anteprima]**. Nella pagina Aggiungi e visualizza anteprima, modifica i valori dei parametri.

Per creare un&#39;offerta con immagini, trascina le immagini nella pagina Set di offerte Test&amp;Target. Seleziona **[!UICONTROL Anteprima]** e scegli un predefinito immagine per un’immagine o tutte le immagini del set di offerte.

Dopo averlo creato, salvate il set di offerte.

Consulta [Creare un set di offerte](creating-offer-set.md#creating_an_offer_set).

## 3. Invia il set di offerte ad Adobe Target Standard/Premium

Nella pagina Set di offerte Test&amp;Target, seleziona **[!UICONTROL Invia offerte]** e immettere le credenziali di accesso nella finestra di dialogo Accesso Test&amp;Target. Consulta [Invia set di offerte ad Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
