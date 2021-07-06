---
title: '"Avvio rapido: video"'
description: Introduzione e avvio rapido ad Adobe Dynamic Media Classic Video per aiutarti a iniziare rapidamente a usare.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Visualizzatori,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1425'
ht-degree: 43%

---

# Avvio rapido: video{#quick-start-video}

Adobe Dynamic Media Classic Video è una soluzione end-to-end che semplifica la pubblicazione di video adattivi di alta qualità per lo streaming su diversi schermi, tra cui desktop, iOS, Android™, BlackBerry® e dispositivi mobili Windows®. Un set video adattivo raggruppa versioni dello stesso video codificate con diversi bitrate e formati quali 400, 800 e 100 kbps. Il computer desktop o il dispositivo mobile rileva l’ampiezza di banda disponibile.

Ad esempio, un dispositivo mobile iOS può rilevare un’ampiezza di banda 3G, 4G o Wi-Fi. Quindi seleziona automaticamente il video con la codifica corretta tra i vari bitrate presenti nel set video adattivo. Il video viene inviato in streaming a computer desktop, dispositivi mobili o tablet.

Inoltre, la qualità video viene modificata automaticamente e in modo dinamico in base alle condizioni della rete sul computer desktop o sul dispositivo mobile. Inoltre, se un cliente entra in modalità a schermo intero su un desktop, il set video adattivo risponde utilizzando una risoluzione migliore, migliorando l’esperienza di visualizzazione del cliente. L’utilizzo di Adaptive Video Sets offre la migliore riproduzione possibile per i clienti che riproducono video Dynamic Media Classic su più schermi e dispositivi.

Per determinare quale video codificato riprodurre o selezionare per la riproduzione, il lettore video utilizza l’algoritmo seguente:

1. Il lettore video carica il frammento video iniziale in base al bit rate più vicino al valore impostato per il &quot;bitrate iniziale&quot; nel lettore stesso.
1. Il lettore video commuta in base ai cambiamenti della velocità della larghezza di banda utilizzando i seguenti criteri:

   1. Player sceglie il flusso di banda più alto sotto o uguale alla larghezza di banda stimata.
   1. Il lettore considera solo l&#39;80% della larghezza di banda disponibile. Tuttavia, se sta cambiando, è più conservativo solo al 70% per evitare sovrastimazioni e dover immediatamente tornare indietro.

Per informazioni tecniche, consulta la logica dell’algoritmo in [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) .

Per la gestione di set video singoli e di set video adattivi, Dynamic Media Classic supporta le seguenti funzioni:

* Caricamento di video da numerosi formati video e formati audio supportati e codifica dei video nel formato MP4 H.264 per la riproduzione su schermi diversi. È possibile utilizzare predefiniti video adattivi di Dynamic Media Classic, predefiniti di codifica video singoli o personalizzare la propria codifica per controllare la qualità e le dimensioni del video.

   Quando viene generato un set video adattivo, questo include video MP4.

   >[!NOTE]
   >
   >I video master/sorgente e qualsiasi altro video in formato sorgente sono *non* aggiunti a un set video adattivo.

* sottotitoli video nei visualizzatori Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light e nella navigazione dei capitoli video nei visualizzatori Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light.

   Consultate [Aggiunta di sottotitoli a video](adding-captions-video.md).

   Consultate [Aggiunta di marcatori capitolo a video](adding-chapter-markers-video.md).

