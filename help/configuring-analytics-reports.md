---
title: Configurazione dei rapporti di Adobe Analytics
description: Scoprite come configurare  rapporti Adobe Analytics.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 51%

---


# Configurazione dei rapporti di Adobe Analytics{#configuring-adobe-analytics-reports}

Per comunicare ad Adobe Analytics quali informazioni includere nei rapporti, passate alla schermata Configurazione Adobe Analytics. Dopo aver configurato i rapporti, questa schermata riporta, per ogni evento del visualizzatore di cui si desidera ottenere informazioni, una variabile Adobe Analytics  corrispondente e una variabile Dynamic Media Classic. Queste combinazioni di eventi per visualizzatori  variabile Adobe Analytics e variabile Dynamic Media Classic determinano le informazioni riportate.

Oltre ad associare gli eventi del visualizzatore con le variabili, nella schermata Configurazione Adobe Analytics sono disponibili strumenti per attivare, modificare ed eliminare degli eventi del visualizzatore.

>[!NOTE]
>
>Ogni volta che modificate  impostazioni di Adobe Analytics Report all&#39;interno  Adobe Analytics, è necessario accedere nuovamente ad  Adobe Analytics dall&#39;interno  Adobe Dynamic Media Classic, salvare nuovamente  impostazioni di configurazione Adobe Analytics e quindi ripubblicare.

