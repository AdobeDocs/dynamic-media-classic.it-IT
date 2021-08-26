---
title: Esportare risorse da Dynamic Media Classic
description: Scopri come esportare risorse da Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: 20a5e54a9f3fa442d3a993afae07aa5b1b13e9c3
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 52%

---

# Esportare risorse da Dynamic Media Classic{#exporting-assets-from-dmc}

È possibile salvare le risorse modificate in Dynamic Media Classic in un&#39;unità di rete locale. Le risorse esportate vengono raccolte in un file ZIP per il download o l’invio tramite e-mail.

Il file .zip compresso ha una dimensione massima di 1 GB per il processo di esportazione. Inoltre, è consentito un massimo di 500 risorse totali per processo di esportazione.

Nella schermata Processi di Dynamic Media Classic viene conservata una registrazione dei processi di esportazione.

**Per esportare le risorse da Dynamic Media Classic:**

1. Seleziona le risorse da esportare, quindi vai a **[!UICONTROL File]** > **[!UICONTROL Esporta]**.
1. Nella finestra Esporta risorse selezionate, fate clic su **[!UICONTROL Opzioni immagini]** e specificate una delle seguenti opzioni (gli amministratori stabiliscono quali opzioni rendere disponibili agli utenti):

   * **[!UICONTROL Predefiniti]** : facoltativamente, scegli un predefinito immagine per formattare la risorsa quando la esporti. Se scegliete un predefinito per immagini, le altre opzioni di formattazione non sono disponibili, poiché vengono adottati i formati specificati dal predefinito.

   * **[!UICONTROL Conversione]** : consente di convertire il file della risorsa o l’immagine originale.

   * **[!UICONTROL Dimensioni]**  - È possibile selezionare una dimensione standard. In alternativa, è possibile selezionare **[!UICONTROL Altro]** dall&#39;elenco a discesa **[!UICONTROL Dimensioni]**, scegliere l&#39;unità di misura desiderata e specificare la larghezza e l&#39;altezza.

      Consulta anche [Specificare le opzioni di esportazione disponibili per gli utenti di Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL Formato]**  - Scegli un formato immagine.

   * **[!UICONTROL Colore]** : scegli RGB, CMYK o Grigio.

   * **[!UICONTROL Risoluzione]** : scegli 72 ppi, 150 ppi o 300 ppi.

   * **[!UICONTROL Nome processo]** : è possibile assegnare un nome di processo all&#39;esportazione.

   * **[!UICONTROL Invia e-mail a]** : se lo desideri, immetti facoltativamente un indirizzo e-mail per inviare le risorse tramite e-mail. Nel messaggio e-mail viene riportato l’URL mediante il quale il destinatario può scaricare le risorse.

1. Selezionare **[!UICONTROL Esporta]**.

Sono supportate tre azioni di esportazione di base:

* File originale (esporta il file originale della risorsa)
* Converti con predefinito (formatta la risorsa mediante un predefinito per immagini)
* Converti senza predefinito (specificate i modificatori per immagini nella finestra di dialogo di esportazione)

Non è possibile esportare i seguenti tipi di risorsa. Tutti gli altri generano un’esportazione.

* Set di immagini
* Set di rendering
* Set 360 gradi
* Set di file multimediali
* Set con bitrate multiplo
* eCatalog

Inoltre, non è possibile esportare i modelli come “file originale”.

Mediante la conversione è possibile esportare i seguenti tipi di risorsa:

* Immagini
* Modelli
* Immagini regolate
* PDF (genera pagine convertite)
* PostScript®

Se si selezionano numerosi elementi da esportare e di tipi di risorse diversi, si possono verificare i seguenti comportamenti:

* Tutti i tipi di risorse che non possono essere esportati vengono rimossi dall’elenco prima dell’invio del processo
* Se viene richiesta una conversione, vengono elaborati tutti i tipi che possono essere convertiti; gli altri vengono invece esportati come file originali
