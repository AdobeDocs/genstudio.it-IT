---
title: Adobe GenStudio per le note sulla versione di Beta per gli esperti di prestazioni marketing
description: Scopri le funzioni e i miglioramenti più recenti di Adobe GenStudio per gli esperti di marketing delle prestazioni.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 7085fa5a12a6ed36c9310f8f691969d9c1366d36
workflow-type: tm+mt
source-wordcount: '1348'
ht-degree: 0%

---

# Adobe GenStudio per le note sulla versione di Beta per gli esperti di prestazioni marketing

Queste note evidenziano un Adobe GenStudio significativo di correzioni e miglioramenti per gli esperti di marketing delle prestazioni per la settimana che termina il 19 settembre.

## Nuove funzioni e miglioramenti

* **Integrazione con Adobe Experience Manager Assets**. È ora disponibile l’accesso in sola lettura ad Adobe Experience Manager Assets. <!-- GS-2432 -->

* **Miglioramenti al flusso di lavoro Aggiorna modello**.  Gli utenti che aggiornano i modelli ora selezionano il canale per il quale desiderano utilizzare il modello. <!-- GS-4029 -->

* **Prestazioni migliorate per la creazione del caricamento della pagina**. Le dipendenze inutilizzate sono state rimosse dal processo di caricamento della pagina. <!-- GS-3630 -->

* **Supporto e-mail con più sezioni**. Gli editor possono ora generare e-mail contenenti più sezioni e immagini. Possono anche rigenerare frammenti specifici di un’e-mail generata (ad esempio, un titolo). <!-- GS-2436 -->

* **Consente di passare dalla visualizzazione desktop a quella mobile durante la creazione**. Gli utenti possono ora passare dalla visualizzazione desktop a quella mobile per visualizzare in anteprima le varianti di esperienza e-mail. <!-- GS-4314 -->

* Il contenuto ora genera immagini con dimensioni di ritaglio relative alle dimensioni della risorsa originale. <!-- GS-3150 -->

* Ora gli utenti possono selezionare le varianti di immagine generate e utilizzare la funzione Regola ritaglio per ritagliarle durante il flusso di lavoro di creazione. <!-- GS-5538 2342 -->

* La visualizzazione Dettagli di un’esperienza approvata ora mostra una miniatura e lo stato di tutte le risorse a cui si fa riferimento in tale esperienza. <!-- GS-3783 -->

## Problemi noti

I seguenti problemi noti sono pianificati per la risoluzione nella versione GA di GenStudio for Performance Marketers.

* Alcuni problemi di latenza intermittenti interessano alcune operazioni di [!DNL Create] Canvas. <!-- GS-5203 -->

* La generazione dell’e-mail restituisce un messaggio e-mail incompleto. **Soluzione**: aggiorna la pagina e rigenera. <!-- GS-5209 -->

* I modelli possono essere caricati ma non visualizzati. **Soluzione**: carica una risorsa con il campo **[!UICONTROL Campagne]** popolato. Quindi, carica di nuovo il modello. <!-- GS-4815 -->

* Gli utenti devono effettuare due volte l’accesso a un account di canale Meta ads quando hanno effettuato anche l’accesso a Facebook. **Soluzione**: esci da Facebook prima di accedere a un account Meta Ads per il canale. <!-- GS-4806 -->

### Ulteriori miglioramenti e problemi risolti

* Il trascinamento della selezione ora funziona come previsto nell&#39;area del prompt. <!-- GS-3977 -->

* Sono stati risolti i problemi relativi all’utilizzo del tasto TAB per spostarsi tra gli elementi sulla barra di navigazione sinistra. In precedenza, per spostarsi da un elemento all’altro era necessario fare clic.  <!-- GS-2639 -->

* GenStudio ora salva i nomi delle esperienze quando gli utenti modificano il nome durante il caricamento dell’esperienza. <!-- GS-5242 -->

