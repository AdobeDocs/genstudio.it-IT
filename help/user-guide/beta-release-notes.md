---
title: Adobe GenStudio per le note sulla versione di Beta per gli esperti di prestazioni marketing
description: Scopri le funzioni e i miglioramenti più recenti di Adobe GenStudio per gli esperti di marketing delle prestazioni.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 2e40260db0f9972675b103c51f09acbfa83a1cb5
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 0%

---

# Adobe GenStudio per le note sulla versione di Beta per gli esperti di prestazioni marketing

Queste note evidenziano un Adobe GenStudio significativo di correzioni e miglioramenti per gli esperti di marketing delle prestazioni per la settimana che termina il 6 settembre.

## Nuove funzioni

* GenStudio ora supporta l&#39;opzione per visualizzare in anteprima le risorse multimediali nelle viste di [!DNL Insights] tabelle e raccolte. Le miniature video includono un pulsante **Riproduci** con un&#39;opzione di disattivazione audio. <!-- GS-4398 -->

## Problemi noti

I seguenti problemi noti sono pianificati per la risoluzione nella versione GA di GenStudio for Performance Marketers.

* Gli editor rilevano occasionalmente un messaggio di errore &quot;Si è verificato un errore&quot; in [!DNL Create Canvas] durante la generazione dell&#39;immagine. **Soluzione**: se l&#39;errore si ripete, l&#39;utente può disconnettersi, quindi accedere nuovamente a GenStudio e rigenerare l&#39;immagine.  <!-- GS-4813 -->

* [!DNL Create Canvas] esegue il rendering delle immagini negli annunci Meta in modo errato. <!-- GS-4864 -->

* Assets senza campagne può essere caricato correttamente in [!DNL Content] ma potrebbe non essere visibile agli utenti. <!-- GS-4815 -->

* Esiste una discrepanza tra le anteprime MetaAds Canvas e le viste esportate. <!-- GS-4492 4401 -->

* Miniature campagna mancanti da [!DNL Insights]. <!-- GS-4648 -->

* Al momento gli utenti possono selezionare risorse di piccole dimensioni che devono essere ridimensionate, ma l’ingrandimento non è supportato. <!-- GS-3131 -->

* Gli utenti devono accedere due volte a un account di canale Meta Ads quando hanno effettuato anche l’accesso a Facebook. **Soluzione**: esci da Facebook prima di accedere a un account Meta Ads del canale.

* Le immagini caricate non sempre includono i tag avanzati previsti. <!-- GS-4856 -->

### Ulteriori miglioramenti e problemi risolti

* La finestra a comparsa _Aggiungi Assets_ è ora localizzata come previsto. <!-- GS-3834 -->

* Sono stati risolti i problemi relativi alla scalabilità del modello di esperienza Meta ads. <!-- GS-4174 -->

* I campi di testo nel file di esportazione CSV per le e-mail in più parti ora vengono ordinati come previsto. <!-- GS-4013 -->

* Il campo di ricerca [!DNL Content] non scompare più quando un utente preme ripetutamente il tasto **Backspace** per cancellare il testo del campo di ricerca.  <!-- GS-4543 -->

* GenStudio ora carica gli utenti come previsto quando un collaboratore aggiunge una menzione @ a un commento. In precedenza, GenStudio non caricava gli utenti e visualizzava questo errore: `Unable to load users. Refresh the page`. <!-- GS-4113 -->

* GenStudio non visualizza più il messaggio **Si è verificato un errore** quando un editor fa clic su **Seleziona contenuto** durante la creazione dell&#39;e-mail nell&#39;area dei prompt. <!-- GS-4879 -->

## Versioni precedenti di Beta

Le versioni precedenti di Beta includevano i seguenti elementi di rilievo e correzioni.

### In evidenza

* Le linee guida per i canali Instagram e Facebook sono state unite nelle linee guida per i marchi Meta.

