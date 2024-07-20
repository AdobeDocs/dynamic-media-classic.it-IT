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
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 28%

---

# Gestire la cartella Cestino{#managing-the-trash-folder}

Gli elementi eliminati da Adobe Dynamic Media Classic vengono spostati nella cartella Cestino. Gli elementi eliminati rimangono nella cartella per sette giorni finché non vengono ripristinati o eliminati definitivamente. Per esaminare gli elementi eliminati, seleziona l&#39;icona **[!UICONTROL Cestino]** nella parte inferiore della Libreria risorse e visualizza gli elementi nella pagina della cartella Cestino.

Tutti gli utenti possono ripristinare gli elementi della cartella Cestino alle cartelle da cui sono stati eliminati. Possono inoltre svuotare la cartella Cestino di tutto il suo contenuto.

L&#39;eliminazione di elementi dalla cartella Cestino comporta l&#39;eliminazione definitiva di elementi da Adobe Dynamic Media Classic. Gli elementi eliminati dalla cartella Cestino non potranno più essere ripristinati. Per informazioni sulla configurazione delle notifiche per gli amministratori della società quando le risorse stanno per essere eliminate automaticamente dal Cestino, consultate [Impostazioni generali applicazione](application-setup.md#general_settings).

>[!NOTE]
>
>Assets che sono stati spostati nella cartella Cestino sono ancora registrati su Adobe Dynamic Media Classic. Si supponga, ad esempio, di provare a caricare un file con lo stesso nome di un file eliminato nella cartella Cestino. Adobe Dynamic Media Classic tratta la risorsa da caricare come risorsa duplicata. In tal caso, al suo nome viene aggiunto un numero.

## La cartella Cestino {#about-the-trash-folder}

Se eliminate un elemento di una cartella, questo viene inserito nella cartella Cestino e si verifica quanto segue:

* Anche se l’elemento viene rimosso dalla cartella Adobe Dynamic Media Classic, il relativo ID non può essere assegnato a un’altra risorsa finché rimane nella cartella Cestino. Se tenti di caricare una risorsa con lo stesso nome di un file nella cartella Cestino, Adobe Dynamic Media Classic aggiunge un numero al nome della risorsa.
* L’elemento non può essere pubblicato. Anche se l’elemento era contrassegnato per la pubblicazione al momento in cui è stato eliminato, non verrà pubblicato.
* L&#39;elemento rimane nella cartella Cestino finché non viene ripristinato, trascorrono sette giorni oppure un utente sceglie il comando **[!UICONTROL Svuota cestino]**. Trascorsi sette giorni, l’elemento viene eliminato automaticamente da un’operazione di pulizia automatica.

## Ripristinare le risorse dalla cartella Cestino {#restoring-assets-from-the-trash-folder}

Non è necessario che la persona che ha eliminato una risorsa la ripristini; chiunque può ripristinare le risorse dalla cartella Cestino. Le risorse ripristinate vengono riportate nelle cartelle da cui erano state eliminate. Se queste cartelle non esistono più, Adobe Dynamic Media Classic le ricrea e le risorse ripristinate vengono inserite nelle cartelle ricreate.

Per ripristinare le risorse dalla cartella Cestino alle cartelle da cui sono state eliminate, effettua le seguenti operazioni:

1. Nella parte inferiore del pannello Libreria risorse, seleziona l&#39;icona **[!UICONTROL Cestino]** per aprire la cartella Cestino.
1. Seleziona la risorsa o le risorse da ripristinare.
1. Vai a **[!UICONTROL File]** > **[!UICONTROL Ripristina dal cestino]**.

## Eliminazione definitiva delle risorse nella cartella Cestino {#permanently-deleting-assets-in-the-trash-folder}

Quando eliminate le risorse nella cartella Cestino, queste vengono eliminate definitivamente. Le risorse vengono eliminate automaticamente dalla cartella Cestino dopo sette giorni.

È possibile eliminare definitivamente le risorse dalla cartella Cestino selezionando l&#39;icona **[!UICONTROL Cestino]**. Nella pagina Cartella cestino eseguire una delle operazioni seguenti:

* **Eliminazione di singole risorse**: è possibile eliminare definitivamente le risorse. Seleziona le risorse desiderate, quindi fai clic su **[!UICONTROL File]** > **[!UICONTROL Svuota dal cestino]**.

* **Eliminazione di tutte le risorse**: vai a **[!UICONTROL File]** > **[!UICONTROL Svuota cestino]**.

>[!MORELIKETHIS]
>
>* [Elimina risorse](moving-renaming-deleting-assets.md#delete_assets)
