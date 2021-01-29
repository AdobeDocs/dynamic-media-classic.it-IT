---
title: Invio dei set di offerte a  Adobe Target Standard/Premium
description: Scoprite come inviare i set di offerte a  Adobe Target Standard/Premium.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 5%

---


# Invio dei set di offerte a  Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Dopo aver creato o modificato un set di offerte, inviatelo a Target Standard/Premium seguendo la procedura seguente:

1. Nella schermata Set di offerte Test&amp;Target, fate clic su **[!UICONTROL Invia offerte]**.
1. Immettete il codice client e le credenziali di accesso.
1. Fate clic su **[!UICONTROL Accesso]**.

Durante il trasferimento a Target Standard/Premium, il prefisso S7_ viene associato automaticamente all&#39;inizio dei nomi delle offerte. Questo prefisso è associato per essere certi di trovare facilmente le offerte Dynamic Media Classic nell’elenco delle offerte Test&amp;Target. Ad esempio, l’offerta compare come S7_&lt;nome set di offerte>_&lt;nome offerta>.

Dynamic Media Classic inserisce le offerte widget di Target Standard/Premium. Potete utilizzare le offerte Widget per ospitare contenuti di offerte al di fuori di Target Standard/Premium. Le offerte Widget sono simili a quelle standard ospitate al di fuori di Target Standard/Premium. Consentono a Target Standard/Premium di distribuire il contenuto delle offerte memorizzato sul server, per un utilizzo più sofisticato e dinamico. Le offerte Widget recuperano il contenuto da un URL, lo memorizzano nella cache e lo trasmettono per circa due ore. Le offerte Widget forniscono alcune funzionalità di generazione di contenuto dinamico non disponibili per altre offerte esterne a Target Standard/Premium. Se la mbox che distribuisce l&#39;offerta contiene parametri mbox come `mboxProductID` e `mbox.offerId`, i parametri dell&#39;URL `productId=[PRODUCT_ID]`e `offerID=[OFFERID]` vengono aggiunti all&#39;URL richiesto. Questi parametri possono essere utilizzati da un servizio disponibile nell&#39;URL dell&#39;offerta Widget per restituire contenuto all&#39;esterno di Target Standard/Premium che utilizza le informazioni di prodotto o ordine dalle mbox. L&#39;offerta Widget è inoltre accessibile tramite l&#39;API per creare offerte al di fuori di Target Standard/Premium a livello di programmazione.
