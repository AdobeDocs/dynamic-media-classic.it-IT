---
title: Invio dei set di offerte ad Adobe Target Standard/Premium
description: Scopri come inviare i set di offerte in Adobe Target Standard/Premium.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Invio dei set di offerte ad Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Dopo aver creato o modificato un set di offerte, invialo ad Adobe Target Standard/Premium seguendo questi passaggi:

1. Nella schermata Set di offerte Test&amp;Target , fai clic su **[!UICONTROL Offerte push]**.
1. Immetti il codice client e le credenziali di accesso.
1. Fate clic su **[!UICONTROL Accesso]**.

Durante il trasferimento ad Adobe Target Standard/Premium, il prefisso `S7_` viene allegato automaticamente all’inizio dei nomi delle offerte. Questo prefisso viene allegato per garantire che sia possibile trovare facilmente le offerte Dynamic Media Classic nell’elenco delle offerte Test&amp;Target. Ad esempio, l’offerta viene visualizzata come `S7_<name of offer set>_<offer name>`.

Dynamic Media Classic invia le proprie richieste alle offerte widget Adobe Target Standard/Premium. Puoi utilizzare le offerte Widget per ospitare contenuti di offerte personalizzati al di fuori di Adobe Target Standard/Premium. Le offerte Widget sono simili a un&#39;offerta standard ospitata al di fuori di Adobe Target Standard/Premium. Consentono ad Adobe Target Standard/Premium di distribuire il contenuto delle offerte memorizzato sul server, per un utilizzo più sofisticato e dinamico. Le offerte Widget recuperano il contenuto da un URL, lo memorizzano nella cache e lo servono per circa due ore. Le offerte Widget forniscono alcune funzionalità di generazione di contenuti dinamici che altre offerte al di fuori di Adobe Target Standard/Premium non forniscono. Se la mbox che serve l&#39;offerta contiene parametri mbox come `mboxProductID` e `mbox.offerId`, i parametri URL `productId=[PRODUCT_ID]`e `offerID=[OFFERID]` vengono aggiunti all&#39;URL richiesto. Questi parametri possono essere utilizzati da un servizio disponibile presso l’URL dell’offerta Widget per restituire contenuti al di fuori di Adobe Target Standard/Premium che utilizza informazioni di prodotto o ordine dalle mbox. L’offerta Widget è accessibile anche tramite API per creare offerte in modo programmatico al di fuori di Adobe Target Standard/Premium.
