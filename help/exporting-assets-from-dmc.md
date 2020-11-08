---
title: Esportazione di risorse da Dynamic Media Classic
seo-title: Esportazione di risorse da Dynamic Media Classic
description: 'null'
seo-description: Scopri come esportare risorse da Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
translation-type: tm+mt
source-git-commit: 38f5cf5264f9775a225d354ed9dc2f6caee236f2
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 69%

---


# Esportazione di risorse da Dynamic Media Classic{#exporting-assets-from-dmc}

Potete salvare le risorse modificate in Dynamic Media Classic in un’unità di rete locale. Le risorse esportate vengono raccolte in un file ZIP per il download o l’invio tramite e-mail.

Il file .zip compresso ha una dimensione massima di 1 GB per il processo di esportazione. Inoltre, è consentito un massimo complessivo di 500 risorse per il processo di esportazione.

Dynamic Media Classic tiene traccia dei processi di esportazione nella schermata Processi.

**Per esportare le risorse da Dynamic Media Classic**

1. Selezionate le risorse da esportare e scegliete **File** > **Esporta**.
1. Nella finestra Esporta risorse selezionate, fate clic su **Opzioni immagini** e specificate una delle seguenti opzioni (gli amministratori stabiliscono quali opzioni rendere disponibili agli utenti):

   * **Predefiniti** Facoltativamente, scegliete un predefinito per immagini per formattare la risorsa al momento dell’esportazione. Se scegliete un predefinito per immagini, le altre opzioni di formattazione non sono disponibili, poiché vengono adottati i formati specificati dal predefinito.

   * **Conversione** Consente di convertire il file di risorsa o l’immagine originale.

   * **Dimensioni**&#x200B;È possibile selezionare una dimensione standard. In alternativa, potete fare clic su Altro nell’elenco a discesa Dimensione, scegliere l’unità di misura desiderata e specificare la larghezza e l’altezza.

      Consultate anche [Specifica delle opzioni di esportazione disponibili per gli utenti di Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **Formato** Consente di scegliere un formato immagine.

   * **Colore** Scegliete RGB, CMYK o Grigio.

   * **Risoluzione** Scegliete 72, 150 o 300 ppi.

   * **Nome** processo È possibile assegnare un nome di processo all’esportazione.

   * **Invia e-mail a** facoltativamente, immettete un indirizzo e-mail per inviare le risorse tramite e-mail. Nel messaggio e-mail viene riportato l’URL mediante il quale il destinatario può scaricare le risorse.

1. Fate clic su **Esporta**.

Sono supportate tre azioni di esportazione di base:

* File originale (esporta il file originale della risorsa)
* Converti con predefinito (formatta la risorsa mediante un predefinito per immagini)
* Converti senza predefinito (specificate i modificatori per immagini nella finestra di dialogo di esportazione)

Non è possibile esportare i seguenti tipi di risorsa. Con tutti gli altri tipi dovrebbe essere possibile generare un output di esportazione.

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
* PDF (vengono generate pagine convertite)
* PostScript

Se si selezionano numerosi elementi da esportare e di tipi di risorse diversi, si possono verificare i seguenti comportamenti:

* Tutti i tipi di risorse che non possono essere esportati vengono rimossi dall’elenco prima dell’invio del processo
* Se viene richiesta una conversione, vengono elaborati tutti i tipi che possono essere convertiti; gli altri vengono invece esportati come file originali
