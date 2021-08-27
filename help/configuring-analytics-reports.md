---
title: Configurare i rapporti di Adobe Analytics
description: Scopri come configurare i rapporti di Adobe Analytics in Adobe Dynamic Media Classic.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '1228'
ht-degree: 30%

---

# Configurare i rapporti di Adobe Analytics{#configuring-adobe-analytics-reports}

Per comunicare ad Adobe Analytics quali informazioni includere nei rapporti, passate alla schermata Configurazione Adobe Analytics. Dopo aver configurato i rapporti, questa schermata elenca, per ogni evento di visualizzatore di cui desideri ottenere informazioni, una variabile Adobe Analytics corrispondente e una variabile Dynamic Media Classic Adobe. Questi eventi del visualizzatore - combinazioni di variabili Adobe Analytics Adobe variabile Dynamic Media Classic determinano quali informazioni vengono riportate.

Oltre ad associare gli eventi del visualizzatore alle variabili, la schermata Configurazione di Adobe Analytics offre strumenti per attivare, modificare ed eliminare gli eventi del visualizzatore.

>[!NOTE]
>
>Ogni volta che modifichi le impostazioni dei rapporti di Adobe Analytics in Adobe Analytics, assicurati di accedere nuovamente ad Adobe Analytics da Adobe Dynamic Media Classic, salvare nuovamente le impostazioni di configurazione di Adobe Analytics e quindi ripubblicare.

