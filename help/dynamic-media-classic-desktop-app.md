---
title: Adobe App desktop Dynamic Media Classic - Ora disponibile
description: Ulteriori informazioni sull’applicazione desktop Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 1%

---

# Ora disponibile: Adobe app desktop Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Gli utenti di Dynamic Media Classic ora possono accedere a una nuova esperienza di app desktop che non si basa più sulla tecnologia di Flash Adobe nel browser.

Questa nuova app è ora disponibile per Windows® e macOS.

>[!IMPORTANT]
>
>Adobe consiglia di installare la nuova app desktop Adobe Dynamic Media Classic entro il 1° ottobre 2020. In questo modo potrai effettuare una transizione senza problemi prima che il Flash Player Adobe venga dichiarato obsoleto il 31 dicembre 2020. Dopo tale data, non puoi accedere alla versione del browser dell’interfaccia utente Adobe Dynamic Media Classic, etichettata come Dynamic Media Classic nel prodotto.

Consulta le Domande frequenti per la [Nuova esperienza di accesso di Dynamic Media Classic ora disponibile.](/help/new-ui-2020.md)

## Requisiti di sistema per l’app desktop Dynamic Media Classic {#system-requirements-dmc-app} di Adobe

L’app desktop Adobe Dynamic Media Classic è compatibile con i seguenti sistemi operativi:

* macOS 10.10 o successivo.
* Windows® 7 o versione successiva

>[!NOTE]
>
>La notifica di aggiornamento all’interno dell’applicazione desktop Dynamic Media Classic non viene generata per le versioni *secondarie*. I clienti che beneficiano di correzioni in una versione secondaria possono effettuare l’aggiornamento.

## Correzioni nella versione minore (20.21.2) {#minor-release}

* Limitazione nota nel menu a discesa 20.21.1 del server vuota.
* In **[!UICONTROL Opzioni processo di caricamento]**, il valore predefinito per la denominazione dei livelli in **[!UICONTROL Opzioni Photoshop]** è ora **[!UICONTROL Photoshop e Nome livello]**. I livelli del file PSD vengono caricati come immagini a sé stanti.
   * Il valore predefinito precedente di **[!UICONTROL Nome livello]**, denominato le immagini dopo il nome o il numero di livello nel file PSD. Il numero del livello è stato utilizzato se i nomi dei livelli nel file PSD erano nomi di livello Photoshop predefiniti.
   * Il nuovo valore predefinito di **[!UICONTROL Photoshop e Nome livello]** assegna un nome alle immagini dopo il file PSD seguito dal nome del livello o dal numero del livello. Il numero del livello viene usato se il livello nel file PSD ha un nome predefinito di Photoshop.
   * Dato che le immagini di livello in Dynamic Media Classic ora hanno nomi univoci, non verrà effettuato alcun aggiornamento a PSD o Modelli esistenti (quali nomi di livello condivisi nei file PSD originali).
* Miniature delle risorse interrotte.

## Correzioni nell&#39;ultima versione (20.21.1) {#latest-fixes-desktop-app}

* Problemi di accesso a causa di timeout e il seguente messaggio: *Questo utente può essere assegnato al gruppo o ai gruppi senza autorizzazione. Contatta l&#39;amministratore.*
* I predefiniti visualizzatore vengono duplicati a ogni tentativo di password errato.
* Applicazione desktop che non risponde a causa di molte risorse nella cartella principale. (fisso su Windows®; funziona come desiderato su macOS).

## Correzioni nella versione precedente (20.20.2) {#previous-version-fixes-desktop-app}

* Nessuna limitazione sul numero di file che è possibile caricare tramite l&#39;interfaccia utente dell&#39;app desktop sia per macOS che per Windows®.
* Non è necessario disconnettersi dall’app desktop per passare da un’azienda all’altra.
* Ctrl+V per l&#39;operazione Incolla ora funziona su Windows®.
* In futuro, quando verrà rilasciata una nuova versione dell’app desktop, gli utenti riceveranno una notifica all’interno dell’app desktop stessa.

