---
title: Specificare le opzioni di esportazione disponibili per gli utenti di Media Portal
description: Scopri come specificare le opzioni di esportazione disponibili per gli utenti di Media Portal in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 42%

---

# Specificare le opzioni di esportazione disponibili per gli utenti di Media Portal {#specifying-export-options-available-to-media-portal-users}

Se l’amministratore assegna le relative autorizzazioni, gli utenti di Media Portal possono riformattare le immagini al momento dell’esportazione. Ad esempio, possono modificarne le dimensioni, il formato file e la qualità. La riformattazione automatica delle immagini durante l’esportazione consente di risparmiare tempo evitando di dover riformattare le immagini singolarmente. Inoltre, gli amministratori possono creare un predefinito, ossia una raccolta di impostazioni preconfigurate per il formato delle immagini. Quando esportate le immagini potete usare un predefinito in modo da riformattarle in base alle specifiche richieste dalla vostra società.

Le due seguenti restrizioni si applicano se si esportano le risorse immagine tramite una conversione definita dall’utente o se si esportano immagini primarie originali:

* Il file .zip compresso ha una dimensione massima di 1 GB per il processo di esportazione.
* Il limite massimo per il numero di risorse totali per singolo processo di esportazione è di 500 risorse.

Vedi anche [Esportare risorse da Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Per specificare le opzioni di esportazione disponibili per gli utenti di Media Portal:**

1. Sulla barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagine]**.
1. Nella finestra Predefiniti immagine, selezionate una delle seguenti opzioni:

   * **Abilita conversione definita dall&#39;utente**: se selezionata, questa opzione consente agli utenti di scegliere un&#39;altra opzione dall&#39;elenco a discesa **[!UICONTROL Dimensioni]** nella finestra Esporta Assets selezionato. Gli utenti possono quindi scegliere un&#39;unità di misura, ad esempio pixel o centimetri, e quindi specificare la larghezza e l&#39;altezza desiderate. Quando esportate o scaricate questi file, i file immagine vengono riformattati.

     Quando si selezionano **[!UICONTROL pixel]** dall&#39;elenco a discesa **[!UICONTROL Dimensioni]**, la larghezza × l&#39;altezza dell&#39;immagine risultante non possono superare i 100 milioni di pixel. Questa dimensione equivale a 10.000 × 10.000 pixel per un&#39;immagine quadrata o a circa 8.000 × 12.000 pixel per un&#39;immagine con proporzioni 2x3. Questo limite di dimensione non si applica se si esportano immagini primarie originali.

     Deselezionare questa opzione per consentire agli utenti di scaricare i file senza riformattarli durante il download.

   * **Abilita esportazione originale**: consente di esportare le immagini primarie originali. Nel pannello **[!UICONTROL Esporta Assets]** selezionato, gli utenti possono aprire il menu a discesa **[!UICONTROL Conversione]** e scegliere **[!UICONTROL Esporta originale]** per esportare i file originali. Deselezionate questa opzione se desiderate che gli utenti debbano scegliere un predefinito per immagini o singole opzioni di conversione al momento dell’esportazione delle immagini.

>[!MORELIKETHIS]
>
>* [Predefiniti immagine](application-setup.md#image_presets)
>* [Scegli le autorizzazioni di accesso al predefinito immagine per un gruppo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)
