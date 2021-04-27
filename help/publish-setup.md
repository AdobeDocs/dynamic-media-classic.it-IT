---
title: Configurazione pubblicazione
description: Le impostazioni di impostazione della pubblicazione consentono di determinare come le risorse vengono distribuite per impostazione predefinita dai server Dynamic Media Classic ai siti web o alle applicazioni.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Administrator
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '2403'
ht-degree: 47%

---

# Configurazione pubblicazione {#publish-setup}

Le impostazioni della pagina Configurazione pubblicazione determinano il modo in cui le risorse vengono distribuite per impostazione predefinita dai server Dynamic Media Classic ai siti web o alle applicazioni. Se non viene specificata alcuna impostazione, il server Dynamic Media Classic distribuisce una risorsa in base a un&#39;impostazione predefinita in una pagina di impostazione della pubblicazione. Ad esempio, una richiesta di consegna di un’immagine che non include un attributo di risoluzione genera un’immagine con l’impostazione Risoluzione oggetti predefinita nella pagina Image Server.

Gli amministratori possono modificare le impostazioni predefinite nelle pagine Image Server, Image Renderer e Vignette per stabilire le impostazioni predefinite per la distribuzione delle risorse dai server.

Per aprire le pagine Pubblica installazione, fai clic su **Configurazione** > **Impostazione applicazione** > **Impostazioni pubblicazione**.

>[!NOTE]
>
>Le pagine Pubblica configurazione sono destinate ad sviluppatori e programmatori di siti web esperti. Dynamic Media Classic presuppone che gli utenti che modificano le impostazioni in queste pagine abbiano familiarità con Dynamic Media Classic, gli standard e le convenzioni del protocollo HTTP e la tecnologia di imaging di base.

## Image Server {#image-server}

La pagina Image Server stabilisce le impostazioni predefinite per la distribuzione delle immagini dai server di immagini. Le impostazioni sono disponibili in queste cinque categorie (per una descrizione dettagliata delle impostazioni, vedere la pagina Image Server stessa).

Modificare queste impostazioni solo con l&#39;assistenza di un supporto Dynamic Media Classic.

* **Gestione catalogo** : queste impostazioni determinano il modo in cui Dynamic Media Classic e il catalogo interagiscono. A differenza della maggior parte dei server web, le chiamate URL di Dynamic Media Image Server vanno a un file manifesto o catalogo anziché a un file immagine corretto. Il file catalogo (da non confondersi con un eCatalog) contiene un elenco di tutti i contenuti pubblicati sul server immagini e il percorso di ciascuna immagine. Se disponete di un ID Digimarc, inserite i vostri dati nella sezione Informazioni utente Digimarc.

* **Richiedi attributi** : queste impostazioni impongono limiti alle immagini che possono essere consegnate dal server. Ad esempio, il *massimo* **[!UICONTROL Limite dimensione immagine risposta]** è **[!UICONTROL Larghezza]** 5000 e **[!UICONTROL Altezza]** 5000.

* **Attributi richiesta predefiniti** : queste impostazioni si riferiscono all&#39;aspetto predefinito delle immagini.

* **Attributi comuni delle miniature** : queste impostazioni si riferiscono all&#39;aspetto e all&#39;allineamento predefiniti delle immagini in miniatura.

* **Valori predefiniti per i campi del catalogo** : queste impostazioni si riferiscono alla risoluzione e al tipo di miniatura predefinito delle immagini.

* **Attributi di gestione del colore** : queste impostazioni determinano quali profili di colore ICC vengono utilizzati.

* **Attributi di compatibilità** : questa impostazione consente ai paragrafi iniziali e finali nei livelli di testo di essere trattati come nella versione 3.6 per la compatibilità con le versioni precedenti.

