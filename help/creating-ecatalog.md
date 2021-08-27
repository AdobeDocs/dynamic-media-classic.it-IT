---
title: Creare un eCatalog
description: Scopri come creare un eCatalog in Adobe Dynamic Media Classic.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 57%

---

# Creazione di un eCatalog {#creating-an-ecatalog}

Quando si crea un eCatalog occorre ordinare le pagine, scegliere il layout delle pagine e collegare le pagine tracciando delle mappe immagine e inserendo i dati necessari per rollover e collegamenti ipertestuali. Se desiderato, potete personalizzare il sommario in modo da presentare agli utenti i nomi delle pagine anziché i numeri di pagina nel visualizzatore dell’eCatalog.

## Creare un eCatalog {#create}

Puoi includere file di immagine e file PDF nel tuo eCatalog.

Quando create un eCatalog, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** incide su set e relativi membri nei seguenti modi:

| Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- |
| Sì | Pubblicato | Pubblicato |
| No | Non pubblicato | I membri del set conservano il proprio stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per creare un eCatalog:**

1. Iniziate a creare l’eCatalog mediante una di queste tecniche:

   * **Seleziona prima i file**  - Nel pannello Sfoglia, seleziona i file e vai a  **[!UICONTROL Genera]**  >  **[!UICONTROL eCatalogs]**.

   * **Inizia dalla schermata**  eCatalog - Vai a  **[!UICONTROL Build]**  >  **[!UICONTROL eCatalogs]**. Selezionate una cartella nella Libreria risorse e trascinate i file da tale cartella alla scheda Ordina pagine della pagina eCatalog.

      >[!NOTE]
      >
      >per visualizzare gli elementi nella Libreria risorse per nome anziché per miniatura, selezionate l’opzione Nome per Visualizzazione predefinita libreria di risorse in Configurazione personale.

1. Selezionate un layout completo per l’eCatalog. Seleziona **[!UICONTROL 1 Su]** per pagine singole, **[!UICONTROL 2 Su]** per pagine affiancate a due pagine oppure **[!UICONTROL Personalizzato]** per pagine affiancate di più di due pagine. Nella finestra di dialogo **[!UICONTROL Modifica layout eCatalog]**, selezionare le opzioni **[!UICONTROL Tutte le pagine affiancate]** e selezionare **[!UICONTROL OK]**.
1. Facoltativamente, modifica il layout delle singole pagine o pagine affiancate selezionandole e scegliendo il pulsante **[!UICONTROL 1 Su]**, **[!UICONTROL 2 Su]** o **[!UICONTROL Personalizzato]**. Nella finestra di dialogo **[!UICONTROL Modifica layout eCatalog]**, selezionare le opzioni **[!UICONTROL Pagine affiancate selezionate]** e selezionare **[!UICONTROL OK]**.
1. Riordinate le pagine in base alle necessità utilizzando una delle seguenti tecniche:

   * **Trascinamento** : consente di trascinare una pagina o un set di pagine affiancate in una nuova posizione. Una barra verticale indica la posizione in cui la pagina viene spostata.

   * **Pulsante Sposta a** : seleziona una pagina o un set di pagine affiancate, seleziona  **[!UICONTROL Sposta a]** e scegli la pagina dal menu che desideri visualizzare in precedenza.

   * **Sequenza #**  - Nella vista a elenco, immettere i numeri di pagina nei campi Sequenza # .

1. Al termine dell’operazione, verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Selezionare **[!UICONTROL Salva]**.
1. Nella finestra di dialogo Salva, selezionate una cartella in cui memorizzare l’eCatalog. Nel campo Nome file, digitate il nome del set.
1. Selezionare **[!UICONTROL Salva]**.

   Puoi visualizzare l&#39;anteprima dell&#39;eCatalog, dopo averlo salvato, selezionando **[!UICONTROL Anteprima]**.

## Modificare un eCatalog {#editing-an-ecatalog}

Sia che modifichi un set pubblicato che un set non pubblicato, l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** influisce sul set e sui membri impostati nei seguenti modi:

