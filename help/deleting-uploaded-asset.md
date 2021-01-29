---
title: Eliminazione di una risorsa caricata
description: Scoprite come eliminare una risorsa caricata.
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 88%

---


# Eliminazione di una risorsa caricata{#deleting-an-uploaded-asset}

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
|--- |--- |--- |
| op | Obbligatorio | delete |
| shared_secret | Obbligatorio | Chiave segreta condivisa della società. |
| <ul><li>Per immagini:nome_immagine</li><li>Per risorse vettoriali:fxg_name</li></ul> | Obbligatorio | Nome della risorsa da eliminare. |

**URL immagine campione:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Esempio di URL vettoriale:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
