---
title: Adobe GenStudio per le note sulla versione di Beta per gli esperti di prestazioni marketing
description: Scopri le funzioni e i miglioramenti più recenti di Adobe GenStudio per gli esperti di marketing delle prestazioni.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: d1904bfe6e5775f71290c2fc7aa185ac2a4a4668
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Adobe GenStudio per le note sulla versione di Beta per gli esperti di prestazioni marketing

Queste note evidenziano un Adobe GenStudio significativo di correzioni e miglioramenti per gli esperti di marketing delle prestazioni per la settimana che termina il 13 settembre.

## Miglioramenti

* Il selettore di contenuto [!DNL Create] è stato reimpostato per migliorare il caricamento delle risorse. <!-- GS-2586 -->

## Problemi noti

I seguenti problemi noti sono pianificati per la risoluzione nella versione GA di GenStudio for Performance Marketers.

* Alcuni problemi di latenza intermittenti interessano alcune operazioni di [!DNL Create] Canvas. <!-- GS-5203 -->

* La generazione dell’e-mail restituisce un messaggio e-mail incompleto. **Soluzione**: aggiorna la pagina e rigenera. <!-- GS-5209 -->

* I modelli possono essere caricati ma non visualizzati. **Soluzione**: crea o carica una risorsa e immetti il nome di un gruppo di risorse nel campo **[!UICONTROL Campagne]**. L&#39;assegnazione della risorsa a [!DNL Campaign] aggiunge il valore dei metadati del nome del gruppo. Quindi, carica di nuovo il modello. <!-- GS-4815 -->

* Miniature campagna mancanti da [!DNL Insights]. <!-- GS-4648 -->

* Gli utenti devono accedere due volte a un account di canale Meta Ads quando hanno effettuato anche l’accesso a Facebook. **Soluzione**: esci da Facebook prima di accedere a un account Meta Ads del canale. <!-- GS-4806 -->

### Ulteriori miglioramenti e problemi risolti

* L&#39;area di lavoro [!DNL Create] ora esegue correttamente il rendering delle immagini nei Meta Ads. <!-- GS-4864 -->

* Anche se possono esistere discrepanze tra le anteprime Meta Ads Canvas e le viste esportate, le esperienze esportate funzionano come previsto. <!-- GS-4492 4401 -->

* Le immagini caricate ora includono i tag avanzati previsti. <!-- GS-4856 -->

* Il file CSV di esportazione dei metadati ora contiene le immagini come previsto. In precedenza, il file ZIP conteneva il file di esportazione CSV e i file NULL invece delle immagini.  <!-- GS-5107 -->

* Gli utenti possono ora immettere testo nel campo Dettagli modello **[!UICONTROL Caricato da]** come previsto. In precedenza, l’icona di caricamento impediva agli utenti di immettere testo. <!-- GS-4887 -->

* Una volta eliminato il brand, gli utenti non vengono più reindirizzati alla visualizzazione Dettaglio del brand. <!-- GS-2663 -->

* Gli editor non ricevono più il seguente errore durante l&#39;invio di varianti per la revisione e l&#39;approvazione: `You have no access to view comments on this Object`. <!-- GS-5140 -->

* È stato aggiornato il modello e-mail utilizzato dal flusso di lavoro Revisione e approvazioni. <!-- GS-5239 -->

* GenStudio ora visualizza un messaggio di errore quando si verifica un errore di rete durante il caricamento del selettore di modelli. <!-- GS-4682 -->

* Sono stati risolti dei problemi relativi allo spostamento da una scheda di risorse, esperienza o modelli all’oggetto selezionato. <!-- GS-4390 -->

* Il popup _Aggiungi Assets_ è ora localizzato quando viene aperto da Crea area di lavoro.  <!-- GS-4867 -->

* La convalida del brand ora viene attivata per le varianti rigenerate. In precedenza, se un editor rigenerava varianti di una bozza esistente, la convalida non veniva attivata. <!-- GS-3971 -->

## Versioni precedenti di Beta

Le versioni precedenti di Beta includevano i seguenti elementi di rilievo e correzioni.

### In evidenza

* GenStudio ora supporta l&#39;opzione per visualizzare in anteprima le risorse multimediali nelle viste di [!DNL Insights] tabelle e raccolte. Le miniature video includono un pulsante **Riproduci** con un&#39;opzione di disattivazione audio. <!-- GS-4398 -->

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

* **Ridimensionamento MetaAds**: gli editor possono ridimensionare le proporzioni MetaAds. (fisso 8/16)

* **Account di accesso limitati [!DNL Insights]**: l&#39;accesso [!DNL Insights] ora supporta un solo account per cliente. (fisso 8/16)

### Ulteriori miglioramenti e problemi risolti

* La finestra a comparsa _Aggiungi Assets_ è ora localizzata come previsto. <!-- GS-3834 -->

* Sono stati risolti i problemi relativi alla scalabilità del modello di esperienza Meta ads. <!-- GS-4174 -->

* I campi di testo nel file di esportazione CSV per le e-mail in più parti ora vengono ordinati come previsto. <!-- GS-4013 -->

* Il campo di ricerca [!DNL Content] non scompare più quando un utente preme ripetutamente il tasto **Backspace** per cancellare il testo del campo di ricerca.  <!-- GS-4543 -->

* GenStudio for Performance Marketers ora carica gli utenti come previsto quando un collaboratore aggiunge una menzione `@` a un commento. In precedenza, gli utenti non venivano caricati e veniva visualizzato un errore: `Unable to load users. Refresh the page`. <!-- GS-4113 -->

* GenStudio non visualizza più il messaggio **Si è verificato un errore** quando un editor fa clic su **Seleziona contenuto** durante la creazione dell&#39;e-mail nell&#39;area dei prompt. <!-- GS-4879 -->

* Il nome del posizionamento del feed di pagina _Dettagli esperienza_ ora specifica il feed di Facebook o Instagram. (fisso 8/16)

* Il ritaglio di immagini e video di dimensioni maggiori è ora coerente quando l&#39;utente passa dalla visualizzazione _Panoramica risorse_ alla visualizzazione _Dettagli risorse_. (fisso 8/16)

* Il conteggio dei risultati della ricerca nella schermata Attributi non visualizza più `0 of` prima che un utente effettui l&#39;accesso. (corretto 8/16) <!-- GS-3665 -->

* Facendo clic sul campo di conteggio **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Risorsa]** non si cancellano più le impostazioni di ricerca e filtro. (corretto 8/16) <!-- GS-3476 -->

* GenStudio visualizza un errore quando un utente tenta di immettere le credenziali nella visualizzazione [!DNL Insights]. (risolto il 29/8) <!-- GS-4689 -->

* Il caricamento delle linee guida per il marchio non riesce a causa di problemi con la piattaforma di storage ACP. (risolto il 22/8) <!-- GS-4369 -->

* Il menu a discesa dell&#39;area dei prompt [!DNL Brands] visualizza un elemento spinner alla fine dell&#39;elenco [!DNL Brands] durante la creazione dell&#39;e-mail. (risolto il 22/8) <!-- GS-4077 -->
