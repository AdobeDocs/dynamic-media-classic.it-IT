---
title: Configurazione pubblicazione
description: Le impostazioni di Impostazione pubblicazione consentono di determinare il modo in cui le risorse vengono consegnate per impostazione predefinita dai server Adobe Dynamic Media Classic ai siti Web o alle applicazioni.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
topic: Administration, Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '2383'
ht-degree: 30%

---

# Configurazione pubblicazione {#publish-setup}

Le impostazioni della pagina Impostazione pubblicazione determinano il modo in cui le risorse vengono consegnate per impostazione predefinita dai server Adobe Dynamic Media Classic ai siti Web o alle applicazioni. Se non viene specificata alcuna impostazione, il server Adobe Dynamic Media Classic distribuisce una risorsa in base a un’impostazione predefinita in una pagina Impostazione pubblicazione. Ad esempio, una richiesta di consegna di un&#39;immagine che non include un attributo di risoluzione restituisce un&#39;immagine con l&#39;impostazione Default Object Resolution (Risoluzione oggetto predefinita) nella pagina Image Server.

Gli amministratori possono modificare le impostazioni predefinite nelle pagine Image Server, Image Renderer e Vignettatura per definire le impostazioni predefinite per la consegna delle risorse dai server.

Per aprire le pagine di Impostazione pubblicazione, vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Configurazione applicazione]** > **[!UICONTROL Impostazione pubblicazione]**.

>[!NOTE]
>
>Le pagine di Impostazione pubblicazione sono destinate all&#39;utilizzo da parte di sviluppatori e programmatori esperti di siti Web. Adobe Dynamic Media Classic presuppone che gli utenti che modificano le impostazioni su queste pagine abbiano familiarità con Adobe Dynamic Media Classic, gli standard e le convenzioni del protocollo HTTP e la tecnologia di imaging di base.

## Image Server {#image-server}

La pagina Image Server stabilisce le impostazioni predefinite per la consegna di immagini dai server immagini. Le impostazioni sono disponibili in queste cinque categorie (per una descrizione dettagliata delle impostazioni, consultate la pagina Image Server).

Modificare queste impostazioni solo con l&#39;assistenza di un responsabile del supporto Adobe Dynamic Media Classic.

* **[!UICONTROL Gestione catalogo]**: queste impostazioni determinano il modo in cui Adobe Dynamic Media Classic e il catalogo interagiscono. A differenza della maggior parte dei server Web, le chiamate URL del server immagini Dynamic Media vanno a un file manifesto o catalogo anziché a un file immagine propriamente detto. Il file catalogo (da non confondere con un eCatalog) contiene un elenco di tutti i contenuti pubblicati sul server immagini. Contiene anche il percorso di ogni immagine. Se disponete di un ID Digimarc, inserite i vostri dati nella sezione Informazioni utente Digimarc.

* **[!UICONTROL Attributi richiesta]**: queste impostazioni impongono limiti alle immagini che possono essere consegnate dal server. Ad esempio, il *massimo* **[!UICONTROL limite dimensioni immagine di risposta]** è **[!UICONTROL larghezza]** 5000 e **[!UICONTROL altezza]** 5000.

* **[!UICONTROL Attributi di richiesta predefiniti]**: queste impostazioni riguardano l&#39;aspetto predefinito delle immagini.

* **[!UICONTROL Attributi miniatura comuni]**: queste impostazioni riguardano l&#39;aspetto e l&#39;allineamento predefiniti delle immagini miniatura.

* **[!UICONTROL Impostazioni predefinite per i campi catalogo]**: queste impostazioni riguardano la risoluzione e il tipo di miniatura predefinito delle immagini.

* **[!UICONTROL Attributi gestione colore]**: queste impostazioni determinano quali profili colore ICC vengono utilizzati.

* **[!UICONTROL Attributi di compatibilità]**: questa impostazione consente ai paragrafi iniziali e finali nei livelli di testo di essere trattati come nella versione 3.6 per compatibilità con le versioni precedenti.

