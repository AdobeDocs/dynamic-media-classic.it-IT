---
title: Configurazione personale
description: Tutti gli utenti possono modificare le impostazioni nella schermata Configurazione personale di Dynamic Media Classic.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 28%

---

# Configurazione personale {#personal-setup}

Le impostazioni della schermata Configurazione personale possono essere modificate da tutti gli utenti. Per aprire la schermata Configurazione personale, scegliete Configurazione > Configurazione personale.

>[!NOTE]
>
>Nella schermata Configurazione personale è indicato il ruolo utente in Dynamic Media Classic: Amministratore, amministratore o utente della società.

Le impostazioni della schermata Configurazione personale controllano il comportamento predefinito del pannello Sfoglia, il modo in cui ricevete i messaggi e-mail e le impostazioni della password. Dopo aver modificato queste impostazioni, fate clic su Salva.

## Informazioni sul mio account

Identifica il vostro nome e nome dell’account, il nome utente (indirizzo e-mail) e il ruolo utente che vi è stato assegnato.

## Desktop

* **Cancella cache immagine** : rimuove dal computer tutti i file immagine memorizzati nella cache di Adobe Dynamic Media.
* **Cancella cache risorse** : rimuove dal computer tutti i file di risorse della cache Adobe Dynamic Media.

Oltre a cancellare l’immagine e la cache delle risorse utilizzando l’app desktop, puoi cancellare manualmente la cache direttamente dal file system. In base al sistema operativo in uso, passa a quanto segue:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**Per installare Adobe Dynamic Media Creative Suite Extension:**

1. In Dynamic Media Classic, sulla barra degli strumenti, fai clic su **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**, in Estensione Creative Suite, fai clic su **[!UICONTROL Scarica ora]** per scaricare il file `s7csxs.zxp`.
1. Fai clic sui collegamenti **[!UICONTROL Installazione]** e **[!UICONTROL Requisiti di sistema]** per ulteriori informazioni sull&#39;estensione.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li>Click libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, click flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014 > mac64.</li><li>Click libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-click on the Adobe illustrator CC 2014 icon and click Show Package Contents from context menu).</li><li>Return to the same libraries folder, click `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Browser

* **Dimensione miniatura** : determina le dimensioni predefinite delle miniature nella vista Griglia del pannello Sfoglia.
* **Vista libreria risorse predefinita** : determina se le risorse nella libreria delle risorse per i set di build vengono visualizzate come miniature o per nome. Se dovete gestire grandi quantità di risorse nella libreria, è consigliabile visualizzarle per nome. Ad esempio, se state creando un eCatalog di grandi dimensioni contenente numerosi file PDF, potete visualizzare le risorse per nome per ridurre la lunghezza dell’elenco.
* **Ordine di navigazione predefinito** : determina l’ordine in cui le risorse vengono visualizzate per impostazione predefinita nel pannello Sfoglia. Scegliete un criterio di ordinamento nel menu e specificate se l’ordine deve essere crescente o decrescente.
* **Percorso di navigazione predefinito** : consente di impostare il percorso di ricerca sul valore predefinito, sull’ultima cartella selezionata o su un percorso specifico da individuare e identificare. Potete inoltre impostare il percorso Sfoglia per ordinare file e cartelle in ordine ascendente o discendente.
* **Vista di navigazione predefinita** : determina se la vista Griglia o Elenco è la vista predefinita visualizzata alla prima apertura del pannello Sfoglia.
* **Visualizzazione schermata iniziale**  - Determina se visualizzare schermate introduttive, inclusa la schermata iniziale.
* **Mostra descrizioni comandi** : determina se le descrizioni comandi vengono visualizzate quando si posiziona il puntatore su pulsanti, menu e collegamenti di navigazione. Le descrizioni comandi descrivono gli elementi dell’interfaccia utente sullo schermo.
* **Sfondo a scacchiera**  - Visualizza un livello a scacchiera dietro le immagini, consentendo di vedere facilmente le aree trasparenti di un&#39;immagine che ha un canale alfa.
* **Mostra dimensione file** : visualizza le dimensioni del file di una risorsa durante la navigazione.
* **Includi UDF nella ricerca** : per migliorare le prestazioni del sistema per la maggior parte delle ricerche di metadati eseguite, deselezionate (impostazione predefinita).

   Se invece la maggior parte delle ricerche di metadati richiedono l’inclusione dei campi definiti dall’utente, potete selezionare e attivare questa opzione. In alternativa, invece di includere i campi definiti dall’utente, potete usare la Ricerca avanzata per consentire una ricerca più mirata e rapida.

   Consultate [Eseguire una ricerca avanzata](searching-assets.md#conducting_an_advanced_search).

   Consultate [Campi definiti dall’utente](application-setup.md#user_defined_fields).

* **Tipo**  di ricerca di base: è possibile scegliere tra due opzioni:  **** Contiene la stringa completa per il valore specificato;  **** StartsWithin esegue la ricerca dall&#39;inizio della stringa e restituisce i risultati più velocemente di  **[!UICONTROL Contains]**. Ciascuna opzione sostituisce l&#39;impostazione predefinita impostata in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Impostazioni generali applicazione]** dall&#39;amministratore.
* **Show Command Feedback**  - Selezionare questa opzione per attivare la visualizzazione delle richieste di comando sul server; deseleziona per disattivare.
* **Mostra finestra di dialogo durante l’esportazione** : seleziona questa opzione per visualizzare una finestra di dialogo a comparsa durante un’esportazione. Se deselezioni (disattiva) questa opzione, puoi comunque passare alla pagina Processi per recuperare i risultati dell’esportazione.

## E-mail

* **Opzioni e-mail**  - Scegli come desideri che Dynamic Media Classic ti informi via e-mail al termine dei processi di caricamento e pubblicazione. Potete ricevere notifiche relative al completamento dei processi solo in caso di avvertenze o errori.
* **Ambito e-mail** : determina se ricevere tutte le e-mail di processo per la tua azienda o solo e-mail sui processi di caricamento e pubblicazione avviati.
* **Tipi di e-mail**  - Determina se ricevere informazioni al completamento dei processi di caricamento e pubblicazione.

## Lingua

* **Lingua preferita** : determina la lingua che desideri utilizzare per l’interfaccia.

## Password

* **Password corrente**  - Inserisci la password della password attuale.
* **Nuova password**  - Immettere una nuova password valida. La password deve soddisfare i seguenti requisiti:
   * La lunghezza deve essere compresa tra 8 e 25 caratteri.
   * Contenere almeno una lettera minuscola.
   * Contenere almeno una lettera maiuscola.
   * Contenere almeno un numero.
   * Contenere almeno uno dei seguenti caratteri speciali: `# $ & - _ : { }`
* **Nuovo tipo di password** : inserisci nuovamente la nuova password per confermare che la stai inserendo correttamente.
* **Scadenza password** : determina se la password scade dopo 72 giorni come misura di sicurezza. Se scegliete Sì, trascorsi i 72 giorni verrà chiesto di creare una nuova password.