* Ora gli utenti possono modificare correttamente il titolo di un’esperienza. In precedenza, il testo del titolo veniva impostato automaticamente sul testo originale dopo che un utente aveva tentato di modificarlo. <!-- GS-5246 -->
* Le immagini selezionate ora vengono riprodotte nell’area di lavoro come previsto durante la creazione di e-mail in più parti. <!-- GS-5263 -->

* Tutte le stringhe nella pagina dei dettagli Esperienze [!DNL Content] sono ora localizzate. <!-- GS-5016 -->

* Gli utenti possono ora eliminare un prodotto la cui visualizzazione Dettagli è aperta in [!DNL Products]. <!-- GS-5057 -->

* È stato migliorato il messaggio visualizzato in GenStudio quando una ricerca non produce risultati corrispondenti. <!-- GS-4544 -->

* I valori dell&#39;attributo `aria-label` per i valori del filtro di ricerca sono ora tradotti come previsto. <!-- GS-5388 -->

* Gli utenti possono ora eliminare le risorse duplicate nell&#39;area del prompt dell&#39;area di lavoro di [!DNL Create].  <!-- GS-5233 -->

* Il filtro Account ora funziona come previsto con esperienze, risorse e attributi. <!-- GS-4812 -->

* Sono stati risolti i problemi relativi ai caratteri nei metadati e nei modelli di annunci per migliorarne la leggibilità e l’accessibilità. <!-- GS-5354 -->

* Le modifiche ai titoli delle bozze ora persistono come previsto. In precedenza, i titoli venivano ripristinati al nome predefinito dopo la modifica. <!-- GS-2951 -->

#### Correzioni di modelli

* La funzione di ridimensionamento ora funziona come previsto con più immagini nei Meta Ad Template. In precedenza, GenStudio non ridimensionava le immagini per tutti i modelli selezionati. <!-- GS-4696 -->

* L&#39;eliminazione di un modello ora aggiorna la pagina [!DNL Content] come previsto. <!-- GS-5397 -->

* Gli utenti possono ora scegliere i valori per [!DNL Personas], [!DNL Brands] o [!DNL Products] solo dal menu a discesa. In precedenza, la finestra di dialogo _Caricamento modello_ consentiva agli utenti di immettere qualsiasi nome [!DNL Persona], [!DNL Brand] o [!DNL Product]. <!-- GS-5072 5071-->

* Il pulsante **[!UICONTROL Indietro]** è ora disabilitato durante il processo di caricamento del modello. <!-- GS-5358 -->

* Tutte le stringhe nella visualizzazione dei dettagli di [!DNL Create] Select template sono ora localizzate. <!-- GS-5025 -->

## Versioni precedenti di Beta

Le versioni precedenti di Beta includevano i seguenti elementi di rilievo e correzioni.

### In evidenza

* Il selettore di contenuto [!DNL Create] è stato reimpostato per migliorare il caricamento delle risorse. <!-- GS-2586 -->

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

* **Ridimensionamento dei metadati**: gli editor possono ridimensionare le proporzioni dei metadati. (fisso 8/16)

* **Account di accesso limitati [!DNL Insights]**: l&#39;accesso [!DNL Insights] ora supporta un solo account per cliente. (fisso 8/16)

### Ulteriori miglioramenti e problemi risolti

* L&#39;area di lavoro [!DNL Create] ora esegue correttamente il rendering delle immagini negli annunci Meta. (risolto il 13 settembre) <!-- GS-4864 -->

* Anche se possono esistere discrepanze tra le anteprime Meta ads Canvas e le viste esportate, le esperienze esportate funzionano come previsto. (risolto il 13 settembre) <!-- GS-4492 4401 -->

* Le immagini caricate ora includono i tag avanzati previsti. (risolto il 13 settembre) <!-- GS-4856 -->

* Il file CSV di esportazione dei Meta Ads ora contiene le immagini come previsto. In precedenza, il file ZIP conteneva il file di esportazione CSV e i file NULL invece delle immagini. (risolto il 13 settembre) <!-- GS-5107 -->

