---
title: desktop Adobe Dynamic Media Classic
description: Ulteriori informazioni sull'applicazione desktop Adobe Dynamic Media Classic ora disponibile.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
source-git-commit: afc347201b13c3b91ec5e1bd3ac5304442772f8d
workflow-type: tm+mt
source-wordcount: '1994'
ht-degree: 0%

---

# Disponibile ora: app desktop Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Gli utenti di Adobe Dynamic Media Classic ora hanno accesso a una nuova esperienza di app desktop che non si basa più sulla tecnologia Adobe Flash nel browser.

Questa nuova app è ora disponibile per Windows® e macOS.

>[!IMPORTANT]
>
>Adobe consiglia di installare la nuova app desktop Adobe Dynamic Media Classic entro il 1° ottobre 2020. In questo modo sarà possibile effettuare una transizione senza intoppi prima che Adobe Flash Player venga dichiarato obsoleto il 31 dicembre 2020. Dopo tale data, non è possibile accedere alla versione del browser dell’interfaccia utente di Adobe Dynamic Media Classic, etichettata come Adobe Dynamic Media Classic nel prodotto.

Domande frequenti sull&#39;accesso a [New Adobe Dynamic Media Classic ora disponibile.](/help/using/new-ui-2020.md)

## Requisiti di sistema per l’app desktop Adobe Dynamic Media Classic {#system-requirements-dmc-app}

L’app desktop Adobe Dynamic Media Classic è compatibile con i seguenti sistemi operativi:

* macOS 10.10 o versione successiva.
* Windows® 7 o versione successiva.

