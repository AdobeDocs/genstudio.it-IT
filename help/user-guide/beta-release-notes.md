---
title: Adobe GenStudio per le note sulla versione di Beta per gli esperti di prestazioni marketing
description: Scopri le funzioni e i miglioramenti più recenti di Adobe GenStudio per gli esperti di marketing delle prestazioni.
source-git-commit: 16f44baf646d696da3572ac2c17a5efb7c8f7fc6
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---


# Adobe GenStudio per le note sulla versione di Beta per gli esperti di prestazioni marketing

Queste note evidenziano un Adobe GenStudio significativo di correzioni e miglioramenti per gli esperti di marketing delle prestazioni per la settimana che termina il 6 settembre.

## Problemi noti

I seguenti problemi noti sono pianificati per la risoluzione nella versione GA di GenStudio for Performance Marketers.

* Gli editor rilevano occasionalmente un messaggio di errore &quot;Si è verificato un errore&quot; in [!DNL Create Canvas] durante la generazione dell&#39;immagine. **Soluzione**: se l&#39;errore si ripete, l&#39;utente può disconnettersi, quindi accedere nuovamente a GenStudio e rigenerare l&#39;immagine.  <!-- GS-4813 -->

* [!DNL Create Canvas] esegue il rendering delle immagini negli annunci Meta in modo errato. <!-- GS-4864 -->

* Assets senza campagne può essere caricato correttamente in [!DNL Content] ma potrebbe non essere visibile agli utenti. <!-- GS-4815 -->

* Esiste una discrepanza tra le anteprime MetaAds Canvas e le viste esportate. <!-- GS-4492 4401 -->

* Miniature campagna mancanti da [!DNL Insights]. <!-- GS-4648 -->

* Al momento gli utenti possono selezionare risorse di piccole dimensioni che devono essere ridimensionate, ma l’ingrandimento non è supportato. <!-- GS-3131 -->

* Gli utenti devono accedere due volte a un account di canale Meta Ads quando hanno effettuato anche l’accesso a Facebook. **Soluzione**: esci da Facebook prima di accedere a un account Meta Ads del canale.

### Risoluzione dei problemi noti

* GenStudio visualizza un errore quando un utente tenta di immettere le credenziali nella visualizzazione [!DNL Insights]. (risolto il 29/8) <!-- GS-4689 -->

## Versioni precedenti di Beta

Le versioni precedenti di Beta includevano i seguenti elementi di rilievo e correzioni.

### In evidenza

* **Punteggio di convalida basato su percentuale**: la convalida del brand visualizza ora il punteggio di convalida del brand come percentuale anziché come valore di esito positivo/negativo. (fisso 8/16)

* **Interfaccia di estrazione del marchio aggiornata**: l&#39;estrazione del marchio ora mostra il completamento del processo di estrazione come percentuale. (fisso 8/16)

* **Carico incrementale del brand durante l&#39;estrazione**: le linee guida per il brand ora vengono caricate in modo incrementale nell&#39;interfaccia utente. (fisso 8/16)

* **Creazione di e-mail con più sezioni**: gli utenti possono ora creare e-mail composte da elementi distinti per titolo, immagine, corpo e CTA. (fisso 8/16)

* **Ridimensionamento dei metadati**: gli editor possono ridimensionare le proporzioni dei metadati. (fisso 8/16)

* **Account di accesso Approfondimenti limitati**: l&#39;accesso Approfondimenti ora supporta un solo account per cliente. (fisso 8/16)

### Ulteriori miglioramenti e problemi risolti

* Il nome del posizionamento del feed di pagina _Dettagli esperienza_ ora specifica il feed di Facebook o Instagram. (fisso 8/16)

* Il ritaglio di immagini e video di dimensioni maggiori è ora coerente quando l&#39;utente passa dalla visualizzazione _Panoramica risorse_ alla visualizzazione _Dettagli risorse_. (fisso 8/16)

* Il conteggio dei risultati della ricerca nella schermata Attributi non visualizza più `0 of` prima che un utente effettui l&#39;accesso. (corretto 8/16) <!-- GS-3665 -->

* Facendo clic sul campo di conteggio **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Risorsa]** non si cancellano più le impostazioni di ricerca e filtro. (corretto 8/16) <!-- GS-3476 -->

### Problemi noti risolti nelle precedenti versioni di Beta

* Il caricamento delle linee guida per il marchio non riesce a causa di problemi con la piattaforma di storage ACP. (risolto il 22/8) <!-- GS-4369 -->

* Il menu a discesa dell&#39;area dei prompt [!DNL Brands] visualizza un elemento spinner alla fine dell&#39;elenco [!DNL Brands] durante la creazione dell&#39;e-mail. (risolto il 22/8) <!-- GS-4077 -->

