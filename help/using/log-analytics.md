---
title: Accedere ad Adobe Analytics
description: Scopri come accedere ad Adobe Analytics da Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# Accedere ad Adobe Analytics{#log-in-to-adobe-analytics}

Prima di effettuare l’accesso per configurare i rapporti di Adobe Analytics e associare le variabili di rapporto di Adobe Analytics agli eventi di Adobe Dynamic Media Classic, verifica di essere membro del gruppo Accesso al servizio Web in Adobe Analytics. I membri di questo gruppo possono accedere a tutti i rapporti nelle suite di rapporti specificate tramite l’API dei servizi web di Experience Cloud, indipendentemente dalle autorizzazioni impostate nell’interfaccia. Per aggiungere un membro al gruppo, in Adobe Analytics vai a **[!UICONTROL Strumenti di amministrazione]** > **[!UICONTROL Gestione utente]** > **[!UICONTROL Modifica gruppi]**.

Quando effettui l’accesso, puoi inserire l’ID organizzazione Experience Cloud per utilizzare l’implementazione di analisi video più recente. Se scegli di non inserire l&#39;ID, la generazione di rapporti video continua a funzionare. Tuttavia, può causare la mancata integrazione corretta dei dati con altri dati per quel client dall’esterno di Adobe Dynamic Media Classic.

>[!NOTE]
>
>Se è stata effettuata la migrazione dell’account Adobe Analytics all’autenticazione basata su Adobe IMS (Identity Management System) per l’accesso, l’immissione delle credenziali dirette non funziona.

## Accedere ad Adobe Analytics da Adobe Dynamic Media Classic {#log-in-to-analytics-from-dmc}

Inizia integrando Dynamic Media Classic con Adobe Analytics OAuth. L’integrazione di Adobe Analytics OAuth con Dynamic Media Classic in genere viene eseguita una sola volta per utente.

