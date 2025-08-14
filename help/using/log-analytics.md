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
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Accedere ad Adobe Analytics{#log-in-to-adobe-analytics}

Verifica di essere membro del gruppo con accesso ai servizi Web in Adobe Analytics. Esegui questa operazione prima di accedere per configurare i rapporti di Adobe Analytics e far corrispondere le variabili di rapporto di Adobe Analytics agli eventi di Adobe Dynamic Media Classic. I membri di questo gruppo possono accedere a tutti i rapporti nelle suite di rapporti specificate. Puoi farlo utilizzando l’API dei servizi web di Experience Cloud, indipendentemente dalle autorizzazioni impostate nell’interfaccia. Per aggiungere un membro al gruppo, in Adobe Analytics vai a **[!UICONTROL Strumenti di amministrazione]** > **[!UICONTROL Gestione utente]** > **[!UICONTROL Modifica gruppi]**.

Quando effettui l’accesso, puoi inserire l’ID organizzazione di Experience Cloud per utilizzare l’implementazione di analisi video più recente. Se scegli di non inserire l&#39;ID, la generazione di rapporti video continua a funzionare. Tuttavia, può causare la mancata integrazione dei dati con altri dati per quel client dall’esterno di Adobe Dynamic Media Classic.

>[!NOTE]
>
>Se è stata effettuata la migrazione dell’account Adobe Analytics all’autenticazione basata su Adobe IMS (Identity Management System) per l’accesso, l’immissione delle credenziali dirette non funziona.

## Accedere ad Adobe Analytics da Adobe Dynamic Media Classic {#log-in-to-analytics-from-dmc}

Inizia integrando Dynamic Media Classic con Adobe Analytics OAuth. L’integrazione di Adobe Analytics OAuth con Dynamic Media Classic in genere viene eseguita una sola volta per utente.

1. Accedi a [Adobe Developer Console](https://developer.adobe.com/console). Assicurati che il tuo account disponga delle autorizzazioni di amministratore per l’organizzazione per la quale è richiesta l’integrazione.
1. Selezionare la società appropriata dall&#39;elenco a discesa nell&#39;angolo superiore destro della home page. La schermata seguente ha solo scopo informativo; il nome effettivo della società che selezioni può variare.

   ![Crea un nuovo progetto](assets/analytics-oauth1.png)

1. Effettuare una delle seguenti operazioni:

   * Nella parte superiore della pagina, dalla scheda **[!UICONTROL Home]**, seleziona **[!UICONTROL Crea nuovo progetto]**.
   * Nella parte superiore della pagina, dalla scheda **[!UICONTROL Progetti]**. Nell&#39;angolo destro della pagina, seleziona **[!UICONTROL Crea nuovo progetto]**.

1. Nella pagina del progetto, seleziona **[!UICONTROL Aggiungi API]**.
1. Nella pagina **[!UICONTROL Aggiungi API]**, seleziona **[!UICONTROL Adobe Analytics]**.
1. Seleziona **[!UICONTROL Avanti]** nell&#39;angolo inferiore destro della pagina.

   ![Aggiungi un&#39;API](assets/analytics-oauth2.png)

1. Nella pagina **[!UICONTROL `Configure API`]**, seleziona **[!UICONTROL AUTENTICAZIONE UTENTE OAuth]**.
1. Seleziona **[!UICONTROL Avanti]** nell&#39;angolo inferiore destro della pagina.
1. Nella pagina **[!UICONTROL `Configure API`]**, selezionare **[!UICONTROL OAUTH 2.0 Web]**.
1. Nel campo di testo **[!UICONTROL URI di reindirizzamento predefinito]**, immettere il seguente percorso esattamente come mostrato:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. Nel campo di testo **[!UICONTROL Schema URI di reindirizzamento]**, immettere il percorso seguente esattamente come mostrato:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Nell&#39;angolo inferiore destro della pagina, seleziona **[!UICONTROL Salva API configurata]**.
1. Nel pannello di navigazione, sul lato sinistro della pagina Adobe Analytics, in **[!UICONTROL Credenziali]**, seleziona **[!UICONTROL Web OAuth]**.
1. In **[!UICONTROL Dettagli credenziali]** eseguire le operazioni seguenti:
   * In **[!UICONTROL ID client]**, seleziona **[!UICONTROL Copia]** per copiare il valore. È necessario questo valore per la successiva configurazione di Analytics nell’applicazione desktop Dynamic Media Classic che deve seguire.
   * In **[!UICONTROL Segreto client]**, selezionare **[!UICONTROL Recupera segreto client]** per visualizzare il valore associato. Seleziona **[!UICONTROL Copia]** per copiare il valore. Questo valore è necessario per la successiva configurazione di Adobe Analytics nell’applicazione desktop Dynamic Media Classic che deve seguire.

## Configurare Adobe Analytics in Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Dopo la configurazione iniziale di Adobe Analytics in Dynamic Media Classic, l’unica volta che devi ripetere la configurazione è nei seguenti casi:
>
>* In Analytics viene aggiunto un nuovo rapporto e l’utente desidera iniziare a inviare dati a quel nuovo rapporto.
>* Il server di tracciamento viene aggiornato in Adobe Analytics.
>* In un rapporto viene introdotta una nuova variabile di tracciamento e desideri collegare una variabile Viewer specifica nell’interfaccia utente di Dynamic Media Classic a tale nuova variabile di Analytics.
>

1. Nell&#39;angolo superiore destro dell&#39;applicazione desktop Adobe Dynamic Media Classic, passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]**.
1. Nel pannello a sinistra, in **[!UICONTROL Configurazione applicazione]**, seleziona **[!UICONTROL Adobe Analytics]**.
1. Nella pagina **[!UICONTROL Configurazione Adobe Analytics]**, seleziona **[!UICONTROL Accesso Adobe Analytics]**.
1. Nella finestra di dialogo **[!UICONTROL Accesso Adobe Analytics]**, incolla i rispettivi valori copiati in precedenza nel campo **[!UICONTROL ID CLIENT]** e nel campo **[!UICONTROL SEGRETO CLIENT]**.
1. Nell&#39;angolo inferiore destro della finestra di dialogo, seleziona **[!UICONTROL Accedi]** ed esegui l&#39;accesso ad Adobe IMS (Identity Management Services).

   Dopo aver effettuato l&#39;accesso, viene nuovamente visualizzata la finestra di dialogo Accesso ad Adobe Analytics insieme all&#39;elenco a discesa **[!UICONTROL COMPANIES]**, avviato dalle società disponibili.

1. Scegliere un&#39;azienda dall&#39;elenco a discesa **[!UICONTROL AZIENDE]**.

   Dopo aver selezionato una società, diventa visibile l&#39;elenco a discesa **[!UICONTROL SUITE]**, avviato dalle suite di rapporti disponibili per la società selezionata.

1. Dall&#39;elenco a discesa **[!UICONTROL SUITE]**, scegli una suite di rapporti.

   >[!NOTE]
   >
   >Per impostazione predefinita, l&#39;utente deve essere consapevole del fatto che gli elenchi a discesa **[!UICONTROL COMPANIES]** e **[!UICONTROL SUITES]** sono vuoti. Di conseguenza, l’utente deve selezionare un valore da ciascun elenco.

1. Selezionare **[!UICONTROL OK]** per salvare la configurazione.

   >[!NOTE]
   >
   >Il campo **[!UICONTROL Adobe Analytics Server]** viene compilato con un server di tracciamento di terze parti consigliato che corrisponde allo spazio dei nomi Analytics quando si seleziona **[!UICONTROL OK]**. Se utilizzi un server di tracciamento diverso, aggiornalo in questo campo per evitare la perdita di dati.

1. Nell&#39;angolo in basso a sinistra della pagina Configurazione di Adobe Analytics, seleziona **[!UICONTROL Salva]** per assicurarti che la configurazione dell&#39;account Adobe Analytics sia aggiornata.

>[!MORELIKETHIS]
>
>* [Configurare i rapporti di Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
