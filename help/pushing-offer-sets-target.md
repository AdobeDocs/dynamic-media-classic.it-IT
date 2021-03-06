---
title: Invio di set di offerte push ad Adobe Target Standard/Premium
description: Scopri come inviare i set di offerte ad Adobe Target Standard/Premium da Adobe Dynamic Media Classic.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Invio di set di offerte push ad Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Dopo aver creato o modificato un set di offerte, invialo ad Adobe Target Standard/Premium seguendo questi passaggi:

1. Nella schermata Set di offerte Test&amp;Target , seleziona **[!UICONTROL Offerte push]**.
1. Immetti il codice client e le credenziali di accesso.
1. Seleziona **[!UICONTROL Login]**.

Durante il trasferimento ad Adobe Target Standard/Premium, il prefisso `S7_` viene allegato automaticamente all’inizio dei nomi delle offerte. Questo prefisso viene allegato per garantire che sia possibile trovare facilmente le offerte Adobe Dynamic Media Classic nell’elenco delle offerte Test&amp;Target. Ad esempio, l’offerta viene visualizzata come `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic include le offerte dei widget Adobe Target Standard/Premium. Puoi utilizzare le offerte Widget per ospitare contenuti di offerte personalizzati al di fuori di Adobe Target Standard/Premium. Le offerte Widget sono simili a un&#39;offerta standard ospitata al di fuori di Adobe Target Standard/Premium. Consentono ad Adobe Target Standard/Premium di distribuire il contenuto delle offerte memorizzato sul server, per un utilizzo più sofisticato e dinamico. Le offerte Widget possono recuperare il contenuto da un URL, memorizzarlo nella cache e servirlo per circa due ore. Le offerte Widget forniscono alcune funzionalità di generazione di contenuti dinamici che altre offerte al di fuori di Adobe Target Standard/Premium non forniscono. Se la mbox che serve l&#39;offerta contiene parametri mbox come `mboxProductID` e `mbox.offerId`, i parametri URL `productId=[PRODUCT_ID]`e `offerID=[OFFERID]` vengono aggiunti all&#39;URL richiesto. Questi parametri possono essere utilizzati da un servizio disponibile presso l’URL dell’offerta Widget per restituire contenuti al di fuori di Adobe Target Standard/Premium che utilizza informazioni di prodotto o ordine dalle mbox. L’offerta Widget è accessibile anche tramite API per creare offerte in modo programmatico al di fuori di Adobe Target Standard/Premium.
