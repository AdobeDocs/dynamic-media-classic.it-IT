---
title: Configurazione personale
seo-title: Configurazione personale
description: 'null'
seo-description: Tutti gli utenti possono modificare le impostazioni della schermata Configurazione personale di Dynamic Media Classic.
uuid: 29 cb 825 a-f 158-4 a 1 e -9 d 5 f -7636 ee 411 b 6 e
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/setup
discoiquuid: 6314 e 7 b 7-5 bde -4 fe 2-8674-e 4 fc 525 d 4 d 1 c
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Configurazione personale {#personal-setup}

Le impostazioni della schermata Configurazione personale possono essere modificate da tutti gli utenti. Per aprire la schermata Configurazione personale, scegliete Configurazione &gt; Configurazione personale.

>[!NOTE]
>
>la schermata Configurazione personale indica qual è il vostro ruolo utente in Scene7 Publishing System: Amministratore società, Amministratore o Utente.

Le impostazioni della schermata Configurazione personale controllano il comportamento predefinito del pannello Sfoglia, il modo in cui ricevete i messaggi e-mail e le impostazioni della password. Dopo aver modificato queste impostazioni, fate clic su Salva.

## Informazioni sul mio account

Identifica il vostro nome e nome dell’account, il nome utente (indirizzo e-mail) e il ruolo utente che vi è stato assegnato.

### Versione Desktop

Fate clic su Installa per installare la versione desktop di Scene7 Publishing System sul disco rigido locale. In alternativa, fate clic su Reinstalla per installare di nuovo la versione desktop.

### Plug-in di Illustrator per la funzione Web-stampa

Sui computer con Windows 7 o 8, per installare il plug-in di Adobe Illustrator per la funzione Web-stampa è necessario disporre dei privilegi di amministratore e accedere come amministratore in Windows. Dopo l’installazione, il plug-in sarà disponibile in Adobe Illustrator.

Supportano il plug-in le seguenti versioni di Adobe Illustrator:

* Adobe Illustrator 18 in Adobe Creative Cloud 2014.
* Adobe Illustrator 17 in Adobe Creative Cloud.
* Adobe Illustrator 16 in Adobe Creative Suite 6.

Le piattaforme che supportano Adobe Illustrator includono:

* Apple Mac OS X 10.7 o versione successiva.
* Windows® 8, 32 bit e 64 bit.
* Windows® 7, 32 bit e 64 bit.
* Windows XP, 32 bit e 64 bit (solo per Adobe Illustrator 16 in Adobe Creative Suite 6).

Consultate anche [Pubblicazione di modelli](quick-start-template-publishing.md).

## Per installare il plug-in sul disco rigido locale

1. Nella pagina Configurazione personale di Scene7 Publishing System, sotto Plug-in di Illustrator per la funzione Web-stampa, fate clic su **Scarica ora** per scaricare il file **Illustrator Plug-in for Web-to-Print.zip**.
1. Decomprimete il file ZIP in una cartella temporanea.

   Nel livello principale del file decompresso è presente un file di istruzioni che contiene ulteriori informazioni sul plug-in.

1. In base al sistema operativo installato, effettuate una delle seguenti operazioni:

### Windows

| Programma in esecuzione | Procedura |
|--- |--- |
| Adobe Illustrator 18 in Adobe Creative Cloud 2014 | <ul><li>Dal livello principale della cartella decompressa, fate clic su CC-2014.</li><li>In base alla versione di Adobe Illustrator che state utilizzando, fate clic su win32 o win64.</li><li>Fate clic su libreries &gt; flames, quindi copiate `aflame.dll` nella cartella di esecuzione di Adobe Illustrator, Ad esempio, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Nota**: Questo percorso di esempio è per la posizione a 64 bit; la posizione a 32 bit può essere disponibile in Program Files (Programmi) (x 86). <br/><ul><li>Tornate nella cartella libraries, fate clic su flamingo e copiate `aflamingo.dll` nella stessa cartella di esecuzione di Adobe Illustrator utilizzata in precedenza. </li><li>Tornate infine nella cartella win32 o win64 che avevate selezionato al punto 2 e copiate `AdobeS7FXGFileFormat.aip` nella cartella dei plug-in di Adobe Illustrator, Ad esempio, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Nota**: Questo percorso di esempio è per la posizione a 64 bit; la posizione a 32 bit può essere disponibile in Program Files (Programmi) (x 86). |
| Adobe Illustrator 17 in Adobe Creative Cloud | <ul><li>Dal livello principale della cartella decompressa, fate clic su CC. </li><li>In base alla versione di Adobe Illustrator che state utilizzando, fate clic su win32 o win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. Ad esempio, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Nota**: Questo percorso di esempio è per la posizione a 64 bit; la posizione a 32 bit può essere disponibile in Program Files (Programmi) (x 86). |
| Adobe Illustrator 16 in Adobe Creative Suite 6 | <ul><li>Dal livello principale della cartella decompressa, fate clic su 6.0. </li><li>In base alla versione di Adobe Illustrator che state utilizzando, fate clic su win32 o win64. </li><li>Copiate AdobeS7FXGFileFormat.aip nella cartella dei plug-in di Adobe Illustrator, Ad esempio, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Nota**: Questo percorso di esempio è per la posizione a 64 bit; la posizione a 32 bit può essere disponibile in Program Files (Programmi) (x 86). |

### Mac

| Programma in esecuzione | Procedura |
|--- |--- |
| Adobe Illustrator 18 in Adobe Creative Cloud 2014 | <ul><li>Dal livello principale della cartella decompressa, fate clic su CC-2014 &gt; mac64.</li><li>Fate clic su libraries &gt; flame, quindi copiate la cartella `aflame.framework` nella cartella di esecuzione di Adobe Illustrator, Ad esempio, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. Per aprire la cartella del contenuto del pacchetto di Adobe Illustrator, fate clic con il pulsante destro del mouse sull'icona Adobe Illustrator CC 2014 e fate clic su Mostra contenuto pacchetto dal menu contestuale.</li><li>Tornate nella cartella libraries, fate clic su `flamingo` e copiate la cartella `aflamingo.framework` nella stessa cartella di esecuzione di Adobe Illustrator utilizzata in precedenza.</li><li>Tornate infine nella cartella mac 64 che avevate selezionato al punto 1 e copiate la cartella `AdobeS7FXGFileFormat.aip` nella cartella dei plug-in di Adobe Illustrator, Ad esempio, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 17 in Adobe Creative Cloud | <ul><li>Dal livello principale della cartella decompressa, fate clic su CC &gt; mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. Ad esempio, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 16 in Adobe Creative Suite 6 | <ul><li>Dal livello principale della cartella decompressa, fate clic su 6.0 &gt; mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. Ad esempio, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul> |

È ora possibile utilizzare il plug-in in Adobe Illustrator.

### Browser

* **Dimensione miniatura**
   * Specifica le dimensioni predefinite delle miniature delle immagini per la visualizzazione Griglia nel pannello Sfoglia.
* **Visualizzazione predefinita libreria di risorse**
   * Specifica se le risorse della libreria di risorse per la creazione di set devono essere visualizzate come miniature o per nome. Se dovete gestire grandi quantità di risorse nella libreria, è consigliabile visualizzarle per nome. Ad esempio, se state creando un eCatalog di grandi dimensioni contenente numerosi file PDF, potete visualizzare le risorse per nome per ridurre la lunghezza dell’elenco.
* **Ordine di navigazione predefinito**
   * Specifica l’ordine predefinito in cui le risorse vengono visualizzate nel pannello Sfoglia. Scegliete un criterio di ordinamento nel menu e specificate se l’ordine deve essere crescente o decrescente.
* **Percorso predefinito per Sfoglia**
   * Consente di impostare la posizione predefinita per Sfoglia: l’ultima cartella selezionata o un percorso specifico a cui passate e che identificate. Potete inoltre impostare il percorso Sfoglia per ordinare file e cartelle in ordine ascendente o discendente.
* **Visualizzazione browser predefinita**
   * Specifica se la visualizzazione Griglia o Elenco è la visualizzazione predefinita quando il pannello Sfoglia viene aperto per la prima volta.
* **Visualizzazione schermata introduttiva**
   * Specifica se devono essere visualizzate le schermate introduttive, inclusa la schermata di benvenuto.
* **Mostra descrizioni**
   * Specifica se devono essere visualizzate le descrizioni dei comandi quando si passa il puntatore su pulsanti, menu e collegamenti di navigazione. Le descrizioni descrivono gli elementi sullo schermo.
* **Sfondo a scacchi**
   * Visualizza uno sfondo a scacchi dietro le immagini che consente di vedere facilmente le aree trasparenti di un’immagine che contiene un canale alfa.
* **Mostra dimensione file**
   * Visualizza la dimensione file di una risorsa individuata in Sfoglia.
* **Conferma all’uscita da SPS**
   * Presenta una finestra di conferma prima di uscire da Scene7 Publishing System.
* **Includi UDF nella ricerca**
   * Questa opzione è deselezionata (impostazione predefinita) per migliorare le prestazioni del sistema per la maggior parte delle ricerche per metadati.

Se invece la maggior parte delle ricerche di metadati richiedono l’inclusione dei campi definiti dall’utente, potete selezionare e attivare questa opzione. In alternativa, invece di includere i campi definiti dall’utente, potete usare la Ricerca avanzata per consentire una ricerca più mirata e rapida.

Consultate [Eseguire una ricerca avanzata](searching-assets.md#conducting_an_advanced_search).

Consultate [Campi definiti dall’utente](application-setup.md#user_defined_fields).

* **Tipo ricerca di base**
   * Scegliete un tipo di ricerca di base: Contiene oppure Inizia con.
* **Mostra funzioni di Media Portal**
   * Selezionate questa opzione per accedere alle funzioni di Media Portal, ad esempio Carrello.
* **Mostra feedback comando**
   * Mostra le richieste di comandi al server.
* **Mostra finestra di dialogo durante esportazione**
   * Presenta una finestra di dialogo quando si esegue un’esportazione. Se deselezionate questa opzione, potete comunque recuperare i risultati dell’esportazione dalla pagina Processi.

## E-mail

* **Opzioni e-mail**
   * Scegliete come desiderate che Dynamic Media Classic vi informi tramite e-mail quando vengono completati i processi di caricamento e pubblicazione. Potete ricevere notifiche relative al completamento dei processi solo in caso di avvertenze o errori.
* **Ambito e-mail**
   * Specifica se ricevere un’e-mail per tutti i processi della società o solo per quelli di caricamento e pubblicazione avviati da voi stessi.
* **Tipi di e-mail**
   * Specifica se ricevere notifiche al completamento dei processi di caricamento e di pubblicazione.
* **Lingua**
* **Lingua preferita**
   * Determina la lingua per l’interfaccia.
* **Password**
* **Nuova password**
   * Immettete una nuova password valida. La password deve soddisfare i seguenti requisiti:
      * Lunghezza maggiore di 8-25 caratteri
      * Contiene almeno una lettera minuscola
      * Contiene almeno una lettera maiuscola
      * Contiene almeno un numero
      * Contiene almeno uno dei caratteri speciali seguenti: # $ &amp;-_: {}

* **Ridigitate la password**
   * Reinserite la nuova password per verificare che sia stata digitata correttamente.
* **Scadenza password**
   * Specifica se la password scade dopo 72 giorni come misura di sicurezza. Se selezionate Sì, al termine dei 72 giorni vi verrà richiesto di creare una nuova password.
