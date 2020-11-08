---
title: Configurazione pubblicazione
seo-title: Configurazione pubblicazione
description: 'null'
seo-description: Le impostazioni della schermata Configurazione pubblicazione specificano il modo in cui le risorse vengono distribuite per impostazione predefinita dai server Dynamic Media Classic ai siti Web o alle applicazioni.
uuid: 196f25c8-abf5-4c5d-8f6f-bc70007a0301
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: cba59093-28b6-4490-b838-d942b72ad1ec
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '2421'
ht-degree: 64%

---


# Configurazione pubblicazione {#publish-setup}

Le impostazioni della schermata Configurazione pubblicazione specificano il modo in cui le risorse vengono distribuite per impostazione predefinita dai server Dynamic Media Classic ai siti Web o alle applicazioni. Se non viene specificata alcuna impostazione, il server Dynamic Media Classic distribuisce una risorsa in base alle impostazioni predefinite in una schermata Impostazione pubblicazione. Ad esempio, la richiesta di distribuire un’immagine che non include un attributo di risoluzione produce nella schermata Server immagini un’immagine con l’impostazione Risoluzione predefinita oggetto.

Gli amministratori possono modificare le impostazioni predefinite delle schermate Server immagini, Modulo di rendering immagini e Vignettatura per configurare nuove impostazioni predefinite per la distribuzione delle risorse dai server.

Per aprire le schermate Impostazione pubblicazione, scegliete Configurazione > Impostazione applicazione e selezionate Impostazione pubblicazione.

>[!NOTE]
>
>le schermate Impostazione pubblicazione sono destinate a sviluppatori e programmatori di siti Web esperti. Dynamic Media Classic presuppone che gli utenti che modificano le impostazioni su queste schermate abbiano familiarità con Dynamic Media Classic, con gli standard e le convenzioni del protocollo HTTP e con la tecnologia di imaging di base.

## Image Server {#image-server}

La schermata Server immagini consente di configurare le impostazioni predefinite per la distribuzione delle immagini dai server. Le impostazioni disponibili sono organizzate nelle cinque categorie indicate di seguito (consultate la schermata Server immagini per una descrizione dettagliata delle impostazioni).

Modificate queste impostazioni solo con l’assistenza di un addetto al supporto per Dynamic Media Classic.

**Gestione** catalogo Queste impostazioni determinano il modo in cui Dynamic Media Classic e il catalogo interagiscono. A differenza della maggior parte dei server Web, le chiamate URL di Dynamic Media Image Server vanno a un file manifesto o catalogo anziché a un file immagine vero e proprio. Il file catalogo (da non confondersi con un eCatalog) contiene un elenco di tutti i contenuti pubblicati sul server immagini e il percorso di ciascuna immagine. Se disponete di un ID Digimarc, inserite i vostri dati nella sezione Informazioni utente Digimarc.

**Attributi** richiesta Queste impostazioni impongono limiti alle immagini che possono essere distribuite dal server. Ad esempio, il limite ** massimo **[!UICONTROL per le dimensioni delle immagini della]** risposta è **[!UICONTROL Larghezza]** 5000 e **[!UICONTROL Altezza]** 5000.

**Attributi** richiesta predefiniti Queste impostazioni interessano l&#39;aspetto predefinito delle immagini.

**Attributi** comuni delle miniature Queste impostazioni interessano l’aspetto e l’allineamento predefiniti delle immagini in miniatura.

**Impostazioni predefinite per i campi** catalogo Queste impostazioni interessano la risoluzione e il tipo predefinito di miniatura delle immagini.

**Attributi** di gestione del colore Queste impostazioni determinano quali profili colore ICC vengono utilizzati.

**Attributi** di compatibilità Questa impostazione consente ai paragrafi iniziali e finali nei livelli di testo di essere trattati come nella versione 3.6 per garantire la compatibilità con le versioni precedenti.

**Supporto** per la localizzazione Queste impostazioni consentono di gestire più attributi della lingua. Consentono inoltre di specificare una stringa di mappa lingua in modo da definire le lingue da supportare per le descrizioni comandi nei visualizzatori.

Ad esempio, se fate parte di una società multinazionale che vende in diversi paesi, potete mettere a punto un visualizzatore localizzato specifico per ciascun paese. A questo scopo, dovete innanzi tutto specificare una stringa di mappa lingua. Quindi, modificate il testo della descrizione comando nel predefinito del visualizzatore aggiungendo le stringhe di testo tradotte per la lingua desiderata.

