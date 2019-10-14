---
title: Gestione della cartella Cestino
seo-title: Gestione della cartella Cestino
description: 'null'
seo-description: Scoprite come gestire la cartella Cestino.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/Categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Gestione della cartella Cestino{#managing-the-trash-folder}

Gli elementi eliminati da Scene7 Publishing System vengono spostati nella cartella Cestino. Se non vengono ripristinati, rimangono sette giorni in questa cartella dopodiché vengono eliminati definitivamente. Per esaminare gli elementi eliminati, fate clic sull’icona Cestino  nella parte inferiore della Libreria risorse per aprire la cartella Cestino.

Tutti gli utenti possono ripristinare gli elementi della cartella Cestino alle cartelle da cui sono stati eliminati. Possono inoltre svuotare la cartella Cestino di tutto il suo contenuto.

L’eliminazione definitiva degli elementi dalla cartella Cestino comporta l’eliminazione degli stessi da Scene7 Publishing System; gli elementi eliminati dalla cartella Cestino non possono più essere ripristinati. Per informazioni sulla configurazione delle notifiche per gli amministratori della società quando le risorse stanno per essere eliminate automaticamente dal Cestino, consultate [Impostazioni generali applicazione](application-setup.md#general_settings).

>[!NOTE]
>
>le risorse spostate nella cartella Cestino sono ancora registrate in Scene7 Publishing System. Se provate a caricare un file con lo stesso nome di un file eliminato presente nella cartella Cestino, Dynamic Media Classic considera la risorsa da caricare come una risorsa duplicata. e aggiunge un numero al nome.

## La cartella Cestino {#about-the-trash-folder}

Se eliminate un elemento di una cartella, questo viene inserito nella cartella Cestino e si verifica quanto segue:

* Sebbene l’elemento sia stato rimosso dalle cartelle di Scene7 Publishing System, il relativo ID non può essere assegnato a un’altra risorsa fintanto che l’elemento si trova nella cartella Cestino. Se provate a caricare una risorsa con lo stesso nome di un file presente nella cartella Cestino, Dynamic Media Classic aggiunge un numero al nome della risorsa.
* L’elemento non può essere pubblicato. Anche se l’elemento era contrassegnato per la pubblicazione al momento in cui è stato eliminato, non verrà pubblicato.
* L’elemento resta nella cartella Cestino finché non viene ripristinato, finché non sono trascorsi sette giorni, o finché un utente non sceglie il comando Svuota il cestino. Trascorsi sette giorni, l’elemento viene eliminato automaticamente da un’operazione di pulizia automatica.

## Ripristino delle risorse dalla cartella Cestino {#restoring-assets-from-the-trash-folder}

Non è necessario che il file venga ripristinato dalla persona che lo ha eliminato: chiunque può ripristinare le risorse dalla cartella Cestino. Le risorse ripristinate vengono riportate nelle cartelle da cui erano state eliminate. Se tali cartelle non esistono più, Scene7 Publishing System le ricrea e le risorse ripristinate vengono inserite nelle cartelle ricreate.

Per ripristinare le risorse dalla cartella Cestino alle cartelle da cui erano state eliminate, effettuate le seguenti operazioni:

1. Fate clic sull’icona Cestino per aprire la cartella Cestino.
1. Selezionate le risorse che desiderate ripristinare.
1. Scegliete File &gt; Ripristina dal cestino.

## Eliminazione definitiva delle risorse nella cartella Cestino {#permanently-deleting-assets-in-the-trash-folder}

Quando eliminate le risorse nella cartella Cestino, queste vengono eliminate definitivamente. Le risorse vengono eliminate automaticamente dalla cartella Cestino dopo sette giorni.

Per eliminare definitivamente le risorse dalla cartella Cestino, fate clic sull’icona Cestino  per aprire la cartella Cestino. Quindi, eliminate le singole risorse o tutte le risorse presenti nella cartella:

* **Eliminazione di singole risorse** Selezionate le risorse da eliminare definitivamente e fate clic su **[!UICONTROL File &gt; Elimina dal cestino]**.

* **Eliminazione di tutte le risorse** Fate clic su **[!UICONTROL File &gt; Elimina cestino]**.

>[!MORELIKETHIS]
>
>* [Eliminare le risorse](moving-renaming-deleting-assets.md#delete_assets)

