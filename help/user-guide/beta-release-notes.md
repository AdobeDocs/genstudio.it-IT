---
title: Note sulla versione di Adobe GenStudio for Performance Marketing Beta
description: Scopri le funzioni e i miglioramenti più recenti di Adobe GenStudio for Performance Marketing.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: f56f3733ead0bfcb4f37e10b66577e1ef597b76d
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---

# Note sulla versione di Adobe GenStudio for Performance Marketing Beta

Queste note mettono in evidenza correzioni e miglioramenti significativi apportati ad Adobe GenStudio for Performance Marketing nella settimana che termina il 27 settembre.

## Nuove funzioni e miglioramenti

* GenStudio ora può estrarre informazioni di utenti tipo e prodotti da un PDF caricato e compilare i campi correlati. <!-- GS-3806 -->

* Gli utenti possono ora filtrare [!DNL Content] risorse ed esperienze in base al nome dell&#39;utente che ha caricato la risorsa. <!-- GS-1808 -->

* La sezione [!DNL Additional details] è stata rinominata [!DNL Messaging preferences] nella pagina dei dettagli [!DNL Products]. <!-- GS-5133 5134 -->

* È stato aggiunto un pulsante [!DNL Add persona] alla pagina _Aggiungi il tuo primo utente tipo_. <!-- GS-5132 -->

## Problemi noti

I seguenti problemi noti sono pianificati per la risoluzione nella versione GA di GenStudio for Performance Marketing.

* I modelli possono essere caricati ma non visualizzati. **Soluzione**: carica una risorsa con il campo **[!UICONTROL Campagne]** popolato. Quindi, carica di nuovo il modello. <!-- GS-4815 5650-->

* Gli utenti non possono ritagliare manualmente i metadati dopo averli ridimensionati. <!-- GS-5871 -->

* Gli utenti devono effettuare due volte l’accesso a un account di canale Meta ads quando hanno effettuato anche l’accesso a Facebook. Soluzione alternativa: esci da Facebook prima di accedere a un account di canale Meta ads. <!-- GS-3009 -->

### Ulteriori miglioramenti e problemi risolti

* Sono stati risolti problemi di latenza intermittenti con alcune operazioni di [!DNL Create] Canvas. <!-- GS-5203 -->

* Gli utenti non dovranno più accedere due volte a un account di canale Meta ads quando accedono anche a Facebook. <!-- GS-4806 -->

* La generazione dell’e-mail ora non produce più un messaggio e-mail incompleto. <!-- GS-5209 -->

* La creazione di una campagna nel flusso di lavoro dei modelli ora memorizza gli ID come previsto.  <!-- GS-4923 -->

* Il selettore per più archivi ora elenca gli archivi in ordine alfabetico. <!-- GS-5553 -->

* Sono stati risolti i problemi relativi ai formati di file di esportazione CSV per lingue diverse dall’inglese. <!-- GS-5141 -->

* Gli utenti possono ora fare clic sul pulsante [!DNL Create] _Lavoro recente_ **[!UICONTROL Visualizza tutte le bozze]** durante il caricamento delle bozze. In precedenza, se si faceva clic su questo pulsante prima del caricamento di tutte le bozze, venivano caricate solo alcune bozze e il pulsante **[!UICONTROL Visualizza tutte le bozze]** non era disponibile. <!-- GS-3938 -->

* L&#39;area di lavoro [!DNL Create] visualizza ora il pulsante **[!UICONTROL Visualizza tutte le bozze]** come previsto quando l&#39;area di lavoro visualizza più di quattro bozze. <!-- GS-5588 -->

* La ricerca ora funziona come previsto nella scheda _Attributi_. <!-- GS-5658 -->

* L’animazione Shimmer viene ora ridimensionata correttamente durante il caricamento dell’esperienza. <!-- GS-5574 -->

* Le anteprime delle miniature per le e-mail in più parti ora vengono riprodotte come previsto in [!DNL Content]. <!-- GS-5258 -->

* È stato risolto un problema relativo a Workfront con il pulsante **[!UICONTROL Invia per approvazione]**. <!-- GS-5847 -->

* Sono stati risolti i problemi relativi al caricamento di shimmer nella visualizzazione Lavoro recente di [!DNL Create]. <!-- GS-5589 -->

* L’immissione di un termine di ricerca genera ora una sola chiamata di ricerca, come previsto.  <!-- GS-2999 -->

* È stato corretto il rendering immagini di metadati generati da annunci dopo l’esportazione. <!-- GS-5749 -->

* Il simbolo `%` viene ora visualizzato correttamente nelle impostazioni internazionali DEU, FRA ed ESP quando gli utenti ingrandiscono o riducono le varianti e-mail nell&#39;area di lavoro C[!DNL Create]. <!-- GS-5007 -->

#### Localizzazione

Questa versione include miglioramenti alla localizzazione nell&#39;interfaccia del prodotto, in particolare in [!DNL Create]. I seguenti componenti dell&#39;interfaccia sono stati localizzati: <!-- GS-5295 -->

* Tutte le stringhe nell&#39;area _Prompt_ (titolo parametri, nomi di opzioni del menu a discesa e testo segnaposto prompt) <!-- GS-5027 -->

* Tutte le stringhe nella finestra _Ridimensiona_ per i meta annunci generati in [!DNL Create] <!-- GS-5035 -->

* Tutte le stringhe nell&#39;area _Lavoro recente_ in [!DNL Create] <!-- GS-5037 -->

* Le stringhe di opzione del menu a discesa Marchi, Utenti tipo e Prodotto nell&#39;area Prompt <!-- GS-5293 -->

* La stringa **Zoom per adattarsi allo schermo** visualizzata durante la generazione di e-mail e annunci multimediali <!-- GS-5063 -->

* Formati di data e ora, **Bozza senza titolo** stringa e messaggi di errore nei nomi di annunci e-mail e metadati <!-- GS-5023 5022 5048-->

* La scheda [!DNL Content] _Assets_ visualizza le stringhe e il simbolo di percentuale (%) <!-- GS-4983 4984-->

* Il simbolo di percentuale (%) utilizzato nel tasso di click-through di Approfondimenti > Esperienze <!-- GS-4279 -->

* Messaggio di errore visualizzato quando si verifica un errore di sistema durante la creazione di annunci e-mail o di metadati<!-- GS-5061 -->

* Separatore decimale per la frase &quot;Conteggio parole per frase&quot; nella pagina Dettagli esperienza approfondimenti <!-- GS-4986 -->

* Stringhe nel menu Esporta per un annuncio Meta generato con un modello. <!-- GS-5031 -->

