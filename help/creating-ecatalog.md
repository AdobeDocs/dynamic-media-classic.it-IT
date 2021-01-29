---
title: Creazione di un eCatalog
description: Scoprite come creare un eCatalog.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 78%

---


# Creazione di un eCatalog{#creating-an-ecatalog}

Quando si crea un eCatalog occorre ordinare le pagine, scegliere il layout delle pagine e collegare le pagine tracciando delle mappe immagine e inserendo i dati necessari per rollover e collegamenti ipertestuali. Se desiderato, potete personalizzare il sommario in modo da presentare agli utenti i nomi delle pagine anziché i numeri di pagina nel visualizzatore dell’eCatalog.

## Creazione di un eCatalog  {#create}

In un eCatalog potete includere file di immagini e file PDF.

Quando create un eCatalog, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un eCatalog**

1. Iniziate a creare l’eCatalog mediante una di queste tecniche:

   **Selezionate** prima i fileNel pannello Sfoglia, selezionate i file e fate clic su Genera > eCatalog.

   **Iniziate dalla** schermata eCatalogFate clic su Genera > eCatalog. Selezionate una cartella nella Libreria risorse e trascinate i file da tale cartella alla scheda Ordina pagine della pagina eCatalog.

   ***nota**: Per visualizzare gli elementi nella Libreria risorse per nome invece della miniatura, selezionate l’opzione Nome per Visualizzazione predefinita libreria di risorse in Configurazione personale. *

1. Selezionate un layout completo per l’eCatalog. Per ottenere pagine singole, fate clic sul pulsante 1 immagine ; per disporre le pagine in coppie di pagine affiancate, fate clic su 2 immagini ; per disporle come più pagine affiancate, fate clic sul pulsante Personalizzato . Viene visualizzata la finestra di dialogo Modifica layout eCatalog. Selezionate le opzioni Tutte le pagine affiancate e fate clic su **OK**.
1. Se necessario, potete impostare un diverso layout per pagine singole e affiancate selezionandole e scegliendo il pulsante 1 immagine, 2 immagini o Personalizzato. Viene visualizzata la finestra di dialogo Modifica layout eCatalog. Selezionate le opzioni Pagine affiancate selezionate e fate clic su **OK**.
1. Riordinate le pagine in base alle necessità utilizzando una delle seguenti tecniche:

   **** TrascinamentoTrascinare una pagina o un set di pagine affiancate in una nuova posizione. Una barra verticale indica la posizione in cui la pagina viene spostata.

   **Pulsante Sposta a:** consente di selezionare una pagina o un set di pagine affiancate, fare clic sul pulsante Sposta a e scegliere la pagina dal menu che si desidera visualizzare prima della pagina.

   **Sequenza #** In List View, immettere i numeri di pagina nei campi Sequenza #.

1. Al termine dell’operazione, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **Salva**.
1. Nella finestra di dialogo Salva, selezionate una cartella in cui memorizzare l’eCatalog. Nel campo Nome file, digitate il nome del set.
1. Fate clic su **Salva**.

   Per visualizzare l’anteprima dell’eCatalog, dopo averlo salvato, fate clic su **Anteprima**.

## Modifica di un eCatalog  {#editing-an-ecatalog}

A seconda se modificate un set pubblicato o non pubblicato, l’opzione **Pubblica dopo il salvataggio** incide su set e relativi membri nei seguenti modi:

| Il set è già pubblicato | Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio delle modifiche | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
|--- |--- |--- |--- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il proprio stato di pubblicazione. Tutti i nuovi membri del set aggiunti durante la modifica conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un eCatalog**

1. Fate clic sul pulsante rollover **Modifica** dell’eCatalog.
1. Apportate le modifiche necessarie.
1. Al termine dell’operazione di modifica, verificate che l’opzione **Pubblica dopo il salvataggio** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Fate clic su **Salva**, selezionate una cartella di archiviazione, immettete un nome per il set e fate clic su **Salva**.

## Eliminazione di un eCatalog  {#deleting-an-ecatalog}

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un eCatalog**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più eCatalog.
1. Nella barra di navigazione globale, fate clic su **File** > **Elimina** > **Elimina**.

## Personalizzazione del sommario  {#customizing-the-table-of-contents-toc}

Dynamic Media Classic fornisce numeri di pagina predefiniti nell’eCatalog nella scheda Ordina pagine della schermata eCatalog. Per i nomi di pagina personalizzati, potete modificare le etichette di pagina contenute nel sommario. Si consiglia di rinominare la copertina anteriore e quella posteriore. Ad esempio, la copertina anteriore può essere &quot;Copertina&quot; invece di &quot;Pagina 0-1&quot;.

Potete creare un sommario personalizzato per l’eCatalog manualmente oppure importando i nomi di pagina da un file CSV (solo Mac) o XML.

>[!NOTE]
>
>per reimpostare i titoli di pagina predefiniti, selezionate Etichette di sommario nella scheda Ordina pagine e scegliete Ripristina titoli predefiniti (Tutto).

### Inserimento manuale dei nomi delle pagine  {#manually-entering-page-names}

Per inserire manualmente i nomi delle pagine uno alla volta, aprite la scheda Ordina pagine della schermata eCatalog. Fate clic nel campo relativo al numero di pagina e inserite un nome. Inserite un nome per ogni pagina che desiderate denominare.

### Importazione di nomi di pagina  {#importing-page-names}

L’importazione dei nomi di pagina è consigliata se disponete di un eCatalog con numerose pagine. Potete importare i nomi da un file XML o delimitato da tabulazioni.

L’etichetta del sommario è memorizzata nel campo Dati utente di un’immagine; formattate questi dati come un elenco di `name=<value>` ` pairs separated by two question marks “??” `. Ad esempio, per impostare un’etichetta per un campo di sommario denominato tocEN &quot;, impostate i dati utente dell’immagine su:

tocEN=&lt;etichetta_pagina_EN>

Per impostare etichette diverse per i campi di sommario denominati tocEN e tocFR:

tocEN=&lt;etichetta_pagina_EN>??tocFR=&lt;etichetta_pagina_FR>

Per importare il campo Dati utente in un file delimitato da tabulazioni, includete i dati utente del campo:

| IPSID | Dati utente |
|--- |--- |
| `<image_IPS_ID>` | tocEN=&lt;etichetta_pagina_EN>??tocFR=&lt;etichetta_pagina_FR> |

Per importare il campo Dati utente in un file XML, includete l’attributo `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Per importare nomi di pagina da un file XML o delimitato da tabulazioni, fate clic sul pulsante Etichette di sommario e scegliete Importa. Viene visualizzata la finestra di dialogo Carica metadati. Fate clic sul pulsante Sfoglia e importate il file CSV (solo Mac) o XML che consente di associare ciascuna pagina a un nome di pagina. 
