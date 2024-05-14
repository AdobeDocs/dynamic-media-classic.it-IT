---
title: "Guida rapida: Video in Adobe Dynamic Media Classic"
description: Introduzione e Guida rapida a Adobe Dynamic Media Classic Video per aiutarti a iniziare subito a utilizzare il prodotto.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '1443'
ht-degree: 28%

---

# Guida introduttiva: Video in Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video è una soluzione end-to-end che consente di pubblicare facilmente video adattivi di alta qualità per lo streaming su più schermi, tra cui dispositivi mobili desktop, iOS, Android™, BlackBerry® e Windows®. Un set video adattivo raggruppa versioni dello stesso video codificate con diversi bitrate e formati quali 400, 800 e 100 kbps. Il computer desktop o il dispositivo mobile rileva l’ampiezza di banda disponibile.

Ad esempio, un dispositivo mobile iOS può rilevare un’ampiezza di banda 3G, 4G o Wi-Fi. Quindi seleziona automaticamente il video con la codifica corretta tra i vari bitrate presenti nel set video adattivo. Il video viene inviato in streaming a computer desktop, dispositivi mobili o tablet.

Inoltre, la qualità video viene modificata automaticamente e in modo dinamico in base alle condizioni della rete sul computer desktop o sul dispositivo mobile. Inoltre, se un cliente entra in modalità a tutto schermo su un desktop, il set video adattivo risponde con una risoluzione migliore, migliorando l’esperienza di visualizzazione del cliente. L’utilizzo di set video adattivi offre la migliore riproduzione possibile. È ideale per i clienti che riproducono video Adobe Dynamic Media Classic su più schermi e dispositivi.

Per determinare quale video codificato riprodurre o selezionare per la riproduzione, il lettore video utilizza l’algoritmo seguente:

1. Il lettore video carica il frammento video iniziale in base al bitrate più vicino al valore impostato per &quot;bitrate iniziale&quot; nel lettore stesso.
1. Il lettore video cambia in base alle modifiche apportate alla velocità della larghezza di banda utilizzando i seguenti criteri:

   1. Il lettore sceglie il flusso di larghezza di banda più alto al di sotto o uguale alla larghezza di banda stimata.
   1. Il lettore considera solo l&#39;80% della larghezza di banda disponibile. Tuttavia, se si sta passando, è più prudente solo al 70% per evitare di sopravvalutare e tornare immediatamente indietro.

Vedi la logica dell’algoritmo in [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) per informazioni tecniche su di esso.

Per la gestione di singoli video e set di video adattivi, Adobe Dynamic Media Classic supporta quanto segue:

* Caricamento di video da numerosi formati video supportati. Caricamento di formati audio e codifica video in formato MP4 H.264 per la riproduzione su più schermi. È possibile utilizzare predefiniti per video adattivi Adobe Dynamic Media Classic, predefiniti per codifica video singola o personalizzare la propria codifica per controllare la qualità e le dimensioni del video.

