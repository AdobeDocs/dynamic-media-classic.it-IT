---
title: Carica una risorsa immagine raster
description: Scopri come caricare un’immagine raster in Adobe Dynamic Media Classic
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 67%

---

# Carica una risorsa immagine raster {#uploading-an-image-asset-or-a-vector-asset}

Prima di poter caricare una risorsa immagine o vettoriale, richiedete una chiave segreta condivisa. Usate questa chiave segreta condivisa per ottenere un token di caricamento Quindi utilizzi il token di caricamento per caricare le risorse di immagini raster.

>[!IMPORTANT]
>
>A partire dal 1° maggio 2023, le risorse UGC in Dynamic Media saranno disponibili per l’uso fino a 60 giorni dalla data di caricamento. Dopo 60 giorni, le risorse verranno rimosse.

>[!NOTE]
>
>Il supporto per risorse vettoriali UGC nuove o esistenti in Adobe Dynamic Media Classic è terminato il 30 settembre 2021.

## Richiedi una chiave con segreto condiviso {#requesting-a-shared-secret-key}

Richiedi *chiave shared-secret* da [utilizzo dell’Admin Console per creare un caso di supporto.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) Nel tuo caso di supporto, richiedi una chiave con segreto condiviso.

Nel messaggio e-mail, fornite il nome della società che desiderate usare per caricare le risorse immagine. Dopo aver ricevuto la chiave da Adobe Dynamic Media Classic, salvarla localmente per utilizzarla in futuro.

## Recuperare il token di caricamento {#retrieving-the-upload-token}

L’utilizzo di un *token di caricamento* fa sì che nessuno debba usare la chiave segreta condivisa per caricare le risorse. Garantisce inoltre la legittimità del caricamento e la provenienza da una fonte affidabile.

Il token di caricamento è una stringa alfanumerica disponibile solo per un periodo di tempo limitato. Utilizza i seguenti URL, sostituendo la chiave con segreto condiviso, in modo da poter recuperare il token di caricamento.

* Immagine raster
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`In questo esempio, la chiave shared-secret è `fece4b21-87ee-47fc-9b99-2e29b78b602`

<!-- * Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9` -->

Per impostazione predefinita, il token di caricamento scade cinque minuti (300 secondi) dopo averlo ottenuto. Per richiedere più tempo, includete nell’URL il parametro `expires` e il tempo desiderato, in secondi. Ad esempio, con il seguente URL immagine di esempio si ottiene un token di caricamento che sarà valido per 1800 secondi:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

La risposta corretta per le immagini è simile alla seguente:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Salvate localmente il token di caricamento per poterlo usare per richieste future.

Per ottenere un token di caricamento, potete usare i seguenti campi nella stringa URL di richiesta:

| Parametro URL | Richiesto o facoltativo | Valore |
| --- | --- | --- |
| op | Obbligatorio | get_uploadtoken |
| shared_secret | Obbligatorio | Chiave segreta condivisa della società che esegue il caricamento. |
| expires | Facoltativo | Validità del token di caricamento, in secondi. Se non viene specificato, viene applicato il valore predefinito di 300 secondi. |

