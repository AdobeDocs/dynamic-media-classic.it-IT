---
title: '"Avvio rapido: Integrazione Adobe Target Standard/Premium"'
description: Introduzione e avvio rapido ad Adobe Target Standard/Premium per aiutarti a iniziare rapidamente a usare le tecniche di integrazione di Adobe Target Standard/Premium.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 12%

---

# Avvio rapido: Integrazione Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium mette il controllo direttamente nelle mani degli addetti al marketing per eseguire in modo rapido e continuo più test A/B e multivariati, misurare l’efficacia e aumentare la pertinenza dei contenuti online tramite segmentazione, targeting e personalizzazione automatizzata.

Dynamic Media Classic consente di creare offerte e set di offerte per le campagne Adobe Target Standard/Premium. Ad esempio, puoi creare un set di offerte con tre varianti della stessa risorsa rich media. Quindi puoi fare in modo che Adobe Target Standard/Premium determini quale risorsa fornisce un incremento di conversione migliore. Potete creare offerte e set di offerte da un modello base o da immagini singole. Dopo che il set di offerte è stato inviato o salvato in Adobe Target Standard/Premium, dove le offerte sono associate a mbox ed esperienze, Adobe Target Standard/Premium può eseguire campagne. Queste campagne determinano quale variazione di un sito web è probabile che funzioni meglio per i click-through e la conversione.

Per una maggiore personalizzazione del contenuto dinamico di Dynamic Media Classic, utilizza le offerte HTML di Adobe Target Standard/Premium. Per ulteriori informazioni, consulta la [documentazione di Adobe Target Standard/Premium](https://experienceleague.adobe.com/docs/target.html) .

>[!NOTE]
>
>Per utilizzare Adobe Target Standard/Premium con Dynamic Media Classic è necessario un account Adobe Target Standard/Premium valido.

Questa guida rapida è stata progettata per aiutarti a iniziare rapidamente a usare i set di offerte HTML di Adobe Target Standard/Premium. Seguite i passaggi da 1 a 3. Alla fine di ciascun passaggio è riportato un riferimento a un argomento correlato con ulteriori informazioni.

## 1. Inserisci l&#39;URL Adobe Target Standard/Premium nella pagina Impostazioni generali dell&#39;applicazione

Dynamic Media Classic richiede l&#39;URL di Adobe Target Standard/Premium per l&#39;integrazione con Adobe Target Standard/Premium. Copia la parte dell&#39;URL Adobe Target Standard/Premium fino a `.com` incluso e inseriscilo nella pagina Impostazioni generali dell&#39;applicazione **[!UICONTROL Dynamic Media Classic]**, nel gruppo **[!UICONTROL Server]**, **[!UICONTROL Nome server di test&amp;Target]**. Consulta [Integrazione di Dynamic Media Classic con Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Creare il set di offerte

Usate un modello o immagini con parametri per creare un set di offerte. Puoi creare set di offerte HTML nella pagina Set di offerte Test&amp;Target . Per aprire questa pagina, seleziona il modello o le immagini, quindi fai clic su **[!UICONTROL Build]** > **[!UICONTROL Set di offerte Test&amp;Target]** nella barra di navigazione globale.

Per creare un&#39;offerta con un modello, fai clic su **[!UICONTROL Aggiungi e visualizza anteprima]**. Nella pagina Aggiungi e visualizza anteprima modificare i valori dei parametri.

Per creare un’offerta con immagini, trascina le immagini nella pagina Set di offerte Test&amp;Target . Fai clic su **[!UICONTROL Anteprima]** e scegli un predefinito immagine per un&#39;immagine o per tutte le immagini nel set di offerte.

Dopo averlo creato, salvate il set di offerte.

Consultate [Creazione di un set di offerte](creating-offer-set.md#creating_an_offer_set).

## 3. Invia il set di offerte ad Adobe Target Standard/Premium

Nella pagina Set di offerte Test&amp;Target , fai clic su **[!UICONTROL Offerte push]** e immetti le tue credenziali di accesso nella finestra di dialogo Accesso a Test&amp;Target . Consulta [Invio dei set di offerte ad Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