>[!NOTE]
> Per impostare le opzioni di supporto per la localizzazione, [utilizzate il Admin Console  per creare un caso di supporto.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Nel caso di assistenza, richiedi aiuto.

Per ulteriori informazioni sull’impostazione del **supporto per la localizzazione**, consultate [Considerazioni per l’impostazione della localizzazione delle risorse](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considerazioni per l’impostazione della localizzazione delle risorse {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Per impostare le opzioni di supporto per la localizzazione in Dynamic Media Classic, ad esempio il campo Mappa lingua, [usate l’Admin Console  per creare un caso di supporto.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Nel caso di assistenza, richiedi aiuto.

Un modo comune di utilizzare Dynamic Media Classic consiste nel gestire le immagini dei prodotti sui siti Web di e-commerce. Le aziende internazionali devono poter gestire risorse per prodotti simili ma diverse da paese a paese. In genere si tratta di poche differenze per una piccola parte dei contenuti multimediali. La gestione di tali differenze copiando tutte le risorse per ciascuno dei paesi e sostituendo solo quelle differenti richiede molto lavoro e contraddice il concetto di singola risorsa master. Le differenze nelle risorse possono spaziare da video specifici per i singoli paesi con tracce audio distinte, a cavi elettrici diversi da usare con un prodotto. Dynamic Media Classic utilizza un meccanismo di ricerca di base. Potete definire l’ordine di suffissi per risorse che il server immagini deve seguire per le ricerche, a partire dalla lingua richiesta.

**Come vengono localizzate le risorse**

La lingua per una richiesta IS (Image Serving) è identificata con il seguente comando IS/IR (Image Rendering):

`locale=`

Questo comando accetta una stringa di ID della lingua (locid) che non fa distinzione tra maiuscole e minuscole. L’ID della lingua è in genere una stringa di 2-6 caratteri composta di lettere e trattino basso (_).

IS supports arbitrary printable ASCII strings.The `locale=` command has a global scope, meaning that it is applied to the entire request, including all nested IS and IR requests, referenced templates, and image layers. Non sono supportate più lingue per richiesta, ad esempio una lingua diversa per ciascun livello. Tuttavia, è possibile consentire sostituzioni esplicite nelle richieste nidificate.

If `locale=` is not specified, `attribute::DefaultLocale` is passed to the translation engines. Limited input validation is applied to the `locale=` value. Empty `locale=` values are permitted. Because `locale=` has a global scope, `attribute::DefaultLocale` is provided by the main catalog for the entire request.

Some of the benefits of using `locale=` and `attribute::DefaultLocale` include the following:

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
| Set di immagini e set di file multimediali | L’intero set di immagini può essere diverso per alcune impostazioni internazionali, ad esempio quando un eCatalog è completamente diverso, con la traduzione da set di immagini generico a set specifico per una lingua gestita dal visualizzatore.Più frequentemente, i singoli ID di un set generico possono fare riferimento a contenuti localizzati. Ad esempio, la maggior parte delle foto di un apparecchio saranno uguali per tutte le lingue, eccetto la foto del pannello di controllo. IS traduce automaticamente gli ID e non è quindi necessario generare set di immagini specifici per le diverse lingue. |

**Implementazione della localizzazione delle risorse**

Dynamic Media Classic e Image Server dispongono di un&#39;interfaccia che consente la localizzazione di immagini e contenuti statici.

Senza localizzazione, un URL di Image Server si presenta come segue:

`https://server/is/image/company/image`

With localization, an Image Server URL adds the `locale=` parameter to the path, as in the following:

`https://server/is/image/company/image?locale=de_DE`

On receipt of the http call by the Image Server, the `locale=` parameter is parsed through the localeMap field found in **Setup** > **Application Setup** > **Publish Setup** > **Image Server** > **Localization Support** group.

Il campo Mappa lingua contiene un elenco di voci separate con il simbolo di barra verticale (|).

Ogni voce è un elenco di valori separati da virgola. The first value is the search value that is passed by the `locale=` parameter. I valori rimanenti sono valori di suffisso/sostituzione che vengono provati in successione finché uno corrisponde a un’immagine esistente.

L’applicazione del valore di suffisso o di sostituzione dipende dall’impostazione Lingua globale in **Configurazione** > **Impostazione applicazione** > **Configurazione pubblicazione** > **Image Server** > **Supporto per la localizzazione**.

>[!NOTE]
>
>Al momento l&#39;impostazione Lingua globale è possibile solo se l&#39;impostazione avviene tramite l&#39;API, non tramite l&#39;interfaccia Dynamic Media Classic.

**Esempio di suffisso**

| URL | ID di Mappa lingua | Risultato |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Osservate che non è definita alcuna lingua globale. Il parametro di lingua de_DE viene associato alla prima voce nella Mappa lingua. Il primo valore corrispondente _DE viene aggiunto come suffisso alla risorsa image_DE che viene ricercata in Image Server e, se trovata, viene restituita. In caso contrario, viene utilizzato come suffisso il secondo valore “” e viene restituita l’immagine stessa. |

**Esempio di sostituzione**

| URL | Lingua globale e ID di Mappa lingua | Risultato |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | In questo esempio di sostituzione, il parametro della lingua globale GlobalLocale è impostato su main. Il parametro di lingua de_DE viene associato alla prima voce nella Mappa lingua. La sottostringa GlobalLocale viene trovata e sostituita con il primo valore corrispondente “de” nella Mappa lingua: image-de-01. Se questo viene trovato in Image Server, viene restituito. In caso contrario, viene sostituito il secondo valore e si ottiene image-main-01. |

Se nell’URL non viene specificata alcuna lingua, Image Server applica all’URL la lingua predefinita, se questa è definita.

If an unknown or empty locale parameter is supplied with `locale=`, then the localeMap is scanned for the empty value “starting with,”. È importante configurare questo parametro affinché una lingua predefinita possa essere applicata alle lingue sconosciute.

**Informazioni defaultImage**

Image Server prova in successione le opzioni per la lingua richiesta. Se non viene trovata alcuna corrispondenza, le opzioni della lingua vengono applicate all’immagine predefinita defaultImage e viene restituita la versione corrispondente. Pertanto, ciascuna impostazione internazionale deve includere un’opzione per l’immagine senza localizzazione, oppure le versioni localizzate di defaultImage devono essere rese disponibili in Dynamic Media Classic.

**Scenari per l’individuazione della Mappa lingua**

Supponiamo che si intendano supportare le seguenti lingue:

`en, en_us, en_uk, de, de_at, de_de, fr`

You map these locales to the suffixes `_E`, `_G`, and `_F`, for English, German, and French, respectively. Per tutti gli esempi, l’ID di immagine di input generico è `myImg`.

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

You could also have a dedicated locSuffix, such as U, just for unknown locales, and force to the default image if no `_U` exists, as in the following:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Oppure, potete impostare la mappatura direttamente sull’ID generico:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*Individuare la Mappa lingua con una ricerca a più livelli*

Spesso è utile raggruppare le lingue in base a gruppi che condividono uno stesso standard, ad esempio tre diversi tipo di interfaccia per Europa, Medio Oriente e Nord America. A questo scopo si può ricorrere alla ricerca a più livelli.

In questo esempio, supponiamo di voler supportare raccolte diverse per gli utenti nei paesi occidentali (Western) e mediorientali (Middle Eastern). Entrambe le raccolte sono basate sulla raccolta di immagini generica e per entrambe alcune immagini sono aggiunte o modificate. Both collections are then further refined for specific locales, such as `m1, m2` for two middle-eastern variants, and `w1, w2,` and `w3` for three Western locales, except that images are shared for `w1` and `w3`. Le lingue sconosciute sono associate solo alla raccolta generica e non hanno accesso alle immagini per lingue specifiche. Esempio della mappa:

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

Using the first example as a basis, images for all languages may have the suffixes `_1`, `_2`, or `_3`. Images that are specific to French locales may have the suffixes `_22` or `_23` suffix. And images that are specific to German locales may have the suffixes `_470` or `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | ID di output per la ricerca |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Tutti gli altri | myImg_1, myImg_2, myImg_3 |

**Considerazioni importanti per l’implementazione del supporto per la localizzazione**

* La localizzazione è limitata alle chiamate per risorse basate su ID e non può essere utilizzata per le chiamate per risorse basate su percorso. Di conseguenza, quando si chiama un video con una specifica lingua, questo deve essere chiamato perché come società/ID risorsa e non come percorso completo del video. Non potete pertanto utilizzare RTMP con la localizzazione poiché questo supporta solo le chiamate video basate su percorso.
* Quando l’opzione Mappa lingua è attiva, non è possibile utilizzare un set di file multimediali diversi contenente un singolo video, poiché tale chiamata avrebbe esito negativo. Per risolvere questo inconveniente è possibile aggiungere un singolo video a un set di video adattivi. Quindi, aggiungete il set di video adattivi al set di file multimediali diversi.
* Alcune richieste non sono localizzate. Questo è il caso ad esempio delle richieste per i contenuti dei set di video adattivi. Per poter utilizzare i set di video adattivi con la localizzazione è pertanto necessario inserirli all’interno di un set di file multimediali diversi. Then, call the set into a Mixed Media viewer with the `locale=` parameter.

## Modulo di rendering immagini {#image-renderer}

La schermata Modulo di rendering immagini consente di definire le impostazioni predefinite per la distribuzione di set di immagini dai server di rendering. Sono disponibili impostazioni nelle cinque categorie indicate di seguito (consultate la schermata Server immagini per una descrizione dettagliata delle impostazioni):

**Gestione** catalogo Queste impostazioni determinano il modo in cui Dynamic Media Classic e il file del catalogo interagiscono. Le chiamate URL del server di rendering Dynamic Media Classic vengono effettuate al catalogo, che a sua volta richiama per distribuire le immagini dal server. Modificate queste impostazioni solo con l’assistenza di un addetto al supporto per Dynamic Media Classic.

**Attributi** di sessione Queste impostazioni specificano i parametri di errore, l&#39;URL per gli URL relativi delle immagini e se è consentita la sovrapposizione degli oggetti.

**Attributi** materiale predefiniti Queste impostazioni specificano le impostazioni predefinite di risoluzione e nitidezza per le immagini.

**Attributi** immagine di risposta Queste impostazioni interessano l&#39;aspetto predefinito delle immagini.

**Attributi** di gestione del colore Queste impostazioni interessano le impostazioni di colore predefinite delle immagini.

## Vignettatura {#vignette}

La schermata Vignettatura contiene impostazioni che specificano l’aspetto predefinito delle vignettature (consultate la schermata per una descrizione dettagliata delle opzioni).
