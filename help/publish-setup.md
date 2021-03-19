---
title: Configurazione pubblicazione
description: Le impostazioni di impostazione della pubblicazione consentono di determinare come le risorse vengono distribuite per impostazione predefinita dai server Dynamic Media Classic ai siti web o alle applicazioni.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Amministratore
translation-type: tm+mt
source-git-commit: 5efad4fff11c9818d43d46ebbbce5335ee1e72b8
workflow-type: tm+mt
source-wordcount: '2422'
ht-degree: 64%

---


# Configurazione pubblicazione {#publish-setup}

Le impostazioni della schermata Publish Setup determinano il modo in cui le risorse vengono distribuite per impostazione predefinita dai server Dynamic Media Classic ai siti web o alle applicazioni. Se non viene specificata alcuna impostazione, il server Dynamic Media Classic distribuisce una risorsa in base a un&#39;impostazione predefinita in una schermata di impostazione della pubblicazione. Ad esempio, la richiesta di distribuire un’immagine che non include un attributo di risoluzione produce nella schermata Server immagini un’immagine con l’impostazione Risoluzione predefinita oggetto.

Gli amministratori possono modificare le impostazioni predefinite delle schermate Server immagini, Modulo di rendering immagini e Vignettatura per configurare nuove impostazioni predefinite per la distribuzione delle risorse dai server.

Per aprire le schermate di impostazione della pubblicazione, fai clic su **Configurazione** > **Impostazione applicazione** > **Impostazioni di pubblicazione**.

>[!NOTE]
>
>le schermate Impostazione pubblicazione sono destinate a sviluppatori e programmatori di siti Web esperti. Dynamic Media Classic presuppone che gli utenti che modificano le impostazioni su questi schermi abbiano familiarità con Dynamic Media Classic, gli standard e le convenzioni del protocollo HTTP e la tecnologia di imaging di base.

## Image Server {#image-server}

La schermata Server immagini consente di configurare le impostazioni predefinite per la distribuzione delle immagini dai server. Le impostazioni disponibili sono organizzate nelle cinque categorie indicate di seguito (consultate la schermata Server immagini per una descrizione dettagliata delle impostazioni).

Modificare queste impostazioni solo con l&#39;assistenza di un supporto Dynamic Media Classic.

**Gestione** catalogoQueste impostazioni determinano il modo in cui Dynamic Media Classic e il catalogo interagiscono. A differenza della maggior parte dei server web, le chiamate URL di Dynamic Media Image Server vanno a un file manifesto o catalogo anziché a un file immagine corretto. Il file catalogo (da non confondersi con un eCatalog) contiene un elenco di tutti i contenuti pubblicati sul server immagini e il percorso di ciascuna immagine. Se disponete di un ID Digimarc, inserite i vostri dati nella sezione Informazioni utente Digimarc.

**Richiedi** attributiQueste impostazioni impongono limiti alle immagini che possono essere consegnate dal server. Ad esempio, il *massimo* **[!UICONTROL Limite dimensione immagine risposta]** è **[!UICONTROL Larghezza]** 5000 e **[!UICONTROL Altezza]** 5000.

**Default Request** AttributesQueste impostazioni riguardano l&#39;aspetto predefinito delle immagini.

**Common Thumbnail** AttributesQueste impostazioni riguardano l&#39;aspetto e l&#39;allineamento predefiniti delle immagini in miniatura.

**Valori predefiniti per** i campi del catalogoQueste impostazioni si riferiscono alla risoluzione e al tipo di miniatura predefinito delle immagini.

**Attributi di gestione** del coloreQueste impostazioni determinano quali profili di colore ICC vengono utilizzati.

**** Attributi di compatibilitàQuesta impostazione consente ai paragrafi iniziali e finali nei livelli di testo di essere trattati come nella versione 3.6 per la compatibilità con le versioni precedenti.

**Supporto** localizzazioneQueste impostazioni consentono di gestire più attributi internazionali. Consentono inoltre di specificare una stringa di mappa lingua in modo da definire le lingue da supportare per le descrizioni comandi nei visualizzatori.

Ad esempio, se fate parte di una società multinazionale che vende in diversi paesi, potete mettere a punto un visualizzatore localizzato specifico per ciascun paese. A questo scopo, dovete innanzi tutto specificare una stringa di mappa lingua. Quindi, modificate il testo della descrizione comando nel predefinito del visualizzatore aggiungendo le stringhe di testo tradotte per la lingua desiderata.

