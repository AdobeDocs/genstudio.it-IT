---
title: Adobe GenStudio per le note sulla versione di Beta per gli esperti di prestazioni marketing
description: Scopri le funzioni e i miglioramenti più recenti di Adobe GenStudio.
source-git-commit: 382026b07e123a1e49813b766f69496f6a8f38eb
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 2%

---


# Adobe GenStudio per le note sulla versione di Beta per gli esperti di prestazioni marketing

Queste note mettono in evidenza importanti correzioni e miglioramenti di Adobe GenStudio per la settimana che termina il 16 agosto.

## In evidenza

Lo sviluppo delle funzioni di GenStudio è rapido e continuo. Le nuove funzioni principali includono:

### Marchio

Il pannello di convalida del marchio è stato migliorato per migliorare l’esperienza utente, con le seguenti modifiche:

* _Punteggio di convalida basato su percentuale_: la convalida del brand visualizza ora il punteggio di convalida del brand come percentuale anziché come valore di esito positivo/negativo.

* _Interfaccia di estrazione del marchio aggiornata_: l&#39;estrazione del marchio ora mostra il completamento del processo di estrazione come percentuale.

* _Carico incrementale del brand durante l&#39;estrazione_: le linee guida per il brand ora vengono caricate in modo incrementale nell&#39;interfaccia utente.

* _Semplificazione dello schema delle linee guida per la copia_: i campi `unique attributes` e `frequent keywords` sono stati rimossi dallo schema delle linee guida per la copia, semplificando il processo di configurazione delle linee guida.

* _Generazione immagine: selezione categoria_: gli utenti possono ora selezionare le linee guida per le immagini specifiche per le proprie esigenze di rigenerazione immagine.

### Creare

* **Creazione di e-mail con più sezioni**: gli utenti possono ora creare e-mail composte da elementi distinti per titolo, immagine, corpo e CTA.

* **Ridimensionamento dei metadati**: i creatori possono ridimensionare le proporzioni dei metadati.

### Approfondimenti

* **Account di accesso Approfondimenti limitati**: l&#39;accesso Approfondimenti ora supporta un solo account per cliente.

## Miglioramenti e problemi risolti

Questa versione include le seguenti correzioni aggiuntive.

### Approfondimenti

* Il nome del posizionamento del feed di pagina _Dettagli esperienza_ ora specifica il feed di Facebook o Instagram.

* Il ritaglio di immagini e video di dimensioni maggiori è ora coerente quando l&#39;utente passa dalla visualizzazione _Panoramica risorse_ alla visualizzazione _Dettagli risorsa_.

* Il conteggio dei risultati della ricerca nella schermata Attributi non visualizza più `0 of` prima che un utente effettui l&#39;accesso. <!-- GS- 3665 -->

* Facendo clic sul campo di conteggio **[!UICONTROL Insight]** > **[!UICONTROL Risorsa]** non si cancellano più le impostazioni di ricerca e filtro. <!-- GS-3476 -->

## Problemi noti

I seguenti problemi noti saranno risolti dalla versione GA di GenStudio for Performance Marketers.

### Analisi

* Le azioni attivate dai pulsanti **[!UICONTROL Aggiungi modelli]** e **[!UICONTROL Carica]** non sono attualmente tracciate. <!-- GS-3505 -->

### Marchio

* Un creatore può pubblicare correttamente un brand, ma i membri dell’organizzazione non possono visualizzarlo. <!-- XI-2197 -->

### Creare

* Il ritaglio delle immagini negli annunci Meta non è coerente. <!-- GS-3739 -->

* I modelli composti da più gruppi di elementi di pagina non superano la convalida del brand. <!-- GS-4037 -->

### Approfondimenti

* Errori di accesso negato si verificano con l&#39;endpoint `/admin/addOffer` (servizio di provisioning). **Risoluzione 8/12**. <!-- GS-4047 -->

* **I valori di spesa a livello di campagna** non sono precisi. Al momento i dati non sono coerenti tra Facebook Ads Manager e il data lake. <!-- GS-3202 -->

### Recensioni e approvazioni

* I creatori possono modificare le risorse dopo l’approvazione prima di pubblicarle. Gli approvatori non ricevono alcuna notifica di queste modifiche.