Consultate [Accedere ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Consulta [Pubblicare informazioni sulla configurazione](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Assegnare variabili Adobe Analytics ad Adobe eventi e variabili del visualizzatore Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Utilizza la schermata Configurazione di Adobe Analytics per associare gli eventi del visualizzatore alle variabili di Adobe Analytics e alle variabili di Adobe Dynamic Media Classic. Per ogni evento del visualizzatore, scegli una variabile Adobe Analytics e una variabile Dynamic Media Classic di Adobe. Per istruzioni su come aprire la schermata Configurazione Adobe Analytics, consultate [Accedere ad Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Per assegnare variabili Adobe Analytics ad Adobe eventi e variabili del visualizzatore Dynamic Media Classic:**

1. Dopo aver effettuato l&#39;accesso ad Adobe Analytics da Adobe Dynamic Media Classic e aver selezionato una suite di rapporti, nella pagina Configurazione Adobe Analytics, nella colonna della tabella a destra, attiva un evento visualizzatore selezionando **[!UICONTROL Abilita]**.
1. Nella colonna Variabili visualizzare il selettore della coppia di variabili selezionando il pulsante freccia per l’evento visualizzatore desiderato.

   Consultate [Eventi dei visualizzatori](configuring-analytics-reports.md#viewer_events).

1. Aggiungi una variabile Adobe Dynamic Media Classic .

   Vedi [Adobe di variabili Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Aggiungete una variabile di Adobe Analytics.
1. (Facoltativo) Per aggiungere un&#39;altra coppia di variabili, selezionare **[!UICONTROL Aggiungi]**.
1. Selezionare **[!UICONTROL Salva]**.

   Dopo aver selezionato **[!UICONTROL Salva]**, l’evento visualizzatore, la relativa variabile Adobe Analytics e la relativa variabile Dynamic Media Classic Adobe, sono elencati nella schermata Configurazione di Adobe Analytics.

1. Nell&#39;angolo in basso a destra, selezionare **[!UICONTROL Chiudi]**.
1. Vai a **[!UICONTROL Pubblica]** > **[!UICONTROL Invia pubblicazione]** per eseguire una pubblicazione di Image Server.

   La pubblicazione è necessaria in modo che le informazioni contenute nei visualizzatori siano disponibili sui server Adobe Dynamic Media Classic.

### Eventi dei visualizzatori {#viewer-events}

Gli eventi del visualizzatore descrivono le azioni eseguite dagli utenti con i visualizzatori Adobe Dynamic Media Classic. Quando un utente avvia una determinata azione, ad esempio selezionando una miniatura o avviando o arrestando un video, il visualizzatore &quot;trasmette&quot; un evento alla pagina web, insieme ai dati associati a tale evento.

La tabella di seguito descrive gli eventi dei visualizzatori che potete aggiungere alla schermata Configurazione Adobe Analytics.

| Evento visualizzatore | Supporto per la piattaforma di visualizzatori HTML5 e visualizzatori | Descrizione |
| --- | --- | --- |
| LOAD (Caricamento) | **X** (eCatalog, zoom a comparsa, set 360 gradi, video, zoom) | Quando un utente avvia un visualizzatore |
| PAGE (Pagina) | **X** (eCatalog) | Negli eCatalogs, quando un utente compie una pagina; nei visualizzatori zoom di destinazione, quando un utente seleziona una destinazione o un campione di colore diverso. |
| SWAP (Scambio) | **X** (eCatalog, zoom a comparsa, set 360 gradi, video, zoom) | Quando un utente seleziona un&#39;altra miniatura per visualizzare un&#39;altra immagine. |
| ITEM (Elemento) | **X** (eCatalog) | Nei visualizzatori che supportano le mappe di immagine in cui sono definiti i rollover, quando un utente passa il puntatore su una mappa immagine per leggere il testo di rollover. |
| HREF | **X** (eCatalog) | Nei visualizzatori che supportano le mappe immagine, quando un utente seleziona un URL in una mappa immagine. |
| TARGET (Destinazione) |  | Nei visualizzatori zoom di destinazione, quando un utente seleziona una destinazione di zoom per ingrandire una parte dell’immagine. |
| SEARCH (Ricerca) |  | Negli eCatalog, quando un utente effettua una ricerca di parole. |
| PLAY (Riproduzione) | **X** (video) | Nei visualizzatori video, quando un utente seleziona Riproduci per avviare la riproduzione di un video.<br><br>**Nota:** se utilizzi la generazione di rapporti video basati su heartbeat di Adobe Analytics, non è necessario mappare alcuna variabile a questo evento del visualizzatore quando configuri Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video HTML5 e file multimediali diversi standard di Dynamic Media Classic Adobe. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consulta [Abilita rapporti video Adobe Analytics](enabling-analytics-video-reports.md). |
| PAUSE (Pausa) | **X** (video) | Nei visualizzatori video, quando un utente seleziona **[!UICONTROL Pausa]** per bloccare un video.<br><br>**Nota:** se utilizzi la generazione di rapporti video basati su heartbeat di Adobe Analytics, non è necessario mappare alcuna variabile a questo evento del visualizzatore quando configuri Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video HTML5 e file multimediali diversi standard di Dynamic Media Classic Adobe. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consulta [Abilita rapporti video Adobe Analytics](enabling-analytics-video-reports.md). |
| STOP (Interruzione) | **X** (video) | Nei visualizzatori video, quando un utente seleziona **[!UICONTROL Stop]** per interrompere la riproduzione di un video.<br><br>**Nota:** se utilizzi la generazione di rapporti video basati su heartbeat di Adobe Analytics, non è necessario mappare alcuna variabile a questo evento del visualizzatore quando configuri Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video HTML5 e file multimediali diversi standard di Dynamic Media Classic Adobe. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consulta [Abilita rapporti video Adobe Analytics](enabling-analytics-video-reports.md). |
| MILESTONE (Pietra miliare) | **X**  (Video) | Nei visualizzatori video, vengono generati degli eventi milestone (pietra miliare) quando l’utente guarda una percentuale di video pari a 0, 25, 50, 75 o 100.<br><br>**Nota:** se utilizzi la generazione di rapporti video basati su heartbeat di Adobe Analytics, non è necessario mappare alcuna variabile a questo evento del visualizzatore quando configuri Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat funziona con i visualizzatori video HTML5 e file multimediali diversi standard di Dynamic Media Classic Adobe. Il lettore video genera dati di tracciamento per la visualizzazione in Adobe Analytics Video Reports. Consulta [Abilita rapporti video Adobe Analytics](enabling-analytics-video-reports.md). |
| SWATCH (Campione) | **X** (zoom a comparsa, zoom) | Questo evento visualizzatore è mappato all’evento visualizzatore PAGINA in Adobe Dynamic Media Classic. |
| ZOOM | **X** (eCatalog, set 360 gradi, zoom) | Questo evento non è seguito da Adobe Analytics. |
| PAN (Panning) | **X** (eCatalog, set 360 gradi, zoom) | Questo evento non è seguito da Adobe Analytics. |
| SPIN (Set a 360 gradi) | **X** (Set a 360 gradi) | Questo evento non è seguito da Adobe Analytics. |

### Adobe di variabili Dynamic Media Classic {#scene-variables}

Per ogni evento visualizzatore nella schermata Configurazione Adobe Analytics, scegli una variabile Adobe Analytics e un *Adobe variabile Dynamic Media Classic*. Ad Adobe, le variabili Dynamic Media Classic rappresentano i dati che è possibile ottenere per un rapporto. La variabile `searchTerm`, ad esempio, riporta le parole chiavi utilizzate nelle ricerche effettuate negli eCatalog.

La tabella seguente descrive Adobe di variabili Dynamic Media Classic:

| Variabile Adobe Dynamic Media Classic | Descrizione |
| --- | --- |
| asset | Adobe ID risorsa Dynamic Media Classic o file del percorso video. |
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

## Attivare, modificare ed eliminare gli eventi del visualizzatore {#activating-editing-and-deleting-viewer-events}

Nella schermata Configurazione Adobe Analytics, potete attivare, modificare e quindi eliminare gli eventi dei visualizzatori:

* **Attiva**  - Seleziona  **** Abilita o  **** Disabilita per disattivare un evento visualizzatore selezionato.

* **Modifica** : seleziona un evento visualizzatore e seleziona il pulsante grigio  **[!UICONTROL Visualizza/]** Modifica variabili . Negli elenchi a discesa Variabile Dynamic Media Classic Adobe e Variabile Adobe Analytics , scegli una variabile diversa da ciascun rispettivo elenco. Per ulteriori informazioni, consulta [Assegnazione di variabili Adobe Analytics agli eventi e alle variabili del visualizzatore Dynamic Media Classic](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables) di Adobe.

* **Elimina**  - Seleziona un evento visualizzatore e seleziona il pulsante grigio  **[!UICONTROL Visualizza/]** Modifica variabili . Selezionare **[!UICONTROL Elimina]**.