1. Accesso [Console Adobe Developer](https://developer.adobe.com/console). Assicurati che il tuo account disponga delle autorizzazioni di amministratore per l’organizzazione per la quale è richiesta l’integrazione.
1. Selezionare la società appropriata dall&#39;elenco a discesa nell&#39;angolo superiore destro della home page. La schermata seguente ha solo scopo informativo; il nome effettivo della società che selezioni può variare.

   ![Crea un nuovo progetto](assets/analytics-oauth1.png)

1. Effettuare una delle seguenti operazioni:

   * Nella parte superiore della pagina, dalla sezione **[!UICONTROL Home]** , seleziona **[!UICONTROL Crea nuovo progetto]**.
   * Nella parte superiore della pagina, dalla sezione **[!UICONTROL Progetti]** scheda. Nell’angolo destro della pagina, seleziona **[!UICONTROL Crea nuovo progetto]**.

1. Nella pagina del progetto, seleziona **[!UICONTROL Aggiungi API]**.
1. Il giorno **[!UICONTROL Aggiungere un’API]** pagina, seleziona **[!UICONTROL Adobe Analytics]**.
1. Nell’angolo inferiore destro della pagina, seleziona **[!UICONTROL Successivo]**.

   ![Aggiungere un’API](assets/analytics-oauth2.png)

1. Il giorno **[!UICONTROL `Configure API`]** pagina, seleziona **[!UICONTROL AUTENTICAZIONE UTENTE OAuth]**.
1. Nell’angolo inferiore destro della pagina, seleziona **[!UICONTROL Successivo]**.
1. Il giorno **[!UICONTROL `Configure API`]** pagina, seleziona **[!UICONTROL Web OAUTH 2.0]**.
1. In **[!UICONTROL URI di reindirizzamento predefinito]** immetti il seguente percorso esattamente come mostrato:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. In **[!UICONTROL Pattern URI di reindirizzamento]** immetti il seguente percorso esattamente come mostrato:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Nell’angolo inferiore destro della pagina, seleziona **[!UICONTROL Salva API configurata]**.
1. Nel pannello di navigazione, sul lato sinistro della pagina Adobe Analytics, in **[!UICONTROL Credenziali]**, seleziona **[!UICONTROL Web OAuth]**.
1. Sotto **[!UICONTROL Dettagli delle credenziali]**, eseguire le operazioni seguenti:
   * Sotto **[!UICONTROL ID client]**, seleziona **[!UICONTROL Copia]** per copiare il valore. È necessario questo valore per la successiva configurazione di Analytics nell’applicazione desktop Dynamic Media Classic che deve seguire.
   * Sotto **[!UICONTROL Segreto client]**, seleziona **[!UICONTROL Recupera segreto client]** per visualizzare il valore associato. Seleziona **[!UICONTROL Copia]** per copiare il valore. È necessario questo valore per la successiva configurazione di Adobe Analytics nell’applicazione desktop Dynamic Media Classic che deve seguire.

## Configurare Adobe Analytics in Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Dopo la configurazione iniziale di Adobe Analytics in Dynamic Media Classic, l’unica volta che devi ripetere la configurazione è nei seguenti casi:
>
>* In Analytics viene aggiunto un nuovo rapporto e l’utente desidera iniziare a inviare dati a quel nuovo rapporto.
>* Il server di tracciamento viene aggiornato in Adobe Analytics.
>* In un rapporto viene introdotta una nuova variabile di tracciamento e desideri collegare una variabile Viewer specifica nell’interfaccia utente di Dynamic Media Classic a tale nuova variabile di Analytics.
>

1. Nell&#39;angolo superiore destro dell&#39;applicazione desktop Adobe Dynamic Media Classic, passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]**.
1. Nel pannello a sinistra, sotto **[!UICONTROL Impostazione applicazione]**, seleziona **[!UICONTROL Adobe Analytics]**.
1. Il giorno **[!UICONTROL Configurazione Adobe Analytics]** pagina, seleziona **[!UICONTROL Accesso ad Adobe Analytics]**.
1. In **[!UICONTROL Accesso ad Adobe Analytics]** nella finestra di dialogo **[!UICONTROL ID CLIENT]** e **[!UICONTROL SEGRETO CLIENT]** incolla i rispettivi valori copiati in precedenza.
1. Nell&#39;angolo inferiore destro della finestra di dialogo, selezionate **[!UICONTROL Login]** ed eseguire l’accesso ad Adobe IMS (Identity Management Services).

   Una volta effettuato l&#39;accesso, viene visualizzata di nuovo la finestra di dialogo Accesso ad Adobe Analytics insieme al **[!UICONTROL AZIENDE]** dall&#39;elenco a discesa, avviato dalle società disponibili.

1. Dalla sezione **[!UICONTROL AZIENDE]** scegliere un&#39;azienda.

   Dopo aver selezionato un&#39;azienda, **[!UICONTROL SUITE]** L’elenco a discesa, avviato dalle suite di rapporti disponibili per la società selezionata, diventa visibile.

1. Dalla sezione **[!UICONTROL SUITE]** scegliere una suite di rapporti.

   >[!NOTE]
   >
   >Per impostazione predefinita, l’utente deve essere consapevole del fatto che entrambi **[!UICONTROL AZIENDE]** e **[!UICONTROL SUITE]** gli elenchi a discesa sono vuoti. Di conseguenza, l’utente deve selezionare un valore da ciascun elenco.

1. Seleziona **[!UICONTROL OK]** in modo da poter salvare la configurazione.

   >[!NOTE]
   >
   >Il **[!UICONTROL Server Adobe Analytics]** viene compilato con un server di tracciamento di terze parti suggerito che corrisponde allo spazio dei nomi analytics quando selezioni **[!UICONTROL OK]**. Se utilizzi un server di tracciamento diverso, aggiornalo in questo campo per evitare la perdita di dati.

1. Nell’angolo inferiore sinistro della pagina Configurazione di Adobe Analytics, seleziona **[!UICONTROL Salva]** per assicurarti che la configurazione dell’account Adobe Analytics sia aggiornata.

>[!MORELIKETHIS]
>
>* [Configurare i rapporti di Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
