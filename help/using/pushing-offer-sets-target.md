---
title: Invia set di offerte ad Adobe Target Standard/Premium
description: Scopri come inviare set di offerte ad Adobe Target Standard/Premium da Adobe Dynamic Media Classic.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Invia set di offerte ad Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Dopo aver creato o modificato un set di offerte, invialo ad Adobe Target Standard/Premium seguendo questi passaggi:

1. Nella schermata Set offerte Test&amp;Target, seleziona **[!UICONTROL Invia offerte]**.
1. Immetti il codice cliente e le credenziali di accesso.
1. Seleziona **[!UICONTROL Login]**.

Durante il trasferimento ad Adobe Target Standard/Premium, il prefisso `S7_` viene associato automaticamente all’inizio dei nomi delle offerte. Questo prefisso è allegato per garantire che tu possa trovare facilmente le offerte Adobe Dynamic Media Classic nell’elenco delle offerte Test&amp;Target. Ad esempio, l’offerta viene visualizzata come `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic introduce le offerte di widget Adobe Target Standard/Premium. Puoi utilizzare le offerte Widget per ospitare il contenuto delle offerte al di fuori di Adobe Target Standard/Premium. Le offerte di widget sono simili alle offerte standard ospitate al di fuori di Adobe Target Standard/Prermium. Consentono ad Adobe Target Standard/Premium di distribuire contenuti di offerte memorizzati sul server, consentendo un utilizzo più sofisticato e dinamico. Le offerte dei widget possono recuperare il contenuto da un URL, memorizzarlo nella cache e distribuirlo per circa due ore. Le offerte di widget forniscono alcune funzionalità di generazione di contenuti dinamici, diversamente da altre offerte al di fuori di Adobe Target Standard/Premium. Se la mbox che serve l’offerta contiene parametri mbox come `mboxProductID` e `mbox.offerId`, il `productId=[PRODUCT_ID]`e `offerID=[OFFERID]` I parametri URL vengono aggiunti all’URL richiesto. Questi parametri possono essere utilizzati da un servizio disponibile all’URL dell’offerta Widget per restituire contenuto esterno a Adobe Target Standard/Premium che utilizza informazioni su prodotti o ordini provenienti dalle mbox. L’offerta Widget è accessibile anche tramite l’API per creare in modo programmatico offerte al di fuori di Adobe Target Standard/Premium.
