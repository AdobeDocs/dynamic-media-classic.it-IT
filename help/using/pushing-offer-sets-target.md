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
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 8a9d304ced3a218ae6393961a278f5ab9581c229
workflow-type: tm+mt
source-wordcount: 283
ht-degree: 0%

---

# Invia set di offerte ad Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Dopo aver creato o modificato un set di offerte, invialo ad Adobe Target Standard/Premium seguendo questi passaggi:

1. Nella schermata Set offerte Test &amp; Target, seleziona **[!UICONTROL Offerte push]**.
1. Immetti il codice cliente e le credenziali di accesso.
1. Seleziona **[!UICONTROL Accesso]**.

Durante il trasferimento ad Adobe Target Standard/Premium, il prefisso `S7_` viene aggiunto automaticamente all&#39;inizio dei nomi delle offerte. Questo prefisso viene aggiunto per garantire che tu possa trovare facilmente le offerte Adobe Dynamic Media Classic nell’elenco delle offerte di Test &amp; Target. Ad esempio, l&#39;offerta verrà visualizzata come `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic invia le offerte dei widget in Adobe Target Standard/Premium. Puoi utilizzare le offerte Widget per ospitare i contenuti offerti su Adobe Target Standard/Premium. Le offerte di widget sono paragonabili a quelle di offerte standard in hosting presso Adobe Target Standard/Premium. Consentono ad Adobe Target Standard/Premium di implementare il contenuto delle offerte memorizzato sul server, consentendo un utilizzo più sofisticato e dinamico. Le offerte Widget recuperano il contenuto da un URL, memorizzandolo nella cache e distribuendolo per due ore. Le offerte Widget forniscono alcune funzionalità di generazione di contenuti dinamici, diversamente da altre offerte al di fuori di Adobe Target Standard/Premium. Se la mbox che serve l&#39;offerta contiene parametri mbox, ad esempio `mboxProductID` e `mbox.offerId`, i parametri URL `productId=[PRODUCT_ID]` e `offerID=[OFFERID]` vengono aggiunti all&#39;URL richiesto. Un servizio disponibile all’URL dell’offerta Widget utilizza questi parametri per restituire contenuto esterno a Adobe Target Standard/Premium che utilizza informazioni su prodotti o ordini provenienti dalle mbox. L’offerta Widget è accessibile anche tramite l’API, in modo da poter creare in modo programmatico offerte al di fuori di Adobe Target Standard/Premium.
