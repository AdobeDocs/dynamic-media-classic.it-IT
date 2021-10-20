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
source-git-commit: 8111895ac527b92b152382ea80b7b383659f00a9
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 1%

---

# Accedere ad Adobe Analytics{#log-in-to-adobe-analytics}

Prima di accedere per configurare i rapporti di Adobe Analytics e associare le variabili di rapporto di Adobe Analytics agli eventi di Adobe Dynamic Media Classic, verifica di essere membro del gruppo Accesso ai servizi Web in Adobe Analytics. I membri di questo gruppo possono accedere a tutti i rapporti nelle suite di rapporti specificate tramite l’API Web Services di Experience Cloud, indipendentemente dalle autorizzazioni impostate nell’interfaccia. Per aggiungere un membro al gruppo, in Adobe Analytics vai a **[!UICONTROL Strumenti di amministrazione]** > **[!UICONTROL Gestione utente]** > **[!UICONTROL Modifica gruppi]**.

Quando effettui l’accesso, puoi immettere l’ID organizzazione Experience Cloud per utilizzare la più recente implementazione di video analytics. Se scegli di non inserire il tuo ID, la generazione di rapporti video continuerà a funzionare. Tuttavia, può causare l’integrazione corretta dei dati con altri dati per quel client dall’esterno di Adobe Dynamic Media Classic.

>[!NOTE]
>
>Se l’account Adobe Analytics è stato migrato all’autenticazione basata su Adobe IMS (Identity Management System) per l’accesso, l’immissione delle credenziali dirette non funziona.

## Accedere ad Adobe Analytics da Adobe Dynamic Media Classic {#log-in-to-analytics-from-dmc}

Inizia integrando Dynamic Media Classic con Adobe Analytics OAuth. In genere, l’integrazione di Adobe Analytics OAuth con Dynamic Media Classic viene eseguita una sola volta per utente.

