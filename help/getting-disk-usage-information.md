---
title: Ottenimento delle informazioni sull’utilizzo dello spazio su disco
seo-title: Ottenimento delle informazioni sull’utilizzo dello spazio su disco
description: 'null'
seo-description: Scoprite come ottenere informazioni sull'utilizzo dello spazio su disco.
uuid: 01361693-53 d 0-4072-b 7 c 3-f 284631 d 28 cf
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 6763546 d -83 c 4-42 dc -879 f -6 bbfc 8 b 56482
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# Ottenimento delle informazioni sull’utilizzo dello spazio su disco {#getting-disk-usage-information}

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
|--- |--- |--- |
| op | Obbligatorio | disk_info |
| shared_secret | Obbligatorio | Chiave segreta condivisa della società |

L’esempio seguente illustra il codice necessario per ottenere informazioni sull’utilizzo dello spazio su disco per la società 000Company:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```

