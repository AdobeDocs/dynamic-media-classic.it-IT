---
title: Specificare le opzioni di esportazione disponibili per gli utenti di Media Portal
description: Scopri come specificare le opzioni di esportazione disponibili per gli utenti di Media Portal in Adobe Dynamic Media Classic.
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 70%

---

# Specificare le opzioni di esportazione disponibili per gli utenti di Media Portal {#specifying-export-options-available-to-media-portal-users}

Se l’amministratore assegna le relative autorizzazioni, gli utenti di Media Portal possono riformattare le immagini al momento dell’esportazione. Ad esempio, possono modificarne le dimensioni, il formato file e la qualità. La riformattazione automatica delle immagini durante l’esportazione consente di risparmiare tempo evitando di dover riformattare le immagini singolarmente. Inoltre, gli amministratori possono creare un predefinito, ossia una raccolta di impostazioni preconfigurate per il formato delle immagini. Quando esportate le immagini potete usare un predefinito in modo da riformattarle in base alle specifiche richieste dalla vostra società.

Se esportate le risorse di immagini mediante una conversione definita dall’utente o se esportate le immagini principali originali, tenete presenti le due limitazioni seguenti:

* Il file .zip compresso ha una dimensione massima di 1 GB per il processo di esportazione.
* Il limite massimo per il numero di risorse totali per singolo processo di esportazione è di 500 risorse.

Consulta anche [Esportare risorse da Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Per specificare le opzioni di esportazione disponibili per gli utenti di Media Portal:**

1. Nella barra di navigazione globale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti immagini]**.
1. Nella finestra Predefiniti immagine, selezionate una delle seguenti opzioni:

   * **Abilita conversione definita dall’utente** : se selezionata, questa opzione consente agli utenti di scegliere un’altra opzione dall’elenco a discesa  **** delle dimensioni nella finestra Esporta risorse selezionate. Gli utenti possono quindi scegliere un’unità di misura quali pixel o centimetri e specificare la larghezza e l’altezza desiderate. Quando esportate o scaricate questi file, i file immagine vengono riformattati.

      Se dall’elenco a discesa **[!UICONTROL Dimensione]** vengono scelti i **[!UICONTROL pixel]**, i valori di larghezza x altezza risultanti per l’immagine non possono superare i 100 milioni di pixel. Questa dimensione corrisponde a 10.000 x 10.000 pixel per un’immagine quadrata o circa 8.000 x 12.000 pixel per un’immagine con proporzioni 2x3. Questo limite di dimensione non è applicabile se esportate le immagini principali originali.

      Deselezionate questa opzione se desiderate che gli utenti possano solo scaricare i file senza modificarne il formato in fase di scaricamento.

   * **Abilita esportazione originale** : consente di esportare le immagini master originali. Nel pannello **[!UICONTROL Esporta risorse selezionate]**, gli utenti possono aprire il menu a discesa **[!UICONTROL Conversione]** e scegliere **[!UICONTROL Esporta originale]** per esportare i file originali. Deseleziona questa opzione se vuoi obbligare gli utenti a scegliere un predefinito per immagini o a scegliere le opzioni di conversione al momento dell’esportazione delle immagini.

>[!MORELIKETHIS]
>
>* [Predefiniti immagine](application-setup.md#image_presets)
>* [Scegliere le autorizzazioni di accesso ai predefiniti per immagini per un gruppo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