* Organizzare, sfogliare e ricercare i video sfruttando appieno i metadati, per una gestione efficiente delle risorse video. 
* Distribuire set video adattivi sul web e su desktop e dispositivi mobili, inclusi iPhone, iPad, Android™, BlackBerry® e i telefoni Windows®.

   Lo streaming video adattivo è supportato su varie piattaforme iOS.

   Per informazioni aggiornate, consulta la [Guida di riferimento visualizzatori di Adobi](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html) .

   Dynamic Media Classic supporta la riproduzione video mobile per video MP4 H.264. È possibile trovare i dispositivi BlackBerry® che supportano questo formato video nel seguente sito web:

   Vedi [Formati video supportati su BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   È possibile trovare i dispositivi Windows® che supportano questo formato video nel seguente percorso:

   Vedere [Formati video supportati su Windows® Phone](https://docs.microsoft.com/en-us/).

* Riproduci il video utilizzando i predefiniti per visualizzatori di Dynamic Media Classic, tra cui:

   * Visualizzatori per singoli video.
   * Visualizzatori per contenuti multimediali misti che combinano video e immagini.

* Configurare i lettori video per soddisfare le esigenze di branding.
* Integrare video nel sito Web oppure nel sito o nell’applicazione mobile con un semplice URL video o codice incorporato.

**Guida introduttiva**

La seguente descrizione dettagliata del flusso di lavoro è stata progettata per aiutarti a iniziare rapidamente a usare i set di video adattivi in Dynamic Media Classic. Alla fine di ciascun passaggio è riportato un riferimento a un argomento correlato con ulteriori informazioni.

## 1. Caricamento e codifica dei video

Potete caricare e generare i set di video adattivi utilizzando uno dei due scenari seguenti:

* **Carica video precodificati** : se i video sono già stati codificati all’esterno di Dynamic Media Classic, nella barra di navigazione globale fai clic su  **** Carica per sfogliare e caricare i file video MP4 direttamente in Dynamic Media Classic. Fate clic su **[!UICONTROL Genera]** > **[!UICONTROL Set video adattivi]**. Individuate i file video. Trascinate i file video desiderati nella tabella Set video adattivo, quindi salvate il set.
* **Carica video sorgente principali**  - Se i video non sono codificati, fai clic su  **** Carica nella barra di navigazione globale per caricare i file sorgente video master (non MP4) e fai clic su Codifica classica Dynamic Media in file MP4 per te. Nella finestra di dialogo **[!UICONTROL Opzioni processo di caricamento]**, in **[!UICONTROL Opzioni video]**, seleziona **[!UICONTROL Video adattivo]**.

   Questa opzione preferita consente di creare un set di video adattivi che applica automaticamente al video il predefinito di codifica corretto, da 16:9 o 4:3, in base alle dimensioni del video caricato. Quando inviate il processo di caricamento, viene automaticamente creato un set di video adattivi che comprende tre codifiche video con le proporzioni appropriate.

   Oppure, nella stessa finestra di dialogo **[!UICONTROL Opzioni processo]**, in **[!UICONTROL Opzioni video]**, espandi **[!UICONTROL Predefiniti codifica singola]**. Seleziona i singoli predefiniti di codifica video desiderati da **Desktop**, **Mobile (iPhone, iPad, Android™)** e **Tablet (iPad, Android™)** in modo da creare i file MP4.

* In alternativa, è possibile rielaborare un video principale utilizzando la funzione **[!UICONTROL Rielabora]** . I video appena codificati vengono aggiunti al set video adattivo esistente.

Consultate [Caricamento e codifica dei video](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Facoltativo**

Dynamic Media Classic offre numerosi predefiniti di codifica video. Questi predefiniti riflettono le impostazioni di codifica video più comuni utilizzate oggi e sono ottimizzati per la riproduzione su pagine di destinazione.

Tuttavia, qualora sia richiesta ulteriore personalizzazione, gli amministratori possono creare dei predefiniti video per personalizzare le dimensioni e l’esperienza di riproduzione video per gli utenti finali. Gli amministratori possono aggiungere e gestire i predefiniti video dalla pagina Predefiniti video disponibile in **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Predefiniti video]** > **[!UICONTROL Predefiniti codifica singola]**. La pagina Predefiniti video offre opzioni per aggiungere, modificare, eliminare e attivare i predefiniti per video.

Consultate [Utilizzo dei predefiniti di codifica video](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Anteprima dei video in un visualizzatore video

Per vedere in che modo un video verrà riprodotto per gli utenti finali su un computer desktop, un sito Web o un dispositivo mobile, selezionate il video nel pannello Sfoglia e fate clic su **[!UICONTROL Anteprima]**.

Consultate [Anteprima dei video in un visualizzatore video](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

È possibile riprodurre il video nella pagina Anteprima. È inoltre possibile scegliere diversi visualizzatori video per scoprire come appare il video in diversi lettori. È consigliato utilizzare il lettore video HTML5 per la riproduzione per schermi diversi su computer desktop, tablet e dispositivi mobili.

**Facoltativo**

Personalizzazione dei predefiniti per visualizzatori : Dynamic Media Classic offre predefiniti per visualizzatori per la distribuzione di video. Tali predefiniti determinano l’aspetto del visualizzatore e la modalità di funzionamento dei controlli di riproduzione. Per personalizzare il visualizzatore video, gli amministratori possono aggiungere e gestire i predefiniti per visualizzatore dalla pagina Predefiniti visualizzatore. Per aprire questa pagina, nell’angolo in alto a destra di Dynamic Media Classic, fai clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Predefiniti visualizzatore]**. Dalla pagina Predefiniti visualizzatore è possibile aggiungere, modificare, eliminare e attivare i predefiniti per visualizzatore.

Consultate [Utilizzo dei predefiniti per visualizzatori video](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

## 3. Distribuzione di video nei siti web e nei siti mobili

Per integrare i video nel sito Web, potete effettuare una delle seguenti operazioni:

* Visualizza il video nella relativa finestra a comparsa o modale, nel qual caso utilizza la funzione **[!UICONTROL Copia URL]** .

   Per ottenere l’URL per un video, nella vista Griglia o Elenco selezionatelo nel pannello Sfoglia. Fai clic su **[!UICONTROL Anteprima]**, quindi fai clic su **[!UICONTROL Copia URL]** a destra di `Universal_HTML5_Viewer`.

   Quando fai clic su **[!UICONTROL Copia URL]**, l&#39;URL viene copiato negli Appunti. Inserite questo codice nell’HTML del sito Web, del sito mobile o dell’applicazione. 

   >[!NOTE]
   >
   >gli URL diventano attivi solo dopo la pubblicazione del video o del set di video adattivi.

* Visualizza il video incorporato nella pagina web, nel qual caso utilizza la funzione **[!UICONTROL Incorpora codice]** .

   Per ottenere il codice da incorporare per un video, nella vista Griglia o Elenco selezionate il video nel pannello Sfoglia. Fai clic su **[!UICONTROL Anteprima]** > **[!UICONTROL Elenco visualizzatori]**. Nella colonna Azioni della tabella, fai clic su **[!UICONTROL Incorpora codice]** a destra di `Universal_HTML5_Video`. Non è possibile modificare il codice.

   Fai clic su **[!UICONTROL Chiudi]** e incolla il codice di incorporamento nelle pagine web.

   >[!NOTE]
   >
   >Incorpora codice è attivato solo dopo la pubblicazione del video o del set di video adattivi.

Consultate [Implementazione dei video nei siti Web e siti mobili](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Best practice per la codifica video](uploading-encoding-videos.md#best_practices_for_video_encoding)

