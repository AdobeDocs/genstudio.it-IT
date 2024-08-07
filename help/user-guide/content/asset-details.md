---
title: Dettagli risorsa
description: GenStudio archivia i contenuti approvati con metadati avanzati per la ricerca e il tracciamento delle prestazioni.
feature: Attributes, Assets
source-git-commit: ba7dced9e62f797cd43a0bd8d8263828ec5c3d5e
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 1%

---


# Dettagli risorsa

GenStudio archivia i contenuti approvati con metadati avanzati per il discovery e il tracciamento delle prestazioni.

A ogni risorsa (inclusi esperienze e modelli) sono associati _dettagli_ (metadati) che consentono di identificare, tenere traccia, utilizzare e apprendere dalle prestazioni dei contenuti.

I tipi di metadati delle risorse includono [metadati di sistema](#system-metadata) e [metadati definiti dall&#39;utente](#user-defined-metadata).

## Metadati di sistema

Alcuni metadati di risorse vengono raccolti automaticamente quando una risorsa viene caricata. Non è possibile modificare i metadati di sistema predefiniti.

I metadati predefiniti memorizzati e acquisiti per una risorsa includono il nome del file, le dimensioni, l’origine e altro ancora.

### Tag generati

Quando le risorse vengono approvate e memorizzate in [!DNL Content], GenStudio utilizza le funzionalità di intelligenza artificiale e machine learning di Adobe per generare tag in base alle funzioni delle risorse, ad esempio colore e tono, oppure parole chiave che identificano le funzioni delle risorse. Non è possibile modificare i tag.

### Metadati del contenuto generato

Le informazioni utilizzate per generare una nuova risorsa o esperienza diventano metadati, ad esempio il prompt utilizzato. Non è possibile modificare la richiesta dopo l’approvazione del contenuto, ma è possibile utilizzarla come punto di partenza per la generazione di qualcosa di nuovo.

## Metadati definiti dall&#39;utente

I metadati definiti dall’utente aggiungono un contesto di marketing al contenuto della risorsa, consentendo agli addetti al marketing di comprendere meglio come utilizzarla e interagire con essa.

Quando [carichi una risorsa](/help/user-guide/content/manage-assets.md#add-assets), puoi definire un set di dettagli facoltativi della risorsa presenti in GenStudio come metadati.

### Dettagli metadati

La tabella seguente descrive i metadati (dettagli risorsa) che puoi definire durante la creazione di una risorsa.

| Campo | Descrizione | Modificabile | Obbligatorio |
| ------------- | ----------- | -------- | -------- |
| Nome campagna (nome progetto) | Metadati predefiniti acquisiti e memorizzati con la risorsa | Y | N |
| Marchio | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) aggiunto a GenStudio e pubblicato per l&#39;utilizzo | Y | N |
| Prodotti | [[!DNL Products]](/help/user-guide/guidelines/products.md) aggiunti a GenStudio per l&#39;utilizzo | Y | N |
| Persone | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) aggiunti a GenStudio per l&#39;utilizzo | Y | N |
| Canali | Tipi di contenuto in GenStudio per cui viene utilizzata la risorsa, ad esempio e-mail e annunci Meta | Y | N |
| Intervallo temporale | Intervallo temporale per il quale la risorsa è stata utilizzata, ad esempio trimestre, stagione, anno e così via. Esempio: `Winter 2023` | Y | N |
| Regione | Aree per le quali viene utilizzata la risorsa. Esempi: `North America`, `APAC`, `Italy` | Y | N |
| Lingua | Lingue per cui viene utilizzata la risorsa. Esempio: `Spanish` | Y | N |
| Parole chiave | Parole chiave utilizzate per identificare lo scopo della risorsa | Y | N |

## Visualizza dettagli risorsa

**Per visualizzare i dettagli della risorsa**:

1. In _[!DNL Content]_, seleziona una risorsa.

1. Nella visualizzazione delle risorse, controlla la sezione _[!UICONTROL Dettagli]_ a destra.

   Se la sezione _[!UICONTROL Dettagli]_ non è visibile, fare clic sull&#39;icona **[!UICONTROL Informazioni]** (i).

>[!TIP]
>
>Puoi visualizzare i dettagli della risorsa anche da [!DNL Insights]. Insights fornisce statistiche di utilizzo e contesto delle prestazioni per le diverse esperienze. In _[!DNL Insights]_, selezionare la sezione **[!UICONTROL Assets]**.

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
