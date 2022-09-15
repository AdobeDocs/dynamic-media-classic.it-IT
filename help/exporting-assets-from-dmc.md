---
title: Esportare risorse da Adobe Dynamic Media Classic
description: Scopri come esportare risorse da Adobe Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 51%

---

# Esportare risorse da Adobe Dynamic Media Classic{#exporting-assets-from-dmc}

È possibile salvare le risorse modificate in Adobe Dynamic Media Classic in un&#39;unità di rete locale. Le risorse esportate vengono raccolte in un file ZIP per il download o l’invio tramite e-mail.

Il file .zip compresso ha una dimensione massima di 1 GB per il processo di esportazione. Inoltre, è consentito un massimo di 500 risorse totali per processo di esportazione.

Nella schermata Processi, Adobe Dynamic Media Classic registra i processi di esportazione.

**Per esportare le risorse da Adobe Dynamic Media Classic:**

1. Seleziona le risorse da esportare, quindi vai a **[!UICONTROL File]** > **[!UICONTROL Esporta]**.
1. Nella finestra Esporta risorse selezionate, fate clic su **[!UICONTROL Opzioni immagini]** e specificate una delle seguenti opzioni (gli amministratori stabiliscono quali opzioni rendere disponibili agli utenti):

   * **[!UICONTROL Predefiniti]** - Facoltativamente, scegli un predefinito per immagini per formattare la risorsa quando la esporti. Se scegliete un predefinito per immagini, le altre opzioni di formattazione non sono disponibili, poiché vengono adottati i formati specificati dal predefinito.

   * **[!UICONTROL Conversione]** - Convertire il file della risorsa o l&#39;immagine originale.

   * **[!UICONTROL Dimensione]** - È possibile selezionare una dimensione standard. Oppure, puoi selezionare **[!UICONTROL Altro]** dal **[!UICONTROL Dimensione]** dall’elenco a discesa, scegli l’unità di misura desiderata e specifica la larghezza e l’altezza.

      Vedi anche [Specificare le opzioni di esportazione disponibili per gli utenti di Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL Formato]** - Scegli un formato immagine.

   * **[!UICONTROL Colore]** - Scegli RGB, CMYK o Grigio.

   * **[!UICONTROL Risoluzione]** - Scegli 72 ppi, 150 ppi o 300 ppi.

   * **[!UICONTROL Nome processo]** - È possibile assegnare un nome di processo all&#39;esportazione.

   * **[!UICONTROL Invia e-mail a]** - Se si desidera inviare le risorse tramite e-mail, è possibile inserire un indirizzo e-mail. Nel messaggio e-mail viene riportato l’URL mediante il quale il destinatario può scaricare le risorse.

1. Seleziona **[!UICONTROL Esporta]**.

Sono supportate tre azioni di esportazione di base:

* File originale (esporta il file originale della risorsa)
* Converti con predefinito (formatta la risorsa mediante un predefinito per immagini)
* Converti senza predefinito (specificate i modificatori per immagini nella finestra di dialogo di esportazione)

Non è possibile esportare i seguenti tipi di risorsa. Tutti gli altri generano un’esportazione.

* Set di immagini
* Set di rendering
* Set 360 gradi
* Set di file multimediali
* Set a più byte
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
