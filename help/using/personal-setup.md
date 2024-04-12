---
title: Configurazione personale
description: Tutti gli utenti possono modificare le impostazioni nella schermata Personal Setup (Impostazione personale) di Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 23%

---

# Configurazione personale {#personal-setup}

Le impostazioni della schermata Configurazione personale possono essere modificate da tutti gli utenti. Per aprire la schermata Impostazione personale, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**.

>[!NOTE]
>
>Nella schermata Impostazione personale viene visualizzato il ruolo utente in Adobe Dynamic Media Classic: Amministratore società, Amministratore o Utente.

Le impostazioni della schermata Configurazione personale controllano il comportamento predefinito del pannello Sfoglia, il modo in cui ricevete i messaggi e-mail e le impostazioni della password. Ricorda di selezionare **[!UICONTROL Salva]** dopo aver modificato queste impostazioni.

## Informazioni sul mio account

Identifica il vostro nome e nome dell’account, il nome utente (indirizzo e-mail) e il ruolo utente che vi è stato assegnato.

## Desktop

* **Cancella cache immagini** - Rimuove dal computer tutti i file immagine Dynamic Medie memorizzati nella cache di Adobe.
* **Cancella cache risorse** - Rimuove dal computer tutti i file di risorse Adobe Dynamic Medie memorizzati nella cache.

Oltre a cancellare l’immagine e la cache delle risorse utilizzando l’app desktop, puoi cancellare manualmente la cache direttamente dal file system. In base al sistema operativo in uso, accedi a:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**Per installare Adobe Dynamic Medie Creative Suite Extension:**

1. In Adobe Dynamic Media Classic, nella barra degli strumenti, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**, in Estensione Creative Suite, seleziona **[!UICONTROL Scarica ora]** per scaricare `s7csxs.zxp` file.
1. Seleziona la **[!UICONTROL Installazione]** e **[!UICONTROL Requisiti di sistema]** collegamenti per ulteriori informazioni sull’estensione.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator's package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Browser

* **[!UICONTROL Dimensione miniatura]** - Determina le dimensioni predefinite delle miniature in Visualizzazione griglia nel pannello Sfoglia.
* **[!UICONTROL Visualizzazione predefinita libreria risorse]** - Determina se le risorse nella Libreria risorse per i set di build vengono visualizzate come miniature o per nome. Se dovete gestire grandi quantità di risorse nella libreria, è consigliabile visualizzarle per nome. Ad esempio, se state creando un eCatalog di grandi dimensioni contenente numerosi file PDF, potete visualizzare le risorse per nome per ridurre la lunghezza dell’elenco.
* **[!UICONTROL Ordine di navigazione predefinito]** - Determina l’ordine in cui le risorse vengono visualizzate per impostazione predefinita nel pannello Sfoglia. Scegliete un criterio di ordinamento nel menu e specificate se l’ordine deve essere crescente o decrescente.
* **[!UICONTROL Percorso predefinito per la navigazione]** : consente di impostare il percorso di navigazione sul valore predefinito, sull’ultima cartella visualizzata o su un percorso specifico da individuare e identificare. Potete inoltre impostare il percorso Sfoglia per ordinare file e cartelle in ordine ascendente o discendente.
* **[!UICONTROL Visualizzazione Sfoglia predefinita]** - Determina se la vista griglia o la vista a elenco è quella predefinita visualizzata la prima volta che si apre il pannello Sfoglia.
* **[!UICONTROL Visualizzazione schermata introduttiva]** - Determina se sono presenti schermate introduttive, inclusa la schermata introduttiva.
* **[!UICONTROL Mostra descrizioni]** - Determina se le descrizioni comandi vengono visualizzate quando si sposta il puntatore su pulsanti, menu e collegamenti di spostamento. Le descrizioni descrivono gli elementi dell’interfaccia utente su schermo.
* **[!UICONTROL Sfondo a scacchi]** - Visualizza un livello a scacchiera dietro le immagini, consentendo di vedere facilmente le aree trasparenti di un&#39;immagine con un canale alfa.
* **[!UICONTROL Mostra dimensione file]** : visualizza la dimensione del file di una risorsa durante la navigazione.
* **[!UICONTROL Includi FDU nella ricerca]** : deselezionata (impostazione predefinita) per migliorare le prestazioni del sistema per la maggior parte delle ricerche di metadati eseguite.

  Se invece la maggior parte delle ricerche di metadati richiedono l’inclusione dei campi definiti dall’utente, potete selezionare e attivare questa opzione. In alternativa, invece di includere i campi definiti dall’utente, potete usare la Ricerca avanzata per consentire una ricerca più mirata e rapida.

  Consultate [Eseguire una ricerca avanzata](searching-assets.md#conducting_an_advanced_search).

  Consultate [Campi definiti dall’utente](application-setup.md#user_defined_fields).

* **[!UICONTROL Tipo di ricerca di base]** - È possibile scegliere tra due opzioni: **[!UICONTROL Contiene]** cerca nella stringa completa il valore specificato; **[!UICONTROL Inizia con]** esegue la ricerca dall&#39;inizio della stringa e restituisce i risultati più rapidamente di **[!UICONTROL Contiene]**. Entrambe le opzioni sostituiscono il valore predefinito impostato in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali applicazione]** dall&#39;amministratore.
* **[!UICONTROL Mostra feedback comando]** - Selezionare per attivare la visualizzazione delle richieste di comandi al server; deselezionare per disattivarla.
* **[!UICONTROL Mostra finestra di dialogo durante esportazione]** - Selezionare per visualizzare una finestra di dialogo a comparsa durante un&#39;esportazione. Se deselezioni (disattivi) questa opzione, puoi comunque passare alla pagina Processi per recuperare i risultati dell’esportazione.

## E-mail

* **[!UICONTROL Opzioni e-mail]** : scegli come desideri che Adobe Dynamic Media Classic ti informi tramite e-mail quando i processi di caricamento e pubblicazione sono completati. Potete ricevere notifiche relative al completamento dei processi solo in caso di avvertenze o errori.
* **[!UICONTROL Ambito e-mail]** - Determina se si ricevono tutti i messaggi di posta elettronica per la società o solo quelli relativi ai processi di caricamento e pubblicazione avviati.
* **[!UICONTROL Tipi di e-mail]** - Determina se sei informato quando vengono completati i processi di caricamento e pubblicazione.

## Lingua

* **[!UICONTROL Lingua preferita]** - Determina la lingua che si desidera utilizzare per l&#39;interfaccia.

## Password

* **[!UICONTROL Password corrente]** - Immettere la password attuale.
* **[!UICONTROL Nuova password]** - Immettere una nuova password valida. La password deve soddisfare i seguenti requisiti:
   * Deve contenere tra 8 e 25 caratteri.
   * Contenere almeno una lettera minuscola.
   * Contenere almeno una lettera maiuscola.
   * Contenere almeno un numero.
   * Contengono almeno uno dei seguenti caratteri speciali: `# $ & - _ : { }`
* **[!UICONTROL Ridigitate la password]** - Immettere nuovamente la nuova password per confermare che la si sta immettendo correttamente.
* **[!UICONTROL Scadenza password]** - Determina se la password scade dopo 72 giorni come misura di sicurezza. Se si seleziona Sì, viene richiesto di creare una password dopo 72 giorni.
