---
title: Configurazione dei rapporti di Adobe Analytics
seo-title: Configurazione dei rapporti di Adobe Analytics
description: 'null'
seo-description: Scopri come configurare i rapporti di Adobe Analytics.
uuid: bf 210 f 68-dcb 0-4 e 86-be 04-0 a 8 b 2117 ef 2 a
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: f 4 c 8 c 2 b 3-cc 95-416 f -9 a 5 d-da 81 c 231 dfc 2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Configurazione dei rapporti di Adobe Analytics{#configuring-adobe-analytics-reports}

Per comunicare ad Adobe Analytics quali informazioni includere nei rapporti, passate alla schermata Configurazione Adobe Analytics. Dopo aver configurato i rapporti, questa schermata riporta, per ogni evento del visualizzatore su cui desiderate informazioni, una variabile Adobe Analytics e Dynamic Media Classic corrispondente. Queste combinazioni di variabile variabile-Adobe Analytics - Variabile Dynamic Media Classic di Adobe Analytics determinano le informazioni riportate.

Oltre ad associare gli eventi del visualizzatore con le variabili, nella schermata Configurazione Adobe Analytics sono disponibili strumenti per attivare, modificare ed eliminare degli eventi del visualizzatore.

>[!NOTE]
>
>Quando modificate le impostazioni di Adobe Analytics Report dall’interno di Adobe Analytics, accedete ad Adobe Analytics da Adobe Scene7 Publishing System, salvate nuovamente le impostazioni di configurazione Adobe Analytics e quindi effettuate di nuovo la pubblicazione.

Consultate [Accedere ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Consultate [Pubblicazione delle informazioni di configurazione](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Assegnazione delle variabili Adobe Analytics agli eventi e alle variabili di visualizzatore Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Utilizzate la schermata Configurazione Adobe Analytics per associare gli eventi dei visualizzatori alle variabili di Adobe Analytics e Dynamic Media Classic. Per ogni evento del visualizzatore, scegliete una variabile di Adobe Analytics e una variabile Dynamic Media Classic. Per istruzioni su come aprire la schermata Configurazione Adobe Analytics, consultate [Accedere ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Per assegnare variabili Adobe Analytics agli eventi e alle variabili di visualizzatore Dynamic Media Classic**

1. After you log in to Adobe Analytics from within Dynamic Media Classic and select a report suite, on the Adobe Analytics Configuration page, in the far right column of the table, activate a viewer event by clicking **Enable**.
1. Per visualizzare il selettore della coppia di variabili, nella colonna Variabili fate clic sul pulsante freccia dell’evento visualizzatore desiderato.

   Consultate [Eventi dei visualizzatori](configuring-analytics-reports.md#viewer_events).

1. Aggiungete una variabile Dynamic Media Classic.

   Consultate [Variabili Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Aggiungete una variabile di Adobe Analytics.
1. (Facoltativo) Per aggiungere un’altra coppia di variabile, fate clic su **Aggiungi**.
1. Fate clic su **Salva**.

   Dopo aver fatto clic su Salva, l'evento del visualizzatore, la variabile Adobe Analytics e la relativa variabile Dynamic Media Classic sono elencati nella schermata Configurazione Adobe Analytics.

1. Fate clic **Chiudi**, nell’angolo in basso a destra.
1. Fate clic su **Pubblica** &gt; **Invia pubblicazione** per eseguire un processo di pubblicazione server immagini.

   La pubblicazione è necessaria per rendere le informazioni contenute nei visualizzatori disponibili nei server Dynamic Media Classic.

### Eventi dei visualizzatori {#viewer-events}

Gli eventi dei visualizzatori descrivono azioni eseguite dagli utenti con visualizzatori per contenuti multimediali dinamici. Quando un utente avvia un’azione, ad esempio fa clic su una miniatura oppure avvia o arresta un video, il visualizzatore “trasmette” un evento e i relativi dati alla pagina Web.

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
| PLAY (Riproduzione) | **X** (video) | Nei visualizzatori video, quando un utente fa clic su Riproduci per avviare la riproduzione di un video.<br><br>**Nota:** Se utilizzate i rapporti sui video basati su heartbeat basati su heartbeat Adobe Analytics, non è necessario mappare qualsiasi variabile all'evento visualizzatore quando configurate Adobe Analytics in Dynamic Media Classic. Heartbeat video funziona con i visualizzatori HTML 5 Video Classic Classic e mixedmedia integrati. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| PAUSE (Pausa) | **X** (video) | Nei visualizzatori video, quando un utente fa clic su Pausa per sospendere la riproduzione di un video.<br><br>**Nota:** Se utilizzate i rapporti sui video basati su heartbeat basati su heartbeat Adobe Analytics, non è necessario mappare qualsiasi variabile all'evento visualizzatore quando configurate Adobe Analytics in Dynamic Media Classic. Heartbeat video funziona con i visualizzatori HTML 5 Video Classic Classic e mixedmedia integrati. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| STOP (Interruzione) | **X** (video) | Nei visualizzatori video, quando un utente fa clic su Stop per interrompere la riproduzione di un video.<br><br>**Nota:** Se utilizzate i rapporti sui video basati su heartbeat basati su heartbeat Adobe Analytics, non è necessario mappare qualsiasi variabile all'evento visualizzatore quando configurate Adobe Analytics in Dynamic Media Classic. Heartbeat video funziona con i visualizzatori HTML 5 Video Classic Classic e mixedmedia integrati. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| MILESTONE (Pietra miliare) | **X**  (Video) | Nei visualizzatori video, vengono generati degli eventi milestone (pietra miliare) quando l’utente guarda una percentuale di video pari a 0, 25, 50, 75 o 100.<br><br>**Nota:** Se utilizzate i rapporti sui video basati su heartbeat basati su heartbeat Adobe Analytics, non è necessario mappare qualsiasi variabile all'evento visualizzatore quando configurate Adobe Analytics in Dynamic Media Classic. Heartbeat video funziona con i visualizzatori HTML 5 Video Classic Classic e mixedmedia integrati. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| SWATCH (Campione) | X (zoom a comparsa, zoom) | Questo evento per visualizzatori viene mappato sull’evento visualizzatore PAGE in Scene7 Publishing System. |
| ZOOM | **X** (eCatalog, set 360 gradi, zoom) | Questo evento non è seguito da Adobe Analytics.<br> |
| PAN (Panning) | **X** (eCatalog, set 360 gradi, zoom) | Questo evento non è seguito da Adobe Analytics.<br> |
| SPIN (Set a 360 gradi) | **X** (Set a 360 gradi) | Questo evento non è seguito da Adobe Analytics.<br> |


### Variabili Dynamic Media Classic {#scene-variables}

For each viewer event on Adobe Analytics Configuration screen, choose a Adobe Analytics variable and a *Dynamic Media Classic variable*. Le variabili Dynamic Media Classic rappresentano i dati che potete ottenere per un rapporto. La variabile `searchTerm`, ad esempio, riporta le parole chiavi utilizzate nelle ricerche effettuate negli eCatalog.

Nella tabella seguente sono descritte le variabili Dynamic Media Classic.

| Variabile Dynamic Media Classic | Descrizione |
|--- |:--- |
| asset | ID risorsa Scene7 Publishing System o percorso del file video. |
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

## Attivazione, modifica ed eliminazione degli eventi dei visualizzatori {#activating-editing-and-deleting-viewer-events}

Nella schermata Configurazione Adobe Analytics, potete attivare, modificare e quindi eliminare gli eventi dei visualizzatori:

**Attivazione** per **attivare o disattivare l** 'evento visualizzatore selezionato.

**Modifica** Consente di selezionare un evento di visualizzatore e fare clic **sul pulsante Visualizza/modifica** variabili in grigio. Negli elenchi a discesa Variabile Media Classic Classic e Variabile Adobe Analytics, scegliete una variabile diversa da ogni rispettivo elenco. Per ulteriori informazioni, consultate Assegnazione delle variabili Adobe Analytics agli eventi e alle variabili di visualizzatore Dynamic Media Classic.

**Eliminazione** Consente di selezionare un evento di visualizzatore e fare clic **sul pulsante Visualizza/modifica** variabili in grigio. Fate clic su **Elimina**.