## Scarica e installa l’app desktop Adobe Classic più recente su macOS o Windows® {#installation-dmc-app}

Consultate anche:

* [Scarica e installa in silenzio l&#39;ultima app desktop Adobe Dynamic Media Classic su Mac](#install-silent-mac-dmc-app)
* [Scarica e installa in modalità automatica l’app desktop Adobe Classic più recente su Windows®](#install-silent-windows-dmc-app)

1. Disinstalla sul sistema le versioni precedenti dell’app desktop Dynamic Media Classic.

1. Scarica l’ultimo programma di installazione per l’app desktop Dynamic Media Classic ad Adobe.

   * L’ultima versione (20.21.2) è disponibile dal seguente indirizzo:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
      * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)
   * La versione precedente (20.21.1) è disponibile nel seguente sito:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
      * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)


<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Effettua una delle seguenti operazioni in base al programma di installazione scaricato.

   * **Per macOS**  - Nella finestra di dialogo  **[!UICONTROL Trascina e rilascia per]** l&#39;installazione, trascina  **[!UICONTROL Adobe Dynamic Media]** Classic e rilascialo su  **[!UICONTROL Applicazioni]**.

      ![Trascinare l’installazione su macOS](/help/assets/dragondrop-install1.png)

   * Nella cartella **[!UICONTROL Applicazioni]** , tocca l’icona Adobe Dynamic Media Classic .
   * Nella finestra di dialogo, tocca **[!UICONTROL Apri]** per aprire l’app desktop Adobe Dynamic Media Classic.

      ![Apri app scaricata](/help/assets/open-dmclassicapp1.png)

   * **Per Windows**  - Esegui il binario di installazione e segui le istruzioni sullo schermo per installare l&#39;app desktop.

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso Adobe Dynamic Media Classic:

   ![Accesso a Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali che hai usato per accedere a Dynamic Media Classic nel browser.

   Per il **[!UICONTROL Server]** da utilizzare, vedi la seguente mappatura per l&#39;ambiente di produzione:

   | URL browser | Nome server app desktop |
   |---|---|
   | https://s7sps1.scene7.com/ | Produzione NA (Nord America) |
   | https://s7sps3.scene7.com/ | Produzione EMEA (Europa, Medio Oriente e Africa) |
   | https://s7sps5.scene7.com/ | Produzione APAC (Asia-Pacifico) |

1. Dopo l’accesso, noterai l’esperienza dell’interfaccia utente del browser familiare. Puoi continuare la tua attività quotidiana di Dynamic Media Classic come sempre nell’app desktop.

## Scarica e *silenzioso* installa l&#39;ultima app desktop Adobe Dynamic Media Classic su macOS {#install-silent-mac-dmc-app}

Consultate anche:

* [Scarica e installa l’app desktop Adobe Classic più recente su Mac o Windows®](#installation-dmc-app)
* [Scarica e installa in modalità automatica l’app desktop Adobe Classic più recente su Windows®](#install-silent-windows-dmc-app)

Per scaricare e *silenzioso* installare l&#39;ultima versione dell&#39;app desktop Adobe Dynamic Media Classic su macOS:

1. Disinstalla sul sistema le versioni precedenti dell’app desktop Dynamic Media Classic.

1. Scarica l’ultimo programma di installazione per l’app desktop Adobe Dynamic Media Classic per macOS.

   * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)

1. Montare l&#39;immagine disco scaricata (.DMG) in una posizione di montagna utilizzando il seguente comando:

   `hdiutil attach adobe-dynamic-media-classic-20.21.2.dmg -mountpoint <mount_point_path>`

1. Copia il file .APP in **[!UICONTROL Applicazioni]** utilizzando il seguente comando:

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso Adobe Dynamic Media Classic:

   ![Accesso a Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali che hai usato per accedere a Dynamic Media Classic nel browser.

   Per il **[!UICONTROL Server]** da utilizzare, vedi la seguente mappatura per l&#39;ambiente di produzione:

   | URL browser | Nome server app desktop |
   |---|---|
   | https://s7sps1.scene7.com/ | Produzione NA (Nord America) |
   | https://s7sps3.scene7.com/ | Produzione EMEA (Europa, Medio Oriente e Africa) |
   | https://s7sps5.scene7.com/ | Produzione APAC (Asia-Pacifico) |

## Scarica e *silenzioso* installa l&#39;app desktop Dynamic Media Classic più recente su Windows® {#install-silent-windows-dmc-app}

Il comando utilizzato è per un&#39;installazione silenziosa MSI di base. Tuttavia, il programma di installazione dell’app desktop Dynamic Media Classic è un programma di installazione MSI InstallScript creato utilizzando InstallShield. Quando si esegue il programma di installazione in modalità record, qualsiasi interazione dell&#39;utente viene registrata in un file di risposta. Questo file di risposta viene quindi utilizzato per un&#39;installazione silenziosa come descritto in [Esecuzione di installazioni in modalità silenziosa.](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Consultate anche:

* [Scarica e installa l’app desktop Adobe Classic più recente su Mac o Windows®](#installation-dmc-app)
* [Scarica e installa in silenzio l’ultima app desktop Adobe Dynamic Media Classic su macOS](#install-silent-mac-dmc-app)

Per scaricare e *silenzioso* installare l&#39;ultima versione dell&#39;app desktop Adobe Dynamic Media Classic su Windows®:

1. Disinstalla sul sistema le versioni precedenti dell’app desktop Dynamic Media Classic.

1. Scarica l’ultimo programma di installazione per l’app desktop Dynamic Media Classic ad Adobe.

   * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

1. Esegui il programma di installazione in modalità record utilizzando il seguente comando:

   `adobe-dynamic-media-classic-20.21.2.exe /r /f1"C:\Setup.iss"`

1. Nella finestra del programma di installazione dell&#39;interfaccia grafica, seguire i passaggi per l&#39;installazione in modo che le interazioni/gli ingressi, come il percorso di installazione, vengano registrati nel file `Setup.iss`.

1. Copia il file `Setup.iss` creato e `adobe-dynamic-media-classic-20.21.2.exe` in un altro computer.

1. Esegui il seguente comando per un&#39;installazione invisibile all&#39;utente:

   `adobe-dynamic-media-classic-20.21.2.exe /s /f1"C:\Setup.iss"`

   I dettagli sui parametri della riga di comando sono disponibili in [Setup.exe e Update.exe Parametri della riga di comando.](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso Adobe Dynamic Media Classic:

   ![Accesso a Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali che hai usato per accedere a Dynamic Media Classic nel browser.

   Per il **[!UICONTROL Server]** da utilizzare, vedi la seguente mappatura per l&#39;ambiente di produzione:

   | URL browser | Nome server app desktop |
   |---|---|
   | https://s7sps1.scene7.com/ | Produzione NA (Nord America) |
   | https://s7sps3.scene7.com/ | Produzione EMEA (Europa, Medio Oriente e Africa) |
   | https://s7sps5.scene7.com/ | Produzione APAC (Asia-Pacifico) |


## Procedura dettagliata sull’utilizzo dell’app desktop Dynamic Media Classic {#dmc-app-video-walk-through}

Guarda un video introduttivo su come utilizzare Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (Lunghezza: 2 minuti e 36 secondi).[

## Cancellazione della cache delle immagini e delle risorse sul computer utilizzando l’app desktop {#clear-cache}

1. Nell’app desktop Dynamic Media Classic, nell’angolo in alto a destra, tocca **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**.
1. Nella pagina **[!UICONTROL Configurazione personale]**, sotto l&#39;intestazione **[!UICONTROL Desktop]**, effettuare una delle seguenti operazioni:
   * Per rimuovere dal computer tutti i file immagine memorizzati nella cache di Adobe Dynamic Media, tocca **[!UICONTROL Cancella cache immagine]**, quindi tocca **[!UICONTROL OK]**.
   * Per rimuovere dal computer tutti i file di risorse memorizzati nella cache di Adobe Dynamic Media, tocca **[!UICONTROL Cancella cache risorse]**, quindi tocca **[!UICONTROL OK]**.
1. Nell’angolo in basso a destra della pagina, tocca **[!UICONTROL Chiudi]**.

### Cancellazione manuale della cache delle immagini e delle risorse

Oltre a cancellare l’immagine e la cache delle risorse utilizzando l’app desktop, puoi cancellare manualmente la cache direttamente dal file system.

1. In base al sistema operativo in uso, passa a quanto segue:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limitazione nota in Dynamic Media Classic 20.21.1

* L&#39;elenco a discesa **[!UICONTROL Server]** è vuoto dopo l&#39;aggiornamento all&#39;app desktop Dynamic Media Classic 20.21.1 - Scenario: Installa ed accedi a Dynamic Media Classic 20.20.1 o 20.20.2, quindi chiudi l&#39;applicazione. Quindi esegui l&#39;aggiornamento a Dynamic Media Classic 20.21.1. Quando tenti di accedere, l&#39;elenco a discesa **[!UICONTROL Server]** nella finestra di dialogo **[!UICONTROL Accedi al tuo account]** è vuoto. Per risolvere questo problema, è necessario [cancellare manualmente la cache](#clear-cache) (vedi i passaggi sopra).

## Limitazioni note in Dynamic Media Classic 20.20.1 (risolto in 20.20.2)

**_Applicabile solo a Windows®: esiste un limite al numero di file che possono essere caricati tramite l’interfaccia utente dell’app desktop?_**<br>Sì, è possibile caricare un massimo di 150 file alla volta tramite l’interfaccia utente dell’app desktop.

**_Si applica a Windows® e macOS - Come si passa da un&#39;azienda all&#39;altra?_**<br>Per passare da un’azienda all’altra, procedi come segue:

* Nell’app Dynamic Media Classic, seleziona la nuova società dall’elenco a discesa dell’azienda .
* Quando viene visualizzata la finestra a comparsa, tocca **[!UICONTROL OK]** per disconnetterti e chiudere l’app.

   ![Per utilizzare la nuova società, riavvia l’app](/help/assets/dmclassic-new-company1.png)

* Riavvia Dynamic Media Classic, quindi accedi come di consueto per lavorare con la nuova azienda.

## Suggerimenti

**_Impossibile visualizzare il pannello Carrello multimediale nella pagina di destinazione di Dynamic Media Classic._**<br>In Dynamic Media Classic, tocca**[!UICONTROL Configurazione > Configurazione personale ]**. Nella sezione Browser , accertati che sia selezionato**[!UICONTROL Mostra funzionalità MediaPortal ]**. Tocca**[!UICONTROL Salva > Chiudi ]**.

**_Lo stato di pubblicazione (indicatore verde) di una risorsa non viene riportato correttamente._**<br>Nell’interfaccia utente del browser, era necessario un nuovo accesso all’interfaccia utente per visualizzare lo stato di pubblicazione corretto delle risorse. Nell’app desktop, in Adobe è stata introdotta un’icona**[!UICONTROL Aggiorna ]**nella barra degli strumenti, a destra del pulsante**[!UICONTROL Seleziona Nessuno ]**. Tocca l’icona**[!UICONTROL Aggiorna ]**per visualizzare lo stato più recente di tutte le risorse sulla pagina specificata. Non è necessario eseguire nuovamente l’accesso come con l’interfaccia utente del browser.

![Icona ](/help/assets/refresh-icon1.png)
*AggiornaIcona Aggiorna*

**_Non vedo predefiniti per set di batch che funzionano nell’app desktop._**<br>Tocca**[!UICONTROL Carica > Opzioni processo > Predefiniti set di batch ]**. Assicurati che il**[!UICONTROL Batch Set Preset ]**pertinente sia abilitato. Fai clic su**[!UICONTROL Salva e invia caricamento ]**.
