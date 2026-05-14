---
title: Configurare i rapporti di Adobe Analytics
description: Scopri come configurare i rapporti di Adobe Analytics in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T17:43:06.354Z'
TQID: 'https://experienceleague.adobe.com/GiljiYJVAfOfWB78ZruSnTP01haCDv9fLKESpq7t5YA'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 1251
ht-degree: 20%

---

# Configurare i rapporti di Adobe Analytics{#configuring-adobe-analytics-reports}

Per comunicare ad Adobe Analytics le informazioni desiderate nei rapporti di Adobe Analytics, passa alla schermata Configurazione di Adobe Analytics. Dopo i rapporti di configurazione, in questa schermata vengono elencate, per ogni evento visualizzatore di cui desideri avere informazioni, una variabile Adobe Analytics e una variabile Adobe Dynamic Media Classic corrispondenti. Questi eventi visualizzatore-Variabile di Adobe Analytics-Combinazioni di variabili di Adobe Dynamic Media Classic determinano le informazioni riportate.

Oltre ad associare gli eventi visualizzatore alle variabili, la schermata Configurazione di Adobe Analytics offre strumenti per attivare, modificare ed eliminare gli eventi visualizzatore.

>[!NOTE]
>
>Ogni volta che modifichi le impostazioni dei rapporti di Adobe Analytics in Adobe Analytics, accertati di accedere nuovamente ad Adobe Analytics da Adobe Dynamic Media Classic, salvare nuovamente le impostazioni di configurazione di Adobe Analytics, quindi ripubblicare.