* Gli utenti possono ora immettere testo nel campo Dettagli modello **[!UICONTROL Caricato da]** come previsto. In precedenza, l’icona di caricamento impediva agli utenti di immettere testo. (risolto il 13 settembre) <!-- GS-4887 -->

* Una volta eliminato il brand, gli utenti non vengono più reindirizzati alla visualizzazione Dettaglio del brand. (risolto il 13 settembre) <!-- GS-2663 -->

* Gli editor non ricevono più il seguente errore durante l&#39;invio di varianti per revisione e approvazione: `You have no access to view comments on this Object`. (risolto il 13 settembre) <!-- GS-5140 -->

* È stato aggiornato il modello e-mail utilizzato dal flusso di lavoro Revisione e approvazioni. (risolto il 13 settembre) <!-- GS-5239 -->

* GenStudio ora visualizza un messaggio di errore quando si verifica un errore di rete durante il caricamento del selettore di modelli. (risolto il 13 settembre) <!-- GS-4682 -->

* Sono stati risolti dei problemi relativi allo spostamento da una scheda di risorse, esperienza o modelli all’oggetto selezionato. (risolto il 13 settembre) <!-- GS-4390 -->

* Il popup _Aggiungi Assets_ è ora localizzato quando viene aperto da Crea area di lavoro. (risolto il 13 settembre) <!-- GS-4867 -->

* La convalida del brand ora viene attivata per le varianti rigenerate. In precedenza, se un editor rigenerava varianti di una bozza esistente, la convalida non veniva attivata. (risolto il 13 settembre) <!-- GS-3971 -->

* La finestra a comparsa _Aggiungi Assets_ è ora localizzata come previsto. (corretto: 9/5) <!-- GS-3834 -->

* Sono stati risolti i problemi relativi alla scalabilità del modello di esperienza Meta ads. (corretto: 9/5) <!-- GS-4174 -->

* I campi di testo nel file di esportazione CSV per le e-mail in più parti ora vengono ordinati come previsto. (corretto: 9/5) <!-- GS-4013 -->

* Il campo di ricerca [!DNL Content] non scompare più quando un utente preme ripetutamente il tasto **Backspace** per cancellare il testo del campo di ricerca. (corretto: 9/5) <!-- GS-4543 -->

* GenStudio for Performance Marketers ora carica gli utenti come previsto quando un collaboratore aggiunge una menzione `@` a un commento. In precedenza, gli utenti non venivano caricati e veniva visualizzato un errore: `Unable to load users. Refresh the page`. (risolto il 29/8) <!-- GS-4113 -->

* GenStudio non visualizza più il messaggio **Si è verificato un errore** quando un editor fa clic su **Seleziona contenuto** durante la creazione dell&#39;e-mail nell&#39;area dei prompt. <!-- GS-4879 -->

* Il nome del posizionamento del feed di pagina _Dettagli esperienza_ ora specifica il feed di Facebook o Instagram. (fisso 8/16)

* Il ritaglio di immagini e video di dimensioni maggiori è ora coerente quando l&#39;utente passa dalla visualizzazione _Panoramica risorse_ alla visualizzazione _Dettagli risorse_. (fisso 8/16)

* Il conteggio dei risultati della ricerca nella schermata Attributi non visualizza più `0 of` prima che un utente effettui l&#39;accesso. (corretto 8/16) <!-- GS-3665 -->

* Facendo clic sul campo di conteggio **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Risorsa]** non si cancellano più le impostazioni di ricerca e filtro. (corretto 8/16) <!-- GS-3476 -->

* GenStudio visualizza un errore quando un utente tenta di immettere le credenziali nella visualizzazione [!DNL Insights]. (risolto il 29/8) <!-- GS-4689 -->

* Il caricamento delle linee guida per il marchio non riesce a causa di problemi con la piattaforma di storage ACP. (risolto il 22/8) <!-- GS-4369 -->

* Il menu a discesa dell&#39;area dei prompt [!DNL Brands] visualizza un elemento spinner alla fine dell&#39;elenco [!DNL Brands] durante la creazione dell&#39;e-mail. (risolto il 22/8) <!-- GS-4077 -->
