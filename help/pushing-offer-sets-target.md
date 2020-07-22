---
title: Invio dei set di offerte a  Adobe Target Standard/Premium
seo-title: Invio dei set di offerte a  Adobe Target Standard/Premium
description: 'null'
seo-description: Scoprite come inviare i set di offerte a  Adobe Target Standard/Premium.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 5%

---


# Invio dei set di offerte a  Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Dopo aver creato o modificato un set di offerte, inviatelo ad Target Standard/Premium seguendo la procedura seguente:

1. In the Test&amp;Target Offer Set screen, click **[!UICONTROL Push Offers]**.
1. Immettete il codice client e le credenziali di accesso.
1. Fate clic su **[!UICONTROL Accesso]**.

Durante il trasferimento ad Target Standard/Premium, il prefisso S7_ viene aggiunto automaticamente all&#39;inizio dei nomi delle offerte. Questo prefisso è associato per garantire che sia possibile trovare facilmente le offerte Dynamic Media Classic nell&#39;elenco delle offerte Test&amp;Target. Ad esempio, l’offerta compare come S7_&lt;nome set di offerte>_&lt;nome offerta>.

Dynamic Media Classic consente di accedere alle offerte widget Target Standard/Premium. Potete utilizzare le offerte Widget per ospitare contenuti di offerte al di fuori di Target Standard/Premium. Le offerte Widget sono simili alle offerte standard ospitate al di fuori di Target Standard/Premium. Consentono ad Target Standard/Premium di distribuire il contenuto delle offerte memorizzato sul server, per un utilizzo più sofisticato e dinamico. Le offerte Widget recuperano il contenuto da un URL, lo memorizzano nella cache e lo trasmettono per circa due ore. Le offerte Widget offrono alcune funzionalità di generazione di contenuti dinamici non disponibili per altre offerte esterne ad Target Standard/Premium. If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. Questi parametri possono essere utilizzati da un servizio disponibile presso l&#39;URL dell&#39;offerta Widget per restituire contenuti all&#39;esterno di Target Standard/Premium che utilizza informazioni su prodotti o ordini dalle mbox. L&#39;offerta Widget è inoltre accessibile tramite l&#39;API per creare offerte all&#39;esterno di Target Standard/Premium a livello di programmazione.