Consulta [Attivare o disattivare i predefiniti per video adattivi](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Vedi anche [Predefiniti video](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) video di formazione.

Quando viene generato un set video adattivo, questo include video MP4.

>[!NOTE]
>
>I video principali/sorgente e qualsiasi altro video in formato sorgente sono *non* aggiunto a un set video adattivo.

* Sottotitoli video nei visualizzatori Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light e nella navigazione dei capitoli video nei visualizzatori Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light.

  Consulta [Aggiungere didascalie a un video](adding-captions-video.md).

  Consulta [Aggiungere marcatori capitolo a un video](adding-chapter-markers-video.md).

* Organizzare, sfogliare e ricercare i video sfruttando appieno i metadati, per una gestione efficiente delle risorse video. 
* Distribuisci set video adattivi sul Web, sui desktop e sui dispositivi mobili, inclusi i telefoni iPhone, iPad, Android™, BlackBerry® e Windows®.

  Lo streaming video adattivo è supportato su varie piattaforme iOS.

  Scopri il supporto più recente in [Guida di riferimento per i visualizzatori di Adobi](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources).

  Adobe Dynamic Media Classic supporta la riproduzione di video per dispositivi mobili per video MP4 H.264. <!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  I dispositivi Windows® che supportano questo formato video sono disponibili nei seguenti percorsi:

  [Formati video supportati su Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs).

* Riproduci il video utilizzando i predefiniti visualizzatore Adobe Dynamic Media Classic, inclusi i seguenti elementi:

   * Visualizzatori video singoli.
   * Visualizzatori per contenuti multimediali misti che combinano video e immagini.

* Configurare i lettori video per soddisfare le esigenze di branding.
* Integrare video nel sito Web oppure nel sito o nell’applicazione mobile con un semplice URL video o codice incorporato.

Guarda i seguenti video di formazione:
* [Panoramica video MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [Anteprima video MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [Caricamento video MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Panoramica streaming](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Guida rapida**

La seguente descrizione dettagliata del flusso di lavoro è stata progettata per aiutarti a iniziare rapidamente a utilizzare i set per video adattivi in Adobe Dynamic Media Classic. Dopo ogni passaggio, viene inserito un riferimento incrociato a un titolo di argomento in cui è possibile trovare ulteriori informazioni.

## 1. Caricare e codificare i video

Potete caricare e generare i set di video adattivi utilizzando uno dei due scenari seguenti:

* **Caricare video precodificati**: se i tuoi video erano già codificati esternamente da Adobe Dynamic Media Classic, nella barra di navigazione globale seleziona **[!UICONTROL Carica]**. Sfoglia e carica i file video MP4 direttamente su Adobe Dynamic Media Classic. Quindi, vai a **[!UICONTROL Genera]** > **[!UICONTROL Set video adattivi]**. Individuate i file video. Trascinate i file video desiderati nella tabella Set video adattivo, quindi salvate il set.
* **Carica video sorgente principale**: se i video non sono codificati, nella barra di navigazione globale seleziona **[!UICONTROL Carica]** per caricare i file sorgente video primari (non MP4). Adobe Dynamic Media Classic li codifica automaticamente in file MP4. In **[!UICONTROL Opzioni processo di caricamento]** finestra di dialogo, sotto **[!UICONTROL Opzioni eVideo]**, seleziona **[!UICONTROL Video adattivo]**.

  Con questa opzione preferita, puoi creare set di video adattivi. Il predefinito di codifica corretto viene applicato automaticamente al video, 16:9 o 4:3, in modo che corrisponda alle dimensioni del video caricato. Quando invii il processo di caricamento, viene automaticamente creato un set di video adattivi che include tre impostazioni di codifica video nelle proporzioni corrette.

  Oppure, nello stesso **[!UICONTROL Opzioni processo]** finestra di dialogo, sotto **[!UICONTROL Opzioni eVideo]**, espandi **[!UICONTROL Predefiniti codifica singola]**. Selezionate i singoli predefiniti di codifica video desiderati. Puoi selezionare **Desktop**, **Mobile (iPhone, iPad, Android™)**, e **Tablet (iPad, Android™)** per creare i file MP4.

* In alternativa, è possibile rielaborare un video principale utilizzando **[!UICONTROL Rielaborazione]** funzionalità. I video appena codificati vengono aggiunti al set video adattivo esistente.

Consulta [Caricare e codificare i video](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Facoltativo**

Adobe Dynamic Media Classic offre numerosi predefiniti per la codifica video. Questi predefiniti riflettono le impostazioni di codifica video più comuni attualmente in uso e sono ottimizzati per la riproduzione su pagine di destinazione.

Tuttavia, qualora sia richiesta ulteriore personalizzazione, gli amministratori possono creare dei predefiniti video per personalizzare le dimensioni e l’esperienza di riproduzione video per gli utenti finali. Gli amministratori possono aggiungere e gestire predefiniti video dalla pagina Predefiniti video disponibile in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Predefiniti per video]** > **[!UICONTROL Predefiniti codifica singola]**. La pagina Predefiniti video offre opzioni per aggiungere, modificare, eliminare e attivare i predefiniti per video.

Consulta [Utilizzare i predefiniti di codifica video](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Visualizzare l’anteprima dei video in un visualizzatore video

Per vedere come viene riprodotto un video per gli utenti finali su un desktop, sul sito Web o su un dispositivo mobile, seleziona il video nel pannello Sfoglia. Quindi seleziona **[!UICONTROL Anteprima]**.

Consulta [Anteprima di video in un visualizzatore video](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

È possibile riprodurre il video nella pagina Anteprima. Puoi anche scegliere diversi visualizzatori video per scoprire come il tuo video appare in diversi lettori. È consigliato utilizzare il lettore video HTML5 per la riproduzione per schermi diversi su computer desktop, tablet e dispositivi mobili.

**Facoltativo**

Personalizzazione dei predefiniti per visualizzatori: Adobe Dynamic Media Classic offre predefiniti per visualizzatori per la distribuzione di video. Tali predefiniti determinano l’aspetto del visualizzatore e la modalità di funzionamento dei controlli di riproduzione. Per personalizzare il visualizzatore video, gli amministratori possono aggiungere e gestire i predefiniti per visualizzatore dalla pagina Predefiniti visualizzatore. Per aprire questa pagina, nell’angolo superiore destro di Adobe Dynamic Media Classic, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**. Dalla pagina Predefiniti visualizzatore è possibile aggiungere, modificare, eliminare e attivare i predefiniti per visualizzatore.

Consulta [Utilizzare i predefiniti visualizzatore video](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Vedi anche [Predefiniti video](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) video di formazione.

## 3. Distribuire video sui siti web e mobili

Per integrare i video nel sito Web, potete effettuare una delle seguenti operazioni:

* Visualizzare il video nella propria finestra a comparsa o modale, nel qual caso utilizzare il **[!UICONTROL Copia URL]** funzionalità.

  Per ottenere l’URL per un video, nella vista Griglia o Elenco selezionatelo nel pannello Sfoglia. Seleziona **[!UICONTROL Anteprima]** e quindi selezionare **[!UICONTROL Copia URL]** a destra di `Universal_HTML5_Viewer`.

  Quando selezioni **[!UICONTROL Copia URL]**, l’URL viene copiato negli Appunti. Inserite questo codice nell’HTML del sito Web, del sito mobile o dell’applicazione. 

  >[!NOTE]
  >
  >gli URL diventano attivi solo dopo la pubblicazione del video o del set di video adattivi.

* Visualizza il video incorporato nella pagina web, nel qual caso utilizza **[!UICONTROL Codice di incorporamento]** funzionalità.

  Per ottenere il codice da incorporare per un video, nella vista Griglia o Elenco selezionate il video nel pannello Sfoglia. Vai a **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**. Nella colonna Azioni della tabella, seleziona **[!UICONTROL Codice di incorporamento]** a destra di `Universal_HTML5_Video`. Non è possibile modificare il codice.

  Seleziona **[!UICONTROL Chiudi]** e incolla il codice da incorporare in una o più pagine web.

  >[!NOTE]
  >
  >Il codice di incorporamento viene attivato solo dopo la pubblicazione del video o del set di video adattivi.

Consulta [Distribuire video sui siti Web e mobili](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Best practice per la codifica video](uploading-encoding-videos.md#best_practices_for_video_encoding)