* **Supporto per la localizzazione** : queste impostazioni consentono di gestire più attributi di impostazione internazionale. Consentono inoltre di specificare una stringa di mappa lingua in modo da definire le lingue da supportare per le descrizioni comandi nei visualizzatori.

   Ad esempio, se fate parte di una società multinazionale che vende in diversi paesi, potete mettere a punto un visualizzatore localizzato specifico per ciascun paese. A questo scopo, dovete innanzi tutto specificare una stringa di mappa lingua. Quindi, modificate il testo della descrizione comando nel predefinito del visualizzatore aggiungendo le stringhe di testo tradotte per la lingua desiderata.

   >[!NOTE]
   > Per impostare le opzioni di supporto per la localizzazione, [utilizza l&#39;Admin Console per creare un caso di supporto.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Nel tuo caso di assistenza, richiedi aiuto per la configurazione.

   Per ulteriori informazioni sull’impostazione del **supporto per la localizzazione**, consultate [Considerazioni per l’impostazione della localizzazione delle risorse](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considerazioni per l’impostazione della localizzazione delle risorse {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Per impostare le opzioni di supporto per la localizzazione in Dynamic Media Classic, ad esempio il campo Mappa lingua, [utilizza l&#39;Admin Console per creare un caso di supporto.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Nel tuo caso di assistenza, richiedi aiuto per la configurazione.

Un modo comune per utilizzare Dynamic Media Classic è gestire le immagini del prodotto sui siti web di e-commerce. Le aziende internazionali devono poter gestire risorse per prodotti simili ma diverse da paese a paese. Di solito le differenze sono per alcune parti del media complessivo. La gestione di tali differenze copiando tutte le risorse per ciascuno dei paesi e sostituendo solo quelle differenti richiede molto lavoro e contraddice il concetto di singola risorsa master. Le differenze nelle risorse possono spaziare da video specifici per i singoli paesi con tracce audio distinte, a cavi elettrici diversi da usare con un prodotto. Dynamic Media Classic utilizza un meccanismo di ricerca di base. Potete definire l’ordine di suffissi per risorse che il server immagini deve seguire per le ricerche, a partire dalla lingua richiesta.

#### Come vengono localizzate le risorse

La lingua per una richiesta IS (Image Serving) è identificata con il seguente comando IS/IR (Image Rendering):

`locale=`

Questo comando accetta una stringa di ID della lingua (locid) che non fa distinzione tra maiuscole e minuscole. L’ID della lingua è in genere una stringa di 2-6 caratteri composta di lettere e trattino basso (_).

IS supporta stringhe ASCII stampabili arbitrarie. Il comando `locale=` ha un ambito globale, il che significa che viene applicato all&#39;intera richiesta, incluse tutte le richieste IS e IR nidificate, i modelli di riferimento e i livelli immagine. Non sono supportate più lingue per richiesta, ad esempio una lingua diversa per ciascun livello. Tuttavia, è possibile consentire sostituzioni esplicite nelle richieste nidificate.

Se `locale=` non è specificato, `attribute::DefaultLocale` viene passato ai motori di traduzione. Al valore `locale=` viene applicata una convalida di input limitata. Sono consentiti valori `locale=` vuoti. Poiché `locale=` ha un ambito globale, `attribute::DefaultLocale` viene fornito dal catalogo principale per l’intera richiesta.

Alcuni dei vantaggi dell&#39;utilizzo di `locale=` e `attribute::DefaultLocale` includono:

* Condivisione di contenuti per più lingue
* Accesso a contenuti specifici in base alla lingua con ID generici
* Flessibilità nelle convenzioni di denominazione e nella gestione dei contenuti in base alla lingua, ad esempio prefisso o suffisso oppure contenuti specifici in base alla lingue in un catalogo a parte
* Supporto dell&#39;accesso alle versioni specifiche delle impostazioni internazionali.
* Gli oggetti aggregati, ad esempio i set di immagini, possono a volte contenere riferimenti generici a contenuti potenzialmente specifici per le impostazioni internazionali.
* Supporta tutti i contenuti gestiti da cataloghi che necessitano di localizzazione, tra cui immagini, set di immagini, vignette, materiali e record di configurazione dei visualizzatori.
* Riduzione al minimo delle modifiche da apportare ai meccanismi del database IPS e del manifesto IS
* Quando la RFC IS-63 è implementata, viene aggiunto il supporto per contenuti statici come video e interfacce.
* La lingua predefinita è configurabile.

#### Esempi applicativi

| Applicazione | Scenario |
|--- |--- |
| Localizzazione del visualizzatore | Dopo l’implementazione di cataloghi di contenuti statici, la localizzazione è controllata completamente dal parametro locale= che viene associato a tutte le richieste inviate a IS. I record di configurazione, le interface, le schermate iniziali e così via possono disporre o meno di varianti in base alla lingua. Il contenuto corretto viene fornito da IS e non è necessario che l’utente sappia quali contenuti sono localizzati e i relativi ID. |
| Immagini e video | Le multinazionali utilizzano spesso una combinazione di contenuti generici e specifici per lingua. Un riferimento a un’immagine o un video può quindi essere generico e, se disponibile, IS ne fornisce la versione localizzata. |
| Set di immagini e set di file multimediali | L’intero set di immagini può essere diverso per alcune impostazioni internazionali, ad esempio quando un eCatalog è diverso, con la traduzione da un set di immagini generico a uno specifico per le impostazioni internazionali gestito dal visualizzatore. Più comunemente, i singoli ID in un set generico possono fare riferimento a contenuti localizzati. Ad esempio, la maggior parte delle foto di un apparecchio può essere la stessa in tutte le lingue, ad eccezione della foto del Pannello di controllo Campaign. IS traduce automaticamente gli ID e non è quindi necessario generare set di immagini specifici per le diverse lingue. |

#### Implementazione della localizzazione delle risorse

Dynamic Media Classic e Image Server dispongono di un&#39;interfaccia che consente la localizzazione di immagini e contenuti statici.

Senza localizzazione, un URL di Image Server si presenta come segue:

`https://server/is/image/company/image`

Con la localizzazione, un URL di Image Server aggiunge il parametro `locale=` al percorso, come segue:

`https://server/is/image/company/image?locale=de_DE`

Al ricevimento della chiamata http da parte del server di immagini, il parametro `locale=` viene analizzato attraverso il campo localeMap disponibile nel gruppo ****[!UICONTROL Configurazione]**** > ****[!UICONTROL Impostazione applicazione]**** > ****[!UICONTROL Configurazione pubblicazione]**** > ****[!UICONTROL Image Server]**** > ****[!UICONTROL Supporto localizzazione]****.

Il campo Mappa lingua contiene un elenco di voci separate con il simbolo di barra verticale (|).

Ogni voce è un elenco di valori separati da virgola. Il primo valore è il valore di ricerca trasmesso dal parametro `locale=`. I valori rimanenti sono suffissi/valori di sostituzione che vengono poi provati fino a quando non si ottiene un&#39;immagine esistente.

L’applicazione del valore di suffisso o di sostituzione dipende dall’impostazione Lingua globale in ****[!UICONTROL Configurazione]**** > ****[!UICONTROL Impostazione applicazione]**** > ****[!UICONTROL Configurazione pubblicazione]**** > ****[!UICONTROL Image Server]**** > ****[!UICONTROL Supporto per la localizzazione]****.

>[!NOTE]
>
>L’impostazione Global Locale è possibile solo quando la imposti tramite l’API e non all’interno dell’interfaccia di Dynamic Media Classic.

**Esempio di suffisso:**

| URL | ID di Mappa lingua | Risultato |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Osservate che non è definita alcuna lingua globale. Il parametro di lingua de_DE viene associato alla prima voce nella Mappa lingua. Il primo valore corrispondente _DE viene aggiunto come suffisso alla risorsa image_DE che viene ricercata in Image Server e, se trovata, viene restituita. In caso contrario, viene utilizzato come suffisso il secondo valore “” e viene restituita l’immagine stessa. |

**Esempio di sostituzione:**

| URL | Lingua globale e ID di Mappa lingua | Risultato |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | In questo esempio di sostituzione, il parametro della lingua globale GlobalLocale è impostato su main. Il parametro di lingua de_DE viene associato alla prima voce nella Mappa lingua. La sottostringa GlobalLocale viene trovata e sostituita con il primo valore corrispondente `de` nella localeMap: `image-de-01`. Se questo viene trovato in Image Server, viene restituito. In caso contrario, viene sostituito il secondo valore e si ottiene `image-main-01`. |

Se nell’URL non viene specificata alcuna lingua, Image Server applica all’URL la lingua predefinita, se questa è definita.

Se con `locale=` viene fornito un parametro locale sconosciuto o vuoto, viene eseguita la scansione della Mappa locale per individuare il valore vuoto &quot;inizia con&quot;. È importante che le impostazioni internazionali predefinite siano applicate alle impostazioni internazionali sconosciute.

#### Informazioni su defaultImage

Image Server prova in successione le opzioni per la lingua richiesta. Se non viene trovata alcuna corrispondenza, le opzioni internazionali vengono applicate a defaultImage e viene restituita la versione corrispondente. Pertanto, ogni impostazione internazionale deve includere un&#39;opzione per l&#39;immagine senza localizzazione, oppure le versioni localizzate defaultImage sono rese disponibili in Dynamic Media Classic.

#### Scenari per l’individuazione della Mappa lingua

Supponiamo che si intendano supportare le seguenti lingue:

`en, en_us, en_uk, de, de_at, de_de, fr`

Queste impostazioni internazionali vengono mappate sui suffissi `_E`, `_G` e `_F` rispettivamente per inglese, tedesco e francese. Per tutti gli esempi, l’ID di immagine di input generico è `myImg`.

##### Comportamento standard per l’individuazione della Mappa lingua

Gli ID delle lingue vengono mappati sui suffissi corrispondenti. Se nel catalogo non viene trovato alcun ID per una lingua, viene provato l’ID generico. Osservate come i valori locSuffix vuoti vengono associati all’ID generico.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | ID di output per la ricerca |
|--- |--- |
| en,en_us, en_uk | myImg_E, myImg |
| de,de_de,de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Tutti gli altri | - |

##### Individuazione della Mappa lingua quando la lingua è sconosciuta

Potete associare le lingue sconosciute a ID specifici o generici. Ad esempio, è possibile mappare le impostazioni internazionali sconosciute agli ID inglesi, o se non esistono, agli ID generici.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | ID di output per la ricerca |
|--- |--- |
| de,de_de,de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Tutti gli altri | myImg_E, myImg |

È inoltre possibile disporre di un suffisso locSuffix dedicato, ad esempio U, solo per le impostazioni internazionali sconosciute e forzare l&#39;immagine predefinita se non esiste `_U`, come illustrato di seguito:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Oppure, potete impostare la mappatura direttamente sull’ID generico:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### Individuare la Mappa lingua con una ricerca a più livelli

Spesso è utile raggruppare le lingue in base a gruppi che condividono uno stesso standard, ad esempio tre diversi tipo di interfaccia per Europa, Medio Oriente e Nord America. A questo scopo si può ricorrere alla ricerca a più livelli.

In questo esempio, supponiamo di voler supportare raccolte diverse per gli utenti nei paesi occidentali (Western) e mediorientali (Middle Eastern). Entrambe le raccolte sono basate sulla raccolta di immagini generica e per entrambe alcune immagini sono aggiunte o modificate. Entrambe le raccolte vengono quindi perfezionate ulteriormente per impostazioni internazionali specifiche, ad esempio `m1, m2` per due varianti medio-orientali e `w1, w2,` e `w3` per tre impostazioni internazionali, tranne per il fatto che le immagini sono condivise per `w1` e `w3`. Le lingue sconosciute sono associate solo alla raccolta generica e non hanno accesso alle immagini per lingue specifiche. Esempio della mappa:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | ID di output per la ricerca |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Tutti gli altri | mylmg |

##### Ricerca della Mappa lingua mediante la ricerca di ID specifici

Alcune convenzioni di denominazione delle immagini non supportano ID immagine generici. Gli ID generici da questa richiesta devono essere associati a un ID specifico nel catalogo. Tuttavia, in alcuni casi l’ID specifico esatto non è noto.

Utilizzando il primo esempio come base, le immagini per tutte le lingue potrebbero avere i suffissi `_1`, `_2` o `_3`. Le immagini specifiche per le impostazioni internazionali francesi possono avere il suffisso `_22` o `_23` . E le immagini specifiche per le impostazioni internazionali tedesche potrebbero avere i suffissi `_470` o `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | ID di output per la ricerca |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Tutti gli altri | myImg_1, myImg_2, myImg_3 |

##### Considerazioni importanti per l’implementazione del supporto per la localizzazione

* La localizzazione è limitata alle chiamate per risorse basate su ID e non può essere utilizzata per le chiamate per risorse basate su percorso. Di conseguenza, quando si chiama un video con una specifica lingua, questo deve essere chiamato perché come società/ID risorsa e non come percorso completo del video. Non è possibile utilizzare rtmp con la localizzazione perché questo metodo è destinato solo alle chiamate video basate sul percorso.
* Quando l’opzione Mappa lingua è attiva, non è possibile utilizzare un set di file multimediali diversi contenente un singolo video, poiché tale chiamata avrebbe esito negativo. Per risolvere questo problema, è possibile aggiungere un singolo video a un set video adattivo. Quindi, aggiungete il set di video adattivi al set di file multimediali diversi.
* Alcune richieste non sono localizzate. Questo è il caso ad esempio delle richieste per i contenuti dei set di video adattivi. Pertanto, se desideri utilizzare i set video adattivi con la localizzazione, inserisci il set video adattivo all’interno di un set di file multimediali diversi. Quindi, chiama il set in un visualizzatore di file multimediali diversi con il parametro `locale=` .

## Modulo di rendering immagini {#image-renderer}

La pagina Image Renderer stabilisce le impostazioni predefinite per la distribuzione di set di immagini dai server di rendering delle immagini. Le impostazioni sono disponibili nelle cinque categorie seguenti (per una descrizione dettagliata delle impostazioni, vedere la pagina Image Server stessa):

* **Gestione catalogo** : queste impostazioni determinano il modo in cui Dynamic Media Classic e il file di catalogo interagiscono. Le chiamate URL al server di rendering Dynamic Media Classic vengono effettuate al catalogo, che a sua volta effettua chiamate per distribuire immagini dal server. Modificare queste impostazioni solo con l&#39;assistenza di un supporto Dynamic Media Classic.

* **Attributi di sessione** : queste impostazioni stabiliscono i parametri di errore, l&#39;URL per gli URL delle immagini relative e se è consentita la sovrapposizione degli oggetti.

* **Attributi del materiale predefiniti** : queste impostazioni stabiliscono le impostazioni predefinite di risoluzione e nitidezza per le immagini.

* **Attributi immagine di risposta** : queste impostazioni si riferiscono all&#39;aspetto predefinito delle immagini.

* **Attributi di gestione del colore** : queste impostazioni si riferiscono alle impostazioni di colore predefinite delle immagini.

## Vignettatura {#vignette}

La pagina Vignetta offre impostazioni per stabilire l’aspetto predefinito delle vignette (consulta la pagina stessa per una descrizione dettagliata delle opzioni).