>[!NOTE]
> Per impostare le opzioni di supporto per la localizzazione, [utilizza l&#39;Admin Console per creare un caso di supporto.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Nel tuo caso di assistenza, richiedi aiuto per la configurazione.

Per ulteriori informazioni sull’impostazione del **supporto per la localizzazione**, consultate [Considerazioni per l’impostazione della localizzazione delle risorse](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considerazioni per l’impostazione della localizzazione delle risorse {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Per impostare le opzioni di supporto per la localizzazione in Dynamic Media Classic, ad esempio il campo Mappa lingua, [utilizza l&#39;Admin Console per creare un caso di supporto.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Nel tuo caso di assistenza, richiedi aiuto per la configurazione.

Un modo comune per utilizzare Dynamic Media Classic è gestire le immagini del prodotto sui siti web di e-commerce. Le aziende internazionali devono poter gestire risorse per prodotti simili ma diverse da paese a paese. In genere si tratta di poche differenze per una piccola parte dei contenuti multimediali. La gestione di tali differenze copiando tutte le risorse per ciascuno dei paesi e sostituendo solo quelle differenti richiede molto lavoro e contraddice il concetto di singola risorsa master. Le differenze nelle risorse possono spaziare da video specifici per i singoli paesi con tracce audio distinte, a cavi elettrici diversi da usare con un prodotto. Dynamic Media Classic utilizza un meccanismo di ricerca di base. Potete definire l’ordine di suffissi per risorse che il server immagini deve seguire per le ricerche, a partire dalla lingua richiesta.

**Come vengono localizzate le risorse**

La lingua per una richiesta IS (Image Serving) è identificata con il seguente comando IS/IR (Image Rendering):

`locale=`

Questo comando accetta una stringa di ID della lingua (locid) che non fa distinzione tra maiuscole e minuscole. L’ID della lingua è in genere una stringa di 2-6 caratteri composta di lettere e trattino basso (_).

IS supporta stringhe ASCII stampabili arbitrarie.Il comando `locale=` ha un ambito globale, ovvero viene applicato all&#39;intera richiesta, incluse tutte le richieste IS e IR nidificate, i modelli di riferimento e i livelli immagine. Non sono supportate più lingue per richiesta, ad esempio una lingua diversa per ciascun livello. Tuttavia, è possibile consentire sostituzioni esplicite nelle richieste nidificate.

Se `locale=` non è specificato, `attribute::DefaultLocale` viene passato ai motori di traduzione. Al valore `locale=` viene applicata una convalida di input limitata. Sono consentiti valori `locale=` vuoti. Poiché `locale=` ha un ambito globale, `attribute::DefaultLocale` viene fornito dal catalogo principale per l’intera richiesta.

Alcuni dei vantaggi dell&#39;utilizzo di `locale=` e `attribute::DefaultLocale` includono:

* Condivisione di contenuti per più lingue
* Accesso a contenuti specifici in base alla lingua con ID generici
* Flessibilità nelle convenzioni di denominazione e nella gestione dei contenuti in base alla lingua, ad esempio prefisso o suffisso oppure contenuti specifici in base alla lingue in un catalogo a parte
* Supporto di accesso diretto alle versioni per lingue diverse
* Aggregazione di oggetti, ad esempio set di immagini, con riferimenti generici a contenuti che possono essere specifici per determinate lingue
* Supporto di tutti i contenuti gestiti da cataloghi che potrebbero richiedere localizzazione, come immagini, set di immagini, vignettature, materiali e record di configurazione del visualizzatore
* Riduzione al minimo delle modifiche da apportare ai meccanismi del database IPS e del manifesto IS
* Supporto per contenuti statici come video e interfacce da aggiungere con l’implementazione di RFC IS-63
* La lingua predefinita è configurabile.

**Esempi applicativi**

| Applicazione | Scenario |
|--- |--- |
| Localizzazione del visualizzatore | Dopo l’implementazione di cataloghi di contenuti statici, la localizzazione è controllata completamente dal parametro locale= che viene associato a tutte le richieste inviate a IS. I record di configurazione, le interface, le schermate iniziali e così via possono disporre o meno di varianti in base alla lingua. Il contenuto corretto viene fornito da IS e non è necessario che l’utente sappia quali contenuti sono localizzati e i relativi ID. |
| Immagini e video | Le multinazionali utilizzano spesso una combinazione di contenuti generici e specifici per lingua. Un riferimento a un’immagine o un video può quindi essere generico e, se disponibile, IS ne fornisce la versione localizzata. |
| Set di immagini e set di file multimediali | L’intero set di immagini può essere diverso per alcune impostazioni internazionali, ad esempio quando un eCatalog è completamente diverso, con la traduzione da un set di immagini generico a uno specifico per le impostazioni internazionali gestito dal visualizzatore.Più comunemente, i singoli ID in un set generico possono fare riferimento a contenuti localizzati. Ad esempio, la maggior parte delle foto di un apparecchio saranno uguali per tutte le lingue, eccetto la foto del pannello di controllo. IS traduce automaticamente gli ID e non è quindi necessario generare set di immagini specifici per le diverse lingue. |

**Implementazione della localizzazione delle risorse**

Dynamic Media Classic e Image Server dispongono di un&#39;interfaccia che consente la localizzazione di immagini e contenuti statici.

Senza localizzazione, un URL di Image Server si presenta come segue:

`https://server/is/image/company/image`

Con la localizzazione, un URL di Image Server aggiunge il parametro `locale=` al percorso, come segue:

`https://server/is/image/company/image?locale=de_DE`

Al ricevimento della chiamata http da parte del server di immagini, il parametro `locale=` viene analizzato attraverso il campo localeMap disponibile nel gruppo **Configurazione** > **Impostazione applicazione** > **Configurazione pubblicazione** > **Image Server** > **Supporto localizzazione**.

Il campo Mappa lingua contiene un elenco di voci separate con il simbolo di barra verticale (|).

Ogni voce è un elenco di valori separati da virgola. Il primo valore è il valore di ricerca trasmesso dal parametro `locale=`. I valori rimanenti sono valori di suffisso/sostituzione che vengono provati in successione finché uno corrisponde a un’immagine esistente.

L’applicazione del valore di suffisso o di sostituzione dipende dall’impostazione Lingua globale in **Configurazione** > **Impostazione applicazione** > **Configurazione pubblicazione** > **Image Server** > **Supporto per la localizzazione**.

>[!NOTE]
>
>L’impostazione Global Locale è attualmente possibile solo quando la imposti tramite l’API e non all’interno dell’interfaccia di Dynamic Media Classic.

**Esempio di suffisso**

| URL | ID di Mappa lingua | Risultato |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Osservate che non è definita alcuna lingua globale. Il parametro di lingua de_DE viene associato alla prima voce nella Mappa lingua. Il primo valore corrispondente _DE viene aggiunto come suffisso alla risorsa image_DE che viene ricercata in Image Server e, se trovata, viene restituita. In caso contrario, viene utilizzato come suffisso il secondo valore “” e viene restituita l’immagine stessa. |

**Esempio di sostituzione**

| URL | Lingua globale e ID di Mappa lingua | Risultato |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | In questo esempio di sostituzione, il parametro della lingua globale GlobalLocale è impostato su main. Il parametro di lingua de_DE viene associato alla prima voce nella Mappa lingua. La sottostringa GlobalLocale viene trovata e sostituita con il primo valore corrispondente “de” nella Mappa lingua: image-de-01. Se questo viene trovato in Image Server, viene restituito. In caso contrario, viene sostituito il secondo valore e si ottiene image-main-01. |

Se nell’URL non viene specificata alcuna lingua, Image Server applica all’URL la lingua predefinita, se questa è definita.

Se con `locale=` viene fornito un parametro locale sconosciuto o vuoto, viene eseguita la scansione della Mappa locale per individuare il valore vuoto &quot;inizia con&quot;. È importante configurare questo parametro affinché una lingua predefinita possa essere applicata alle lingue sconosciute.

**Informazioni defaultImage**

Image Server prova in successione le opzioni per la lingua richiesta. Se non viene trovata alcuna corrispondenza, le opzioni della lingua vengono applicate all’immagine predefinita defaultImage e viene restituita la versione corrispondente. Pertanto, ogni impostazione internazionale deve includere un&#39;opzione per l&#39;immagine senza localizzazione, oppure le versioni localizzate defaultImage devono essere rese disponibili in Dynamic Media Classic.

**Scenari per l’individuazione della Mappa lingua**

Supponiamo che si intendano supportare le seguenti lingue:

`en, en_us, en_uk, de, de_at, de_de, fr`

Queste impostazioni internazionali vengono mappate sui suffissi `_E`, `_G` e `_F` rispettivamente per inglese, tedesco e francese. Per tutti gli esempi, l’ID di immagine di input generico è `myImg`.

*Comportamento standard per l’individuazione della Mappa lingua*

Gli ID delle lingue vengono mappati sui suffissi corrispondenti. Se nel catalogo non viene trovato alcun ID per una lingua, viene provato l’ID generico. Osservate come i valori locSuffix vuoti vengono associati all’ID generico.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | ID di output per la ricerca |
|--- |--- |
| en,en_us, en_uk | myImg_E, myImg |
| de,de_de,de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Tutti gli altri | - |

*Individuazione della Mappa lingua quando la lingua è sconosciuta*

Potete associare le lingue sconosciute a ID specifici o generici. In questo esempio, potete mappare le lingue sconosciute agli ID per l’inglese oppure, se questi non esistono, a ID generici.

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

*Individuare la Mappa lingua con una ricerca a più livelli*

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

*Ricerca della Mappa lingua mediante la ricerca di ID specifici*

Alcune convenzioni per la denominazione delle immagini potrebbero non supportare gli ID di immagini generici. Gli ID generici da questa richiesta devono essere associati a un ID specifico nel catalogo. Tuttavia, in alcuni casi l’ID specifico esatto potrebbe non essere noto.

Utilizzando il primo esempio come base, le immagini per tutte le lingue possono avere i suffissi `_1`, `_2` o `_3`. Le immagini specifiche per le impostazioni internazionali francesi possono avere il suffisso `_22` o `_23` . E le immagini specifiche per le impostazioni internazionali tedesche possono avere i suffissi `_470` o `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | ID di output per la ricerca |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Tutti gli altri | myImg_1, myImg_2, myImg_3 |

**Considerazioni importanti per l’implementazione del supporto per la localizzazione**

* La localizzazione è limitata alle chiamate per risorse basate su ID e non può essere utilizzata per le chiamate per risorse basate su percorso. Di conseguenza, quando si chiama un video con una specifica lingua, questo deve essere chiamato perché come società/ID risorsa e non come percorso completo del video. Non potete pertanto utilizzare RTMP con la localizzazione poiché questo supporta solo le chiamate video basate su percorso.
* Quando l’opzione Mappa lingua è attiva, non è possibile utilizzare un set di file multimediali diversi contenente un singolo video, poiché tale chiamata avrebbe esito negativo. Per risolvere questo inconveniente è possibile aggiungere un singolo video a un set di video adattivi. Quindi, aggiungete il set di video adattivi al set di file multimediali diversi.
* Alcune richieste non sono localizzate. Questo è il caso ad esempio delle richieste per i contenuti dei set di video adattivi. Per poter utilizzare i set di video adattivi con la localizzazione è pertanto necessario inserirli all’interno di un set di file multimediali diversi. Quindi, chiama il set in un visualizzatore di file multimediali diversi con il parametro `locale=` .

## Modulo di rendering immagini {#image-renderer}

La schermata Modulo di rendering immagini consente di definire le impostazioni predefinite per la distribuzione di set di immagini dai server di rendering. Sono disponibili impostazioni nelle cinque categorie indicate di seguito (consultate la schermata Server immagini per una descrizione dettagliata delle impostazioni):

**Gestione** catalogoQueste impostazioni determinano il modo in cui Dynamic Media Classic e il file di catalogo interagiscono. Le chiamate URL al server di rendering Dynamic Media Classic vengono effettuate al catalogo, che a sua volta effettua chiamate per distribuire immagini dal server. Modificare queste impostazioni solo con l&#39;assistenza di un supporto Dynamic Media Classic.

**Attributi** della sessioneQueste impostazioni stabiliscono i parametri di errore, l&#39;URL per gli URL delle immagini relative e se è consentita la sovrapposizione degli oggetti.

**Default Material** AttributesQueste impostazioni stabiliscono le impostazioni predefinite di risoluzione e nitidezza per le immagini.

**Risposta** Attributi immagineQueste impostazioni riguardano l&#39;aspetto predefinito delle immagini.

**Color Management** AttributesQueste impostazioni si riferiscono alle impostazioni di colore predefinite delle immagini.

## Vignettatura {#vignette}

La schermata Vignettatura contiene impostazioni che specificano l’aspetto predefinito delle vignettature (consultate la schermata per una descrizione dettagliata delle opzioni).
