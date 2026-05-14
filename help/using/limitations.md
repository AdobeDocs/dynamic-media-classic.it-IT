---
title: Limitazioni di Dynamic Media
description: Scopri le best practice e i limiti applicati quando crei un set di immagini o un set 360 gradi o carichi un PDF. Scopri anche le combinazioni di browser Web e sistemi operativi non supportate per Dynamic Media.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Asset Management,Image Sets,Spin Sets,eCatalog
role: User
exl-id: ee30a2c1-2b26-41bd-8758-e7337a3727bb
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:02:23.354Z'
TQID: 'https://experienceleague.adobe.com/7dtiaPb7sWkPb5gocOc8xLOnz3U3gJuSdaW2LSkajMk'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 352
ht-degree: 1%

---

# Limitazioni per elementi multimediali dinamici

Le sezioni seguenti descrivono le limitazioni di Dynamic Media.

Questo argomento include le sezioni seguenti:

* [Best practice e limiti applicati da Dynamic Media ai tipi di risorse](#best-practice-enforced-limits)
* [Combinazioni di browser Web e sistemi operativi non supportate per Dynamic Media](#unsupported-browser-os)

## Best practice e limiti applicati da Dynamic Media ai tipi di risorse {#best-practice-enforced-limits}

Quando crei un set 360 gradi o un set di immagini o carichi PDF per l’estrazione di una pagina, Adobe consiglia le seguenti best practice. Adobe applica inoltre i seguenti limiti:

| Risorsa: tipo di limite | Best practice | Limite imposto |
| --- | --- | --- |
| **Immagine**: numero di ritagli avanzati per immagine | 5 | 100 |
| **Tutti i set**: numero di risorse duplicate per set | Nessun duplicato | 20‡ |
| **Tutti i set**: numero massimo di risorse per set | 5-10 immagini per set | 1000 |
| **Set 360 gradi**: numero massimo di righe/colonne per set 2D | 12-18 immagini per set | 1000 |
| **PDF**: numero massimo di pagine per un PDF da considerare per l&#39;estrazione |  | 100 (per tutti i PDF) |

‡ Si consiglia di non avere risorse duplicate in un set. Il limite è di 20 duplicati per una singola risorsa. Se aggiungi un altro duplicato per quella risorsa, all’interno di quel set, la richiesta restituisce un errore o ignora il duplicato.

<!-- See also [Dynamic Media limitations](/help/using/assets/limitations.md). -->

## Combinazioni di browser Web e sistemi operativi non supportate per Dynamic Media {#unsupported-browser-os}

<!-- CQDOC-19433 -->

Adobe Dynamic Media non supporta le seguenti combinazioni di browser web e sistemi operativi.

* Internet Explorer 11 + Windows 7
* Internet Explorer 11 + Windows 8.1
* Internet Explorer 11 + Windows Phone 8.1
* Aggiornamento Internet Explorer 11 + Windows Phone 8.1
* Safari 6 + iOS 6.0.1
* Safari 7 + iOS 7.1
* Safari 7 + OS X 10.9 Mavericks
* Safari 8 + iOS 8.4
* Safari 8 + OS X 10.10 Yosemite

## Fine del supporto per Secure Socket Layer 2.0 e 3.0 e Transport Layer Security 1.0 e 1.1 {#tls}

<!-- 
CQDOC-19433 (original ticket)
and CQDOC-19792 (removed as per this ticket December 5, 2022) 
-->

A decorrere dal 30 aprile 2024, Adobe Dynamic Media cesserà il supporto per i seguenti elementi:

* SSL (Secure Socket Layer) 2.0
* SSL 3.0
* TLS (Transport Layer Security) 1.0 e 1.1
* Le seguenti crittografie deboli in TLS 1.2:
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384`
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_RSA_WITH_AES_256_GCM_SHA384`
   * `TLS_RSA_WITH_AES_256_CBC_SHA256`
   * `TLS_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_AES_128_GCM_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_256_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_128_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_3DES_EDE_CBC_SHA`
   * `TLS_RSA_WITH_SDES_EDE_CBC_SHA`

