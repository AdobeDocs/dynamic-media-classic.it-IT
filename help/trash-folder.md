---
title: Gestione della cartella Cestino
description: Scopri come gestire la cartella Cestino.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Gestione risorse
role: Business Practitioner
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 39%

---

# Gestione della cartella Cestino{#managing-the-trash-folder}

Gli elementi eliminati da Dynamic Media Classic vengono spostati nella cartella Cestino. I file eliminati rimangono in questa cartella per sette giorni finché non vengono ripristinati o eliminati definitivamente. Per esaminare gli elementi eliminati, fai clic sull&#39;icona **[!UICONTROL Elimina]** nella parte inferiore della libreria delle risorse e visualizza gli elementi nella pagina della cartella Cestino .

Tutti gli utenti possono ripristinare gli elementi della cartella Cestino alle cartelle da cui sono stati eliminati. Possono inoltre svuotare la cartella Cestino di tutto il suo contenuto.

L&#39;eliminazione definitiva degli elementi dalla cartella Cestino comporta l&#39;eliminazione definitiva degli elementi da Dynamic Media Classic; gli elementi eliminati dalla cartella Cestino non possono più essere ripristinati. Per informazioni sulla configurazione delle notifiche per gli amministratori della società quando le risorse stanno per essere eliminate automaticamente dal Cestino, consultate [Impostazioni generali applicazione](application-setup.md#general_settings).

>[!NOTE]
>
>Le risorse spostate nella cartella Cestino sono ancora registrate in Dynamic Media Classic. Se tenti di caricare un file con lo stesso nome di un file eliminato nella cartella Cestino, Dynamic Media Classic considera la risorsa da caricare come una risorsa duplicata. e aggiunge un numero al nome.

## La cartella Cestino {#about-the-trash-folder}

Se eliminate un elemento di una cartella, questo viene inserito nella cartella Cestino e si verifica quanto segue:

* Sebbene l’elemento sia stato rimosso dalle cartelle di Dynamic Media Classic, il relativo ID non può essere assegnato a un’altra risorsa mentre rimane nella cartella Cestino. Se tenti di caricare una risorsa con lo stesso nome di un file nella cartella Cestino, Dynamic Media Classic aggiunge un numero al nome della risorsa.
* L’elemento non può essere pubblicato. Anche se l’elemento era contrassegnato per la pubblicazione al momento in cui è stato eliminato, non verrà pubblicato.
* L&#39;elemento rimane nella cartella Cestino fino a quando non viene ripristinato, sette giorni dopo, o qualcuno sceglie il comando **[!UICONTROL Svuota il Cestino]**. Trascorsi sette giorni, l’elemento viene eliminato automaticamente da un’operazione di pulizia automatica.

## Ripristino delle risorse dalla cartella Cestino  {#restoring-assets-from-the-trash-folder}

Non è necessario che il file venga ripristinato dalla persona che lo ha eliminato: chiunque può ripristinare le risorse dalla cartella Cestino. Le risorse ripristinate vengono riportate nelle cartelle da cui erano state eliminate. Se queste cartelle non esistono più, Dynamic Media Classic le ricrea e le risorse ripristinate vengono inserite nelle cartelle ricreate.

Per ripristinare le risorse dalla cartella Cestino alle cartelle da cui sono state eliminate, procedi come segue:

1. Nella parte inferiore del pannello Libreria risorse, fai clic sull&#39;icona **[!UICONTROL Elimina]** per aprire la cartella Cestino.
1. Selezionate le risorse che desiderate ripristinare.
1. Fai clic su **[!UICONTROL File]** > **[!UICONTROL Ripristina da cestino]**.

## Eliminazione definitiva delle risorse nella cartella Cestino {#permanently-deleting-assets-in-the-trash-folder}

Quando eliminate le risorse nella cartella Cestino, queste vengono eliminate definitivamente. Le risorse vengono eliminate automaticamente dalla cartella Cestino dopo sette giorni.

Per eliminare definitivamente le risorse dalla cartella Cestino, fai clic sull&#39;icona **[!UICONTROL Cestino]** . Nella pagina della cartella Cestino eseguire una delle operazioni seguenti:

* **Eliminazione di singole risorse**  - Seleziona le risorse da eliminare definitivamente, quindi fai clic su  **[!UICONTROL File]**  >  **[!UICONTROL Elimina dal cestino]**.

* **Eliminazione di tutte le risorse**  - Fai clic su  **[!UICONTROL File]**  >  **[!UICONTROL Elimina cestino]**.

>[!MORELIKETHIS]
>
>* [Eliminare le risorse](moving-renaming-deleting-assets.md#delete_assets)