Consultate [Accedere ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Consultate [Pubblicazione delle informazioni di configurazione](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Assegnazione  variabili Adobe Analytics agli eventi e alle variabili del visualizzatore Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Utilizzate la schermata Configurazione Adobe Analytics  per associare gli eventi dei visualizzatori alle variabili  Adobe Analytics e Dynamic Media Classic. Per ogni evento del visualizzatore, scegliete una  variabile Adobe Analytics e una variabile Dynamic Media Classic. Per istruzioni su come aprire la schermata Configurazione Adobe Analytics, consultate [Accedere ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Per assegnare  variabili Adobe Analytics agli eventi e alle variabili del visualizzatore Dynamic Media Classic**

1. Dopo aver effettuato l&#39;accesso a  Adobe Analytics da Dynamic Media Classic e aver selezionato una suite di rapporti, nella pagina  configurazione Adobe Analytics, nella colonna di destra della tabella, attivate un evento visualizzatore facendo clic su **Abilita**.
1. Per visualizzare il selettore della coppia di variabili, nella colonna Variabili fate clic sul pulsante freccia dell’evento visualizzatore desiderato.

   Consultate [Eventi dei visualizzatori](configuring-analytics-reports.md#viewer_events).

1. Aggiungi una variabile di Dynamic Media Classic.

   Vedere [Variabili Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Aggiungete una variabile di Adobe Analytics.
1. (Facoltativo) Per aggiungere un’altra coppia di variabile, fate clic su **Aggiungi**.
1. Fate clic su **Salva**.

   Dopo aver fatto clic su Salva, l’evento del visualizzatore, la relativa variabile Adobe Analytics  e la relativa variabile Dynamic Media Classic sono elencati nella schermata Configurazione  Adobe Analytics.

1. Fate clic **Chiudi**, nell’angolo in basso a destra.
1. Fate clic su **Pubblica** > **Invia pubblicazione** per eseguire un processo di pubblicazione server immagini.

   La pubblicazione è necessaria in modo che le informazioni contenute nei visualizzatori siano disponibili sui server Dynamic Media Classic.

### Eventi dei visualizzatori {#viewer-events}

Gli eventi dei visualizzatori descrivono le azioni eseguite dagli utenti con i visualizzatori Dynamic Media Classic. Quando un utente avvia un’azione, ad esempio fa clic su una miniatura oppure avvia o arresta un video, il visualizzatore “trasmette” un evento e i relativi dati alla pagina Web.

La tabella di seguito descrive gli eventi dei visualizzatori che potete aggiungere alla schermata Configurazione Adobe Analytics.

| Evento visualizzatore | Supporto per la piattaforma di visualizzatori HTML5 e visualizzatori | Descrizione |
|--- |--- |--- |
| LOAD (Caricamento) | **X** (eCatalog, zoom a comparsa, set 360 gradi, video, zoom) | Quando un utente avvia il visualizzatore. |
| PAGE (Pagina) | **X** (eCatalog) | Negli eCatalog, quando un utente volta pagina; nei visualizzatori dello zoom di destinazione, quando un utente seleziona un’altra destinazione o un altro campione colori. |
| SWAP (Scambio) | **X** (eCatalog, zoom a comparsa, set 360 gradi, video, zoom) | Quando un utente fa clic su un’altra miniatura per visualizzare un’altra immagine. |
| ITEM (Elemento) | **X** (eCatalog) | Nei visualizzatori che supportano le mappe di immagine in cui sono definiti i rollover, quando un utente passa il puntatore su una mappa immagine per leggere il testo di rollover. |
| HREF | **X** (eCatalog) | Nei visualizzatori che supportano le mappe di immagine, quando un utente fa clic su un URL all’interno di una mappa immagine. |
| TARGET (Destinazione) |  | Nei visualizzatori delle destinazioni di zoom, quando un utente seleziona una destinazione di zoom per ingrandire parte di un’immagine. |
| SEARCH (Ricerca) |  | Negli eCatalog, quando un utente effettua una ricerca di parole. |
| PLAY (Riproduzione) | **X** (video) | Nei visualizzatori video, quando un utente fa clic su Riproduci per avviare la riproduzione di un video.<br><br>**Nota:** se utilizzate  generazione di rapporti video basati su heartbeat Adobe Analytics, non è necessario mappare le variabili a questo evento del visualizzatore quando configurate  Adobe Analytics in Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video HTML5 e per file multimediali diversi forniti con Dynamic Media Classic. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consultate [Abilitazione  Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| PAUSE (Pausa) | **X** (video) | Nei visualizzatori video, quando un utente fa clic su Pausa per sospendere la riproduzione di un video.<br><br>**Nota:** se utilizzate  generazione di rapporti video basati su heartbeat Adobe Analytics, non è necessario mappare le variabili a questo evento del visualizzatore quando configurate  Adobe Analytics in Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video HTML5 e per file multimediali diversi forniti con Dynamic Media Classic. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consultate [Abilitazione  Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| STOP (Interruzione) | **X** (video) | Nei visualizzatori video, quando un utente fa clic su Stop per interrompere la riproduzione di un video.<br><br>**Nota:** se utilizzate  generazione di rapporti video basati su heartbeat Adobe Analytics, non è necessario mappare le variabili a questo evento del visualizzatore quando configurate  Adobe Analytics in Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video HTML5 e per file multimediali diversi forniti con Dynamic Media Classic. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consultate [Abilitazione  Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| MILESTONE (Pietra miliare) | **X**  (Video) | Nei visualizzatori video, vengono generati degli eventi milestone (pietra miliare) quando l’utente guarda una percentuale di video pari a 0, 25, 50, 75 o 100.<br><br>**Nota:** se utilizzate  generazione di rapporti video basati su heartbeat Adobe Analytics, non è necessario mappare le variabili a questo evento del visualizzatore quando configurate  Adobe Analytics in Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video HTML5 e per file multimediali diversi forniti con Dynamic Media Classic. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consultate [Abilitazione  Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| SWATCH (Campione) | X (zoom a comparsa, zoom) | Questo evento del visualizzatore viene mappato sull’evento del visualizzatore PAGE in Dynamic Media Classic. |
| ZOOM | **X** (eCatalog, set 360 gradi, zoom) | Questo evento non è seguito da Adobe Analytics.<br> |
| PAN (Panning) | **X** (eCatalog, set 360 gradi, zoom) | Questo evento non è seguito da Adobe Analytics.<br> |
| SPIN (Set a 360 gradi) | **X** (Set a 360 gradi) | Questo evento non è seguito da Adobe Analytics.<br> |


### Variabili Dynamic Media Classic {#scene-variables}

Per ogni evento del visualizzatore  schermata Configurazione Adobe Analytics, scegliete una variabile Adobe Analytics  e una variabile Dynamic Media Classic *.* Le variabili di Dynamic Media Classic rappresentano i dati che potete ottenere per un rapporto. La variabile `searchTerm`, ad esempio, riporta le parole chiavi utilizzate nelle ricerche effettuate negli eCatalog.

Nella tabella seguente sono descritte le variabili di Dynamic Media Classic.

| Variabile Dynamic Media Classic | Descrizione |
|--- |:--- |
| asset | ID risorsa Dynamic Media Classic o file del percorso video. |
| viewerId | Numero arbitrario assegnato a ciascun tipo diverso di visualizzatore. |
| pageLabel | In eCatalogs, la pagina visualizzata dal visualizzatore. |
| label | Il valore label (una stringa). |
| frame | La pagina o il riferimento della pagina in un set di immagini. |
| rollover_keyRaw | L’intero valore HREF e non solo la parte elaborata. |
| rollover_keyProc | ID di un elemento con riferimento in una mappa immagine (valido per gli eventi href ed elementi). |
| searchTerm | Termine utilizzato nella ricerca eCatalog. |
| timeStamp | Riproduci, Interrompi e Sospendi scelti nei visualizzatori video. |
| progress | Percentuale di completamento di un evento milestone (pietra miliare). |
| targetId | Il valore id (un numero). |

## Attivazione, modifica ed eliminazione degli eventi dei visualizzatori  {#activating-editing-and-deleting-viewer-events}

Nella schermata Configurazione Adobe Analytics, potete attivare, modificare e quindi eliminare gli eventi dei visualizzatori:

* ****
AttivazioneFate clic su  **** Abilita per attivare o  **** disattivare un evento visualizzatore selezionato.

* ****
Modifica: selezionate un evento del visualizzatore e fate clic sul pulsante  **[!UICONTROL Visualizza/]** Modifica variabili grigio. Negli elenchi a discesa Variabile Dynamic Media Classic e Variabile Adobe Analytics, scegliete una variabile diversa da ciascun rispettivo elenco. Per ulteriori informazioni, consultate Assegnazione  variabili Adobe Analytics agli eventi e alle variabili dei visualizzatori Dynamic Media Classic.

* ****
Eliminazione: selezionate un evento visualizzatore e fate clic sul pulsante  **[!UICONTROL Visualizza/]** ModificaVariabili in grigio. Fate clic su **[!UICONTROL Elimina]**.
