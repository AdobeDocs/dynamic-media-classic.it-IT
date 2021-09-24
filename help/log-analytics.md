---
title: Accedere ad Adobe Analytics
description: Scopri come accedere ad Adobe Analytics da Adobe Dynamic Media Classic.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: d18dbbf89a1bfe4df46cbe7d56cdf6f442595ddb
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 1%

---

# Accedere ad Adobe Analytics{#log-in-to-adobe-analytics}

Prima di accedere per configurare i rapporti di Adobe Analytics e far corrispondere le variabili dei rapporti di Adobe Analytics agli eventi di Adobe Dynamic Media Classic, verifica di essere membro del gruppo Accesso ai servizi Web in Adobe Analytics. I membri di questo gruppo possono accedere a tutti i rapporti nelle suite di rapporti specificate tramite l’API Web Services di Experience Cloud, indipendentemente dalle autorizzazioni impostate nell’interfaccia. Per aggiungere un membro al gruppo, in Adobe Analytics vai a **[!UICONTROL Strumenti di amministrazione]** > **[!UICONTROL Gestione utente]** > **[!UICONTROL Modifica gruppi]**.

Quando effettui l’accesso, puoi immettere l’ID organizzazione Experience Cloud per utilizzare la più recente implementazione di video analytics. Se scegli di non inserire il tuo ID, la generazione di rapporti video continuerà a funzionare. Tuttavia, può causare l’errata integrazione dei dati con altri dati per quel client dall’esterno di Adobe Dynamic Media Classic.

>[!NOTE]
>
>Se l’account Adobe Analytics è stato migrato all’autenticazione basata su Adobe IMS (Identity Management System) per l’accesso, l’immissione delle credenziali dirette non funziona.

**Per accedere ad Adobe Analytics da Adobe Dynamic Media Classic:**

Inizia integrando Dynamic Media Classic con Adobe Analytics OAuth. L’integrazione di Adobe Analytics OAuth con Dynamic Media Classic viene in genere eseguita una sola volta per utente.

1. Accedi a [Adobe Developer Console](https://developer.adobe.com/console). Assicurati che il tuo account disponga delle autorizzazioni di amministratore per l’organizzazione per la quale è richiesta l’integrazione.
1. Seleziona l’azienda appropriata dall’elenco a discesa nell’angolo in alto a destra della home page. (La schermata seguente è a solo scopo informativo; il nome effettivo della società selezionato può variare.)

   ![Crea un nuovo progetto](assets/analytics-oauth1.png)

1. Effettua una delle seguenti operazioni:

   * Nella parte superiore della pagina, dalla scheda **[!UICONTROL Home]** , seleziona **[!UICONTROL Crea nuovo progetto]**.
   * Nella parte superiore della pagina, dalla scheda **[!UICONTROL Progetti]** . Nell’angolo a destra della pagina, seleziona **[!UICONTROL Crea nuovo progetto]**.

1. Nella pagina del progetto, seleziona **[!UICONTROL Aggiungi API]**.
1. Nella pagina **[!UICONTROL Aggiungi un API]**, seleziona **[!UICONTROL Adobe Analytics]**.
1. Nell&#39;angolo in basso a destra della pagina, seleziona **[!UICONTROL Avanti]**.

   ![Aggiungere un’API](assets/analytics-oauth2.png)

1. Nella pagina **[!UICONTROL Configura API]**, seleziona **[!UICONTROL AUTENTICAZIONE UTENTE OAuth]**.
1. Nell&#39;angolo in basso a destra della pagina, seleziona **[!UICONTROL Avanti]**.
1. Nella pagina **[!UICONTROL Configura API]**, seleziona **[!UICONTROL OAUTH 2.0 Web]**.
1. Nel campo di testo **[!UICONTROL URI di reindirizzamento predefinito]**, immetti il percorso seguente esattamente come mostrato:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. Nel campo di testo **[!UICONTROL Pattern URI di reindirizzamento]**, immetti il percorso seguente esattamente come mostrato:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Nell&#39;angolo in basso a destra della pagina, seleziona **[!UICONTROL Salva API configurata]**.
1. Nel pannello di navigazione, sul lato sinistro della pagina Adobe Analytics, in **[!UICONTROL Credenziali]**, seleziona **[!UICONTROL OAuth Web]**.
1. In **[!UICONTROL Dettagli credenziali]**, procedi come segue:
   * In **[!UICONTROL ID client]**, seleziona **[!UICONTROL Copia]** per copiare il valore. Questo valore è necessario per la successiva configurazione di Analytics nell’applicazione desktop Dynamic Media Classic che verrà seguita.
   * In **[!UICONTROL Segreto client]**, seleziona **[!UICONTROL Recupera segreto client]** per visualizzare il valore associato. Seleziona **[!UICONTROL Copia]** per copiare il valore. È necessario questo valore per la successiva configurazione di Adobe Analytics nell’applicazione desktop Dynamic Media Classic che verrà seguita.

**Configurare Adobe Analytics nell’applicazione desktop Dynamic Media Classic**

>[!NOTE]
>
>Dopo la configurazione iniziale di Adobe Analytics in Dynamic Media Classic, l’unica volta che è necessario ripristinare la configurazione è nei casi seguenti:
>
>* In Analytics viene aggiunto un nuovo rapporto e l’utente desidera iniziare a inviare i dati a tale nuovo rapporto.
>* Il server di tracciamento viene aggiornato in Adobe Analytics.
>* Una nuova variabile di tracciamento viene introdotta in un rapporto e desideri collegare una variabile Visualizzatore specifica nell’interfaccia utente di Dynamic Media Classic a tale nuova variabile di Analytics.

>


1. Nell&#39;angolo in alto a destra dell&#39;applicazione desktop Adobe Dynamic Media Classic, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]**.
1. Nel pannello a sinistra, in **[!UICONTROL Impostazione applicazione]**, selezionare **[!UICONTROL Adobe Analytics]**.
1. Nella pagina **[!UICONTROL Configurazione Adobe Analytics]**, seleziona **[!UICONTROL Accesso Adobe Analytics]**.
1. Nella finestra di dialogo **[!UICONTROL Accesso Adobe Analytics]**, incollare i rispettivi valori copiati in precedenza nel campo ID client e nel campo Segreto client .
1. Esegui l’accesso IMS.

   Una volta effettuato l&#39;accesso, diventa visibile l&#39;elenco a discesa **[!UICONTROL COMPANIES]**, avviato dalle aziende disponibili.

1. Dall&#39;elenco a discesa **[!UICONTROL AZIENDE]** , scegli una società.

   Dopo aver selezionato una società, diventa visibile l&#39;elenco a discesa **[!UICONTROL SUITES]**, avviato dalle suite di rapporti disponibili per la società selezionata.

1. Dall&#39;elenco a discesa **[!UICONTROL SUITES]** , scegli una suite di rapporti.

   >[!NOTE]
   >
   >Per impostazione predefinita, l’utente deve essere consapevole del fatto che gli elenchi a discesa **[!UICONTROL COMPANIES]** e **[!UICONTROL SUITES]** sono vuoti. Di conseguenza, l’utente deve selezionare un valore da ciascun elenco. —>

1. Seleziona **[!UICONTROL OK]** per salvare la configurazione.

>[!MORELIKETHIS]
>
>* [Configurare i rapporti di Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

