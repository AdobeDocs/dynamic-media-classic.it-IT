---
title: Creazione di un eCatalog
seo-title: Creazione di un eCatalog
description: 'null'
seo-description: Scoprite come creare un ecatalog.
uuid: 2 aff 05 c 2-7052-426 c-b 61 d -7 f 9091 f 7 ace 8
contentOwner: admin
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/category/ecatalogs
discoiquuid: 28889 c 60-596 a -40 d 2-85 d 4-f 48 a 4 f 86 b 932
translation-type: tm+mt
source-git-commit: 1941567db5c154620bb0dcd12e363d7eebc61b20

---


# Creazione di un eCatalog{#creating-an-ecatalog}

Quando si crea un eCatalog occorre ordinare le pagine, scegliere il layout delle pagine e collegare le pagine tracciando delle mappe immagine e inserendo i dati necessari per rollover e collegamenti ipertestuali. Se desiderato, potete personalizzare il sommario in modo da presentare agli utenti i nomi delle pagine anziché i numeri di pagina nel visualizzatore dell’eCatalog.

## Creazione di un eCatalog {#create}

In un eCatalog potete includere file di immagini e file PDF.

Quando create un eCatalog, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un eCatalog**

1. Iniziate a creare l’eCatalog mediante una di queste tecniche:

   **Selezionate prima i file** nel pannello Sfoglia, selezionate i file e fate clic su Genera &gt; ecatalog.

   **Iniziate dalla schermata ecatalog** fate clic su Genera &gt; ecatalog. Selezionate una cartella nella Libreria risorse e trascinate i file da tale cartella alla scheda Ordina pagine della pagina eCatalog.

   ***note**: To view the items in the Asset Library by name instead of thumbnail, select the Name option for Default Asset Library View in Personal Setup. *

1. Selezionate un layout completo per l’eCatalog. Per ottenere pagine singole, fate clic sul pulsante 1 immagine ; per disporre le pagine in coppie di pagine affiancate, fate clic su 2 immagini ; per disporle come più pagine affiancate, fate clic sul pulsante Personalizzato . Viene visualizzata la finestra di dialogo Modifica layout eCatalog. Select the All Spreads options and click **OK**.
1. Se necessario, potete impostare un diverso layout per pagine singole e affiancate selezionandole e scegliendo il pulsante 1 immagine, 2 immagini o Personalizzato. Viene visualizzata la finestra di dialogo Modifica layout eCatalog. Select the Selected Spreads options and click **OK**.
1. Riordinate le pagine in base alle necessità utilizzando una delle seguenti tecniche:

   **Trascinare** trascinate una pagina o un set di pagine affiancate in una nuova posizione. Una barra verticale indica la posizione in cui la pagina viene spostata.

   **Sposta a:** selezionate una pagina o un set di pagine affiancate, fate clic sul pulsante Sposta a e scegliete la pagina nel menu da inserire prima della pagina.

   **Sequenza #** In Visualizzazione Elenco, immettete i numeri di pagina nei campi Sequenza #.

1. Al termine dell’operazione, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **Salva**.
1. Nella finestra di dialogo Salva, selezionate una cartella in cui memorizzare l’eCatalog. Nel campo Nome file, digitate il nome del set.
1. Fate clic su **Salva**.

   Per visualizzare l’anteprima dell’eCatalog, dopo averlo salvato, fate clic su **Anteprima**.

## Modifica di un eCatalog {#editing-an-ecatalog}

A seconda se modificate un set pubblicato o non pubblicato, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Il set è già pubblicato | Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio delle modifiche | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono il loro stato pubblicato. Tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione o pubblicazione non pubblicato. |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un eCatalog**

1. Fate clic sul pulsante rollover **Modifica** dell’eCatalog.
1. Apportate le modifiche necessarie.
1. Al termine dell’operazione di modifica, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **Salva**, selezionate una cartella di archiviazione, immettete un nome per il set e fate clic su **Salva**.

## Eliminazione di un eCatalog {#deleting-an-ecatalog}

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un eCatalog**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più eCatalog.
1. Nella barra di navigazione globale, fate clic su **File** &gt; **Elimina** &gt; **Elimina**.

## Personalizzazione del sommario {#customizing-the-table-of-contents-toc}

Dynamic Media Classic fornisce numeri di pagina predefiniti nell'ecatalog nella scheda Ordina pagine della schermata ecatalog. Per i nomi di pagina personalizzati, potete modificare le etichette di pagina contenute nel sommario. Si consiglia di rinominare la copertina anteriore e quella posteriore. Ad esempio, la copertina anteriore può leggere «Copertina» invece di «Pagina 0-1». »»

Potete creare un sommario personalizzato per l’eCatalog manualmente oppure importando i nomi di pagina da un file CSV (solo Mac) o XML.

>[!NOTE]
>
>per reimpostare i titoli di pagina predefiniti, selezionate Etichette di sommario nella scheda Ordina pagine e scegliete Ripristina titoli predefiniti (Tutto).

### Inserimento manuale dei nomi delle pagine {#manually-entering-page-names}

Per inserire manualmente i nomi delle pagine uno alla volta, aprite la scheda Ordina pagine della schermata eCatalog. Fate clic nel campo relativo al numero di pagina e inserite un nome. Inserite un nome per ogni pagina che desiderate denominare.

### Importazione di nomi di pagina {#importing-page-names}

L’importazione dei nomi di pagina è consigliata se disponete di un eCatalog con numerose pagine. Potete importare i nomi da un file XML o delimitato da tabulazioni.

L'etichetta del sommario viene memorizzata nel campo Dati utente di un'immagine; formattare questi dati come elenco `name=<value>`` pairs separated by two question marks “??” `. Ad esempio, per impostare un'etichetta per un campo di sommario denominato tocen ", impostate i Dati utente dell'immagine su:

tocEN=&lt;etichetta_pagina_EN&gt;

Per impostare etichette diverse per i campi di sommario denominati tocEN e tocFR:

tocEN=&lt;etichetta_pagina_EN&gt;??tocFR=&lt;etichetta_pagina_FR&gt;

Per importare il campo Dati utente in un file delimitato da tabulazioni, includete i dati utente del campo:

| IPSID | Dati utente |
|--- |--- |
| `<image_IPS_ID>` | tocEN=&lt;etichetta_pagina_EN&gt;??tocFR=&lt;etichetta_pagina_FR&gt; |

Per importare il campo Dati utente in un file XML, includete l’attributo `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Per importare nomi di pagina da un file XML o delimitato da tabulazioni, fate clic sul pulsante Etichette di sommario e scegliete Importa. Viene visualizzata la finestra di dialogo Carica metadati. Fate clic sul pulsante Sfoglia e importate il file CSV (solo Mac) o XML che consente di associare ciascuna pagina a un nome di pagina. 
