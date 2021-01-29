---
title: '"Avvio rapido: Integrazione di Dynamic Media Classic e  Adobe Analytics"'
description: Introduzione e avvio rapido all'integrazione di Dynamic Media Classic e  Adobe Analytics per aiutarvi a imparare a usare rapidamente.
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 45%

---


# Avvio rapido: Integrazione di Dynamic Media Classic e  Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics è il prodotto leader di settore che offre agli addetti marketing un punto unico da cui misurare, analizzare e ottimizzare i dati integrati da tutte le iniziative online attraverso più canali di marketing.

Dopo aver integrato  Adobe Analytics con Dynamic Media Classic, potete ottenere rapporti sul comportamento dei visitatori di siti Web che utilizzano i visualizzatori Dynamic Media Classic sul vostro sito Web. Ad esempio, quando un visitatore del sito Web fa clic su una destinazione di zoom in un visualizzatore zoom Dynamic Media Classic,  Adobe Analytics registra questa azione.  rapporti Adobe Analytics possono raccogliere informazioni cumulative sulle attività degli utenti nei visualizzatori Dynamic Media Classic.

Utilizzando i rapporti di Adobe Analytics, potete ricavare un’immagine chiara delle attività dei clienti sul vostro sito Web. Potete determinare quali presentazioni di prodotto hanno portato alla conversione da visitatore a cliente e quali non suscitano l’interesse dei visitatori.

Consultate anche [Misurazione dei video in Adobe Analytics](https://docs.adobe.com/content/help/en/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Per integrare Analytics con Dynamic Media Classic e generare report di Analytics è necessario un account  Adobe Analytics valido.

**Avvio rapido**

Questa sezione è stata progettata per aiutarvi a usare in breve tempo Adobe Analytics Instrumentation Kit.

**1. Accedi a  Adobe Analytics tramite Dynamic Media Classic e scarica  variabili di report Adobe Analytics**

>[!NOTE]
>
>Prima di poter configurare  rapporti Adobe Analytics e far corrispondere  variabili di rapporti Adobe Analytics agli eventi di Dynamic Media Classic, verificare di essere stato aggiunto come membro del gruppo Web Service Access in  Adobe Analytics. I membri di questo gruppo possono accedere a tutti i rapporti della suite specificata tramite Marketing Cloud’s Web Services API a prescindere dalle autorizzazioni impostate nell’interfaccia. Per aggiungere un membro al gruppo, in Adobe Analytics fate clic su **Admin Tools** > **User Management** > **Edit Groups** (Strumenti amministrazione > Gestione utenti > Modifica gruppi).

Dopo aver verificato di essere membro del gruppo Web Service Access, in Dynamic Media Classic fare clic su **Setup** > **Impostazione applicazione** > **Adobe Analytics**. Nella pagina di configurazione di Adobe Analytics, fate clic su **Accesso ad Adobe Analytics**.

Consultate [Accedere ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Nella  finestra di dialogo Accesso Adobe Analytics, digitate l&#39;ID organizzazione Marketing Cloud (facoltativo) e le credenziali complete, quindi fate clic su **Login**. Dall’elenco a discesa Report Suite (Suite rapporti), selezionate il nome della suite di rapporti che intendete usare.

**2. Assegnare  variabili dei rapporti Adobe Analytics agli eventi dei visualizzatori Dynamic Media Classic e alle variabili Dynamic Media Classic**

Nella pagina Configurazione Adobe Analytics, specificate le informazioni desiderate nei rapporti di Adobe Analytics. Per ogni evento del visualizzatore Dynamic Media Classic sul quale desiderate informazioni, scegliete una variabile Adobe Analytics  (dalla suite di rapporti) e una variabile Dynamic Media Classic.

* Gli eventi del visualizzatore descrivono l’attività utente che desiderate analizzare nei rapporti.
* Le variabili di Dynamic Media Classic descrivono i dati sugli eventi utente che si desidera distribuire nei rapporti.

La configurazione di Adobe Analytics offre anche strumenti per l’attivazione, la modifica e l’eliminazione degli eventi dei visualizzatori.

Dopo aver fatto clic su Salva nella schermata Configurazione  Adobe Analytics, il codice di tracciamento personalizzato per misurare l’attività degli utenti viene inserito nei visualizzatori Dynamic Media Classic. Questa funzionalità consente di tenere traccia dell’attività utente nei rapporti Adobe Analytics.

Consultate [Configurazione dei rapporti di Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Pubblicare i visualizzatori Dynamic Media Classic**

Pubblicate i visualizzatori Dynamic Media Classic in modo che i visualizzatori (con il codice per il monitoraggio dell&#39;attività degli utenti  rapporti Adobe Analytics) vengano caricati sui server Dynamic Media Classic. In seguito alla pubblicazione, queste informazioni vengono incluse nei visualizzatori e possono essere utilizzate per le analisi Adobe Analytics.

Consultate [Pubblicazione delle informazioni di configurazione](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Inserire i visualizzatori Dynamic Media Classic nel sito Web**

Inserite nel sito Web i visualizzatori Dynamic Media Classic con  codice di tracciamento Adobe Analytics.

**5. Verificare l’integrazione visualizzando un rapporto di Adobe Analytics**

Per visualizzare i rapporti di Adobe Analytics, passate al sito Web di Adobe Analytics. La pagina Reporting (Rapporti) consente di visualizzare i dati e di creare grafici e tabelle per misurare l’attività degli utenti per diversi visualizzatori.

Consultate [Verificare l’integrazione visualizzando un rapporto di Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
