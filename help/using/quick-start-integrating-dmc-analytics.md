---
title: "Guida introduttiva: Integrare Adobe Dynamic Media Classic e Adobe Analytics"
description: Introduzione e Guida rapida all’integrazione di Adobe Dynamic Media Classic e Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 24%

---

# Guida introduttiva: Integrare Adobe Dynamic Media Classic e Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics è il prodotto leader di settore che offre agli addetti marketing un punto unico da cui misurare, analizzare e ottimizzare i dati integrati da tutte le iniziative online attraverso più canali di marketing.

Dopo aver integrato Adobe Analytics con Adobe Dynamic Media Classic, puoi ottenere rapporti sul comportamento dei visitatori del sito web utilizzando i visualizzatori Adobe Dynamic Media Classic sul tuo sito web. Ad esempio, quando un visitatore di un sito web seleziona una destinazione di zoom in un Visualizzatore zoom di Adobe Dynamic Media Classic, Adobe Analytics registra questa azione. I rapporti di Adobe Analytics possono raccogliere informazioni cumulative sull’attività degli utenti nei visualizzatori Adobe Dynamic Media Classic.

Utilizzando i rapporti di Adobe Analytics, potete ricavare un’immagine chiara delle attività dei clienti sul vostro sito Web. Puoi determinare quali presentazioni di prodotti portano alla conversione e quali non attirano l’interesse dei clienti.

Vedi anche [Misurare i video in Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

>[!NOTE]
>
>È necessario un account Adobe Analytics valido per integrare Analytics con Adobe Dynamic Media Classic e generare i rapporti di Analytics.

Questa sezione è stata progettata per aiutarvi a usare in breve tempo Adobe Analytics Instrumentation Kit.

## 1. Accedi ad Adobe Analytics tramite Adobe Dynamic Media Classic e scarica le variabili di rapporto di Adobe Analytics

>[!NOTE]
>
>Prima di poter configurare i rapporti di Adobe Analytics e associare le variabili di rapporto di Adobe Analytics agli eventi di Adobe Dynamic Media Classic, verifica di essere stato aggiunto come membro del gruppo Accesso al servizio Web in Adobe Analytics. I membri di questo gruppo possono accedere a tutti i rapporti nelle suite di rapporti specificate tramite l’API dei servizi web di Experience Cloud, indipendentemente dalle autorizzazioni impostate nell’interfaccia. Per aggiungere un membro al gruppo, in Adobe Analytics vai a **[!UICONTROL Strumenti di amministrazione]** > **[!UICONTROL Gestione utente]** > **[!UICONTROL Modifica gruppi]**.

Dopo aver verificato di essere membro del gruppo Accesso al servizio Web, in Adobe Dynamic Media Classic passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Adobe Analytics]**. Nella pagina Configurazione di Adobe Analytics, seleziona **[!UICONTROL Accesso ad Adobe Analytics]**.

Consulta [Accedere ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Nella finestra di dialogo Accesso di Adobe Analytics, digita l’ID organizzazione Experience Cloud (facoltativo) e le credenziali complete, quindi seleziona **[!UICONTROL Login]**. Dall’elenco a discesa Report Suite (Suite rapporti), selezionate il nome della suite di rapporti che intendete usare.

## 2. Assegnare le variabili dei rapporti di Adobe Analytics agli eventi visualizzatore Adobe Dynamic Media Classic e alle variabili Adobe Dynamic Media Classic

Nella pagina Configurazione Adobe Analytics, specificate le informazioni desiderate nei rapporti di Adobe Analytics. Per ogni evento visualizzatore Adobe Dynamic Media Classic di cui desideri ricevere informazioni, scegli una variabile Adobe Analytics (dalla suite di rapporti) e una variabile Adobe Dynamic Media Classic.

* Gli eventi del visualizzatore descrivono l’attività utente che desiderate analizzare nei rapporti.
* Le variabili di Adobe Dynamic Media Classic descrivono i dati sugli eventi utente che desideri che vengano consegnati dai rapporti.

La configurazione di Adobe Analytics offre anche strumenti per l’attivazione, la modifica e l’eliminazione degli eventi dei visualizzatori.

Dopo aver selezionato **[!UICONTROL Salva]** nella pagina Configurazione di Adobe Analytics, il codice di tracciamento personalizzato per la misurazione dell’attività dell’utente viene inserito nei visualizzatori Adobe Dynamic Media Classic. Questa funzionalità consente di tenere traccia dell’attività utente nei rapporti Adobe Analytics.

Consulta [Configurare i rapporti di Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Pubblicare i visualizzatori Adobe Dynamic Media Classic

Pubblica i visualizzatori Adobe Dynamic Media Classic in modo che vengano caricati sui server Adobe Dynamic Media Classic (con il codice per il tracciamento delle attività degli utenti nei rapporti di Adobe Analytics). Dopo la pubblicazione, queste informazioni vengono incluse nei visualizzatori e possono essere utilizzate per l’analisi da parte di Adobe Analytics.

Consulta [Pubblica informazioni di configurazione](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Inserire i visualizzatori Adobe Dynamic Media Classic nel sito Web

Inserisci i visualizzatori Adobe Dynamic Media Classic con il codice di tracciamento Adobe Analytics sul tuo sito web.

## 5. Testare l’integrazione di Adobe Analytics visualizzando un rapporto di Adobe Analytics

Per visualizzare i rapporti di Adobe Analytics, passate al sito Web di Adobe Analytics. La pagina Reporting (Rapporti) consente di visualizzare i dati e di creare grafici e tabelle per misurare l’attività degli utenti per diversi visualizzatori.

Consulta [Testare l’integrazione di Adobe Analytics visualizzando un rapporto di Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
