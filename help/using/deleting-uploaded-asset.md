---
title: Eliminare una risorsa immagine raster caricata
description: Scopri come eliminare una risorsa caricata in Adobe Dynamic Media Classic.
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 52%

---

# Eliminare una risorsa caricata{#deleting-an-uploaded-asset}

Per eliminare una risorsa potete usare il parametro `delete`, come segue:

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Di seguito è riportato un esempio di una risposta a seguito dell’eliminazione di una risorsa immagine:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>delete</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Delete request for1442564.tif</title> 
            <message>Your file was successfully deleted</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Nella stringa query URL potete usare i seguenti campi per eliminare una risorsa:

| Parametro URL | Obbligatorio/facoltativo | Valore |
| --- | --- | --- |
| `op` | Obbligatorio | delete |
| `shared_secret` | Obbligatorio | Chiave segreta condivisa della società. |
| `image_name` | Obbligatorio | Nome della risorsa da eliminare. |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>A partire dal 1° maggio 2023, le risorse UGC in Dynamic Media saranno disponibili per l’uso fino a 60 giorni dalla data di caricamento. Dopo 60 giorni, le risorse verranno rimosse.

>[!NOTE]
>
>Il supporto per risorse di immagini vettoriali UGC nuove o esistenti in Adobe Dynamic Media Classic è terminato il 30 settembre 2021.

**URL immagine campione:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
