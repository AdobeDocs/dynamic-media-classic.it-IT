---
title: App desktop Adobe Dynamic Media Classic - Ora disponibile
description: Ulteriori informazioni sull'applicazione desktop Adobe Dynamic Media Classic.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: 358284e6c9888e5188bec35eb7b5408563a71bad
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Ora disponibile: app desktop Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Gli utenti di Adobe Dynamic Media Classic ora hanno accesso a una nuova esperienza di app desktop che non si basa più sulla tecnologia del Flash Adobe nel browser.

Questa nuova app è ora disponibile per Windows® e macOS.

>[!IMPORTANT]
>
>L’Adobe consiglia di installare la nuova app desktop Adobe Dynamic Media Classic entro il 1° ottobre 2020. Procedendo in questo modo potrai ottenere una transizione fluida prima che il Flash Player Adobe venga dichiarato obsoleto il 31 dicembre 2020. Dopo tale data, non è possibile accedere alla versione del browser dell’interfaccia utente di Adobe Dynamic Media Classic, etichettata come Adobe Dynamic Media Classic nel prodotto.

Consulta le Domande frequenti per [È disponibile una nuova esperienza di accesso a Adobe Dynamic Media Classic.](/help/new-ui-2020.md)

## Requisiti di sistema per l’app desktop Adobe Dynamic Media Classic {#system-requirements-dmc-app}

L’app desktop Adobe Dynamic Media Classic è compatibile con i seguenti sistemi operativi:

* macOS 10.10 o versione successiva.
* Windows® 7 o versione successiva.

Consulta i requisiti di sistema completi all&#39;indirizzo [Requisiti di sistema per l’app desktop Adobe Dynamic Media Classic](/help/system-requirements.md).

La notifica di aggiornamento all&#39;interno dell&#39;applicazione desktop Adobe Dynamic Media Classic non viene generata per *non grave* versioni. I clienti che traggono vantaggio dalle correzioni in una versione secondaria possono effettuare l’aggiornamento.

## Risolto solo nella versione più recente (20.22.2) di macOS {#release-feb2022}

