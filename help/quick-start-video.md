---
title: "Avvio rapido: Video in Adobe Dynamic Media Classic"
description: Introduzione e avvio rapido a Adobe Dynamic Media Classic Video per aiutarti a iniziare rapidamente a usare i contenuti.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1808'
ht-degree: 25%

---

# Avvio rapido: Video in Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video è una soluzione end-to-end che semplifica la pubblicazione di video adattivi di alta qualità per lo streaming su più schermi, tra cui desktop, iOS, Android™, BlackBerry® e dispositivi mobili Windows®. Un set video adattivo raggruppa versioni dello stesso video codificate con diversi bitrate e formati quali 400, 800 e 100 kbps. Il computer desktop o il dispositivo mobile rileva l’ampiezza di banda disponibile.

Ad esempio, un dispositivo mobile iOS può rilevare un’ampiezza di banda 3G, 4G o Wi-Fi. Quindi seleziona automaticamente il video con la codifica corretta tra i vari bitrate presenti nel set video adattivo. Il video viene inviato in streaming a computer desktop, dispositivi mobili o tablet.

Inoltre, la qualità video viene modificata automaticamente e in modo dinamico in base alle condizioni della rete sul computer desktop o sul dispositivo mobile. Inoltre, se un cliente entra in modalità a schermo intero su un desktop, il set video adattivo risponde utilizzando una risoluzione migliore, migliorando l’esperienza di visualizzazione del cliente. L’utilizzo di Adaptive Video Sets offre la migliore riproduzione possibile per i clienti che riproducono video Adobe Dynamic Media Classic su schermi e dispositivi multipli.

Per determinare quale video codificato riprodurre o selezionare per la riproduzione, il lettore video utilizza l’algoritmo seguente:

1. Il lettore video carica il frammento video iniziale in base al bit rate più vicino al valore impostato per il &quot;bitrate iniziale&quot; nel lettore stesso.
1. Il lettore video commuta in base ai cambiamenti della velocità della larghezza di banda utilizzando i seguenti criteri:

   1. Player sceglie il flusso di banda più alto sotto o uguale alla larghezza di banda stimata.
   1. Il lettore considera solo l&#39;80% della larghezza di banda disponibile. Tuttavia, se sta cambiando, è più conservativo solo al 70% per evitare sovrastimazioni e dover immediatamente tornare indietro.

Consulta la logica dell’algoritmo in [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) per informazioni tecniche al riguardo.

Per la gestione di set video singoli e di set video adattivi, Adobe Dynamic Media Classic supporta quanto segue:

* Caricamento di video da numerosi formati video e formati audio supportati e codifica di video in formato MP4 H.264 per la riproduzione su più schermi. È possibile utilizzare predefiniti video adattivi Adobe Dynamic Media Classic, predefiniti di codifica video singoli o personalizzare la propria codifica per controllare la qualità e le dimensioni del video.

