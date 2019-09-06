---
title: Specifica delle opzioni di esportazione disponibili per gli utenti di Media Portal
seo-title: Specifica delle opzioni di esportazione disponibili per gli utenti di Media Portal
description: 'null'
seo-description: Scoprite come specificare le opzioni di esportazione disponibili per gli utenti di Media Portal.
uuid: 5258 b 8 a 4-0704-43 cd -97 d 1-c 9 af 2 e 4 e 298 b
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 9 bfd 95 da -3714-4 e 38-98 af -331 a 04 c 685 f 5
translation-type: tm+mt
source-git-commit: 0f6c8e6ac69e29aab7a48425aab76c10170d9ddf

---


# Specifica delle opzioni di esportazione disponibili per gli utenti di Media Portal {#specifying-export-options-available-to-media-portal-users}

Se l’amministratore assegna le relative autorizzazioni, gli utenti di Media Portal possono riformattare le immagini al momento dell’esportazione. Ad esempio, possono modificarne le dimensioni, il formato file e la qualità. La riformattazione automatica delle immagini durante l’esportazione consente di risparmiare tempo evitando di dover riformattare le immagini singolarmente. Inoltre, gli amministratori possono creare un predefinito, ossia una raccolta di impostazioni preconfigurate per il formato delle immagini. Quando esportate le immagini potete usare un predefinito in modo da riformattarle in base alle specifiche richieste dalla vostra società.

Se esportate le risorse di immagini mediante una conversione definita dall’utente o se esportate le immagini principali originali, tenete presenti le due limitazioni seguenti:

* Il file .zip compresso ha una dimensione massima di 1 GB per il processo di esportazione.
* Il limite massimo per il numero di risorse totali per singolo processo di esportazione è di 500 risorse.

Consultate anche [Esportazione delle risorse da Scene7 Publishing System](exporting-assets-scene7-publishing-system.md#exporting_assets_from_scene7_publishing_system).

**Per specificare le opzioni di esportazione disponibili per gli utenti di Media Portal**

1. Fate clic su **Configurazione** &gt; **Predefiniti immagini**.
1. Nella finestra Predefiniti immagine, selezionate una delle seguenti opzioni:

   **Abilita conversione definita dall'utente** Quando selezionata, questa opzione consente agli utenti di scegliere Altro dall'elenco a discesa Dimensione nella finestra Esporta risorse selezionate. Gli utenti possono quindi scegliere un’unità di misura quali pixel o centimetri e specificare la larghezza e l’altezza desiderate. Quando esportate o scaricate questi file, i file immagine vengono riformattati.

   Se dall’elenco a discesa **Dimensione** vengono scelti i **pixel**, i valori di larghezza x altezza risultanti per l’immagine non possono superare i 100 milioni di pixel. Questa dimensione corrisponde a 10.000 x 10.000 pixel per un’immagine quadrata o circa 8.000 x 12.000 pixel per un’immagine con proporzioni 2x3. Questo limite di dimensione non è applicabile se esportate le immagini principali originali.

   Deselezionate questa opzione se desiderate che gli utenti possano solo scaricare i file senza modificarne il formato in fase di scaricamento.

   **Abilita esportazione originale** Consente di esportare le immagini principali originali. Nella finestra di dialogo Esporta risorse selezionate, gli utenti possono aprire il menu Conversione e scegliere Esporta originale per esportare i file originali. Deselezionate questa opzione se desiderate che gli utenti debbano scegliere un predefinito per immagini o singole opzioni di conversione al momento dell’esportazione delle immagini.

>[!MORELIKETHIS]
>
>* [Predefiniti immagine](application-setup.md#image_presets)
>* [Scegliere le autorizzazioni di accesso ai predefiniti per immagini per un gruppo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

