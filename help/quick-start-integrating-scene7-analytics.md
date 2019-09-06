---
title: '" Avvio rapido: Integrazione di Dynamic Media Classic e Adobe Analytics "'
seo-title: '" Avvio rapido: Integrazione di Dynamic Media Classic e Adobe Analytics "'
description: 'null'
seo-description: Introduzione e avvio rapido all'integrazione di Dynamic Media Classic e Adobe Analytic per aiutarvi a imparare a utilizzare.
uuid: 3 f 9 e 2 c 91-15 d 4-4 b 53-8220-9 b 1 ca 57 c 0 b 1 d
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: abec 9 a 85-013 c -4030-b 129-bf 27 a 89 cb 464
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Avvio rapido: Integrazione di Dynamic Media Classic e Adobe Analytics {#quick-start-integrating-scene-and-adobe-analytics}

Adobe Analytics è il prodotto leader di settore che offre agli addetti marketing un punto unico da cui misurare, analizzare e ottimizzare i dati integrati da tutte le iniziative online attraverso più canali di marketing.

Dopo aver integrato Adobe Analytics con Scene 7 Publishing System, potete ottenere rapporti sul comportamento dei visitatori di siti Web utilizzando visualizzatori Dynamic Media Classic sul vostro sito Web. Ad esempio, quando un visitatore fa clic su una destinazione di zoom in un visualizzatore zoom classico di Dynamic Media, Adobe Analytics registra questa azione. I rapporti di Adobe Analytics possono raccogliere informazioni cumulative sull'attività degli utenti nei visualizzatori Dynamic Media Classic.

Utilizzando i rapporti di Adobe Analytics, potete ricavare un’immagine chiara delle attività dei clienti sul vostro sito Web. Potete determinare quali presentazioni di prodotto hanno portato alla conversione da visitatore a cliente e quali non suscitano l’interesse dei visitatori.

Consultate anche [Misurazione dei video in Adobe Analytics](https://marketing.adobe.com/resources/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>per integrare Adobe Analytics con Scene7 Publishing System e generare rapporti di Analytics, è necessario un account valido di Adobe Analytics.

**Avvio rapido**

Questa sezione è stata progettata per aiutarvi a usare in breve tempo Adobe Analytics Instrumentation Kit.

**1. Log in to Adobe Analytics by way of Dynamic Media Classic and download Adobe Analytics report variables**

>[!NOTE]
>
>Prima di configurare i rapporti di Adobe Analytics e far corrispondere le variabili di rapporti di Adobe Analytics agli eventi Dynamic Media Classic, verificate di essere stato aggiunto come membro del gruppo Web Service Access in Adobe Analytics. I membri di questo gruppo possono accedere a tutti i rapporti della suite specificata tramite Marketing Cloud’s Web Services API a prescindere dalle autorizzazioni impostate nell’interfaccia. Per aggiungere un membro al gruppo, in Adobe Analytics fate clic su **Admin Tools** &gt; **User Management** &gt; **Edit Groups** (Strumenti amministrazione &gt; Gestione utenti &gt; Modifica gruppi).

After you have verified that you are a member of the Web Service Access group, in Dynamic Media Classic, click **Setup** &gt; **Application Setup** &gt; **Adobe Analytics**. Nella pagina di configurazione di Adobe Analytics, fate clic su **Accesso ad Adobe Analytics**.

Consultate [Accedere ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Nella finestra di dialogo Accesso ad Adobe Analytics, digitate l'ID organizzazione Marketing Cloud (facoltativo) e le credenziali complete, quindi fate clic **su Accesso**. Dall’elenco a discesa Report Suite (Suite rapporti), selezionate il nome della suite di rapporti che intendete usare.

**2. Assegnare variabili di rapporti di Adobe Analytics agli eventi dei visualizzatori Dynamic Media Classic e alle variabili Dynamic Media Classic**

Nella pagina Configurazione Adobe Analytics, specificate le informazioni desiderate nei rapporti di Adobe Analytics. Per ogni evento del visualizzatore Dynamic Media Classic su cui desiderate informazioni, scegliete una variabile Adobe Analytics (dalla suite di rapporti) e una variabile Dynamic Media Classic.

* Gli eventi del visualizzatore descrivono l’attività utente che desiderate analizzare nei rapporti.
* Le variabili Dynamic Media Classic descrivono i dati degli eventi utente che devono essere presentati dai rapporti.

La configurazione di Adobe Analytics offre anche strumenti per l’attivazione, la modifica e l’eliminazione degli eventi dei visualizzatori.

Dopo aver fatto clic su Salva nella schermata Configurazione Adobe Analytics, il codice di tracciamento personalizzato per la misurazione dell'attività utente viene inserito nei visualizzatori Dynamic Media Classic. Questa funzionalità consente di tenere traccia dell’attività utente nei rapporti Adobe Analytics.

Consultate [Configurazione dei rapporti di Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Pubblicare i visualizzatori per contenuti multimediali dinamici**

Pubblicate i visualizzatori per file multimediali dinamici in modo che i visualizzatori (con codice per il tracciamento dell'attività utente nei rapporti di Adobe Analytics) vengano caricati sui server Dynamic Media Classic. In seguito alla pubblicazione, queste informazioni vengono incluse nei visualizzatori e possono essere utilizzate per le analisi Adobe Analytics.

Consultate [Pubblicazione delle informazioni di configurazione](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Inserire visualizzatori per contenuti multimediali dinamici nel sito Web**

Inserite nel sito Web i visualizzatori Dynamic Media Classic con il codice di tracciamento di Adobe Analytics.

**5. Verificare l’integrazione visualizzando un rapporto di Adobe Analytics**

Per visualizzare i rapporti di Adobe Analytics, passate al sito Web di Adobe Analytics. La pagina Reporting (Rapporti) consente di visualizzare i dati e di creare grafici e tabelle per misurare l’attività degli utenti per diversi visualizzatori.

Consultate [Verificare l’integrazione visualizzando un rapporto di Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
