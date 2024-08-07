---
title: Integrare Adobe Dynamic Media Classic con Adobe Target Standard/Premium
description: Scopri come integrare Adobe Dynamic Media Classic con Adobe Target Standard/Premium.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# Integrare Adobe Dynamic Media Classic con Adobe Target Standard/Premium {#integrating-dmc-with-target}

Prima di integrare [!DNL Adobe Dynamic Media Classic] con [!DNL Target Standard/Premium], è necessario immettere l&#39;URL di destinazione nella schermata Impostazioni generali applicazione [!DNL Adobe Dynamic Media Classic]. Per ottenere l&#39;URL di Target e immetterlo nella pagina Impostazioni generali applicazione, eseguire le operazioni seguenti:

1. In [!DNL Adobe Experience Cloud], accedi al tuo account [!DNL Target Standard/Premium].
1. Dopo aver effettuato l&#39;accesso, nella barra degli indirizzi del browser copiare l&#39;URL fino a `.com` incluso.

   Ad esempio, se l&#39;URL *fittizio* (i percorsi degli URL contengono sempre barre in avanti, non barre rovesciate come in questo esempio) nella barra degli indirizzi è `https:\\www.myfictionalsite.com/categories/admin/home.do`, copiare solo questa parte dell&#39;URL *fittizio*: `https:\\www.myfictionalsite.com`.

1. In [!DNL Adobe Dynamic Media Classic], passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]**.
1. Nella pagina Impostazioni generali applicazione, nel campo **[!UICONTROL Nome server Test&amp;Target]**, incolla l&#39;URL copiato nel passaggio 2.
1. Seleziona **[!UICONTROL Chiudi]**.