Vedi [Attivare o disattivare i predefiniti video adattivi](/help/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Vedi anche [Predefiniti video](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) video di formazione.

Quando viene generato un set video adattivo, questo include video MP4.

>[!NOTE]
>
>I video principali/sorgente e qualsiasi altro formato video sorgente sono *not* aggiunto a un set video adattivo.

* sottotitoli video nei visualizzatori Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light e nella navigazione dei capitoli video nei visualizzatori Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light.

   Vedi [Aggiungere sottotitoli al video](adding-captions-video.md).

   Vedi [Aggiungere marcatori capitolo al video](adding-chapter-markers-video.md).

* Organizzare, sfogliare e ricercare i video sfruttando appieno i metadati, per una gestione efficiente delle risorse video. 
* Distribuire set video adattivi sul web e su desktop e dispositivi mobili, compresi iPhone, iPad, Android™, BlackBerry® e Windows®.

   Lo streaming video adattivo è supportato su varie piattaforme iOS.

   Scopri l’ultimo supporto nella sezione [Guida di riferimento visualizzatori di Adobi](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

   Adobe Dynamic Media Classic supporta la riproduzione video mobile per video MP4 H.264. È possibile trovare i dispositivi BlackBerry® che supportano questo formato video nel seguente sito web:

   Vedi [Formati video supportati su BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   È possibile trovare i dispositivi Windows® che supportano questo formato video nel seguente percorso:

   Vedi [Formati video supportati su Windows® Phone](https://docs.microsoft.com/en-us/).

* Riproduci il video utilizzando i predefiniti per visualizzatori Adobe Dynamic Media Classic, tra cui:

   * Visualizzatori per singoli video.
   * Visualizzatori per contenuti multimediali misti che combinano video e immagini.

* Configurare i lettori video per soddisfare le esigenze di branding.
* Integrare video nel sito Web oppure nel sito o nell’applicazione mobile con un semplice URL video o codice incorporato.

Guarda i seguenti video di formazione:
* [Panoramica video MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [Anteprima video MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [Caricamento video MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Panoramica dello streaming](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Guida introduttiva**

La seguente descrizione dettagliata del flusso di lavoro è stata progettata per aiutarti a iniziare rapidamente a usare i set di video adattivi in Adobe Dynamic Media Classic. Dopo ogni passaggio, è disponibile un riferimento incrociato all’intestazione di un argomento in cui è possibile trovare ulteriori informazioni.

## 1. Caricare e codificare i video

Potete caricare e generare i set di video adattivi utilizzando uno dei due scenari seguenti:

* **Caricare video precodificati** - Se i video sono già stati codificati all’esterno di Adobe Dynamic Media Classic, nella barra di navigazione globale seleziona **[!UICONTROL Carica]** per sfogliare e caricare i file video MP4 direttamente in Adobe Dynamic Media Classic. Quindi, vai a **[!UICONTROL Crea]** > **[!UICONTROL Set video adattivi]**. Individuate i file video. Trascina i file video desiderati nella tabella Set video adattivo e salva il set.
* **Caricare video sorgente principali** - Se i video non sono codificati, nella barra di navigazione globale seleziona **[!UICONTROL Carica]** per caricare i file di origine video principali (non MP4). Adobe Dynamic Media Classic li codifica in file MP4 per voi. In **[!UICONTROL Opzioni processo di caricamento]** finestra di dialogo, sotto **[!UICONTROL Opzioni eVideo]**, seleziona **[!UICONTROL Video adattivo]**.

   Questa opzione preferita consente di creare un set di video adattivi che applica automaticamente al video il predefinito di codifica corretto, da 16:9 o 4:3, in base alle dimensioni del video caricato. Quando si invia il processo di caricamento, viene automaticamente creato un set video adattivo che include tre impostazioni video codificate con le proporzioni corrette.

   Oppure, nello stesso **[!UICONTROL Opzioni processo]** finestra di dialogo, sotto **[!UICONTROL Opzioni eVideo]**, espandi **[!UICONTROL Predefiniti di codifica singoli]**. Seleziona i singoli predefiniti di codifica video da cui vuoi ottenere **Desktop**, **Mobile (iPhone, iPad, Android™)** e **Tablet (iPad, Android™)** in modo da creare i file MP4.

* Oppure, puoi rielaborare un video principale utilizzando la **[!UICONTROL Rielaborazione]** funzionalità. I video appena codificati vengono aggiunti al set video adattivo esistente.

Vedi [Caricare e codificare video](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Facoltativo**

Adobe Dynamic Media Classic offre numerosi predefiniti di codifica video. Questi predefiniti riflettono le impostazioni di codifica video più comuni utilizzate oggi e sono ottimizzati per la riproduzione su pagine di destinazione.

Tuttavia, qualora sia richiesta ulteriore personalizzazione, gli amministratori possono creare dei predefiniti video per personalizzare le dimensioni e l’esperienza di riproduzione video per gli utenti finali. Gli amministratori possono aggiungere e gestire i predefiniti per video dalla pagina Predefiniti video disponibile in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti video]** > **[!UICONTROL Predefiniti di codifica singoli]**. La pagina Predefiniti video offre opzioni per aggiungere, modificare, eliminare e attivare i predefiniti per video.

Vedi [Utilizzare i predefiniti di codifica video](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Anteprima di video in un visualizzatore video

Per vedere come viene riprodotto un video per gli utenti finali su un desktop, un sito web o un dispositivo mobile, seleziona il video nel pannello Sfoglia, quindi seleziona **[!UICONTROL Anteprima]**.

Vedi [Anteprima di video in un visualizzatore video](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

È possibile riprodurre il video nella pagina Anteprima. È inoltre possibile scegliere diversi visualizzatori video per scoprire come appare il video in diversi lettori. È consigliato utilizzare il lettore video HTML5 per la riproduzione per schermi diversi su computer desktop, tablet e dispositivi mobili.

**Facoltativo**

Personalizzazione dei predefiniti per visualizzatori : Adobe Dynamic Media Classic offre predefiniti per visualizzatori per la distribuzione di video. Tali predefiniti determinano l’aspetto del visualizzatore e la modalità di funzionamento dei controlli di riproduzione. Per personalizzare il visualizzatore video, gli amministratori possono aggiungere e gestire i predefiniti per visualizzatore dalla pagina Predefiniti visualizzatore. Per aprire questa pagina, nell’angolo in alto a destra di Adobe Dynamic Media Classic, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**. Dalla pagina Predefiniti visualizzatore è possibile aggiungere, modificare, eliminare e attivare i predefiniti per visualizzatore.

Vedi [Utilizzare i predefiniti per visualizzatori video](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Vedi anche [Predefiniti video](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) video di formazione.

## 3. Distribuire video sui siti web e sui siti mobili

Per integrare i video nel sito Web, potete effettuare una delle seguenti operazioni:

* Visualizza il video nella propria finestra a comparsa o modale, nel qual caso utilizza il **[!UICONTROL Copia URL]** funzionalità.

   Per ottenere l’URL per un video, nella vista Griglia o Elenco selezionatelo nel pannello Sfoglia. Seleziona **[!UICONTROL Anteprima]**, quindi seleziona **[!UICONTROL Copia URL]** al diritto di `Universal_HTML5_Viewer`.

   Quando selezioni **[!UICONTROL Copia URL]**, l’URL viene copiato negli Appunti. Inserite questo codice nell’HTML del sito Web, del sito mobile o dell’applicazione. 

   >[!NOTE]
   >
   >gli URL diventano attivi solo dopo la pubblicazione del video o del set di video adattivi.

* Visualizza il video incorporato nella pagina web, nel qual caso utilizza il **[!UICONTROL Codice di incorporamento]** funzionalità.

   Per ottenere il codice da incorporare per un video, nella vista Griglia o Elenco selezionate il video nel pannello Sfoglia. Vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**. Nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]** al diritto di `Universal_HTML5_Video`. Non è possibile modificare il codice.

   Seleziona **[!UICONTROL Chiudi]** e incolla il codice di incorporamento nelle pagine web.

   >[!NOTE]
   >
   >Incorpora codice è attivato solo dopo la pubblicazione del video o del set di video adattivi.

Vedi [Distribuire video sui siti web e sui siti mobili](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Best practice per la codifica video](uploading-encoding-videos.md#best_practices_for_video_encoding)

