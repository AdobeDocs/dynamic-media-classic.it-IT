---
title: Gestione della cartella Cestino
description: Scopri come gestire la cartella Cestino.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 31%

---

# Gestione della cartella Cestino{#managing-the-trash-folder}

Gli elementi eliminati da Adobe Systems Dynamic Media Classic vengono spostati nella cartella Cestino. Gli eliminati rimangono in questa cartella per sette giorni finché non vengono ripristinati o eliminati definitivamente. Puoi esaminare gli elementi eliminati facendo clic **[!UICONTROL sull&#39;icona del cestino]** nella parte inferiore della libreria delle risorse e visualizzando gli elementi nella pagina della cartella Cestino.

Tutti gli utenti possono ripristinare gli elementi della cartella Cestino alle cartelle da cui sono stati eliminati. Possono inoltre svuotare la cartella Cestino di tutto il suo contenuto.

L&#39;eliminazione di elementi dalla cartella Cestino Elimina definitivamente gli elementi da Adobe Systems Dynamic Media Classic; gli elementi eliminati dalla cartella Cestino non possono più essere ripristinati. Per informazioni sulla configurazione delle notifiche per gli amministratori della società quando le risorse stanno per essere eliminate automaticamente dal Cestino, consultate [Impostazioni generali applicazione](application-setup.md#general_settings).

>[!NOTE]
>
>Assets che sono stati spostati nella cartella Cestino sono ancora registrati su Adobe Systems Dynamic Media Classic. Se tenti di caricare un file con lo stesso nome di un file eliminato nella cartella Cestino, Adobe Systems Dynamic Media Classic tratta il risorsa che desideri caricare come risorsa duplicato. e aggiunge un numero al nome.

## La cartella Cestino {#about-the-trash-folder}

Se eliminate un elemento di una cartella, questo viene inserito nella cartella Cestino e si verifica quanto segue:

* Anche se l&#39;elemento è stato rimosso dal Adobe Systems Dynamic Media cartelle classiche, il suo ID non può essere assegnato a un altro risorsa mentre rimane nella cartella Cestino. Se tenti di caricare un risorsa con lo stesso nome di un file nella cartella Cestino, Adobe Systems Dynamic Media Classic aggiunge un numerale al nome del risorsa.
* L’elemento non può essere pubblicato. Anche se l’elemento era contrassegnato per la pubblicazione al momento in cui è stato eliminato, non verrà pubblicato.
* L&#39;elemento rimane nella cartella Cestino fino a quando non viene ripristinato, passano sette giorni o qualcuno sceglie il **[!UICONTROL vuoto del comando cestino]** . Trascorsi sette giorni, l’elemento viene eliminato automaticamente da un’operazione di pulizia automatica.

## Ripristina risorse dalla cartella Cestino {#restoring-assets-from-the-trash-folder}

Non è necessario per la persona che ha eliminato un risorsa per ripristinarla; chiunque può ripristinare risorse dalla cartella Cestino. Le risorse ripristinate vengono riportate nelle cartelle da cui erano state eliminate. Se queste cartelle non esistono più, Adobe Systems Dynamic Media Classic le ricrea e le risorse ripristinate vengono inserite nelle cartelle ricreate.

Per ripristinare risorse dalla cartella Cestino alle cartelle da cui sono stati eliminati, procedi come segue:

1. Nella parte inferiore del pannello Libreria risorse, selezionate l&#39; **[!UICONTROL icona Cestino]** per aprire la cartella Cestino.
1. Seleziona il risorsa o risorse da ripristinare.
1. Vai a **[!UICONTROL file]** > **[!UICONTROL Ripristina dal Cestino]** .

## Eliminazione definitiva delle risorse nella cartella Cestino {#permanently-deleting-assets-in-the-trash-folder}

Quando eliminate le risorse nella cartella Cestino, queste vengono eliminate definitivamente. Le risorse vengono eliminate automaticamente dalla cartella Cestino dopo sette giorni.

Per eliminare definitivamente risorse dalla cartella Cestino, selezionate l&#39; **[!UICONTROL icona Cestino]** . Nella pagina cartella Cestino, effettuate una delle seguenti operazioni:

* **Eliminazione di singoli risorse** -Seleziona le risorse che desideri eliminare definitivamente, quindi vai a **[!UICONTROL file]** > **[!UICONTROL Empty dal Cestino]** .

* **Eliminazione di tutti i risorse** -Vai a **[!UICONTROL file]** > **[!UICONTROL Cestino]** vuoto.

>[!MORELIKETHIS]
>
>* [Eliminare le risorse](moving-renaming-deleting-assets.md#delete_assets)