* macOS Monterey - La pagina di caricamento dei file è stata bloccata nei caricamenti successivi. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Correzioni nell’ultima versione (20.22.1) {#release-jan2022}

* Editing immagini **[!UICONTROL Salva]** i pulsanti non funzionavano.
* Negli editor di set, il **[!UICONTROL Chiudi]**, **[!UICONTROL Salva]**, e **[!UICONTROL Salva con nome]** diventano disattivati dopo lo scorrimento delle risorse in **[!UICONTROL Aggiungi risorse]** pannello.
* **[!UICONTROL Play]** nella visualizzazione Dettagli video non funzionava.
* Impossibile immettere `d` e `e` in **[!UICONTROL Nome utente]** e **[!UICONTROL Password]** quando si esegue macOS Monterey.
* Le rimanenti API di analisi sono state spostate alla versione 2.0.

## Correzioni nella versione 20.21.3 {#release-sept2021}

* Miniature non funzionanti per le risorse visualizzate dopo un periodo di inattività sull’app desktop.
* L’app desktop non risponde più, in genere dopo le operazioni Set.
* Modalità di offuscamento e blocco delle richieste abilitata automaticamente in **[!UICONTROL Image Server di prova]**.

   Consulta [Test del servizio di test protetto](/help/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* È stato aggiornato il meccanismo di autenticazione con Adobe Analytics. Rilevante per le nuove integrazioni o se alcune variabili Analytics devono essere aggiornate dall’app desktop Dynamic Media Classic.

   Consulta [Accedere ad Adobe Analytics](/help/log-analytics.md) per i passaggi aggiornati.

## Correzioni nella versione 20.21.2 di {#minor-release}

* Limitazione nota in 20.21.1: **[!UICONTROL Server]** L&#39;elenco a discesa nella schermata di accesso era vuoto.
* In entrata **[!UICONTROL Opzioni processo di caricamento]**, Valore predefinito per la denominazione dei livelli in **[!UICONTROL Opzioni Photoshop]**, è ora **[!UICONTROL Photoshop e nome livello]**. I livelli del file PSD vengono caricati come immagini a sé stanti.
   * Il valore predefinito precedente di **[!UICONTROL Nome livello]**, denominate le immagini in base al nome o al numero del livello nel file PSD. Il numero di livello veniva utilizzato se i nomi dei livelli nel file PSD erano nomi di livello predefiniti di Photoshop.
   * Il nuovo valore predefinito di **[!UICONTROL Photoshop e nome livello]**, assegna alle immagini un nome dopo il file PSD seguito dal nome o dal numero del livello. Il numero del livello viene usato se il livello nel file PSD ha un nome predefinito di Photoshop.
   * Dato che ora le immagini dei livelli in Adobe Dynamic Media Classic hanno nomi univoci, non si verificherà alcun aggiornamento ai PSD o ai modelli esistenti (quali nomi dei livelli condivisi nei file PSD originali).
* Miniature di risorse interrotte.

## Correzioni nella versione 20.21.1 di {#latest-fixes-desktop-app}

* Problemi di accesso a causa di un timeout che causano il seguente messaggio: *Questo utente può essere assegnato al gruppo o ai gruppi senza autorizzazione. Contatta l’amministratore.*
* I predefiniti del visualizzatore vengono duplicati a ogni tentativo di password errata.
* L&#39;applicazione desktop non risponde a causa di molte risorse nella cartella principale. (Risolto su Windows®; funziona come desiderato su macOS.)

## Correzioni nella versione 20.20.2 di {#previous-version-fixes-desktop-app}

* Nessun limite al numero di file che è possibile caricare tramite l’interfaccia utente dell’app desktop sia per macOS che per Windows®.
* Non è necessario uscire dall’app desktop per passare da un’azienda all’altra.
* CTRL+V per incollare ora funziona su Windows®.
* In futuro, quando verrà rilasciata una nuova versione dell’app desktop, gli utenti riceveranno una notifica all’interno dell’app desktop stessa.

## Scarica e installa l’app desktop Adobe Dynamic Media Classic più recente su macOS o Windows® {#installation-dmc-app}

Consultate anche:

* [Scarica e installa in modalità silenziosa l’app desktop Adobe Dynamic Media Classic più recente su Mac](#install-silent-mac-dmc-app)
* [Scarica e installa in modalità automatica l’app desktop Adobe Dynamic Media Classic più recente su Windows®](#install-silent-windows-dmc-app)

1. Disinstalla le versioni precedenti dell’app desktop Adobe Dynamic Media Classic sul sistema.

1. Scarica il programma di installazione più recente per l’app desktop Adobe Dynamic Media Classic.

   * La versione più recente è disponibile al seguente indirizzo:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)
   * La versione precedente è disponibile al seguente indirizzo:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)


<!--         * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Effettua una delle seguenti operazioni in base al programma di installazione scaricato.

   * **macOS** -In **[!UICONTROL Trascina per installare]** finestra di dialogo, trascinare **[!UICONTROL Adobe Dynamic Media Classic]** e rilasciarlo su **[!UICONTROL Applicazioni]**.

      ![Trascina e rilascia l’installazione su macOS](/help/assets/dragondrop-install1.png)

   * In **[!UICONTROL Applicazioni]** cartella, tocca l’icona Adobe Dynamic Media Classic.
   * Nella finestra di dialogo, tocca **[!UICONTROL Apri]** per aprire l’app desktop Adobe Dynamic Media Classic.

      ![Apri l’app scaricata](/help/assets/open-dmclassicapp1.png)

   * **Windows** : esegui il file binario di installazione e segui le istruzioni visualizzate per installare l’app desktop.

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso di Adobe Dynamic Media Classic:

   ![Accesso a Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali utilizzate per accedere a Adobe Dynamic Media Classic nel browser.

   Per **[!UICONTROL Server]** per utilizzare, consulta la mappatura seguente per l’ambiente di produzione:

   | Server | URL browser |
   | --- | --- |
   | Produzione NA (Nord America) | https://s7sps1.scene7.com/ |
   | Produzione EMEA (Europa, Medio Oriente e Africa) | https://s7sps3.scene7.com/ |
   | Produzione APAC (Asia-Pacifico) | https://s7sps5.scene7.com/ |

1. Dopo l’accesso, osserva la familiare esperienza di interfaccia utente del browser. Puoi continuare la tua attività giornaliera di Adobe Dynamic Media Classic come di consueto sull’app desktop.

## Scarica e *silenzioso* installa l’app desktop Adobe Dynamic Media Classic più recente su macOS {#install-silent-mac-dmc-app}

Consultate anche:

* [Scarica e installa l’app desktop Adobe Dynamic Media Classic più recente su Mac o Windows®](#installation-dmc-app)
* [Scarica e installa in modalità automatica l’app desktop Adobe Dynamic Media Classic più recente su Windows®](#install-silent-windows-dmc-app)

Per scaricare e *silenzioso* installa la versione più recente dell’app desktop Adobe Dynamic Media Classic su macOS:

1. Disinstalla le versioni precedenti dell’app desktop Adobe Dynamic Media Classic sul sistema.

1. Scarica il programma di installazione più recente per l’app desktop Adobe Dynamic Media Classic per macOS.

   * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. Montare l&#39;immagine disco scaricata (.DMG) in un punto di montaggio utilizzando il comando seguente:

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. Copia il file .APP in **[!UICONTROL Applicazioni]** utilizzando il comando seguente:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso di Adobe Dynamic Media Classic:

   ![Accesso a Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali utilizzate per accedere a Adobe Dynamic Media Classic nel browser.

   Per **[!UICONTROL Server]** per utilizzare, consulta la mappatura seguente per l’ambiente di produzione:

   | Server | URL browser |
   | --- | --- |
   | Produzione NA (Nord America) | https://s7sps1.scene7.com/ |
   | Produzione EMEA (Europa, Medio Oriente e Africa) | https://s7sps3.scene7.com/ |
   | Produzione APAC (Asia-Pacifico) | https://s7sps5.scene7.com/ |

## Scarica e *silenzioso* installa la più recente app desktop Adobe Dynamic Media Classic su Windows® {#install-silent-windows-dmc-app}

Il comando utilizzato è per un&#39;installazione invisibile all&#39;utente di base di MSI. Tuttavia, il programma di installazione dell’app desktop Adobe Dynamic Media Classic è un programma di installazione MSI InstallScript creato utilizzando InstallShield. Quando si esegue il programma di installazione in modalità record, qualsiasi interazione dell&#39;utente viene registrata in un file di risposta. Questo file di risposta viene quindi utilizzato per un’installazione invisibile all’utente come descritto in [Esecuzione delle installazioni in modalità silenziosa](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

Consultate anche:

* [Scarica e installa l’app desktop Adobe Dynamic Media Classic più recente su Mac o Windows®](#installation-dmc-app)

* [Scarica e installa in modalità silenziosa l’app desktop Adobe Dynamic Media Classic più recente su macOS](#install-silent-mac-dmc-app)

Per scaricare e *silenzioso* installa la versione più recente dell’app desktop Adobe Dynamic Media Classic su Windows®:

1. Disinstalla le versioni precedenti dell’app desktop Adobe Dynamic Media Classic sul sistema.

1. Scarica il programma di installazione più recente per l’app desktop Adobe Dynamic Media Classic.

   * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Eseguire il programma di installazione in modalità record utilizzando il comando seguente:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. Nella finestra del programma di installazione dell&#39;interfaccia utente grafica, seguire la procedura di installazione in modo che le interazioni/gli input, come il percorso di installazione, vengano registrati in `Setup.iss` file.

1. Copia il creato `Setup.iss` file e `adobe-dynamic-media-classic-20.22.1.exe` su un altro computer.

1. Eseguire il comando seguente per un&#39;installazione invisibile all&#39;utente:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   I dettagli sui parametri della riga di comando sono disponibili all&#39;indirizzo [Parametri della riga di comando di Setup.exe e Update.exe](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. Quando apri l’applicazione, viene visualizzata la nuova pagina di accesso di Adobe Dynamic Media Classic:

   ![Accesso a Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Per accedere all’app desktop Adobe Dynamic Media Classic, utilizza le stesse credenziali utilizzate per accedere a Adobe Dynamic Media Classic nel browser.

   Per **[!UICONTROL Server]** per utilizzare, consulta la mappatura seguente per l’ambiente di produzione:

   | Server | URL browser |
   | --- | --- |
   | Produzione NA (Nord America) | https://s7sps1.scene7.com/ |
   | Produzione EMEA (Europa, Medio Oriente e Africa) | https://s7sps3.scene7.com/ |
   | Produzione APAC (Asia-Pacifico) | https://s7sps5.scene7.com/ |

## Video introduttivo sull’utilizzo dell’app desktop Adobe Dynamic Media Classic {#dmc-app-video-walk-through}

Osserva un [video introduttivo sull’utilizzo di Adobe Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (Durata: 2 minuti e 36 secondi).

## Cancellazione della cache delle immagini e delle risorse dal computer tramite l’app desktop {#clear-cache}

1. Nell’app desktop Adobe Dynamic Media Classic, nell’angolo superiore destro, tocca **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione personale]**.
1. Il giorno **[!UICONTROL Configurazione personale]** pagina, sotto **[!UICONTROL Desktop]** eseguire una delle operazioni seguenti:
   * Per rimuovere dal computer tutti i file immagine Dynamic Media memorizzati nella cache di Adobe, tocca **[!UICONTROL Cancella cache immagini]**, quindi tocca **[!UICONTROL OK]**.
   * Per rimuovere dal computer tutti i file di risorse Dynamic Media memorizzati nella cache di Adobe, tocca **[!UICONTROL Cancella cache risorse]**, quindi tocca **[!UICONTROL OK]**.
1. Nell’angolo inferiore destro della pagina, tocca **[!UICONTROL Chiudi]**.

### Cancellazione manuale della cache delle immagini e delle risorse

Oltre a cancellare l’immagine e la cache delle risorse utilizzando l’app desktop, puoi cancellare manualmente la cache direttamente dal file system.

1. In base al sistema operativo in uso, accedi a:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limitazione nota in Adobe Dynamic Media Classic 20.21.1

* Il **[!UICONTROL Server]** L’elenco a discesa è vuoto dopo l’aggiornamento all’app desktop Adobe Dynamic Media Classic 20.21.1 - Scenario: installi e accedi a Adobe Dynamic Media Classic 20.20.1 o 20.20.2, quindi chiudi l’applicazione. Quindi esegui l’aggiornamento a Adobe Dynamic Media Classic 20.21.1. Quando tenti di accedere, il **[!UICONTROL Server]** elenco a discesa nella **[!UICONTROL Accedi al tuo account]** la finestra di dialogo è vuota. Per risolvere il problema, è necessario [cancella manualmente la cache](#clear-cache) (vedere i passaggi precedenti).

## Limitazioni note in Adobe Dynamic Media Classic 20.20.1 (risolte in 20.20.2)

**_Applicabile solo a Windows®: esiste un limite al numero di file che è possibile caricare tramite l’interfaccia utente dell’app desktop?_**<br>Sì, è possibile caricare un massimo di 150 file alla volta tramite l’interfaccia dell’app desktop.

**_Applicabile a Windows® e macOS: come passare da un’azienda all’altra?_**<br>Per passare da un’azienda all’altra, effettua le seguenti operazioni:

* Nell’app Adobe Dynamic Media Classic, seleziona la nuova società dall’elenco a discesa azienda.
* Quando viene visualizzata la finestra pop-up, tocca **[!UICONTROL OK]** per uscire e chiudere l&#39;app.

   ![Per utilizzare la nuova società, riavvia l’app](/help/assets/dmclassic-new-company1.png)

* Riavvia Adobe Dynamic Media Classic, quindi accedi come di consueto per lavorare con la nuova azienda.

## Suggerimenti

**_Non riesco a visualizzare il pannello Media Cart sulla pagina di destinazione di Adobe Dynamic Media Classic._**<br>In Adobe Dynamic Media Classic, tocca**[!UICONTROL Configurazione > Impostazione personale ]**. Nella sezione Browser, assicurati che**[!UICONTROL Mostra funzioni Media Portal ]**è selezionato (selezionato). Tocca**[!UICONTROL Salva > Chiudi ]**.

**_Lo stato di pubblicazione (indicatore verde) di una risorsa non viene visualizzato correttamente._**<br>Nell’interfaccia utente del browser, era necessario accedere nuovamente all’interfaccia utente per visualizzare lo stato di pubblicazione corretto delle risorse. Nell’app desktop, Adobe ha introdotto una**[!UICONTROL Aggiorna ]**nella barra degli strumenti, a destra del**[!UICONTROL Seleziona nessuno ]**pulsante. Tocca il**[!UICONTROL Aggiorna ]**per visualizzare lo stato più recente di tutte le risorse sulla pagina specificata. Non è necessario effettuare nuovamente l’accesso come nell’interfaccia utente del browser.

![Icona Aggiorna](/help/assets/refresh-icon1.png)
*Icona Aggiorna*

**_Nell’app desktop non sono disponibili predefiniti per set di batch._**<br>Tocca**[!UICONTROL Carica > Opzioni processo > Predefiniti set di batch ]**. Garantire la**[!UICONTROL Predefinito set di batch ]**è abilitato. Clic**[!UICONTROL Salva e invia caricamento ]**.
