---
title: Ottieni informazioni sull'utilizzo del disco
description: Scopri come ottenere informazioni sull’utilizzo del disco in Adobe Dynamic Media Classic.
uuid: 01361693-53d0-4072-b7c3-f284631d28cf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6763546d-83c4-42dc-879f-6bbfc8b56482
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 77%

---

# Ottieni informazioni sull&#39;utilizzo del disco {#getting-disk-usage-information}

Per ottenere informazioni sull’utilizzo dello spazio su disco da parte di una società, potete usare il parametro `disk_info`, come segue:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Di seguito è riportato un esempio di risposta:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>disk_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Disk Information for d03b7e0b-c9dc-4c6c-af0b-419beeea1c63</title> 
            <message>Total Space available = 1395402342400 bytes. Total Space used = 0 bytes.</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Nella stringa query URL potete usare i seguenti campi per ottenere informazioni sull’utilizzo dello spazio su disco:

| Parametro URL | Obbligatorio/facoltativo | Valore |
| --- | --- | --- |
| op | Obbligatorio | disk_info |
| shared_secret | Obbligatorio | Chiave segreta condivisa della società |

L’esempio seguente illustra il codice necessario per ottenere informazioni sull’utilizzo dello spazio su disco per la società 000Company:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