**URL immagine raster di esempio:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000` -->

**Metodi HTTP consentiti:**
`GET` e `POST`

Ora potete caricare una risorsa immagine.

Consulta [Caricare una risorsa immagine](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Carica una risorsa immagine raster {#uploading-an-image-asset}

Dopo aver recuperato un token di caricamento valido per un periodo di tempo specificato, potete caricare una risorsa immagine. Potete caricare la risorsa come POST multiparte o modulo e inviare gli altri valori come una stringa di richiesta URL, come nell’esempio di seguito:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

Il `upload_token` e `company_name` sono obbligatori.

Consulta [Recuperare il token di caricamento](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consulta [Recuperare una chiave con segreto condiviso](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Potete anche inviare altri valori facoltativi come stringhe di richiesta URL, come nell’esempio di seguito:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

Il `file_limit` parametro specifica il limite di dimensione file in byte. Il parametro `file_exts` specifica le estensioni del nome file consentite per il caricamento. Entrambi questi valori sono facoltativi.

Nell’applicazione è possibile impostare un limite globale per la dimensione dei nomi file e le estensioni di file consentite. Se l’elemento inviato nella richiesta è un sottoinsieme dei limiti globali, viene rispettato. I limiti globali sono indicati di seguito:

| Limite globale  | Valore |
| --- | --- |
| Dimensione file per tutti i client | 20 MB |
| Formati file immagine supportati per il caricamento | BMP, GIF, JPG, PNG, PSD, TIFF |

Il seguente modulo HTML consente a un utente di caricare una risorsa. Il modulo richiede l’inserimento delle informazioni di seguito:

* Nome società.
* Token di caricamento.
* Limite dimensione file.
* Elenco di estensione di nomi file.
* Specifica se mantenere il profilo colore e il nome file associati alla risorsa.
* Se utilizzare Knockout Background. Se attivate Sfondo foratura (Knockout Background), impostate i metodi Angolo (Corner), Tolleranza (Tolerance) e Riempimento (Fill).
Consulta Foratura sfondo in [Opzioni di ottimizzazione immagine al caricamento](image-editing-options-upload.md#image-editing-options-at-upload).
* Nome del file da caricare.

Puoi visualizzare il codice sorgente HTML associato al modulo precedente selezionando [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

In Firefox, fai clic con il pulsante destro del mouse nella finestra del browser, quindi seleziona **[!UICONTROL Visualizza origine pagina]**. Nel codice viene mostrata la stringa di richiesta URL corrispondente e il metodo POST che vengono eseguiti quando l’utente fa clic su **[!UICONTROL Invia]**.

Per visualizzare la risposta XML in Internet Explorer, vai a **[!UICONTROL Visualizza]** > **[!UICONTROL Sorgente]**. Per visualizzare la risposta XML in Firefox, vai a **[!UICONTROL Strumenti]** > **[!UICONTROL Strumenti browser]** > **[!UICONTROL Strumenti per sviluppatori Web]**. Per la visualizzazione delle risposte XML si consiglia Firefox.

Segue un esempio di risposta a seguito di un caricamento riuscito:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>la risorsa caricata (JPG, GIF è così via) viene convertita in formato PTIFF e la risposta invia un collegamento diretto a tale risorsa PTIFF.

La risorsa è come qualsiasi altra risorsa Image Server ed è possibile applicarvi delle query di elaborazione. Ad esempio, con l’URL seguente viene richiesto di ingrandire la risorsa in base alla larghezza e all’altezza specificate.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Inviate la risorsa come POST multiparte o modulo mentre inviate gli altri valori come una stringa query URL. Nella stringa query URL potete usare i seguenti campi per caricare una risorsa:

| Parametro URL | Obbligatorio o facoltativo | Valore |
| --- | --- | --- |
| `op` | Obbligatorio | upload |
| `upload_token` | Obbligatorio | Token di caricamento per la chiave segreta condivisa associata alla società. |
| `company_name` | Obbligatorio | Nome della società che esegue il caricamento. |
| `file_limit` | Facoltativo | Limite dimensione file in byte per la risorsa. |
| `file_exts` | Facoltativo | Elenco di estensioni consentite per il file della risorsa immagine. |
| `preserve_colorprofile` | Facoltativo | Mantiene eventuale profilo colore incorporato durante la conversione in formato PTIFF del file caricato. I valori consentiti sono true o false. Il valore predefinito è false.. |
| `preserve_filename` | Facoltativo | Mantiene il nome file della risorsa caricata. I valori consentiti sono true o false. Il valore predefinito è false.. |

>[!NOTE]
>
>dovete inviare la risorsa da caricare come unico campo in una richiesta POST multiparte.

**URL campione:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Metodo HTTP consentito:**

POST

### Ottieni metadati risorsa per immagini {#getting-asset-metadata-for-images}

Per ottenere i metadati di una risorsa caricata, potete usare `image_info`, come illustrato nell’esempio di seguito:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Un esempio di risposta corretta è simile al seguente:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Nella stringa query URL potete usare i seguenti campi per richiedere informazioni su una risorsa:

| Parametro URL | Richiesto o facoltativo | Valore |
| --- | --- | --- |
| `op` | Obbligatorio | image_info |
| `shared_secret` | Obbligatorio | Chiave segreta condivisa della società. |
| `image_name` | Obbligatorio | Nome dell’immagine. |

**URL campione:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Metodo HTTP consentito:**

GET e POST

<!-- ## Upload a vector asset {#uploading-a-vector-asset}

>[!IMPORTANT]
>
>Support for new or existing UGC vector image assets in Adobe Dynamic Media Classic end on September 30, 2021.

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieve the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieve a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

| Global limit | Value |
| --- | --- |
| File size for all clients | 20 MB |
| Supported vector file formats for upload | AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6) |

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether to preserve the color profile and file name associated with the asset.
* Whether to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method.
See Knockout Background in [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload.

The following HTML code is displayed when you right-click in the browser window, and then select **[!UICONTROL View Source]** for the form shown in the example. The code shows the corresponding URL query string and the POST method that are run when the user selects **[!UICONTROL Submit]**.

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Select Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, go to **[!UICONTROL View]** > **[!UICONTROL Source]**. To view XML response in Firefox, go to **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

| URL Parameter | Required or Optional | Value |
| --- | --- | --- |
| `op` | Required | upload |
| `upload_token` | Required | Upload token for the shared-secret key associated with the company. |
| `company_name` | Required | Name of the company performing the upload. |
| `file_limit` | Optional | File size limit, in bytes, for the asset. |
| `file_exts` | Optional | List of allowable extensions for the asset file. |

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
 -->