---
title: Invia set di offerte ad Adobe Target Standard/Premium
description: Scopri come inviare set di offerte ad Adobe Target Standard/Premium da Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:55:22.850Z'
TQID: 'https://experienceleague.adobe.com/8j9sRn1zhAhgj-wMV6hYix1F9aARZjDUiFZofcVVcBw'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 289
ht-degree: 0%

---

# Invia set di offerte ad Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Dopo aver creato o modificato un set di offerte, invialo ad Adobe Target Standard/Premium seguendo questi passaggi:

1. Nella schermata Set offerte Test&amp;Target, seleziona **[!UICONTROL Invia offerte]**.
1. Immetti il codice cliente e le credenziali di accesso.
1. Seleziona **[!UICONTROL Accesso]**.

Durante il trasferimento ad Adobe Target Standard/Premium, il prefisso `S7_` viene allegato automaticamente all&#39;inizio dei nomi delle offerte. Questo prefisso è allegato per garantire che tu possa trovare facilmente le offerte Adobe Dynamic Media Classic nell’elenco delle offerte Test&amp;Target. Ad esempio, l&#39;offerta verrà visualizzata come `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic introduce le offerte di widget Adobe Target Standard/Premium. Puoi utilizzare le offerte Widget per ospitare i contenuti che hai offerto su Adobe Target Standard/Premium. Le offerte di widget sono simili alle offerte standard ospitate da Adobe Target Standard/Prermium. Consentono ad Adobe Target Standard/Premium di distribuire contenuti di offerte memorizzati sul server, consentendo un utilizzo più sofisticato e dinamico. Le offerte dei widget possono recuperare il contenuto da un URL, memorizzarlo nella cache e distribuirlo per circa due ore. Le offerte di widget forniscono alcune funzionalità di generazione di contenuti dinamici, diversamente da altre offerte al di fuori di Adobe Target Standard/Premium. Se la mbox che serve l&#39;offerta contiene parametri mbox, ad esempio `mboxProductID` e `mbox.offerId`, i parametri URL `productId=[PRODUCT_ID]` e `offerID=[OFFERID]` vengono aggiunti all&#39;URL richiesto. Questi parametri vengono utilizzati da un servizio disponibile all’URL dell’offerta Widget per restituire contenuto esterno a Adobe Target Standard/Premium che utilizza informazioni su prodotti o ordini provenienti dalle mbox. L’offerta Widget è accessibile anche tramite l’API, in modo da poter creare in modo programmatico offerte al di fuori di Adobe Target Standard/Premium.