Vedere [Accesso ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Vedi [Informazioni sulla configurazione della pubblicazione](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Assegnare variabili Adobe Analytics a eventi e variabili visualizzatore Adobe Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Utilizza la schermata Configurazione di Adobe Analytics per associare gli eventi visualizzatore alle variabili Adobe Analytics e Adobe Dynamic Media Classic. Per ogni evento visualizzatore, scegli una variabile Adobe Analytics e una variabile Adobe Dynamic Media Classic. Per istruzioni sull&#39;apertura della schermata Configurazione di Adobe Analytics, vedere [Accesso ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Per assegnare le variabili di Adobe Analytics agli eventi e alle variabili del visualizzatore Adobe Dynamic Media Classic:**

1. Dopo aver effettuato l&#39;accesso ad Adobe Analytics da Dynamic Media Classic e aver selezionato una suite di rapporti, nella colonna di tabella a destra della pagina Configurazione di Adobe Analytics, attiva un evento visualizzatore selezionando **[!UICONTROL Abilita]**.
1. Nella colonna Variabili, visualizza il selettore di coppie di variabili selezionando il pulsante freccia per l’evento visualizzatore desiderato.

   Consultate [Eventi dei visualizzatori](configuring-analytics-reports.md#viewer_events).

1. Aggiungi una variabile Adobe Dynamic Media Classic.

   Vedi [Variabili Adobe Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Aggiungete una variabile di Adobe Analytics.
1. (Facoltativo) Per aggiungere un&#39;altra coppia di variabili, selezionare **[!UICONTROL Aggiungi]**.
1. Seleziona **[!UICONTROL Salva]**.

   Dopo aver selezionato **[!UICONTROL Salva]**, l&#39;evento visualizzatore, la relativa variabile Adobe Analytics e la variabile Adobe Dynamic Media Classic sono elencati nella schermata Configurazione Adobe Analytics.

1. Nell&#39;angolo inferiore destro, selezionare **[!UICONTROL Chiudi]**.
1. Vai a **[!UICONTROL Pubblica]** > **[!UICONTROL Invia pubblicazione]** per eseguire una pubblicazione da server immagini.

   La pubblicazione è necessaria in modo che le informazioni contenute nei visualizzatori siano disponibili sui server di Adobe Dynamic Media Classic.

### Eventi dei visualizzatori {#viewer-events}

Gli eventi visualizzatore descrivono le azioni eseguite dagli utenti con i visualizzatori Dynamic Media Classic. Quando un utente avvia un’azione, ad esempio la selezione di una miniatura o l’avvio o l’arresto di un video, il visualizzatore &quot;trasmette&quot; un evento sulla pagina web. Vengono inviati anche i dati associati a tale evento.

La tabella seguente descrive gli eventi visualizzatore che puoi aggiungere alla schermata Configurazione di Adobe Analytics.

| Evento visualizzatore | Supporto per la piattaforma di visualizzatori HTML5 e visualizzatori | Descrizione |
| --- | --- | --- |
| LOAD (Caricamento) | **X** (eCatalog, zoom a comparsa, set 360 gradi, video, zoom) | Quando un utente avvia un visualizzatore |
| PAGE (Pagina) | **X** (eCatalog) | Nei cataloghi elettronici, quando un utente gira una pagina; nei visualizzatori di zoom mirati, quando un utente seleziona una destinazione diversa o un campione di colore. |
| SWAP (Scambio) | **X** (eCatalog, zoom a comparsa, set 360 gradi, video, zoom) | Quando un utente seleziona una miniatura diversa per visualizzare un’immagine diversa. |
| ITEM (Elemento) | **X** (eCatalog) | Nei visualizzatori che supportano le mappe di immagine in cui sono definiti i rollover, quando un utente passa il puntatore su una mappa immagine per leggere il testo di rollover. |
| HREF | **X** (eCatalog) | Nei visualizzatori che supportano le mappe immagine, quando un utente seleziona un URL in una mappa immagine. |
| TARGET (Destinazione) | | Nei visualizzatori di zoom mirati, quando un utente seleziona una destinazione di zoom per eseguire lo zoom su una parte dell’immagine. |
| SEARCH (Ricerca) | | Negli eCatalog, quando un utente effettua una ricerca di parole. |
| PLAY (Riproduzione) | **X** (video) | Nei visualizzatori video, quando un utente seleziona Riproduci per avviare la riproduzione di un video.<br><br>**Nota:** Se utilizzi rapporti video basati su heartbeat in Adobe Analytics, non è necessario mappare alcuna variabile a questo evento visualizzatore quando configuri Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con visualizzatori Adobe Dynamic Media Classic HTML5 Video e MixedMedia predefiniti. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consulta [Abilitare i rapporti video di Adobe Analytics](enabling-analytics-video-reports.md). |
| PAUSE (Pausa) | **X** (video) | Nei visualizzatori video, quando un utente seleziona **[!UICONTROL Pausa]** per bloccare un video.<br><br>**Nota:** Se utilizzi rapporti video basati su heartbeat in Adobe Analytics, non è necessario mappare alcuna variabile su questo evento visualizzatore quando configuri Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con visualizzatori Adobe Dynamic Media Classic HTML5 Video e MixedMedia predefiniti. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consulta [Abilitare i rapporti video di Adobe Analytics](enabling-analytics-video-reports.md). |
| STOP (Interruzione) | **X** (video) | Nei visualizzatori video, quando un utente seleziona **[!UICONTROL Interrompi]** per interrompere la riproduzione di un video.<br><br>**Nota:** Se utilizzi la generazione di rapporti video basati su heartbeat in Adobe Analytics, non è necessario mappare alcuna variabile a questo evento visualizzatore quando configuri Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con visualizzatori Adobe Dynamic Media Classic HTML5 Video e MixedMedia predefiniti. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consulta [Abilitare i rapporti video di Adobe Analytics](enabling-analytics-video-reports.md). |
| MILESTONE (Pietra miliare) | **X** (video) | Nei visualizzatori video, gli eventi milestone vengono generati quando l&#39;utente guarda lo 0, 25, 50, 75 o 100% del video.<br><br>**Nota:** Se utilizzi la generazione rapporti video basati su heartbeat in Adobe Analytics, non è necessario mappare alcuna variabile a questo evento visualizzatore quando configuri Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con visualizzatori Adobe Dynamic Media Classic HTML5 Video e MixedMedia predefiniti. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consulta [Abilitare i rapporti video di Adobe Analytics](enabling-analytics-video-reports.md). |
| SWATCH (Campione) | **X** (zoom a comparsa, zoom) | Questo evento visualizzatore è mappato all&#39;evento visualizzatore PAGE in Adobe Dynamic Media Classic. |
| ZOOM | **X** (eCatalog, set 360 gradi, zoom) | Questo evento non è seguito da Adobe Analytics. |
| PAN (Panning) | **X** (eCatalog, set 360 gradi, zoom) | Questo evento non è seguito da Adobe Analytics. |
| SPIN (Set a 360 gradi) | **X** (Set a 360 gradi) | Questo evento non è seguito da Adobe Analytics. |

### Variabili Adobe Dynamic Media Classic {#scene-variables}

Per ogni evento visualizzatore nella schermata Configurazione Adobe Analytics, scegli una variabile Adobe Analytics e una *variabile Adobe Dynamic Media Classic*. Le variabili Adobe Dynamic Media Classic rappresentano i dati che puoi ottenere per un rapporto. La variabile `searchTerm`, ad esempio, elenca le parole chiave utilizzate nelle ricerche eCatalog.

La tabella seguente descrive le variabili di Adobe Dynamic Media Classic:

| Variabile Adobe Dynamic Media Classic | Descrizione |
| --- | --- |
| asset | ID risorsa Adobe Dynamic Media Classic o file di percorso video. |
| viewerId | Numero arbitrario assegnato a ciascun tipo diverso di visualizzatore. |
| pageLabel | In eCatalogs, la pagina visualizzata dal visualizzatore. |
| label | Il valore label (una stringa). |
| frame | Pagina o pagine a cui si fa riferimento in un set di immagini. |
| rollover_keyRaw | L&#39;intero valore HREF, non solo qualsiasi parte elaborata di esso. |
| rollover_keyProc | ID di un elemento con riferimento in una mappa immagine (valido per gli eventi href ed elementi). |
| searchTerm | Termine utilizzato nella ricerca eCatalog. |
| timeStamp | Riproduci, Arresta e Pausa selezionati nei visualizzatori video. |
| progress | Percentuale di completamento di un evento milestone (pietra miliare). |
| targetId | Il valore id (un numero). |

## Attivare, modificare ed eliminare gli eventi visualizzatore {#activating-editing-and-deleting-viewer-events}

Nella schermata Configurazione Adobe Analytics, potete attivare, modificare e quindi eliminare gli eventi dei visualizzatori:

* **Attiva**: seleziona **[!UICONTROL Attiva]** per attivare o **[!UICONTROL Disattiva]** per disattivare un evento visualizzatore selezionato.

* **Modifica**: seleziona un evento visualizzatore e fai clic sul pulsante grigio **[!UICONTROL Visualizza/Modifica]** variabili. Negli elenchi a discesa Variabile di Adobe Dynamic Media Classic e Variabile di Adobe Analytics, scegli una variabile diversa da ciascun elenco. Per ulteriori informazioni, vedere [Assegnazione di variabili Adobe Analytics a eventi e variabili del visualizzatore Adobe Dynamic Media Classic](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **Elimina**: seleziona un evento visualizzatore, quindi fai clic sul pulsante grigio **[!UICONTROL Visualizza/Modifica]** variabili. Selezionare **[!UICONTROL Elimina]**.
