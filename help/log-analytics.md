---
title: Accedere ad Adobe Analytics
description: Scopri come accedere ad Adobe Analytics.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 35%

---

# Accedere ad Adobe Analytics{#log-in-to-adobe-analytics}

Prima di effettuare l&#39;accesso per configurare i rapporti di Adobe Analytics e far corrispondere le variabili dei rapporti di Adobe Analytics agli eventi di Dynamic Media Classic, verifica di essere membro del gruppo Accesso al servizio Web in Adobe Analytics. I membri di questo gruppo possono accedere a tutti i rapporti della suite specificata tramite Marketing Cloud’s Web Services API a prescindere dalle autorizzazioni impostate nell’interfaccia. Per aggiungere un membro al gruppo, in Adobe Analytics fate clic su **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]** (Strumenti amministrazione > Gestione utenti > Modifica gruppi).

Quando effettui l&#39;accesso, puoi immettere l&#39;ID organizzazione del Marketing Cloud per utilizzare la più recente implementazione di video analytics. Se scegli di non inserire il tuo ID, la generazione di rapporti video continuerà a funzionare. Tuttavia, può causare l’integrazione corretta dei dati con altri dati per quel client dall’esterno di Dynamic Media Classic.

>[!NOTE]
>
>Se l’account Adobe Analytics è stato migrato all’autenticazione basata su Adobe IMS (Identity Management System) per l’accesso, l’immissione delle credenziali dirette non funziona.

**Per accedere ad Adobe Analytics:**

1. Vicino all&#39;angolo superiore destro della pagina Dynamic Media Classic, tocca **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]**.
1. Nel riquadro a sinistra, sotto **[!UICONTROL Impostazione applicazione]**, toccare **[!UICONTROL Adobe Analytics]**.
1. Nella pagina Configurazione Adobe Analytics, tocca **[!UICONTROL Accesso Adobe Analytics]**.
1. Nella finestra di dialogo **[!UICONTROL Accesso Adobe Analytics]**, immetti il nome dell&#39;azienda, l&#39;ID organizzazione Marketing Cloud (facoltativo), il nome utente e la chiave *segreto condiviso* nel campo di testo **[!UICONTROL Password]**.

   È possibile recuperare la chiave *segreto condiviso* dall&#39;Admin Console di Analytics. Consulta [Come ottenere le credenziali API per gli account utente](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md).

1. Fate clic su **[!UICONTROL Accesso]**.
1. Nel menu a discesa **[!UICONTROL Suite di rapporti]**, scegli una suite di rapporti, quindi fai clic su **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >la prima volta che accedete ad Adobe Analytics, l’elenco a discesa Report Suite (Suite rapporti) è vuoto. e non potete quindi scegliere una suite di rapporti. Dopo il primo accesso, disconnettetevi e tornate alla schermata Adobe Analytics. Accedete di nuovo per poter scegliere una suite di rapporti.

>[!MORELIKETHIS]
>
>* [Configurazione dei rapporti di Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

