---
title: App desktop Adobe Dynamic Media Classic - Ora disponibile
description: Ulteriori informazioni sull’applicazione desktop Adobe Dynamic Media Classic.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: 43e0c03b535d30ffed13e1e389935e34563baa9e
workflow-type: tm+mt
source-wordcount: '2036'
ht-degree: 1%

---

# Ora disponibile: app desktop Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Gli utenti di Adobe Dynamic Media Classic ora possono accedere a una nuova esperienza di app desktop che non si basa più sulla tecnologia di Flash Adobe nel browser.

Questa nuova app è ora disponibile per Windows® e macOS.

>[!IMPORTANT]
>
>Adobe consiglia di installare la nuova app desktop Adobe Dynamic Media Classic entro il 1° ottobre 2020. In questo modo potrai effettuare una transizione senza problemi prima che il Flash Player Adobe venga dichiarato obsoleto il 31 dicembre 2020. Dopo tale data, non puoi accedere alla versione del browser dell’interfaccia utente di Adobe Dynamic Media Classic, etichettata come Adobe Dynamic Media Classic nel prodotto.

Consulta le Domande frequenti per [È ora disponibile una nuova esperienza di accesso Adobe Dynamic Media Classic.](/help/new-ui-2020.md)

## Requisiti di sistema per l’app desktop Adobe Dynamic Media Classic {#system-requirements-dmc-app}

L’app desktop Adobe Dynamic Media Classic è compatibile con i seguenti sistemi operativi:

* macOS 10.10 o successivo.
* Windows® 7 o versione successiva

Vedi tutti i requisiti di sistema in [Requisiti di sistema per l’app desktop Adobe Dynamic Media Classic](/help/system-requirements.md).

La notifica di aggiornamento all’interno dell’applicazione desktop Adobe Dynamic Media Classic non viene generata per *minore* versioni. I clienti che beneficiano di correzioni in una versione secondaria possono effettuare l’aggiornamento.

## Risolto solo nella versione più recente (20.22.2) di macOS {#release-feb2022}