| Il set è già pubblicato | Opzione “Pubblica dopo il salvataggio” selezionata prima del salvataggio delle modifiche | Stato del set dopo il salvataggio | Stato dei membri del set dopo il salvataggio |
| --- | --- | --- | --- |
| Sì | Sì | Pubblicato | Pubblicato |
| Sì | No | Pubblicato | I membri del set esistenti conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). I nuovi membri del set aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |
| No | Sì | Pubblicato | Pubblicato |
| No | No | Non pubblicato | I membri del set esistenti e tutti i nuovi membri aggiunti durante la modifica conservano il loro stato di pubblicazione (Pubblicato o Non pubblicato). |

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per modificare un eCatalog:**

1. Seleziona il pulsante rollover dell’eCatalog **[!UICONTROL Modifica]** .
1. Apportate le modifiche necessarie.
1. Al termine dell’operazione di modifica, verificate che l’opzione **[!UICONTROL Pubblica dopo il salvataggio]** nell’angolo in basso a destra della pagina sia selezionata (impostazione predefinita).
1. Selezionare **[!UICONTROL Salva]**, selezionare una cartella di archiviazione, immettere un nome per il set, quindi selezionare **[!UICONTROL Salva]**.

## Eliminare un eCatalog {#deleting-an-ecatalog}

Quando eliminate un set, viene spostato nel cestino. Tuttavia, i membri (“elementi secondari”) all’interno del set non vengono modificati e mantengono il loro attuale stato di pubblicazione.

Consultate anche [Pubblicazione manuale di risorse](publishing-files.md#manually_publishing_assets) e [Annullamento manuale della pubblicazione di risorse](publishing-files.md#manually_unpublishing_assets).

**Per eliminare un eCatalog:**

1. Nelle visualizzazioni Griglia, Elenco o Dettagli, selezionate uno o più eCatalog.
1. Sulla barra di navigazione globale, vai a **[!UICONTROL File]** > **[!UICONTROL Elimina]** > **[!UICONTROL Elimina]**.

## Personalizzare il sommario {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic fornisce i numeri di pagina predefiniti nell&#39;eCatalog nella scheda Pagine ordine della schermata eCatalog. Per i nomi di pagina personalizzati, potete modificare le etichette di pagina contenute nel sommario. Si consiglia di rinominare la copertina anteriore e quella posteriore. Ad esempio, la copertina anteriore può riportare &quot;Copertina&quot; invece di &quot;Pagina 0-1&quot;.

Potete creare un sommario personalizzato per l’eCatalog manualmente oppure importando i nomi di pagina da un file CSV (solo Mac) o XML.

>[!NOTE]
>
>Per ripristinare i titoli di pagina predefiniti, nella scheda **[!UICONTROL Ordina pagine]** selezionare **[!UICONTROL Etichette sommario]**, quindi selezionare **[!UICONTROL Ripristina valori predefiniti (tutti)]**.

### Inserimento manuale dei nomi delle pagine {#manually-entering-page-names}

Per inserire manualmente i nomi delle pagine uno alla volta, aprite la scheda Ordina pagine della schermata eCatalog. Quindi, nel campo del numero di pagina, immettere un nome per ogni pagina che si desidera assegnare.

### Importare nomi di pagina {#importing-page-names}

L’importazione dei nomi di pagina è consigliata se disponete di un eCatalog con numerose pagine. Potete importare i nomi da un file XML o delimitato da tabulazioni.

L’etichetta del sommario viene memorizzata nel campo Dati utente di un’immagine; formatta questi dati come elenco di `name=<value>` ` pairs separated by two question marks “??” `. Ad esempio, per impostare un’etichetta per un campo di sommario denominato `tocEN`, impostate i Dati utente dell’immagine su:

`tocEN=&lt;EN_page_label>`

Per impostare etichette separate per i campi del sommario denominati `tocEN` e `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Per importare il campo Dati utente in un file delimitato da tabulazioni, includere i dati utente del campo:

| IPSID | Dati utente |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Per importare il campo Dati utente in un file XML, includete l’attributo `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Per importare i nomi di pagina da un file XML o delimitato da tabulazioni, selezionare il pulsante **[!UICONTROL Etichette sommario]** e selezionare **[!UICONTROL Importa]**. Nella finestra di dialogo Carica metadati, seleziona **[!UICONTROL Sfoglia]**, quindi importa il file CSV (solo Mac) o XML che associa ogni pagina a un nome di pagina.