Consulta i requisiti di sistema completi in [Requisiti di sistema per l&#39;app desktop Adobe Dynamic Media Classic](/help/using/system-requirements.md).

La notifica di aggiornamento all&#39;interno dell&#39;applicazione desktop Adobe Dynamic Media Classic non viene generata per *versioni secondarie*. I clienti che traggono vantaggio dalle correzioni in una versione secondaria possono effettuare l’aggiornamento.

## Risolto solo nella versione più recente (20.22.2) di macOS {#release-feb2022}

* macOS Monterey: la pagina di caricamento dei file viene bloccata nei caricamenti successivi. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Correzioni nell’ultima versione (20.22.1) {#release-jan2022}

* Durante la modifica di un&#39;immagine, i pulsanti **[!UICONTROL Salva]** non funzionavano.
* Negli editor set, i pulsanti **[!UICONTROL Chiudi]**, **[!UICONTROL Salva]** e **[!UICONTROL Salva con nome]** sono disabilitati dopo lo scorrimento delle risorse nel pannello **[!UICONTROL Aggiungi Assets]**.
* Il pulsante **[!UICONTROL Riproduci]** nella visualizzazione Dettagli video non ha funzionato.
* Impossibile immettere `d` e `e` nei campi **[!UICONTROL Nome utente]** e **[!UICONTROL Password]** durante l&#39;esecuzione di macOS Monterey.
* Le rimanenti API di analisi sono state spostate alla versione 2.0.

## Correzioni nella versione 20.21.3 {#release-sept2021}

* Miniature non funzionanti per le risorse visualizzate dopo un periodo di inattività sull’app desktop.
* L’app Desktop non risponde, in genere dopo le operazioni Set.
* Modalità di offuscamento e blocco delle richieste abilitata automaticamente in **[!UICONTROL Test Image Server]**.

  Vedere [Servizio di test protetto](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* È stato aggiornato il meccanismo di autenticazione con Adobe Analytics. Rilevante per le nuove integrazioni o se alcune variabili Analytics devono essere aggiornate dall’interno dell’app desktop Dynamic Media Classic.

  Consulta [Accedi ad Adobe Analytics](/help/using/log-analytics.md) per i passaggi aggiornati.

## Correzioni nella versione 20.21.2 di {#minor-release}

* Limite noto in 20.21.1: l&#39;elenco a discesa **[!UICONTROL Server]** nella schermata di accesso era vuoto.
* In **[!UICONTROL Opzioni processo di caricamento]**, il valore predefinito del nome del livello in **[!UICONTROL Opzioni Photoshop]** è ora **[!UICONTROL Photoshop e nome livello]**. I livelli nel file PSD vengono caricati come immagini separate.
   * L&#39;impostazione predefinita precedente di **[!UICONTROL Nome livello]**, ha assegnato alle immagini il nome o il numero del livello nel file PSD. Il numero di livello veniva utilizzato se i nomi dei livelli nel file PSD erano nomi di livello predefiniti di Photoshop.
   * Il nuovo valore predefinito **[!UICONTROL Photoshop e Nome livello]** assegna alle immagini un nome dopo il file PSD seguito dal nome o dal numero del livello. Il numero di livello viene utilizzato se i nomi dei livelli nel file PSD sono nomi di livello predefiniti di Photoshop.
   * Dato che ora le immagini dei livelli in Adobe Dynamic Media Classic hanno nomi univoci, non si verificherà alcun aggiornamento a PSD o ai modelli esistenti (che condividevano i nomi dei livelli nei file PSD originali).
* Miniature di risorse interrotte.

## Correzioni nella versione 20.21.1 di {#latest-fixes-desktop-app}

* Problemi di accesso a causa del timeout che hanno causato il seguente messaggio: *L&#39;utente potrebbe essere assegnato al gruppo o ai gruppi senza autorizzazione. Contatta l&#39;amministratore.*
* I predefiniti del visualizzatore vengono duplicati a ogni tentativo di password errata.
* L&#39;applicazione desktop non risponde a causa di molte risorse nella cartella principale. (Risolto su Windows®; funziona come desiderato su macOS.)

## Correzioni nella versione 20.20.2 di {#previous-version-fixes-desktop-app}

* Nessun limite al numero di file che è possibile caricare tramite l’interfaccia utente dell’app desktop sia per macOS che per Windows®.
* Non è necessario uscire dall’app desktop per passare da un’azienda all’altra.
* CTRL+V per incollare ora funziona su Windows®.
* In futuro, quando verrà rilasciata una nuova versione dell’app desktop, gli utenti riceveranno una notifica all’interno dell’app desktop stessa.

## Scarica e installa l’app desktop Adobe Dynamic Media Classic più recente su macOS o Windows® {#installation-dmc-app}

Vedi anche:

* [Scarica e installa silenziosamente l’app desktop Adobe Dynamic Media Classic più recente su Mac](#install-silent-mac-dmc-app)
* [Scarica e installa silenziosamente la più recente app desktop Adobe Dynamic Media Classic su Windows](#install-silent-windows-dmc-app)

1. Disinstalla le versioni precedenti dell’app desktop Adobe Dynamic Media Classic sul sistema.

1. Scarica il programma di installazione più recente per l’app desktop Adobe Dynamic Media Classic.

   * La versione più recente è disponibile al seguente indirizzo:

      * [macOS (.DMG): download](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE): download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * La versione precedente è disponibile al seguente indirizzo:

      * [macOS (.DMG): download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE): download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Effettua una delle seguenti operazioni in base al programma di installazione scaricato.

   * **macOS** -Nella finestra di dialogo **[!UICONTROL Trascina per installare]**, trascina **[!UICONTROL Adobe Dynamic Media Classic]** e rilascialo su **[!UICONTROL Applicazioni]**.

     ![Trascina l&#39;installazione in macOS](/help/using/assets/dragondrop-install1.png)

   * Nella cartella **[!UICONTROL Applications]**, tocca l&#39;icona Adobe Dynamic Media Classic.
   * Nella finestra di dialogo, tocca **[!UICONTROL Apri]** per aprire l&#39;app desktop Adobe Dynamic Media Classic.

     ![Apri app scaricata](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** - Esegui il file binario del programma di installazione e segui le istruzioni visualizzate per installare l&#39;app desktop.

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso di Adobe Dynamic Media Classic:

   ![Accesso a Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali utilizzate per accedere a Adobe Dynamic Media Classic nel browser.

   Per il **[!UICONTROL Server]** da utilizzare, vedere il mapping seguente per l&#39;ambiente di produzione:

   | Server | URL browser |
   | --- | --- |
   | Produzione NA (Nord America) | https://s7sps1.scene7.com/ |
   | Produzione EMEA (Europa, Medio Oriente e Africa) | https://s7sps3.scene7.com/ |
   | Produzione APAC (Asia-Pacifico) | https://s7sps5.scene7.com/ |

1. Dopo l’accesso, osserva la familiare esperienza di interfaccia utente del browser. Puoi continuare la tua attività giornaliera di Adobe Dynamic Media Classic come di consueto sull’app desktop.

## Scarica e *installa silenziosamente* l&#39;ultima app desktop Adobe Dynamic Media Classic su macOS {#install-silent-mac-dmc-app}

Vedi anche:

* [Scarica e installa l’app desktop Adobe Dynamic Media Classic più recente su Mac o Windows](#installation-dmc-app)
* [Scarica e installa silenziosamente la più recente app desktop Adobe Dynamic Media Classic su Windows](#install-silent-windows-dmc-app)

Per scaricare e *installare silenziosamente* la versione più recente dell&#39;app desktop Adobe Dynamic Media Classic su macOS:

1. Disinstalla le versioni precedenti dell’app desktop Adobe Dynamic Media Classic sul sistema.

1. Scarica il programma di installazione più recente per l’app desktop Adobe Dynamic Media Classic per macOS.

   * [macOS (.DMG): download](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. Montare l&#39;immagine disco scaricata (.DMG) in un punto di montaggio utilizzando il comando seguente:

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. Copiare il file .APP in **[!UICONTROL Applicazioni]** utilizzando il comando seguente:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso di Adobe Dynamic Media Classic:

   ![Accesso a Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali utilizzate per accedere a Adobe Dynamic Media Classic nel browser.

   Per il **[!UICONTROL Server]** da utilizzare, vedere il mapping seguente per l&#39;ambiente di produzione:

   | Server | URL browser |
   | --- | --- |
   | Produzione NA (Nord America) | https://s7sps1.scene7.com/ |
   | Produzione EMEA (Europa, Medio Oriente e Africa) | https://s7sps3.scene7.com/ |
   | Produzione APAC (Asia-Pacifico) | https://s7sps5.scene7.com/ |

## Scarica e *installa in modo invisibile all&#39;utente* la più recente app desktop Adobe Dynamic Media Classic su Windows® {#install-silent-windows-dmc-app}

Il comando utilizzato è per un&#39;installazione invisibile all&#39;utente di base di MSI. Tuttavia, il programma di installazione dell’app desktop Adobe Dynamic Media Classic è un programma di installazione MSI InstallScript creato utilizzando InstallShield. Quando si esegue il programma di installazione in modalità record, qualsiasi interazione dell&#39;utente viene registrata in un file di risposta. Questo file di risposta viene quindi utilizzato per un&#39;installazione invisibile all&#39;utente come descritto in [Installazioni in esecuzione in modalità invisibile all&#39;utente](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

Vedi anche:

* [Scarica e installa l’app desktop Adobe Dynamic Media Classic più recente su Mac o Windows](#installation-dmc-app)

* [Scarica e installa silenziosamente l’app desktop Adobe Dynamic Media Classic più recente su macOS](#install-silent-mac-dmc-app)

Per scaricare e *installare silenziosamente* la versione più recente dell&#39;app desktop Adobe Dynamic Media Classic su Windows®:

1. Disinstalla le versioni precedenti dell’app desktop Adobe Dynamic Media Classic sul sistema.

1. Scarica il programma di installazione più recente per l’app desktop Adobe Dynamic Media Classic.

   * [Windows® (.EXE): download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Eseguire il programma di installazione in modalità record utilizzando il comando seguente:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. Nella finestra del programma di installazione dell&#39;interfaccia utente grafica, seguire la procedura di installazione in modo che le interazioni e gli input, ad esempio il percorso di installazione, vengano registrati nel file `Setup.iss`.

1. Copiare il file `Setup.iss` creato e `adobe-dynamic-media-classic-20.22.1.exe` in un altro computer.

1. Eseguire il comando seguente per un&#39;installazione invisibile all&#39;utente:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   I dettagli sui parametri della riga di comando sono disponibili in [Setup.exe e Update.exe parametri della riga di comando](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso di Adobe Dynamic Media Classic:

   ![Accesso a Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali utilizzate per accedere a Adobe Dynamic Media Classic nel browser.

   Per il **[!UICONTROL Server]** da utilizzare, vedere il mapping seguente per l&#39;ambiente di produzione:

   | Server | URL browser |
   | --- | --- |
   | Produzione NA (Nord America) | https://s7sps1.scene7.com/ |
   | Produzione EMEA (Europa, Medio Oriente e Africa) | https://s7sps3.scene7.com/ |
   | Produzione APAC (Asia-Pacifico) | https://s7sps5.scene7.com/ |

## Video introduttivo sull’utilizzo dell’app desktop Adobe Dynamic Media Classic {#dmc-app-video-walk-through}

Guarda un video di [introduzione sull&#39;utilizzo di Adobe Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) (durata: 2 minuti e 36 secondi).

## Cancellazione della cache delle immagini e delle risorse dal computer tramite l’app desktop {#clear-cache}

1. Nell&#39;app desktop Adobe Dynamic Media Classic, nell&#39;angolo superiore destro, toccare **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**.
1. Nella pagina **[!UICONTROL Installazione personale]**, sotto l&#39;intestazione **[!UICONTROL Desktop]**, eseguire una delle operazioni seguenti:
   * Per rimuovere dal computer tutti i file di immagine memorizzati nella cache di Adobe Dynamic Media, tocca **[!UICONTROL Cancella cache immagini]**, quindi tocca **[!UICONTROL OK]**.
   * Per rimuovere dal computer tutti i file di risorse Adobe Dynamic Media memorizzati nella cache, tocca **[!UICONTROL Cancella cache risorse]**, quindi tocca **[!UICONTROL OK]**.
1. Nell&#39;angolo inferiore destro della pagina, toccare **[!UICONTROL Chiudi]**.

### Cancellazione manuale della cache delle immagini e delle risorse

Oltre a cancellare l’immagine e la cache delle risorse utilizzando l’app desktop, puoi cancellare manualmente la cache direttamente dal file system.

1. In base al sistema operativo in uso, accedi a:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limitazioni note in Adobe Dynamic Media Classic 20.21.1

* L&#39;elenco a discesa **[!UICONTROL Server]** è vuoto dopo l&#39;aggiornamento all&#39;app desktop Adobe Dynamic Media Classic 20.21.1: Scenario: installare e accedere a Adobe Dynamic Media Classic 20.20.1 o 20.20.2, quindi chiudere l&#39;applicazione. Quindi esegui l’aggiornamento a Adobe Dynamic Media Classic 20.21.1. Quando tenti di accedere, l&#39;elenco a discesa **[!UICONTROL Server]** nella finestra di dialogo **[!UICONTROL Accedi al tuo account]** è vuoto. Per risolvere il problema, è necessario [cancellare manualmente la cache](#clear-cache) (vedere i passaggi precedenti).

## Limitazioni note in Adobe Dynamic Media Classic 20.20.1 (risolte in 20.20.2)

**_Valido solo per Windows® - Esiste un limite al numero di file che è possibile caricare tramite l&#39;interfaccia utente dell&#39;app desktop?_**<br>Sì, è possibile caricare un massimo di 150 file alla volta tramite l&#39;interfaccia utente dell&#39;app desktop.

**_Applicabile a Windows® e macOS: come passare da un&#39;azienda all&#39;altra?_**<br>Per passare da un&#39;azienda all&#39;altra, eseguire le operazioni seguenti:

* Nell’app Adobe Dynamic Media Classic, seleziona la nuova società dall’elenco a discesa azienda.
* Quando viene visualizzata la finestra popup, toccare **[!UICONTROL OK]** per uscire e chiudere l&#39;app.

  ![Per utilizzare la nuova società, riavvia l&#39;app](/help/using/assets/dmclassic-new-company1.png)

* Riavvia Adobe Dynamic Media Classic, quindi accedi come di consueto per lavorare con la nuova azienda.

## Suggerimenti

**_Impossibile visualizzare il pannello Media Cart nella pagina di destinazione di Adobe Dynamic Media Classic._**<br>In Adobe Dynamic Media Classic, toccare&#x200B;**[!UICONTROL Configurazione > Configurazione personale &#x200B;]**. Nella sezione Browser, assicurarsi che sia selezionato&#x200B;**[!UICONTROL Mostra funzionalità MediaPortal &#x200B;]**(selezionato). Tocca&#x200B;**[!UICONTROL Salva > Chiudi &#x200B;]**.

**_Lo stato di pubblicazione (indicatore verde) di una risorsa non viene visualizzato correttamente._**<br>Nell&#39;interfaccia utente del browser, era necessario accedere nuovamente all&#39;interfaccia utente per visualizzare lo stato di pubblicazione corretto delle risorse. Nell&#39;app desktop, Adobe ha introdotto un&#39;icona&#x200B;**[!UICONTROL Aggiorna &#x200B;]**&#x200B;nella barra degli strumenti, a destra del pulsante&#x200B;**[!UICONTROL Seleziona nessuno &#x200B;]**. Tocca l&#39;icona&#x200B;**[!UICONTROL Aggiorna &#x200B;]**&#x200B;per visualizzare lo stato più recente di tutte le risorse nella pagina specificata. Non è necessario effettuare un nuovo accesso come nell’interfaccia utente del browser.

![Icona Aggiorna](/help/using/assets/refresh-icon1.png)
*Icona Aggiorna*

**_Nell&#39;app desktop non sono disponibili predefiniti per set di batch._**<br>Tocca&#x200B;**[!UICONTROL Carica > Opzioni processo > Predefiniti set di batch &#x200B;]**. Verificare che il&#x200B;**[!UICONTROL predefinito per set di batch &#x200B;]**&#x200B;sia abilitato. Fai clic su&#x200B;**[!UICONTROL Salva e invia caricamento &#x200B;]**.
