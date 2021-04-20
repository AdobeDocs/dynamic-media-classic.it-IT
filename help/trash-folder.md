---
title: Gestione della cartella Cestino
description: Scopri come gestire la cartella Cestino.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 60%

---


# Gestione della cartella Cestino{#managing-the-trash-folder}

Gli elementi eliminati da Dynamic Media Classic vengono spostati nella cartella Cestino. Se non vengono ripristinati, rimangono sette giorni in questa cartella dopodiché vengono eliminati definitivamente. Per esaminare gli elementi eliminati, fate clic sull’icona Cestino  nella parte inferiore della Libreria risorse per aprire la cartella Cestino.

Tutti gli utenti possono ripristinare gli elementi della cartella Cestino alle cartelle da cui sono stati eliminati. Possono inoltre svuotare la cartella Cestino di tutto il suo contenuto.

L&#39;eliminazione definitiva degli elementi dalla cartella Cestino comporta l&#39;eliminazione definitiva degli elementi da Dynamic Media Classic; gli elementi eliminati dalla cartella Cestino non possono più essere ripristinati. Per informazioni sulla configurazione delle notifiche per gli amministratori della società quando le risorse stanno per essere eliminate automaticamente dal Cestino, consultate [Impostazioni generali applicazione](application-setup.md#general_settings).

>[!NOTE]
>
>Le risorse spostate nella cartella Cestino sono ancora registrate in Dynamic Media Classic. Se tenti di caricare un file con lo stesso nome di un file eliminato nella cartella Cestino, Dynamic Media Classic considera la risorsa da caricare come una risorsa duplicata. e aggiunge un numero al nome.

## La cartella Cestino {#about-the-trash-folder}

Se eliminate un elemento di una cartella, questo viene inserito nella cartella Cestino e si verifica quanto segue:

* Sebbene l’elemento sia stato rimosso dalle cartelle di Dynamic Media Classic, il relativo ID non può essere assegnato a un’altra risorsa mentre rimane nella cartella Cestino. Se tenti di caricare una risorsa con lo stesso nome di un file nella cartella Cestino, Dynamic Media Classic aggiunge un numero al nome della risorsa.
* L’elemento non può essere pubblicato. Anche se l’elemento era contrassegnato per la pubblicazione al momento in cui è stato eliminato, non verrà pubblicato.
* L’elemento resta nella cartella Cestino finché non viene ripristinato, finché non sono trascorsi sette giorni, o finché un utente non sceglie il comando Svuota il cestino. Trascorsi sette giorni, l’elemento viene eliminato automaticamente da un’operazione di pulizia automatica.

## Ripristino delle risorse dalla cartella Cestino  {#restoring-assets-from-the-trash-folder}

Non è necessario che il file venga ripristinato dalla persona che lo ha eliminato: chiunque può ripristinare le risorse dalla cartella Cestino. Le risorse ripristinate vengono riportate nelle cartelle da cui erano state eliminate. Se queste cartelle non esistono più, Dynamic Media Classic le ricrea e le risorse ripristinate vengono inserite nelle cartelle ricreate.

Per ripristinare le risorse dalla cartella Cestino alle cartelle da cui erano state eliminate, effettuate le seguenti operazioni:

1. Fai clic sull&#39;icona Cestino per aprire la cartella Cestino.
1. Selezionate le risorse che desiderate ripristinare.
1. Scegliete File > Ripristina dal cestino.

## Eliminazione definitiva delle risorse nella cartella Cestino  {#permanently-deleting-assets-in-the-trash-folder}

Quando eliminate le risorse nella cartella Cestino, queste vengono eliminate definitivamente. Le risorse vengono eliminate automaticamente dalla cartella Cestino dopo sette giorni.

Per eliminare definitivamente le risorse dalla cartella Cestino, fate clic sull’icona Cestino  per aprire la cartella Cestino. Quindi, eliminate le singole risorse o tutte le risorse presenti nella cartella:

* **Eliminazione di singole** risorseSeleziona le risorse da eliminare definitivamente e fai clic su  **[!UICONTROL File > Elimina dal cestino]**.

* **Eliminazione di tutte le** risorseFai clic su  **[!UICONTROL File > Elimina cestino]**.

>[!MORELIKETHIS]
>
>* [Eliminare le risorse](moving-renaming-deleting-assets.md#delete_assets)