1. Accesso [Console per sviluppatori di Adobe](https://developer.adobe.com/console). Assicurati che il tuo account disponga delle autorizzazioni di amministratore per l’organizzazione per la quale è richiesta l’integrazione.
1. Seleziona l’azienda appropriata dall’elenco a discesa nell’angolo in alto a destra della home page. (La schermata seguente è a solo scopo informativo; il nome effettivo della società selezionato può variare.)

   ![Crea un nuovo progetto](assets/analytics-oauth1.png)

1. Effettua una delle seguenti operazioni:

   * Nella parte superiore della pagina, dalla **[!UICONTROL Pagina principale]** scheda , seleziona **[!UICONTROL Crea nuovo progetto]**.
   * Nella parte superiore della pagina, dalla **[!UICONTROL Progetti]** scheda . Nell’angolo destro della pagina, seleziona **[!UICONTROL Crea nuovo progetto]**.

1. Nella pagina del progetto, seleziona **[!UICONTROL Aggiungi API]**.
1. Sulla **[!UICONTROL Aggiungere un’API]** pagina, seleziona **[!UICONTROL Adobe Analytics]**.
1. Nell’angolo inferiore destro della pagina, seleziona **[!UICONTROL Successivo]**.

   ![Aggiungere un’API](assets/analytics-oauth2.png)

1. Sulla **[!UICONTROL Configurare l’API]** pagina, seleziona **[!UICONTROL OAuth AUTENTICAZIONE UTENTE]**.
1. Nell’angolo inferiore destro della pagina, seleziona **[!UICONTROL Successivo]**.
1. Sulla **[!UICONTROL Configurare l’API]** pagina, seleziona **[!UICONTROL OAUTH 2.0 Web]**.
1. In **[!UICONTROL URI di reindirizzamento predefinito]** campo di testo, immetti il percorso seguente esattamente come mostrato:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. In **[!UICONTROL Pattern URI di reindirizzamento]** campo di testo, immetti il percorso seguente esattamente come mostrato:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Nell’angolo inferiore destro della pagina, seleziona **[!UICONTROL Salva API configurata]**.
1. Nel pannello di navigazione, sul lato sinistro della pagina Adobe Analytics, sotto **[!UICONTROL Credenziali]**, seleziona **[!UICONTROL Web OAuth]**.
1. Sotto **[!UICONTROL Dettagli delle credenziali]**, procedi come segue:
   * Sotto **[!UICONTROL ID client]**, seleziona **[!UICONTROL Copia]** per copiare il valore. Questo valore è necessario per la successiva configurazione di Analytics nell’applicazione desktop Dynamic Media Classic che verrà seguita.
   * Sotto **[!UICONTROL Segreto client]**, seleziona **[!UICONTROL Recupera segreto client]** per visualizzare il valore associato. Seleziona **[!UICONTROL Copia]** per copiare il valore. È necessario questo valore per la successiva configurazione di Adobe Analytics nell’applicazione desktop Dynamic Media Classic che verrà seguita.

## Configurare Adobe Analytics in Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Dopo la configurazione iniziale di Adobe Analytics in Dynamic Media Classic, l’unica volta che devi ripristinare la configurazione è nei casi seguenti:
>
>* In Analytics viene aggiunto un nuovo rapporto e l’utente desidera iniziare a inviare i dati a tale nuovo rapporto.
>* Il server di tracciamento viene aggiornato in Adobe Analytics.
>* Una nuova variabile di tracciamento viene introdotta in un rapporto e desideri collegare una variabile Visualizzatore specifica nell’interfaccia utente di Dynamic Media Classic a quella nuova variabile di Analytics.

>


1. Nell’angolo in alto a destra dell’applicazione desktop Adobe Dynamic Media Classic, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]**.
1. Nel pannello a sinistra, sotto **[!UICONTROL Impostazione applicazione]**, seleziona **[!UICONTROL Adobe Analytics]**.
1. Sulla **[!UICONTROL Configurazione Adobe Analytics]** pagina, seleziona **[!UICONTROL Accesso Adobe Analytics]**.
1. In **[!UICONTROL Accesso Adobe Analytics]** nella finestra di dialogo **[!UICONTROL ID CLIENT]** e **[!UICONTROL SEGRETO CLIENT]** incollare i rispettivi valori copiati in precedenza.
1. Nell’angolo in basso a destra della finestra di dialogo, seleziona Accesso ed esegui l’accesso ad Adobe IMS (Identity Management Services).

   Quando si effettua l’accesso, viene visualizzata nuovamente la finestra di dialogo Accesso Adobe Analytics insieme alla **[!UICONTROL AZIENDE]** elenco a discesa, avviato dalle aziende disponibili.

1. Da **[!UICONTROL AZIENDE]** dall’elenco a discesa, scegli un’azienda.

   Dopo aver selezionato una società, la **[!UICONTROL SUITE]** diventa visibile l’elenco a discesa, avviato dalle suite di rapporti disponibili per l’azienda selezionata.

1. Da **[!UICONTROL SUITE]** dall’elenco a discesa, scegli una suite di rapporti.

   >[!NOTE]
   >
   >Per impostazione predefinita, l’utente deve essere consapevole del fatto che entrambi **[!UICONTROL AZIENDE]** e **[!UICONTROL SUITE]** gli elenchi a discesa sono vuoti. Di conseguenza, l’utente deve selezionare un valore da ciascun elenco.

1. Seleziona **[!UICONTROL OK]** così puoi salvare la configurazione.

   >[!NOTE]
   >
   >La **[!UICONTROL Server Adobe Analytics]** viene compilato con un server di tracciamento di terze parti consigliato che corrisponde allo spazio dei nomi di Analytics quando selezioni **[!UICONTROL OK]**. Se utilizzi un server di tracciamento diverso, aggiornalo in questo campo per evitare la perdita di dati.

1. Nell’angolo in basso a sinistra della pagina Configurazione di Adobe Analytics, seleziona **[!UICONTROL Salva]** per verificare che la configurazione dell’account Adobe Analytics sia aggiornata.

>[!MORELIKETHIS]
>
>* [Configurare i rapporti di Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