* [!DNL Create] elementi di navigazione dell&#39;area di lavoro sono stati semplificati. Nella pagina di destinazione [!DNL Create] viene visualizzato il pannello di navigazione sinistro, ma gli utenti ora utilizzano un pulsante **[!UICONTROL Indietro]** per passare a questo spazio da altre aree di lavoro [!DNL Create].

* Gli elementi di navigazione sono stati migliorati per supportare l’attenzione degli utenti durante l’esecuzione di attività in tutto il prodotto, incluse queste aree di prodotto:

   * Dettagli risorsa, esperienza e modello in [!DNL Content]
   * Esperienza, risorsa, dettagli attributo in [!DNL Insights]
   * Dettagli marchio in [!DNL Brands]
   * Dettagli del prodotto e della persona in Prodotti e utenti tipo

* Gli utenti non dovranno più fare clic sul pulsante **[!UICONTROL Aggiorna]** per visualizzare gli aggiornamenti alle esperienze in [!DNL Content].

* Nella pagina _Dettagli esperienza_ le miniature delle risorse esterne vengono ora visualizzate come HTML.

* È stata migliorata la latenza dell’interfaccia utente dopo l’aggiunta o l’eliminazione di Assets ed Experience.

* Le anteprime dei modelli ora includono testo predefinito più descrittivo. Vedi [Personalizzare un modello](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/content/templates/customize-template#template-preview).

* **Punteggio di convalida basato su percentuale**: la convalida del brand visualizza ora il punteggio di convalida del brand come percentuale anziché come valore di esito positivo/negativo. (fisso 8/16)

* **Interfaccia di estrazione del marchio aggiornata**: l&#39;estrazione del marchio ora mostra il completamento del processo di estrazione come percentuale. (fisso 8/16)

* **Carico incrementale del brand durante l&#39;estrazione**: le linee guida per il brand ora vengono caricate in modo incrementale nell&#39;interfaccia utente. (fisso 8/16)

* **Creazione di e-mail con più sezioni**: gli utenti possono ora creare e-mail composte da elementi distinti per titolo, immagine, corpo e CTA. (fisso 8/16)

* **Ridimensionamento dei metadati**: gli editor possono ridimensionare le proporzioni dei metadati. (fisso 8/16)

* **Account di accesso limitati [!DNL Insights]**: l&#39;accesso [!DNL Insights] ora supporta un solo account per cliente. (fisso 8/16)

### Ulteriori miglioramenti e problemi risolti

* Il nome del posizionamento del feed di pagina _Dettagli esperienza_ ora specifica il feed di Facebook o Instagram. (fisso 8/16)

* Il ritaglio di immagini e video di dimensioni maggiori è ora coerente quando l&#39;utente passa dalla visualizzazione _Panoramica risorse_ alla visualizzazione _Dettagli risorse_. (fisso 8/16)

* Il conteggio dei risultati della ricerca nella schermata Attributi non visualizza più `0 of` prima che un utente effettui l&#39;accesso. (corretto 8/16) <!-- GS-3665 -->

* Facendo clic sul campo di conteggio **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Risorsa]** non si cancellano più le impostazioni di ricerca e filtro. (corretto 8/16) <!-- GS-3476 -->

### Problemi noti risolti nelle precedenti versioni di Beta

* GenStudio visualizza un errore quando un utente tenta di immettere le credenziali nella visualizzazione [!DNL Insights]. (risolto il 29/8) <!-- GS-4689 -->

* Il caricamento delle linee guida per il marchio non riesce a causa di problemi con la piattaforma di storage ACP. (risolto il 22/8) <!-- GS-4369 -->

* Il menu a discesa dell&#39;area dei prompt [!DNL Brands] visualizza un elemento spinner alla fine dell&#39;elenco [!DNL Brands] durante la creazione dell&#39;e-mail. (risolto il 22/8) <!-- GS-4077 -->