* macOS Monterey - La pagina di caricamento dei file viene bloccata nei successivi caricamenti. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Correzioni nell’ultima versione (20.22.1) {#release-jan2022}

* Modifica delle immagini **[!UICONTROL Salva]** i pulsanti non funzionavano.
* Negli editor impostati, il **[!UICONTROL Chiudi]**, **[!UICONTROL Salva]** e **[!UICONTROL Salva con nome]** i pulsanti diventano disattivati dopo lo scorrimento delle risorse nel **[!UICONTROL Aggiungere risorse]** pannello.
* **[!UICONTROL Play]** nella visualizzazione Dettagli video non funzionava.
* Impossibile immettere `d` e `e` in **[!UICONTROL Nome utente]** e **[!UICONTROL Password]** campi durante l’esecuzione di macOS Monterey.
* Le API di Analytics rimanenti sono state spostate nella versione 2.0.

## Problemi risolti nella versione 20.21.3 {#release-sept2021}

* Miniature interrotte per le risorse visualizzate dopo un periodo di inattività dell’app desktop.
* L&#39;app desktop smette di rispondere, in genere dopo le operazioni Imposta.
* Richiedi offuscamento e modalità di blocco abilitata automaticamente in **[!UICONTROL Test Image Serving]**.

   Vedi [Test del servizio Secure Testing](/help/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* È stato aggiornato il meccanismo di autenticazione con Adobe Analytics. Pertinente per le nuove integrazioni o se alcune variabili Analytics devono essere aggiornate dall’app desktop Dynamic Media Classic.

   Vedi [Accedere ad Adobe Analytics](/help/log-analytics.md) per i passaggi aggiornati.

## Problemi risolti nella versione 20.21.2 {#minor-release}

* Limitazione nota alla versione 20.21.1: la **[!UICONTROL Server]** L&#39;elenco a discesa nella schermata di accesso era vuoto.
* In **[!UICONTROL Opzioni processo di caricamento]**, valore predefinito di denominazione livello in **[!UICONTROL Opzioni Photoshop]**, è ora **[!UICONTROL Photoshop e nome livello]**. I livelli del file PSD vengono caricati come immagini a sé stanti.
   * Il valore predefinito precedente di **[!UICONTROL Nome livello]**, le immagini vengono denominate in base al nome o al numero di livello nel file PSD. Il numero del livello veniva utilizzato se i nomi dei livelli nel file PSD erano nomi di livello Photoshop predefiniti.
   * Il nuovo valore predefinito di **[!UICONTROL Photoshop e nome livello]**, assegna un nome alle immagini dopo il file PSD seguito dal nome del livello o dal numero del livello. Il numero del livello viene usato se il livello nel file PSD ha un nome predefinito di Photoshop.
   * Poiché le immagini di livello in Adobe Dynamic Media Classic ora hanno nomi univoci, non verrà eseguito alcun aggiornamento a PSD o Modelli esistenti (quali nomi di livello condivisi nei file PSD originali).
* Miniature delle risorse interrotte.

## Problemi risolti nella versione 20.21.1 {#latest-fixes-desktop-app}

* Problemi di accesso a causa di timeout e il seguente messaggio: *Questo utente può essere assegnato al gruppo o ai gruppi senza autorizzazione. Contattare l&#39;amministratore.*
* I predefiniti visualizzatore vengono duplicati a ogni tentativo di password errato.
* Applicazione desktop che non risponde a causa di molte risorse nella cartella principale. (fisso su Windows®; funziona come desiderato su macOS).

## Problemi risolti nella versione 20.20.2 {#previous-version-fixes-desktop-app}

* Nessun limite al numero di file che è possibile caricare tramite l&#39;interfaccia utente dell&#39;app desktop sia per macOS che per Windows®.
* Non è necessario disconnettersi dall’app desktop per passare da un’azienda all’altra.
* Ctrl+V per l&#39;operazione Incolla ora funziona su Windows®.
* In futuro, quando verrà rilasciata una nuova versione dell’app desktop, gli utenti riceveranno una notifica all’interno dell’app desktop stessa.

## Scarica e installa l’app desktop Adobe Dynamic Media Classic più recente su macOS o Windows® {#installation-dmc-app}

Consultate anche:

* [Scarica e installa in modalità automatica l’app desktop Adobe Dynamic Media Classic più recente su Mac](#install-silent-mac-dmc-app)
* [Scarica e installa in modalità automatica l’app desktop Adobe Dynamic Media Classic più recente su Windows®](#install-silent-windows-dmc-app)

1. Disinstalla sul sistema le versioni precedenti dell’app desktop Adobe Dynamic Media Classic.

1. Scarica il più recente programma di installazione per l’app desktop Adobe Dynamic Media Classic.

   * L’ultima versione è disponibile dal sito:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)
   * La versione precedente è disponibile nel seguente sito:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)


<!--         * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Effettua una delle seguenti operazioni in base al programma di installazione scaricato.

   * **macOS** -In **[!UICONTROL Trascinare per installare]** finestra di dialogo, trascinare **[!UICONTROL Adobe Dynamic Media Classic]** e rilasciarlo su **[!UICONTROL Applicazioni]**.

      ![Installazione tramite trascinamento in macOS](/help/assets/dragondrop-install1.png)

   * In **[!UICONTROL Applicazioni]** tocca l’icona Adobe Dynamic Media Classic .
   * Nella finestra di dialogo, tocca **[!UICONTROL Apri]** per aprire l’app desktop Adobe Dynamic Media Classic.

      ![Apri app scaricata](/help/assets/open-dmclassicapp1.png)

   * **Windows** - Esegui il file binario del programma di installazione e segui le istruzioni visualizzate per installare l’app desktop.

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso Adobe Dynamic Media Classic:

   ![Accesso Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali utilizzate per accedere a Adobe Dynamic Media Classic nel browser.

   Per **[!UICONTROL Server]** per utilizzare, consulta la seguente mappatura per l’ambiente di produzione:

   | Server | URL browser |
   | --- | --- |
   | Produzione NA (Nord America) | https://s7sps1.scene7.com/ |
   | Produzione EMEA (Europa, Medio Oriente e Africa) | https://s7sps3.scene7.com/ |
   | Produzione APAC (Asia-Pacifico) | https://s7sps5.scene7.com/ |

1. Dopo l’accesso, noterai l’esperienza dell’interfaccia utente del browser familiare. Puoi continuare la tua attività quotidiana di Adobe Dynamic Media Classic come sempre nell’app desktop.

## Scarica e *silenzioso* installa l’app desktop Adobe Dynamic Media Classic più recente su macOS {#install-silent-mac-dmc-app}

Consultate anche:

* [Scarica e installa l’app desktop Adobe Dynamic Media Classic più recente su Mac o Windows®](#installation-dmc-app)
* [Scarica e installa in modalità automatica l’app desktop Adobe Dynamic Media Classic più recente su Windows®](#install-silent-windows-dmc-app)

Per scaricare e *silenzioso* installa la versione più recente dell’app desktop Adobe Dynamic Media Classic su macOS:

1. Disinstalla sul sistema le versioni precedenti dell’app desktop Adobe Dynamic Media Classic.

1. Scarica il più recente programma di installazione per l’app desktop Adobe Dynamic Media Classic per macOS.

   * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. Montare l&#39;immagine disco scaricata (.DMG) in una posizione di montagna utilizzando il seguente comando:

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. Copia il file .APP in **[!UICONTROL Applicazioni]** utilizzando il comando seguente:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso Adobe Dynamic Media Classic:

   ![Accesso Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali utilizzate per accedere a Adobe Dynamic Media Classic nel browser.

   Per **[!UICONTROL Server]** per utilizzare, consulta la seguente mappatura per l’ambiente di produzione:

   | Server | URL browser |
   | --- | --- |
   | Produzione NA (Nord America) | https://s7sps1.scene7.com/ |
   | Produzione EMEA (Europa, Medio Oriente e Africa) | https://s7sps3.scene7.com/ |
   | Produzione APAC (Asia-Pacifico) | https://s7sps5.scene7.com/ |

## Scarica e *silenzioso* installa l&#39;app desktop Adobe Dynamic Media Classic più recente su Windows® {#install-silent-windows-dmc-app}

Il comando utilizzato è per un&#39;installazione silenziosa MSI di base. Tuttavia, il programma di installazione dell’app desktop Adobe Dynamic Media Classic è un programma di installazione MSI InstallScript creato utilizzando InstallShield. Quando si esegue il programma di installazione in modalità record, qualsiasi interazione dell&#39;utente viene registrata in un file di risposta. Questo file di risposta viene quindi utilizzato per un&#39;installazione silenziosa come descritto in [Esecuzione di installazioni in modalità silenziosa](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

Consultate anche:

* [Scarica e installa l’app desktop Adobe Dynamic Media Classic più recente su Mac o Windows®](#installation-dmc-app)

* [Scarica e installa in modalità automatica l’app desktop Adobe Dynamic Media Classic più recente su macOS](#install-silent-mac-dmc-app)

Per scaricare e *silenzioso* installa la versione più recente dell’app desktop Adobe Dynamic Media Classic su Windows®:

1. Disinstalla sul sistema le versioni precedenti dell’app desktop Adobe Dynamic Media Classic.

1. Scarica il più recente programma di installazione per l’app desktop Adobe Dynamic Media Classic.

   * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Esegui il programma di installazione in modalità record utilizzando il seguente comando:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. Nella finestra del programma di installazione dell&#39;interfaccia grafica, seguire i passaggi per l&#39;installazione in modo che le interazioni/gli ingressi, come la posizione di installazione, vengano registrati in `Setup.iss` file.

1. Copia i dati creati `Setup.iss` file e `adobe-dynamic-media-classic-20.22.1.exe` in un altro computer.

1. Esegui il seguente comando per un&#39;installazione invisibile all&#39;utente:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   I dettagli sui parametri della riga di comando sono disponibili in [Parametri della riga di comando Setup.exe e Update.exe](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso Adobe Dynamic Media Classic:

   ![Accesso Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali utilizzate per accedere a Adobe Dynamic Media Classic nel browser.

   Per **[!UICONTROL Server]** per utilizzare, consulta la seguente mappatura per l’ambiente di produzione:

   | Server | URL browser |
   | --- | --- |
   | Produzione NA (Nord America) | https://s7sps1.scene7.com/ |
   | Produzione EMEA (Europa, Medio Oriente e Africa) | https://s7sps3.scene7.com/ |
   | Produzione APAC (Asia-Pacifico) | https://s7sps5.scene7.com/ |

## Procedura dettagliata sul video con l’app desktop Adobe Dynamic Media Classic {#dmc-app-video-walk-through}

Guarda un [procedura dettagliata sull’utilizzo di Adobe Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (Lunghezza: 2 minuti e 36 secondi).

## Cancellazione della cache delle immagini e delle risorse sul computer tramite l’app desktop {#clear-cache}

1. Nell’app desktop Adobe Dynamic Media Classic, nell’angolo in alto a destra, tocca **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**.
1. Sulla **[!UICONTROL Configurazione personale]** sotto **[!UICONTROL Desktop]** intestazione, effettuare una delle seguenti operazioni:
   * Per rimuovere dal computer tutti i file immagine memorizzati nella cache di Adobe Dynamic Media, tocca **[!UICONTROL Cancella cache immagine]**, quindi tocca **[!UICONTROL OK]**.
   * Per rimuovere dal computer tutti i file di risorse memorizzati nella cache di Adobe Dynamic Media, tocca **[!UICONTROL Cancella cache risorse]**, quindi tocca **[!UICONTROL OK]**.
1. Nell’angolo in basso a destra della pagina, tocca **[!UICONTROL Chiudi]**.

### Cancellazione manuale della cache delle immagini e delle risorse

Oltre a cancellare l’immagine e la cache delle risorse utilizzando l’app desktop, puoi cancellare manualmente la cache direttamente dal file system.

1. In base al sistema operativo in uso, passa a quanto segue:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limitazione nota in Adobe Dynamic Media Classic 20.21.1

* La **[!UICONTROL Server]** l’elenco a discesa è vuoto dopo l’aggiornamento all’app desktop Adobe Dynamic Media Classic 20.21.1 - Scenario: Installa ed accedi a Adobe Dynamic Media Classic 20.20.1 o 20.20.2, quindi chiudi l&#39;applicazione. Quindi esegui l’aggiornamento a Adobe Dynamic Media Classic 20.21.1. Quando tenti di accedere, la **[!UICONTROL Server]** elenco a discesa nella **[!UICONTROL Accedi al tuo account]** la finestra di dialogo è vuota. Per risolvere questo problema, devi [cancellare manualmente la cache](#clear-cache) (vedi i passaggi precedenti).

## Limitazioni note in Adobe Dynamic Media Classic 20.20.1 (risolto in 20.20.2)

**_Applicabile solo a Windows®: esiste un limite al numero di file che possono essere caricati tramite l’interfaccia utente dell’app desktop?_**<br>Sì, è possibile caricare un massimo di 150 file alla volta tramite l’interfaccia utente dell’app desktop.

**_Applicabile a Windows® e macOS - Come si passa da un&#39;azienda all&#39;altra?_**<br>Per passare da un’azienda all’altra, procedi come segue:

* Nell’app Adobe Dynamic Media Classic, seleziona la nuova società dall’elenco a discesa dell’azienda .
* Quando viene visualizzata la finestra a comparsa, tocca **[!UICONTROL OK]** per disconnetterti e chiudere l’app.

   ![Per utilizzare la nuova società, riavvia l’app](/help/assets/dmclassic-new-company1.png)

* Riavvia Adobe Dynamic Media Classic, quindi accedi come di consueto per lavorare con la nuova azienda.

## Suggerimenti

**_Impossibile visualizzare il pannello Carrello multimediale sulla pagina di destinazione di Adobe Dynamic Media Classic._**<br>In Adobe Dynamic Media Classic, tocca**[!UICONTROL Configurazione > Configurazione personale ]**. Nella sezione Browser , assicurati**[!UICONTROL Mostra funzionalità di MediaPortal ]**è selezionato (selezionato). Tocca**[!UICONTROL Salva > Chiudi ]**.

**_Lo stato di pubblicazione (indicatore verde) di una risorsa non viene riportato correttamente._**<br>Nell’interfaccia utente del browser, era necessario un nuovo accesso all’interfaccia utente per visualizzare lo stato di pubblicazione corretto delle risorse. Nell’app desktop, Adobe ha introdotto un’**[!UICONTROL Aggiorna ]**nella barra degli strumenti, a destra**[!UICONTROL Seleziona nessuno ]**pulsante . Tocca**[!UICONTROL Aggiorna ]**per visualizzare lo stato più recente di tutte le risorse sulla pagina specificata. Non è necessario eseguire nuovamente l’accesso come con l’interfaccia utente del browser.

![Icona Aggiorna](/help/assets/refresh-icon1.png)
*Icona Aggiorna*

**_Non vedo predefiniti per set di batch che funzionano nell’app desktop._**<br>Tocca**[!UICONTROL Carica > Opzioni processo > Predefiniti set di batch ]**. Assicurare la**[!UICONTROL Preimpostazione set di batch ]**è abilitato. Fai clic su**[!UICONTROL Salva e invia caricamento ]**.
