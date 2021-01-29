---
title: Accedere ad Adobe Analytics
description: Scoprite come accedere a  Adobe Analytics.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 36%

---


# Accedere ad Adobe Analytics{#log-in-to-adobe-analytics}

Prima di accedere per configurare  rapporti Adobe Analytics e far corrispondere  variabili di rapporti Adobe Analytics agli eventi Dynamic Media Classic, verificate di essere stato aggiunto come membro del gruppo Web Service Access in  Adobe Analytics. I membri di questo gruppo possono accedere a tutti i rapporti della suite specificata tramite Marketing Cloud’s Web Services API a prescindere dalle autorizzazioni impostate nell’interfaccia. Per aggiungere un membro al gruppo, in Adobe Analytics fate clic su **Admin Tools** > **User Management** > **Edit Groups** (Strumenti amministrazione > Gestione utenti > Modifica gruppi).

Al momento dell’accesso potete immettere l’ID organizzazione Marketing Cloud per utilizzare l’implementazione di analisi video più recente. Se scegliete di non inserire l’ID, la generazione di rapporti video continua a funzionare. Tuttavia, può causare la mancata integrazione corretta dei dati con altri dati per quel client dall&#39;esterno di Dynamic Media Classic.

>[!NOTE]
>
>Se l&#39;account Adobe Analytics  è stato migrato  autenticazione basata su IMS ( Identity Management System) del Adobe per l&#39;accesso, l&#39;immissione delle credenziali dirette non funzionerà.

**Per accedere ad Adobe Analytics**

1. Vicino all&#39;angolo superiore destro della pagina Dynamic Media Classic, toccate **[!UICONTROL Configurazione > Impostazione applicazione]**.
1. Nel riquadro a sinistra, in **[!UICONTROL Impostazione applicazione]**, toccare **[!UICONTROL Adobe Analytics]**.
1. Nella  pagina Configurazione Adobe Analytics, toccare **[!UICONTROL Accesso Adobe Analytics]**.
1. Nella finestra di dialogo **[!UICONTROL Adobe Analytics Login]**, immettere il nome della società, l&#39;ID organizzazione Marketing Cloud (facoltativo), il nome utente e la chiave *segreta condivisa* nel campo di testo **[!UICONTROL Password]**.

   Puoi recuperare la chiave *segreta condivisa* dalla console di amministrazione di Analytics. Consultate [Come ottenere le credenziali API per gli account utente](https://helpx.adobe.com/analytics/kb/how-to-get-api-credentials-for-user-accounts-.html).

1. Fate clic su **[!UICONTROL Accesso]**.
1. Nel menu a discesa **[!UICONTROL Suite di rapporti]**, scegliete una suite di rapporti, quindi fate clic su **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >la prima volta che accedete ad Adobe Analytics, l’elenco a discesa Report Suite (Suite rapporti) è vuoto. e non potete quindi scegliere una suite di rapporti. Dopo il primo accesso, disconnettetevi e tornate alla schermata Adobe Analytics. Accedete di nuovo per poter scegliere una suite di rapporti.

>[!MORELIKETHIS]
>
>* [Configurazione dei rapporti di Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

