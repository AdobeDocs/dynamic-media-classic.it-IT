---
title: '"Avvio rapido: Integrazione di Dynamic Media Classic e Adobe Analytics"'
description: Introduzione e avvio rapido all’integrazione di Dynamic Media Classic e Adobe Analytics per consentirti di iniziare a utilizzare rapidamente.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 41%

---

# Avvio rapido: Integrazione di Dynamic Media Classic e Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics è il prodotto leader di settore che offre agli addetti marketing un punto unico da cui misurare, analizzare e ottimizzare i dati integrati da tutte le iniziative online attraverso più canali di marketing.

Dopo aver integrato Adobe Analytics con Dynamic Media Classic, puoi ottenere rapporti sul comportamento dei visitatori del sito web che utilizzano i visualizzatori Dynamic Media Classic sul tuo sito web. Ad esempio, quando un visitatore di un sito web fa clic su una destinazione di zoom in un visualizzatore zoom Dynamic Media Classic, Adobe Analytics registra questa azione. I rapporti di Adobe Analytics possono raccogliere informazioni cumulative sull’attività dell’utente nei visualizzatori di Dynamic Media Classic.

Utilizzando i rapporti di Adobe Analytics, potete ricavare un’immagine chiara delle attività dei clienti sul vostro sito Web. È possibile determinare quali presentazioni di prodotto portano alla conversione e quali non attraggono l&#39;interesse dei clienti.

Consultate anche [Misurazione dei video in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

>[!NOTE]
>
>È necessario un account Adobe Analytics valido per integrare Analytics con Dynamic Media Classic e generare rapporti di Analytics.

Questa sezione è stata progettata per aiutarvi a usare in breve tempo Adobe Analytics Instrumentation Kit.

## 1. Accedi ad Adobe Analytics tramite Dynamic Media Classic e scarica le variabili di report Adobe Analytics

>[!NOTE]
>
>Prima di poter configurare i rapporti di Adobe Analytics e far corrispondere le variabili dei rapporti di Adobe Analytics agli eventi di Dynamic Media Classic, verifica di essere aggiunto come membro del gruppo Accesso ai servizi Web in Adobe Analytics. I membri di questo gruppo possono accedere a tutti i rapporti della suite specificata tramite Marketing Cloud’s Web Services API a prescindere dalle autorizzazioni impostate nell’interfaccia. Per aggiungere un membro al gruppo, in Adobe Analytics fate clic su **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]** (Strumenti amministrazione > Gestione utenti > Modifica gruppi).

Dopo aver verificato di essere membro del gruppo Accesso al servizio Web, in Dynamic Media Classic fai clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Adobe Analytics]**. Nella pagina di configurazione di Adobe Analytics, fate clic su **[!UICONTROL Accesso ad Adobe Analytics]**.

Consultate [Accedere ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Nella finestra di dialogo Accesso Adobe Analytics, digita l&#39;ID organizzazione Marketing Cloud (facoltativo) e le credenziali complete, quindi fai clic su **[!UICONTROL Accesso]**. Dall’elenco a discesa Report Suite (Suite rapporti), selezionate il nome della suite di rapporti che intendete usare.

## 2. Assegnare le variabili dei rapporti Adobe Analytics agli eventi del visualizzatore Dynamic Media Classic e alle variabili di Dynamic Media Classic

Nella pagina Configurazione Adobe Analytics, specificate le informazioni desiderate nei rapporti di Adobe Analytics. Per ogni evento del visualizzatore Dynamic Media Classic di cui desideri ottenere informazioni, scegli una variabile Adobe Analytics (dalla suite di rapporti) e una variabile Dynamic Media Classic.

* Gli eventi del visualizzatore descrivono l’attività utente che desiderate analizzare nei rapporti.
* Le variabili di Dynamic Media Classic descrivono i dati sugli eventi utente che desideri distribuire nei rapporti.

La configurazione di Adobe Analytics offre anche strumenti per l’attivazione, la modifica e l’eliminazione degli eventi dei visualizzatori.

Dopo aver fatto clic su **[!UICONTROL Salva]** nella pagina Configurazione di Adobe Analytics, nei visualizzatori di Dynamic Media Classic viene inserito un codice di tracciamento personalizzato per la misurazione dell&#39;attività dell&#39;utente. Questa funzionalità consente di tenere traccia dell’attività utente nei rapporti Adobe Analytics.

Consultate [Configurazione dei rapporti di Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Pubblica i visualizzatori Dynamic Media Classic

Pubblica i visualizzatori di Dynamic Media Classic in modo che i visualizzatori (con codice per il tracciamento dell’attività degli utenti nei rapporti di Adobe Analytics) vengano caricati sui server Dynamic Media Classic. In seguito alla pubblicazione, queste informazioni vengono incluse nei visualizzatori e possono essere utilizzate per le analisi Adobe Analytics.

Consultate [Pubblicazione delle informazioni di configurazione](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Posizionare i visualizzatori Dynamic Media Classic nel sito web

Posiziona i visualizzatori Dynamic Media Classic con il codice di tracciamento Adobe Analytics sul tuo sito web.

## 5. Verifica l’integrazione di Adobe Analytics visualizzando un rapporto di Adobe Analytics

Per visualizzare i rapporti di Adobe Analytics, passate al sito Web di Adobe Analytics. La pagina Reporting (Rapporti) consente di visualizzare i dati e di creare grafici e tabelle per misurare l’attività degli utenti per diversi visualizzatori.

Consultate [Verificare l’integrazione visualizzando un rapporto di Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
