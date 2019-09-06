---
title: Invio di set di offerte ad Adobe Target Classic
seo-title: Invio di set di offerte ad Adobe Target Classic
description: 'null'
seo-description: Scoprite come inviare i set di offerte ad Adobe Target Classic.
uuid: 8 c 895 a 7 c -21 b 4-4 d 85-8 b 0 b-a 3 d 2 a 420 bf 2 e
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/target_ classic_ integration
discoiquuid: 39 a 05654-4 f 66-4 f 1 e-aec 5-ebe 6 d 174353 f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Invio di set di offerte ad Adobe Target Classic{#pushing-offer-sets-to-adobe-target-classic}

Dopo aver creato o modificato un set di offerte, inviatelo a Target Classic attenendovi alla seguente procedura:

1. Nella schermata Set di offerte di Target Classic, fate clic sul pulsante Invia offerte.
1. Inserite le credenziali di accesso.
1. Fate clic sul pulsante Accesso.

Durante il trasferimento a Target Classic, il prefisso S 7_ viene aggiunto automaticamente all'inizio dei nomi delle offerte. Questo prefisso viene fornito per garantire che sia possibile trovare facilmente le offerte Dynamic Media Classic nell'elenco delle offerte di Target Classic. Ad esempio, l’offerta compare come S7_&lt;nome set di offerte&gt;_&lt;nome offerta&gt;.

SPS invia un push alle offerte widget Target Classic. Potete utilizzare le offerte Widget per ospitare il contenuto delle offerte all'esterno di Target Classic. Le offerte Widget sono simili a quelle in hosting all'esterno di Target Classic. Consentono a Target Classic di distribuire contenuti delle offerte memorizzate sul server, consentendo un utilizzo più sofisticato e dinamico. Le offerte Widget recuperano il contenuto da un URL, la cache e lo trasmettono per circa due ore. Le offerte Widget offrono alcune funzionalità di generazione di contenuti dinamiche che altre offerte non sono disponibili all'esterno di Target Classic. If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. Questi parametri possono essere utilizzati da un servizio disponibile presso l'URL delle offerte Widget per restituire contenuto all'esterno di Target Classic che utilizza informazioni sul prodotto o sull'ordine dalle mbox. L'offerta Widget è anche accessibile tramite l'API per creare offerte a livello di programmazione al di fuori di Target Classic.
