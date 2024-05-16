---
title: Gestire la cartella Cestino
description: Scopri come gestire la cartella Cestino.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 30%

---

# Gestire la cartella Cestino{#managing-the-trash-folder}

Gli elementi eliminati da Adobe Dynamic Media Classic vengono spostati nella cartella Cestino. Gli elementi eliminati rimangono nella cartella per sette giorni finché non vengono ripristinati o eliminati definitivamente. Puoi esaminare gli elementi eliminati selezionando la **[!UICONTROL Cestino]** nella parte inferiore della libreria delle risorse e visualizzazione degli elementi nella pagina Cartella cestino.

Tutti gli utenti possono ripristinare gli elementi della cartella Cestino alle cartelle da cui sono stati eliminati. Possono inoltre svuotare la cartella Cestino di tutto il suo contenuto.

L&#39;eliminazione di elementi dalla cartella Cestino comporta l&#39;eliminazione definitiva di elementi da Adobe Dynamic Media Classic. Gli elementi eliminati dalla cartella Cestino non potranno più essere ripristinati. Per informazioni sulla configurazione delle notifiche per gli amministratori della società quando le risorse stanno per essere eliminate automaticamente dal Cestino, consultate [Impostazioni generali applicazione](application-setup.md#general_settings).

>[!NOTE]
>
>Le risorse che sono state spostate nella cartella Cestino sono ancora registrate in Adobe Dynamic Media Classic. Se tenti di caricare un file con lo stesso nome di un file eliminato nella cartella Cestino, Adobe Dynamic Media Classic considera la risorsa da caricare come una risorsa duplicata. e aggiunge un numero al nome.

## La cartella Cestino {#about-the-trash-folder}

Se eliminate un elemento di una cartella, questo viene inserito nella cartella Cestino e si verifica quanto segue:

* Anche se l’elemento viene rimosso dalla cartella Adobe Dynamic Media Classic, il relativo ID non può essere assegnato a un’altra risorsa finché rimane nella cartella Cestino. Se tenti di caricare una risorsa con lo stesso nome di un file nella cartella Cestino, Adobe Dynamic Media Classic aggiunge un numero al nome della risorsa.
* L’elemento non può essere pubblicato. Anche se l’elemento era contrassegnato per la pubblicazione al momento in cui è stato eliminato, non verrà pubblicato.
* L&#39;elemento rimane nella cartella Cestino finché non viene ripristinato, non trascorrono sette giorni o l&#39;utente sceglie **[!UICONTROL Svuotare il cestino]** comando. Trascorsi sette giorni, l’elemento viene eliminato automaticamente da un’operazione di pulizia automatica.

## Ripristinare le risorse dalla cartella Cestino {#restoring-assets-from-the-trash-folder}

Non è necessario che la persona che ha eliminato una risorsa la ripristini; chiunque può ripristinare le risorse dalla cartella Cestino. Le risorse ripristinate vengono riportate nelle cartelle da cui erano state eliminate. Se queste cartelle non esistono più, Adobe Dynamic Media Classic le ricrea e le risorse ripristinate vengono inserite nelle cartelle ricreate.

Per ripristinare le risorse dalla cartella Cestino alle cartelle da cui sono state eliminate, effettua le seguenti operazioni:

1. Nella parte inferiore del pannello Libreria risorse, seleziona **[!UICONTROL Cestino]** per aprire la cartella Cestino.
1. Seleziona la risorsa o le risorse da ripristinare.
1. Vai a **[!UICONTROL File]** > **[!UICONTROL Ripristina dal cestino]**.

## Eliminazione definitiva delle risorse nella cartella Cestino {#permanently-deleting-assets-in-the-trash-folder}

Quando eliminate le risorse nella cartella Cestino, queste vengono eliminate definitivamente. Le risorse vengono eliminate automaticamente dalla cartella Cestino dopo sette giorni.

Per eliminare definitivamente le risorse dalla cartella Cestino, seleziona la **[!UICONTROL Cestino]** icona. Nella pagina Cartella cestino eseguire una delle operazioni seguenti:

* **Eliminazione di singole risorse**: seleziona le risorse da eliminare definitivamente, quindi vai a **[!UICONTROL File]** > **[!UICONTROL Svuota dal cestino]**.

* **Eliminazione di tutte le risorse**: vai a **[!UICONTROL File]** > **[!UICONTROL Svuota cestino]**.

>[!MORELIKETHIS]
>
>* [Eliminare risorse](moving-renaming-deleting-assets.md#delete_assets)
