---
title: '"Avvio rapido: Integrare Adobe Dynamic Media Classic e Adobe Analytics"'
description: Introduzione e Guida rapida sull’integrazione di Adobe Dynamic Media Classic e Adobe Analytics per consentirti di iniziare a utilizzare rapidamente.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 27%

---

# Avvio rapido: Integrare Adobe Dynamic Media Classic e Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics è il prodotto leader di settore che offre agli addetti marketing un punto unico da cui misurare, analizzare e ottimizzare i dati integrati da tutte le iniziative online attraverso più canali di marketing.

Dopo aver integrato Adobe Analytics con Adobe Dynamic Media Classic, puoi ottenere rapporti sul comportamento dei visitatori del sito web utilizzando i visualizzatori Adobe Dynamic Media Classic sul tuo sito web. Ad esempio, quando un visitatore di un sito web fa clic su una destinazione di zoom in un visualizzatore zoom Dynamic Media Classic, Adobe Analytics registra questa azione. I rapporti di Adobe Analytics possono raccogliere informazioni cumulative sull’attività dell’utente nei visualizzatori di Adobe Dynamic Media Classic.

Utilizzando i rapporti di Adobe Analytics, potete ricavare un’immagine chiara delle attività dei clienti sul vostro sito Web. È possibile determinare quali presentazioni di prodotto portano alla conversione e quali non attraggono l&#39;interesse dei clienti.

Vedere anche [Misurare i video in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

>[!NOTE]
>
>È necessario un account Adobe Analytics valido per integrare Analytics con Adobe Dynamic Media Classic e generare rapporti di Analytics.

Questa sezione è stata progettata per aiutarvi a usare in breve tempo Adobe Analytics Instrumentation Kit.

## 1. Accedi ad Adobe Analytics tramite Adobe Dynamic Media Classic e scarica le variabili dei rapporti Adobe Analytics

>[!NOTE]
>
>Prima di poter configurare i rapporti di Adobe Analytics e far corrispondere le variabili dei rapporti di Adobe Analytics agli eventi di Adobe Dynamic Media Classic, verifica di essere aggiunto come membro del gruppo Accesso ai servizi Web in Adobe Analytics. I membri di questo gruppo possono accedere a tutti i rapporti nelle suite di rapporti specificate tramite l’API Web Services di Experience Cloud, indipendentemente dalle autorizzazioni impostate nell’interfaccia. Per aggiungere un membro al gruppo, in Adobe Analytics vai a **[!UICONTROL Strumenti di amministrazione]** > **[!UICONTROL Gestione utente]** > **[!UICONTROL Modifica gruppi]**.

Dopo aver verificato di essere membro del gruppo Accesso al servizio Web, in Adobe Dynamic Media Classic, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Adobe Analytics]**. Nella pagina Configurazione Adobe Analytics, seleziona **[!UICONTROL Accesso Adobe Analytics]**.

Consultate [Accedere ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Nella finestra di dialogo Accesso Adobe Analytics, digita l&#39;ID organizzazione Experience Cloud (facoltativo) e le credenziali complete, quindi seleziona **[!UICONTROL Accesso]**. Dall’elenco a discesa Report Suite (Suite rapporti), selezionate il nome della suite di rapporti che intendete usare.

## 2. Assegnare le variabili del rapporto Adobe Analytics agli eventi del visualizzatore Dynamic Media Classic e alle variabili Adobe Dynamic Media Classic

Nella pagina Configurazione Adobe Analytics, specificate le informazioni desiderate nei rapporti di Adobe Analytics. Per ogni evento visualizzatore Dynamic Media Classic di Adobe di cui desideri ottenere informazioni, scegli una variabile Adobe Analytics (dalla suite di rapporti) e un’Adobe di variabile Dynamic Media Classic.

* Gli eventi del visualizzatore descrivono l’attività utente che desiderate analizzare nei rapporti.
* Le variabili Dynamic Media Classic di Adobe descrivono i dati sugli eventi utente che desideri distribuire nei rapporti.

La configurazione di Adobe Analytics offre anche strumenti per l’attivazione, la modifica e l’eliminazione degli eventi dei visualizzatori.

Dopo aver selezionato **[!UICONTROL Salva]** nella pagina Configurazione di Adobe Analytics, il codice di tracciamento personalizzato per la misurazione dell&#39;attività dell&#39;utente viene inserito nei visualizzatori Adobe Dynamic Media Classic. Questa funzionalità consente di tenere traccia dell’attività utente nei rapporti Adobe Analytics.

Consulta [Configurare i rapporti di Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Pubblica i visualizzatori Adobe Dynamic Media Classic

Pubblica i visualizzatori Adobe Dynamic Media Classic in modo che i visualizzatori (con codice per il tracciamento dell’attività degli utenti nei rapporti di Adobe Analytics) vengano caricati sui server Adobe Dynamic Media Classic. In seguito alla pubblicazione, queste informazioni vengono incluse nei visualizzatori e possono essere utilizzate per le analisi Adobe Analytics.

Consulta [Pubblicare informazioni sulla configurazione](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Posiziona Adobe visualizzatori Dynamic Media Classic nel tuo sito web

Inserisci nel tuo sito web l’Adobe visualizzatori Dynamic Media Classic con codice di tracciamento Adobe Analytics .

## 5. Verifica l’integrazione di Adobe Analytics visualizzando un rapporto di Adobe Analytics

Per visualizzare i rapporti di Adobe Analytics, passate al sito Web di Adobe Analytics. La pagina Reporting (Rapporti) consente di visualizzare i dati e di creare grafici e tabelle per misurare l’attività degli utenti per diversi visualizzatori.

Consulta [Testare l&#39;integrazione di Adobe Analytics visualizzando un rapporto di Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
