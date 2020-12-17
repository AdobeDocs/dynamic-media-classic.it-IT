---
title: Caricamento di una risorsa immagine o vettoriale
seo-title: Caricamento di una risorsa immagine o vettoriale
description: 'null'
seo-description: Scoprite come caricare una risorsa immagine o vettoriale.
uuid: d0e4a754-8a49-4b0f-b202-e9003bdb8f20
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: de21dca9-99fe-4183-b647-debfe112fda4
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 84%

---


# Caricamento di una risorsa immagine o vettoriale{#uploading-an-image-asset-or-a-vector-asset}

Prima di poter caricare una risorsa immagine o vettoriale, richiedete una chiave segreta condivisa. Usate questa chiave segreta condivisa per ottenere un token di caricamento con cui potrete caricare le risorse immagine o vettoriali.

## Richiesta di una chiave segreta condivisa  {#requesting-a-shared-secret-key}

Richiedete una *chiave segreta condivisa* di [utilizzando il Admin Console  per creare un caso di supporto.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Nel caso di supporto, richiedete una chiave segreta condivisa.

Nel messaggio e-mail, fornite il nome della società che desiderate usare per caricare le risorse immagine. Dopo aver ricevuto la chiave da Dynamic Media Classic, salvatela localmente per poterla utilizzare in futuro.

## Ottenimento del token di caricamento {#retrieving-the-upload-token}

L’utilizzo di un *token di caricamento* fa sì che nessuno debba usare la chiave segreta condivisa per caricare le risorse. Garantisce inoltre la legittimità del caricamento e la provenienza da una fonte affidabile.

Il token di caricamento è una stringa alfanumerica disponibile solo per un periodo di tempo limitato. Per ottenere il codice di caricamento usate i seguenti URL sostituendo la chiave segreta condivisa.

* Immagine
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`In questo esempio, la chiave segreta condivisa è  `fece4b21-87ee-47fc-9b99-2e29b78b602`

* Vettoriale
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In questo esempio, la chiave segreta condivisa è  `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

Per impostazione predefinita, il token di caricamento scade cinque minuti (300 secondi) dopo averlo ottenuto. Per richiedere più tempo, includete nell’URL il parametro `expires` e il tempo desiderato, in secondi. Ad esempio, con il seguente URL immagine di esempio si ottiene un token di caricamento che sarà valido per 1800 secondi:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

La risposta corretta per le immagini si presenta come di seguito:

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
|--- |--- |--- |
| op | Obbligatorio | get_uploadtoken |
| shared_secret | Obbligatorio | Chiave segreta condivisa della società che esegue il caricamento. |
| expires | Facoltativo | Validità del token di caricamento, in secondi. Se non viene specificato, viene applicato il valore predefinito di 300 secondi. |

**URL immagine campione:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**Esempio di URL vettoriale:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**Metodi HTTP consentiti:** GET e POST

Ora potete caricare una risorsa immagine.

Consultate [Caricamento di una risorsa immagine](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Caricamento di una risorsa immagine  {#uploading-an-image-asset}

Dopo aver recuperato un token di caricamento valido per un periodo di tempo specificato, potete caricare una risorsa immagine. Potete caricare la risorsa come POST multiparte o modulo e inviare gli altri valori come una stringa di richiesta URL, come nell’esempio di seguito:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

I campi `upload_token` e `company_name` sono obbligatori.

Consultate [Ottenimento del token di caricamento](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consultate [Ottenimento di una chiave segreta condivisa](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Potete anche inviare altri valori facoltativi come stringhe di richiesta URL, come nell’esempio di seguito:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

Il parametro `file_limit` specifica il limite di dimensione del file in byte. Il parametro `file_exts` specifica le estensioni del nome file consentite per il caricamento. Entrambi questi valori sono facoltativi.

Nell’applicazione è possibile impostare un limite globale per la dimensione dei nomi file e le estensioni di file consentite. Se l’elemento inviato nella richiesta è un sottoinsieme dei limiti globali, viene rispettato. I limiti globali sono indicati di seguito:

| Limite globale  | Valore |
|--- |--- |
| Dimensione file per tutti i client | 20 MB |
| Formati file immagine supportati per il caricamento | BMP, GIF, JPG, PNG, PSD |

Il seguente modulo HTML consente a un utente di caricare una risorsa. Il modulo richiede l’inserimento delle informazioni di seguito:

* Nome società.
* Token di caricamento.
* Limite dimensione file.
* Elenco di estensione di nomi file.
* Se mantenere o meno il profilo colore e il nome file associati alla risorsa.
* Se utilizzare o meno il Foratura sfondo. Se abilitate Foratura sfondo, impostate Angolo, Tolleranza e Metodo di riempimento. Consultate Foratura dello sfondo in [Opzioni di modifica delle immagini al momento del caricamento](image-editing-options-upload.md#image-editing-options-at-upload).
* Nome del file da caricare

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

Per visualizzare il codice sorgente HTML associato al modulo sopra, fare clic sul seguente collegamento:

[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

In Firefox, fare clic con il pulsante destro del mouse nella finestra del browser, quindi fare clic su **Visualizza origine pagina**. Nel codice viene mostrata la stringa di richiesta URL corrispondente e il metodo POST che vengono eseguiti quando l’utente fa clic su **Invia**.

Per visualizzare la risposta XML in Internet Explorer, fate clic su **Visualizza > Sorgente**. Per visualizzare la risposta XML in Firefox, fare clic su **Strumenti > Sviluppatore Web > Origine pagina**. Per la visualizzazione delle risposte XML si consiglia Firefox.

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

| Parametro URL | Richiesto o facoltativo | Valore |
|--- |--- |--- |
| op | Obbligatorio | upload |
| upload_token | Obbligatorio | Token di caricamento per la chiave segreta condivisa associata alla società. |
| company_name | Obbligatorio | Nome della società che esegue il caricamento. |
| file_limit | Facoltativo | Limite dimensione file in byte per la risorsa. |
| file_exts | Facoltativo | Elenco di estensioni consentite per il file della risorsa immagine. |
| preserve_colorprofile | Facoltativo | Mantiene eventuale profilo colore incorporato durante la conversione in formato PTIFF del file caricato. I valori consentiti sono true o false. Il valore predefinito è false.. |
| preserve_filename | Facoltativo | Mantiene il nome file della risorsa caricata. I valori consentiti sono true o false. Il valore predefinito è false.. |

>[!NOTE]
>
>dovete inviare la risorsa da caricare come unico campo in una richiesta POST multiparte.

**URL campione:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Metodo HTTP consentito:**

POST

### Ottenimento dei metadati di risorsa per immagini  {#getting-asset-metadata-for-images}

Per ottenere i metadati di una risorsa caricata, potete usare `image_info`, come illustrato nell’esempio di seguito:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Esempio di una risposta riuscita:

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
|--- |--- |--- |
| op | Obbligatorio | image_info |
| shared_secret | Obbligatorio | Chiave segreta condivisa della società. |
| image_name | Obbligatorio | Nome dell’immagine. |

**URL campione:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Metodo HTTP consentito:**

GET e POST

## Caricamento di una risorsa vettoriale  {#uploading-a-vector-asset}

Dopo aver recuperato un token di caricamento valido per un periodo di tempo specificato, potete caricare una risorsa vettoriale. Potete caricare la risorsa come POST multiparte o modulo e inviare gli altri valori come una stringa di richiesta URL, come nell’esempio di seguito:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

I campi `upload_token` e `company_name` sono obbligatori.

Consultate [Ottenimento del token di caricamento](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consultate [Ottenimento di una chiave segreta condivisa](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Potete anche inviare altri valori facoltativi come stringhe di richiesta URL, come nell’esempio di seguito:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

Il parametro `file_limit` specifica il limite di dimensione del file in byte. Il parametro `file_exts` specifica le estensioni del nome file consentite per il caricamento. Entrambi questi valori sono facoltativi.

Nell’applicazione è possibile impostare un limite globale per la dimensione dei nomi file e le estensioni di file consentite. Se l’elemento inviato nella richiesta è un sottoinsieme dei limiti globali, viene rispettato. I limiti globali sono indicati di seguito:

| Limite globale  | Valore |
|--- |--- |
| Dimensione file per tutti i client | 20 MB |
| Formati file vettoriali supportati per il caricamento | AI, EPS, PDF (solo se il file PDF è stato aperto e salvato in Adobe Illustrator CS6) |

Il seguente modulo HTML consente a un utente di caricare una risorsa. Il modulo richiede l’inserimento delle informazioni di seguito:

* Nome società.
* Token di caricamento.
* Limite dimensione file.
* Elenco di estensione di nomi file.
* Se mantenere o meno il profilo colore e il nome file associati alla risorsa.
* Se utilizzare o meno il Foratura sfondo. Se abilitate Foratura sfondo, impostate Angolo, Tolleranza e Metodo di riempimento. Consultate Foratura dello sfondo in [Opzioni di modifica delle immagini al momento del caricamento](image-editing-options-upload.md#image-editing-options-at-upload).
* Nome del file da caricare

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

Il codice HTML di seguito viene visualizzato quando fate clic con il pulsante destro del mouse nella finestra del browser e fate clic su **Visualizza sorgente** per il modulo illustrato nella figura. Nel codice viene mostrata la stringa di richiesta URL corrispondente e il metodo POST che vengono eseguiti quando l’utente fa clic su **Invia**.

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
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

Per visualizzare la risposta XML in Internet Explorer, fate clic su **Visualizza** > **Sorgente**. Per visualizzare la risposta XML in Firefox, fate clic su **Visualizza** > **Sorgente pagina**. Per la visualizzazione delle risposte XML si consiglia Firefox.

Segue un esempio di risposta a seguito di un caricamento riuscito:

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
>la risorsa caricata (AI, EPS, PDF e così via) viene convertita in formato FXG e la risposta invia un collegamento diretto a tale risorsa FXG.

La risorsa è come qualsiasi altra risorsa Web-stampa ed è possibile applicarvi delle query di elaborazione. Ad esempio, l’URL seguente converte una risorsa FXG in immagine PNG da 500x500.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Inviate la risorsa come POST multiparte o modulo mentre inviate gli altri valori come una stringa query URL. Nella stringa query URL potete usare i seguenti campi per caricare una risorsa:

| Parametro URL | Richiesto o facoltativo | Valore |
|--- |--- |--- |
| op | Obbligatorio | upload |
| upload_token | Obbligatorio | Token di caricamento per la chiave segreta condivisa associata alla società. |
| company_name | Obbligatorio | Nome della società che esegue il caricamento. |
| file_limit | Facoltativo | Limite dimensione file in byte per la risorsa. |
| file_exts | Facoltativo | Elenco di estensioni consentite per il file della risorsa. |

>[!NOTE]
>
>dovete inviare la risorsa da caricare come unico campo in una richiesta POST multiparte.

**URL campione:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Metodo HTTP consentito:**

POST
