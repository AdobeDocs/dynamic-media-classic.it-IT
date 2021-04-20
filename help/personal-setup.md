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
role: Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1197'
ht-degree: 78%

---


# Configurazione personale {#personal-setup}

Le impostazioni della schermata Configurazione personale possono essere modificate da tutti gli utenti. Per aprire la schermata Configurazione personale, scegliete Configurazione > Configurazione personale.

>[!NOTE]
>
>Nella schermata Configurazione personale è indicato il ruolo utente in Dynamic Media Classic: Amministratore, amministratore o utente della società.

Le impostazioni della schermata Configurazione personale controllano il comportamento predefinito del pannello Sfoglia, il modo in cui ricevete i messaggi e-mail e le impostazioni della password. Dopo aver modificato queste impostazioni, fate clic su Salva.

## Informazioni sul mio account

Identifica il vostro nome e nome dell’account, il nome utente (indirizzo e-mail) e il ruolo utente che vi è stato assegnato.

### Versione Desktop

Fare clic su Installa per installare la versione desktop di Dynamic Media Classic sul disco rigido locale. In alternativa, fate clic su Reinstalla per installare di nuovo la versione desktop.

## Per installare il plug-in sul disco rigido locale

1. Nella pagina Configurazione personale di Dynamic Media Classic, in Plug-in Illustrator per Web-to-Print, fai clic su **Scarica ora** per scaricare il file **Plug-in Illustrator per Web-to-Print.zip** .
1. Decomprimete il file ZIP in una cartella temporanea.

   Nel livello principale del file decompresso è presente un file di istruzioni che contiene ulteriori informazioni sul plug-in.

1. In base al sistema operativo installato, effettuate una delle seguenti operazioni:

### Windows

| Programma in esecuzione | Procedura |
|--- |--- |
| Adobe Illustrator 18 in Adobe Creative Cloud 2014 | <ul><li>Dal livello principale della cartella decompressa, fate clic su CC-2014.</li><li>In base alla versione di Adobe Illustrator che state utilizzando, fate clic su win32 o win64.</li><li>Fate clic su libreries > flames, quindi copiate `aflame.dll` nella cartella di esecuzione di Adobe Illustrator, Ad esempio, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Nota**: Questo percorso di esempio è per la posizione a 64 bit; la posizione a 32 bit può invece rientrare in File di programma (x86).  <br/><ul><li>Tornate nella cartella libraries, fate clic su flamingo e copiate `aflamingo.dll` nella stessa cartella di esecuzione di Adobe Illustrator utilizzata in precedenza. </li><li>Tornate infine nella cartella win32 o win64 che avevate selezionato al punto 2 e copiate `AdobeS7FXGFileFormat.aip` nella cartella dei plug-in di Adobe Illustrator, Ad esempio, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Nota**: Questo percorso di esempio è per la posizione a 64 bit; la posizione a 32 bit può invece rientrare in File di programma (x86). |
| Adobe Illustrator 17 in Adobe Creative Cloud | <ul><li>Dal livello principale della cartella decompressa, fate clic su CC. </li><li>In base alla versione di Adobe Illustrator che state utilizzando, fate clic su win32 o win64.</li><li> Copia `AdobeS7FXGFileFormat.aip` nella cartella dei plug-in di Adobe Illustrator. Ad esempio, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Nota**: Questo percorso di esempio è per la posizione a 64 bit; la posizione a 32 bit può invece rientrare in File di programma (x86). |
| Adobe Illustrator 16 in Adobe Creative Suite 6 | <ul><li>Dal livello principale della cartella decompressa, fate clic su 6.0. </li><li>In base alla versione di Adobe Illustrator che state utilizzando, fate clic su win32 o win64. </li><li>Copiate AdobeS7FXGFileFormat.aip nella cartella dei plug-in di Adobe Illustrator, Ad esempio, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Nota**: Questo percorso di esempio è per la posizione a 64 bit; la posizione a 32 bit può invece rientrare in File di programma (x86). |

### Mac

| Programma in esecuzione | Procedura |
|--- |--- |
| Adobe Illustrator 18 in Adobe Creative Cloud 2014 | <ul><li>Dal livello principale della cartella decompressa, fate clic su CC-2014 > mac64.</li><li>Fate clic su libraries > flame, quindi copiate la cartella `aflame.framework` nella cartella di esecuzione di Adobe Illustrator, Ad esempio, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. Per aprire la cartella dei contenuti del pacchetto di Adobe Illustrator, fai clic con il pulsante destro del mouse sull’icona dell’illustratore di Adobe CC 2014 e fai clic su Mostra contenuti del pacchetto dal menu di scelta rapida.</li><li>Tornate nella cartella libraries, fate clic su `flamingo` e copiate la cartella `aflamingo.framework` nella stessa cartella di esecuzione di Adobe Illustrator utilizzata in precedenza.</li><li>Tornate infine nella cartella mac 64 che avevate selezionato al punto 1 e copiate la cartella `AdobeS7FXGFileFormat.aip` nella cartella dei plug-in di Adobe Illustrator, Ad esempio, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 17 in Adobe Creative Cloud | <ul><li>Dal livello principale della cartella decompressa, fate clic su CC > mac64</li><li>Copia la cartella `AdobeS7FXGFileFormat.aip` nella cartella dei plug-in di Adobe Illustrator. Ad esempio, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 16 nella Creative Suite Adobe 6 | <ul><li>Dal livello principale della cartella decompressa, fate clic su 6.0 > mac64</li><li>Copia la cartella `AdobeS7FXGFileFormat.aip` nella cartella dei plug-in di Adobe Illustrator. Ad esempio, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul> |

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
   * Scegli come desideri che Dynamic Media Classic ti informi via e-mail al termine dei processi di caricamento e pubblicazione. Potete ricevere notifiche relative al completamento dei processi solo in caso di avvertenze o errori.
* **Ambito e-mail**
   * Specifica se ricevere un’e-mail per tutti i processi della società o solo per quelli di caricamento e pubblicazione avviati da voi stessi.
* **Tipi di e-mail**
   * Specifica se ricevere notifiche al completamento dei processi di caricamento e di pubblicazione.
* **Lingua**
* **Lingua preferita**
   * Determina la lingua per l’interfaccia.
* **Password**
* **Nuova password**
   * Immettere una nuova password valida. La password deve soddisfare i seguenti requisiti:
      * Può contenere tra 8 e 25 caratteri
      * Contenere almeno una lettera minuscola
      * Contenere almeno una lettera maiuscola
      * Contenere almeno un numero
      * Contenere almeno uno dei seguenti caratteri speciali: #$&amp;-_:{}
* **Ridigitate la password**
   * Reinserite la nuova password per verificare che sia stata digitata correttamente.
* **Scadenza password**
   * Specifica se la password scade dopo 72 giorni come misura di sicurezza. Se selezionate Sì, al termine dei 72 giorni vi verrà richiesto di creare una nuova password.