* **[!UICONTROL Supporto localizzazione]**: queste impostazioni consentono di gestire più attributi delle impostazioni internazionali. Consentono inoltre di specificare una stringa di mappa lingua in modo da definire le lingue da supportare per le descrizioni comandi nei visualizzatori.

  Ad esempio, se fate parte di una società multinazionale che vende in diversi paesi, potete mettere a punto un visualizzatore localizzato specifico per ciascun paese. A questo scopo, dovete innanzi tutto specificare una stringa di mappa lingua. Quindi modifichi il testo della descrizione comando nel predefinito di un Visualizzatore. È sufficiente aggiungere le stringhe di testo tradotte per la lingua desiderata.

  >[!NOTE]
  > Per impostare le opzioni di supporto per la localizzazione, [ utilizza Admin Console per creare un caso di supporto.](https://helpx.adobe.com/it/enterprise/using/support-for-experience-cloud.html) Nel tuo caso di supporto, richiedi assistenza per la configurazione.

  Per ulteriori informazioni sull’impostazione del **[!UICONTROL supporto per la localizzazione]**, consultate [Considerazioni per l’impostazione della localizzazione delle risorse](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considerazioni per l’impostazione della localizzazione delle risorse {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Se si desidera impostare le opzioni di supporto per la localizzazione in Adobe Dynamic Media Classic, ad esempio il campo Mappa lingua, [utilizzare Admin Console per creare un caso di supporto.](https://helpx.adobe.com/it/enterprise/using/support-for-experience-cloud.html) Nel tuo caso di supporto, richiedi assistenza per la configurazione.

Un modo comune per utilizzare Adobe Dynamic Media Classic è quello di gestire le immagini del prodotto sui siti web e-Commerce. Le aziende internazionali devono poter gestire risorse per prodotti simili ma diverse da paese a paese. Di solito le differenze sono per alcune parti del media generale. Affrontare queste differenze copiando tutte le risorse per ciascuno dei paesi e sovrascrivere solo le differenze è uno sforzo tremendo e contraddice la singola metafora della risorsa primaria. Le differenze nelle risorse possono spaziare da video specifici per i singoli paesi con tracce audio distinte, a cavi elettrici diversi da usare con un prodotto. Adobe Dynamic Media Classic utilizza un meccanismo di ricerca di base. Potete definire l’ordine di suffissi per risorse che il server immagini deve seguire per le ricerche, a partire dalla lingua richiesta.

#### Come vengono localizzate le risorse

La lingua per una richiesta IS (Image Serving) è identificata con il seguente comando IS/IR (Image Rendering):

`locale=`

Questo comando accetta una stringa di ID delle impostazioni internazionali (locId) che non distingue tra maiuscole e minuscole. L&#39;ID delle impostazioni locali è in genere una stringa di 2-6 caratteri composta da lettere e &quot;`_`&quot;.

IS supporta stringhe ASCII stampabili arbitrarie. Il comando `locale=` ha un ambito globale, ovvero viene applicato all&#39;intera richiesta, incluse tutte le richieste IS e IR nidificate, i modelli di riferimento e i livelli immagine. Non sono supportate più lingue per richiesta, ad esempio una lingua diversa per ciascun livello. Tuttavia, è possibile consentire sostituzioni esplicite nelle richieste nidificate.

Se `locale=` non è specificato, `attribute::DefaultLocale` viene passato ai motori di traduzione. Al valore `locale=` viene applicata una convalida di input limitata. Sono consentiti `locale=` valori vuoti. Poiché `locale=` ha un ambito globale, `attribute::DefaultLocale` viene fornito dal catalogo principale per l&#39;intera richiesta.

Alcuni dei vantaggi dell&#39;utilizzo di `locale=` e `attribute::DefaultLocale` includono:

* Condivisione di contenuti per più lingue
* Accesso a contenuti specifici in base alla lingua con ID generici
* Flessibilità nelle convenzioni di denominazione e nella gestione dei contenuti in base alla lingua, ad esempio prefisso o suffisso oppure contenuti specifici in base alla lingue in un catalogo a parte
* Supporta l’accesso a versioni specifiche per le impostazioni internazionali.
* Gli oggetti aggregati, ad esempio i set di immagini, possono talvolta contenere riferimenti generici a contenuti potenzialmente specifici delle impostazioni internazionali.
* Supporta tutti i contenuti gestiti dai cataloghi che richiedono la localizzazione, inclusi immagini, set di immagini, vignettature, materiali e record di configurazione del visualizzatore.
* Riduzione al minimo delle modifiche da apportare ai meccanismi del database IPS e del manifesto IS
* Quando si implementa RFC IS-63, viene aggiunto il supporto per contenuti statici come video e interfacce.
* La lingua predefinita è configurabile.

#### Scenari di applicazione

| Applicazione | Scenario |
| --- | --- |
| Localizzazione visualizzatore | Dopo aver implementato i cataloghi di contenuto statico, la localizzazione viene controllata interamente con il parametro locale=, aggiunto a tutte le richieste effettuate a IS. I record di configurazione, le interface, le schermate iniziali e così via possono disporre o meno di varianti in base alla lingua. Il contenuto corretto viene fornito da IS e non è necessario che l’utente sappia quali contenuti sono localizzati e i relativi ID. |
| Immagini e video | Le multinazionali utilizzano spesso una combinazione di contenuti generici e specifici per lingua. Un riferimento a un’immagine o un video può quindi essere generico e, se disponibile, IS ne fornisce la versione localizzata. |
| Set di immagini e set di file multimediali | L’intero set di immagini può essere diverso per alcune impostazioni internazionali, ad esempio quando un eCatalog è diverso, con la traduzione da un set di immagini generico a uno specifico per le impostazioni internazionali gestito dal visualizzatore. Più comunemente, i singoli ID in un set generico possono fare riferimento a contenuti localizzati. Ad esempio, la maggior parte delle foto di un accessorio può essere la stessa in tutte le lingue, ad eccezione della foto del Pannello di controllo Campaign. IS traduce automaticamente gli ID, quindi non è necessario generare set di immagini specifici per le impostazioni internazionali. |

#### Implementare la localizzazione delle risorse

Adobe Dynamic Media Classic e Image Server dispongono di un&#39;interfaccia che consente la localizzazione di immagini e contenuti statici.

Senza localizzazione, un URL di Image Server si presenta come segue:

`https://server/is/image/company/image`

Con la localizzazione, un URL del server immagini aggiunge il parametro `locale=` al percorso, come illustrato di seguito:

`https://server/is/image/company/image?locale=de_DE`

Al ricevimento della chiamata http da parte del server immagini, il parametro `locale=` viene analizzato attraverso il campo `localeMap` trovato nel gruppo **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Localization Support]**.

Il campo Mappa lingua contiene un elenco di voci separate con il simbolo di barra verticale (|).

Ogni voce è un elenco di valori separati da virgola. Il primo valore è il valore di ricerca passato attraverso il parametro `locale=`. I valori rimanenti sono valori di suffisso/sostituzione che vengono quindi provati finché non si ottiene un&#39;immagine esistente.

L’applicazione del valore di suffisso o di sostituzione dipende dall’impostazione Lingua globale in **[!UICONTROL Configurazione]** > **[!UICONTROL Impostazione applicazione]** > **[!UICONTROL Configurazione pubblicazione]** > **[!UICONTROL Image Server]** > **[!UICONTROL Supporto per la localizzazione]**.

>[!NOTE]
>
>L’impostazione Global Locale (Impostazioni internazionali globali) è possibile solo se impostata tramite l’API, non all’interno dell’interfaccia di Adobe Dynamic Media Classic.

**Esempio di suffisso:**

| URL | ID di Mappa lingua | Risultato | Note |
| --- | --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,` | `fr_FR,_FR,` | Osservate che non è definita alcuna lingua globale. Il parametro locale de_DE corrisponde alla prima voce in `localeMap`. Il primo valore corrispondente _DE viene aggiunto come suffisso alla risorsa image_DE e si tenta di trovarla sul server immagini. Se trovato sul server, viene restituito. In caso contrario, viene utilizzato il secondo valore &quot;&quot; come suffisso, causando la restituzione dell’immagine stessa. |

**Esempio di sostituzione:**

| URL | `GlobalLocale` e `localeMap` ID | Risultato | Note |
| --- | --- | --- | --- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main` | `fr_FR,fr,main` | Nell&#39;esempio di sostituzione precedente, GlobalLocale è impostato su main. Il parametro locale de_DE corrisponde alla prima voce in `localeMap`. La sottostringa GlobalLocale è stata trovata e sostituita con il primo valore corrispondente `de` in `localeMap`: `image-de-01`. Se trovato sul server immagini, viene restituito. In caso contrario, viene sostituito il secondo valore, con conseguente `image-main-01`. |

Se nell’URL non viene specificata alcuna lingua, Image Server applica all’URL la lingua predefinita, se questa è definita.

Se con `locale=` viene fornito un parametro delle impostazioni locali sconosciuto o vuoto, `localeMap` verrà analizzato per individuare il valore vuoto &quot;a partire da&quot;. È importante applicare una lingua predefinita per le lingue sconosciute.

#### Informazioni su defaultImage

Image Server prova in successione le opzioni per la lingua richiesta. Se non viene trovata alcuna corrispondenza, le opzioni internazionali vengono applicate a defaultImage e viene restituita la versione corrispondente. Di conseguenza, ogni lingua deve includere un&#39;opzione per l&#39;immagine senza localizzazione oppure le versioni localizzate predefinite dell&#39;immagine sono disponibili in Adobe Dynamic Media Classic.

#### Scenari per trovare la mappa delle impostazioni locali

Supponiamo che si intendano supportare le seguenti lingue:

`en, en_us, en_uk, de, de_at, de_de, fr`

È possibile mappare queste impostazioni internazionali ai suffissi `_E` (inglese), `_G` (tedesco) e `_F` (francese). Per tutti gli esempi, l&#39;ID immagine di input generico è `myImg`.

##### Comportamento standard per la ricerca di localmap

Gli ID delle lingue vengono mappati sui suffissi corrispondenti. Se nel catalogo non viene trovato alcun ID per una lingua, viene provato l’ID generico. Osserva i valori locSuffix vuoti mappati all’ID generico.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | ID di output per la ricerca |
| --- | --- |
| en, en_us, en_uk | myImg_E, myImg |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Tutti gli altri | : |

##### Ricerca di localeMap quando la lingua è sconosciuta

Potete associare le lingue sconosciute a ID specifici o generici. Ad esempio, puoi mappare le lingue sconosciute agli ID inglesi, o se non esistono, agli ID generici.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | ID di output per la ricerca |
| --- | --- |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Tutti gli altri | myImg_E, myImg |

È inoltre possibile disporre di un locSuffix dedicato, ad esempio U, solo per le impostazioni internazionali sconosciute e forzare l&#39;utilizzo dell&#39;immagine predefinita se non esiste `_U`, come illustrato di seguito:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Oppure, potete impostare la mappatura direttamente sull’ID generico:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### Trovare la mappa delle impostazioni locali utilizzando una ricerca su più livelli

Spesso è utile raggruppare le lingue in base a gruppi che condividono uno stesso standard, ad esempio tre diversi tipo di interfaccia per Europa, Medio Oriente e Nord America. A questo scopo si può ricorrere alla ricerca a più livelli.

Ad esempio, supponiamo che tu voglia supportare raccolte per uso occidentale e mediorientale. Entrambe le raccolte sono basate sulla raccolta di immagini generica e per entrambe alcune immagini sono aggiunte o modificate. Entrambe le raccolte vengono quindi ulteriormente perfezionate per specifiche impostazioni internazionali. Ad esempio, `m1, m2` per due varianti mediorientali e `w1, w2,` e `w3` per tre lingue occidentali, ad eccezione delle immagini condivise per `w1` e `w3`. Le lingue sconosciute sono associate solo alla raccolta generica e non hanno accesso alle immagini per lingue specifiche. Esempio della mappa:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | ID di output per la ricerca |
| --- | --- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Tutti gli altri | mylmg |

##### Trovare la mappa delle impostazioni locali cercando ID specifici

Alcune convenzioni di denominazione delle immagini non supportano ID immagine generici. Gli ID generici da questa richiesta devono essere associati a un ID specifico nel catalogo. Tuttavia, in alcuni casi l’ID specifico esatto non è noto.

Utilizzando il primo esempio come base, le immagini per tutte le lingue potrebbero avere i suffissi `_1`, `_2` o `_3`. Le immagini specifiche delle lingue francesi potrebbero avere il suffisso `_22` o `_23`. E le immagini specifiche delle lingue tedesche potrebbero avere i suffissi `_470` o `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | ID di output per la ricerca |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Tutti gli altri | myImg_1, myImg_2, myImg_3 |

##### Considerazioni importanti durante l’implementazione del supporto per la localizzazione

* La localizzazione è limitata alle chiamate per risorse basate su ID e non può essere utilizzata per le chiamate per risorse basate su percorso. Di conseguenza, quando si chiama un video con una specifica lingua, questo deve essere chiamato perché come società/ID risorsa e non come percorso completo del video. Impossibile utilizzare `RTMP` con la localizzazione perché questo metodo è solo per le videochiamate basate su percorsi.
* Quando l’opzione Mappa lingua è attiva, non è possibile utilizzare un set di file multimediali diversi contenente un singolo video, poiché tale chiamata avrebbe esito negativo. Per risolvere questo problema, puoi aggiungere un singolo video a un set di video adattivi. Quindi, aggiungete il set di video adattivi al set di file multimediali diversi.
* Alcune richieste non sono localizzate. Questo è il caso ad esempio delle richieste per i contenuti dei set di video adattivi. Pertanto, se intendi utilizzare i set video adattivi con localizzazione, inseriscili all’interno di un set di file multimediali diversi. Quindi, chiama il set in un visualizzatore di file multimediali diversi con il parametro `locale=`.

## Modulo di rendering immagini {#image-renderer}

La pagina Image Renderer stabilisce le impostazioni predefinite per la distribuzione di set di immagini dai server di rendering delle immagini. Le impostazioni sono disponibili in queste cinque categorie (consulta la pagina Image Server per una descrizione dettagliata delle impostazioni):

* **[!UICONTROL Gestione catalogo]**: queste impostazioni determinano il modo in cui Adobe Dynamic Media Classic e il file di catalogo interagiscono. Le chiamate URL del server di rendering di Adobe Dynamic Media Classic vengono effettuate al catalogo, che a sua volta chiama per inviare immagini dal server. Modificare queste impostazioni solo con l&#39;assistenza di un responsabile del supporto Adobe Dynamic Media Classic.

* **[!UICONTROL Attributi sessione]**: queste impostazioni stabiliscono i parametri di errore, l&#39;URL per gli URL relativi dell&#39;immagine e se è consentita la sovrapposizione degli oggetti.

* **[!UICONTROL Attributi del materiale predefiniti]**: queste impostazioni stabiliscono le impostazioni predefinite per la risoluzione e la nitidezza delle immagini.

* **[!UICONTROL Attributi immagine di risposta]**: queste impostazioni riguardano l&#39;aspetto predefinito delle immagini.

* **[!UICONTROL Attributi gestione colore]**: queste impostazioni si riferiscono alle impostazioni colore predefinite delle immagini.

## Vignettatura {#vignette}

La pagina Vignettatura offre le impostazioni per definire l&#39;aspetto predefinito delle vignettature (per una descrizione dettagliata delle opzioni, vedere la pagina stessa).
