---
title: Creare un eCatalog
description: Scopri come creare un eCatalog in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 30%

---

# Creazione di un eCatalog {#creating-an-ecatalog}

La creazione di un eCatalog comporta l&#39;ordinamento delle pagine, la scelta del layout di pagina e il collegamento delle pagine mediante il disegno di mappe immagine. Inoltre, richiede l’immissione di dati di rollover e di collegamenti ipertestuali. Se desiderato, potete personalizzare il sommario in modo da presentare agli utenti i nomi delle pagine anziché i numeri di pagina nel visualizzatore dell’eCatalog.

## Creare un eCatalog {#create}

È possibile includere file immagine e PDF nell&#39;eCatalog.

Quando si crea un eCatalog, **[!UICONTROL Pubblica dopo un salvataggio]** influisce sui membri set e set nei modi seguenti:

| Opzione &quot;Pubblica dopo un salvataggio&quot; selezionata prima del salvataggio? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un eCatalog:**

1. Iniziate a creare l’eCatalog mediante una di queste tecniche:

   * **Seleziona prima i file**: nel pannello Sfoglia, seleziona i file e passa a **[!UICONTROL Genera]** > **[!UICONTROL eCatalog]**.

   * **Inizia dalla schermata eCatalog**: vai a **[!UICONTROL Genera]** > **[!UICONTROL eCatalog]**. Seleziona una cartella nella Libreria risorse. Trascinare i file dalla cartella nella scheda Pagine ordine della pagina eCatalog.

     >[!NOTE]
     >
     >per visualizzare gli elementi nella Libreria risorse per nome anziché per miniatura, selezionate l’opzione Nome per Visualizzazione predefinita libreria di risorse in Configurazione personale.

1. Selezionate un layout completo per l’eCatalog. Seleziona **[!UICONTROL 1 immagine]** pagine singole, **[!UICONTROL 2 Su]** per pagine affiancate doppie, oppure **[!UICONTROL Personalizzato]** per pagine affiancate con più di due pagine. In **[!UICONTROL Modifica layout eCatalog]** , selezionare la **[!UICONTROL Tutti gli spread]** opzioni e seleziona **[!UICONTROL OK]**.
1. Se necessario, modificare il layout di singole pagine o pagine affiancate selezionandole e quindi scegliendo **[!UICONTROL 1 immagine]**, **[!UICONTROL 2 Su]**, o **[!UICONTROL Personalizzato]** pulsante. In **[!UICONTROL Modifica layout eCatalog]** , selezionare la **[!UICONTROL Pagine affiancate selezionate]** opzioni e seleziona **[!UICONTROL OK]**.
1. Riordinate le pagine in base alle necessità utilizzando una delle seguenti tecniche:

   * **Trascinamento**: trascina una pagina o pagine affiancate in una nuova posizione. Una barra verticale indica la posizione in cui la pagina viene spostata.

   * **Pulsante Sposta in**: seleziona una pagina o un set di pagine affiancate, seleziona **[!UICONTROL Sposta in]** e scegli la pagina nel menu che vuoi far apparire prima della pagina.

   * **N. sequenza**: in Vista a elenco, immettere i numeri di pagina nei campi #. sequenza

1. Al termine, vicino all’angolo inferiore destro della pagina, assicurati che **[!UICONTROL Pubblica dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**.
1. Nella finestra di dialogo Salva, selezionate una cartella in cui memorizzare l’eCatalog. Nel campo Nome file immettere il nome del set 360 gradi.
1. Seleziona **[!UICONTROL Salva]**.

   Puoi visualizzare in anteprima l’eCatalog dopo averlo salvato selezionando **[!UICONTROL Anteprima]**.

## Modificare un eCatalog {#editing-an-ecatalog}

Sia che si modifichi un set pubblicato o un set non pubblicato, il **[!UICONTROL Pubblica dopo un salvataggio]** influisce sui membri set e set nei modi seguenti:

| Il set è già pubblicato | Opzione Pubblica dopo un salvataggio selezionata prima di salvare la modifica? | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti mantengono lo stato pubblicato. I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un eCatalog:**

1. Seleziona il rollover dell&#39;eCatalog **[!UICONTROL Modifica]** pulsante.
1. Apportate le modifiche necessarie.
1. Al termine della modifica, vicino all’angolo inferiore destro della pagina, assicurati che **[!UICONTROL Pubblica dopo un salvataggio]** (impostazione predefinita).
1. Seleziona **[!UICONTROL Salva]**, selezionare una cartella di archiviazione, immettere un nome per il set e quindi selezionare **[!UICONTROL Salva]**.

## Eliminare un eCatalog

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (o &quot;figli&quot;) all&#39;interno di quel set non sono interessati; invece, ciascuno di essi mantiene il proprio stato pubblicato o non pubblicato esistente.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un eCatalog:**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più eCatalog.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.

## Personalizzare il sommario {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic fornisce i numeri di pagina predefiniti nell&#39;eCatalog nella scheda Pagine ordine della schermata eCatalog. Per i nomi di pagina personalizzati, potete modificare le etichette di pagina contenute nel sommario. Si consiglia di rinominare la copertina anteriore e quella posteriore. Ad esempio, il frontespizio può contenere il testo &quot;Copertina&quot; e non &quot;Pagina 0-1&quot;.

È possibile creare manualmente un sommario personalizzato per l&#39;eCatalog. In alternativa, è possibile importare i nomi delle pagine da un file CSV (solo Mac) o XML.

>[!NOTE]
>
>Per ripristinare i titoli di pagina predefiniti, nella **[!UICONTROL Ordina pagine]** , seleziona **[!UICONTROL Etichette sommario]** e quindi selezionare **[!UICONTROL Ripristina valori predefiniti (tutti)]**.

### Inserimento manuale dei nomi delle pagine {#manually-entering-page-names}

Immettere manualmente i nomi di pagina uno alla volta nella scheda Ordina pagine della schermata eCatalog. Nel campo del numero di pagina immettere un nome per ogni pagina che si desidera denominare.

### Importa nomi di pagina {#importing-page-names}

L’importazione dei nomi di pagina è consigliata se disponete di un eCatalog con numerose pagine. Potete importare i nomi da un file XML o delimitato da tabulazioni.

L’etichetta del sommario viene memorizzata nel campo Dati utente di un’immagine; formatta questi dati come elenco di `name=<value>` ` pairs separated by two question marks "??" `. Ad esempio, per impostare un&#39;etichetta per un campo sommario denominato `tocEN`, imposta i dati utente dell&#39;immagine su:

`tocEN=&lt;EN_page_label>`

Per impostare etichette separate per i campi sommario denominati `tocEN` e `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Per importare il campo Dati utente in un file delimitato da tabulazioni, includere i dati utente del campo:

| IPSID | Dati utente |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Per importare il campo Dati utente in un file XML, includere l&#39;attributo `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Per importare i nomi di pagina da un file XML o delimitato da tabulazioni, selezionare **[!UICONTROL Etichette sommario]** e seleziona **[!UICONTROL Importa]**. Nella finestra di dialogo Carica metadati, seleziona **[!UICONTROL Sfoglia]**, quindi importare il file CSV (solo Mac) o il file XML che associa ogni pagina a un nome di pagina.
