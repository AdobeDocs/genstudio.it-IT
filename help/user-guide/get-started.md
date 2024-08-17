---
title: Introduzione ad Adobe GenStudio per gli esperti di marketing delle prestazioni
description: Scopri come impostare GenStudio per gli esperti di marketing delle prestazioni per generare nuovi contenuti di marketing allineati al brand.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: c9d09801f0bd3732611b01d4a98cc7ebf38884d7
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 1%

---


# Introduzione ad Adobe GenStudio per gli esperti di marketing delle prestazioni

GenStudio for Performance Marketers è una piattaforma completa per la creazione, la valutazione e la gestione di esperienze di marketing che riflettono e aderiscono alla tua identità del brand.

L’accesso delle parti interessate alle sue numerose funzionalità è controllato da ruoli utente assegnati. Il ruolo utente assegnato determina le attività che è possibile eseguire in GenStudio per gli addetti al marketing delle prestazioni. Un amministratore imposta le autorizzazioni, che sono definite nell’e-mail di benvenuto.

Se sei nuovo a strumenti generativi basati sull&#39;intelligenza artificiale o semplicemente curioso dei principi di base di GenStudio for Performance Marketers, consulta [Concetti](concepts.md) e [Scrivi prompt validi](effective-prompts.md).

## Ruoli utente

La creazione e l’implementazione di campagne di marketing moderne richiede la collaborazione tra le parti interessate con responsabilità e competenze diverse.

Tre tipi di ruoli utente di GenStudio for Performance Marketers supportano questa diversità di ruoli organizzativi. Le autorizzazioni sono personalizzate per ciascuno di questi tipi di utenti e supportano le responsabilità di ogni utente nell’organizzazione di marketing.

**I tre tipi di ruolo utente sono**:

* **I creatori** utilizzano le funzionalità di intelligenza artificiale generativa di GenStudio for Performance Marketers per creare risorse di campagne di marketing, richiedere la revisione e l&#39;approvazione del contenuto e pubblicare bozze approvate di questo contenuto. Tutti gli utenti GensStudio possono accedere e utilizzare una risorsa una volta che il suo creatore l’ha salvata in Content (Contenuto).

* **I collaboratori** sono la gamma più ampia di utenti di GenStudio per Performance Marketer. I collaboratori possono visualizzare e approvare i contenuti e sono una parte essenziale del flusso di lavoro, in modo che i contenuti generati corrispondano alle esigenze e agli standard della tua organizzazione.

* **Gli amministratori di sistema** dispongono del set più ampio di autorizzazioni in GenStudio per gli esperti di marketing delle prestazioni. Gli amministratori di sistema possono aggiungere ed eliminare utenti e contenuti. Gli amministratori eseguono l’attività di onboarding essenziale per stabilire i guardrail fondamentali per la creazione e la distribuzione delle risorse della campagna. Gli amministratori implementano questi guardrail caricando informazioni specifiche per il brand e l&#39;organizzazione come [linee guida per il brand](/help/user-guide/guidelines/overview.md).

>[!NOTE]
>Adobe Prima che a qualsiasi utente vengano assegnati questi ruoli, è necessario designare un amministratore come utente avanzato in Admin Console per eseguire attività di configurazione una tantum. Questo ruolo utente avanzato funziona solo nel contesto di Adobe Admin Console. Non ha alcun ruolo nell’interfaccia della piattaforma GenStudio for Performance Marketers. Non esiste un concetto di utente avanzato nelle assegnazioni di ruolo di GenStudio per gli addetti al marketing delle prestazioni.

### Creatori

**I creatori** dispongono delle autorizzazioni di base necessarie per creare risorse GenStudio per gli esperti di marketing delle prestazioni [!DNL Brands], [!DNL Campaigns] e [!DNL Content]. Possono anche modificare ed eliminare le risorse create. GenStudio per gli esperti di marketing delle prestazioni supporta la creazione rapida di centinaia di contenuti. Questi utenti possono generare frammenti di contenuto o intere esperienze che orchestrano parti discrete di contenuti approvati per soddisfare le esigenze di specifiche campagne di marketing.

I creatori interagiscono con GenStudio per le tecnologie di intelligenza artificiale generative dei professionisti del marketing delle prestazioni tramite _prompt_. L’area dei prompt nell’area di lavoro fornisce gli strumenti per inserire i prompt nel contesto delle linee guida di una campagna specifica. Di conseguenza, la qualità e il successo dei contenuti generati dipendono in parte dalla qualità delle linee guida del brand caricate dalla tua organizzazione e dalla specificità del prompt.

Vedere [Scrivi prompt effettivi](effective-prompts.md).

Nella tabella seguente vengono visualizzate le autorizzazioni di creazione predefinite:

| Funzione obsoleta | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | sì |
| [!DNL Campaigns] | sì | sì | sì | sì |
| [!DNL Content] | sì | sì | sì | sì |
| [!DNL Insights] | può configurare solo ad connectors |    |     | sì |
| [!DNL Personas] | sì | sì | sì | sì |
| [!DNL Products] | sì | sì | sì | sì |
| [!DNL Reviews and approvals] | sì | sì | sì | sì |

### Collaboratori

**I collaboratori** possono visualizzare le risorse in GenStudio per gli addetti al marketing delle prestazioni, ma non crearle, modificarle o eliminarle. I collaboratori includono le parti interessate che sono essenziali per il successo del processo di revisione e approvazione dei contenuti, ma che non devono creare o modificare direttamente i contenuti. Esperti legali e manager dei creatori sono esempi di potenziali collaboratori. I collaboratori di GenStudio for Performance Marketers potrebbero disporre delle autorizzazioni necessarie per creare e visualizzare le risorse in altri prodotti Creative Cloud.

Nella tabella seguente vengono visualizzate le autorizzazioni di collaborazione predefinite:

| Funzione obsoleta | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | sì | sì | sì | sì |
| [!DNL Campaigns] | sì | sì | sì | sì |
| [!DNL Content] | sì | sì | sì | sì |
| [!DNL Insights] | no | no | no | sì |
| [!DNL Personas] | sì | sì | sì | sì |
| [!DNL Products] | sì | sì | sì | sì |
| [!DNL Reviews and approvals] | no | no | no | sì |

### Amministratori

**Gli amministratori** creano e assegnano gli utenti a uno qualsiasi dei ruoli supportati da GenStudio for Performance Marketers. Se necessario, possono assegnare nuove autorizzazioni a singoli creatori o collaboratori. Il loro compito più importante è quello di completare le attività iniziali di onboarding che preparano la tua organizzazione a distribuire GenStudio per gli esperti di marketing delle prestazioni.

Nella tabella seguente vengono visualizzate le autorizzazioni di amministratore di sistema predefinite:

| Funzione obsoleta | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | sì | sì | sì | sì |
| [!DNL Campaigns] | sì | sì | sì | sì |
| [!DNL Content] | sì | sì | sì | sì |
| [!DNL Insights] | sì | sì | sì | sì |
| [!DNL Personas] | sì | sì | sì | sì |
| [!DNL Products] | sì | sì | sì | sì |
| [!DNL Reviews and approvals] | sì | sì | sì | sì |


## Prepara GenStudio per gli esperti di marketing delle prestazioni per generare contenuti

Gli amministratori di sistema preparano l’ambiente GenStudio for Performance Marketers della propria organizzazione affinché i creatori e i collaboratori possano creare le risorse delle campagne. Tali compiti preliminari di configurazione comprendono:

1. [Aggiungi linee guida](./guidelines/overview.md) per [!DNL Brands], [!DNL Products] e [!DNL Personas]. Impostare gli elementi costitutivi chiave dell’identità del marchio della tua organizzazione è un prerequisito essenziale per il lavoro di creatori e collaboratori. Puoi caricare i documenti sulle linee guida del brand o inserire manualmente le informazioni sul brand.
   * **Prepara i documenti sulle linee guida**. Più le linee guida del tuo marchio sono descrittive e complete, migliore sarà l’output. Includi brevi esempi di funzioni che ritieni essenziali per il tuo marchio e aggiungi descrizioni di comportamenti che desideri escludere dalla creazione di contenuti. GenStudio for Performance Marketers estrae informazioni da questi documenti caricati e inizia a creare il tuo marchio. Informazioni quali la voce del brand, il canale e le linee guida per le immagini vengono compilate quando GenStudio for Performance Marketers assembla ciascuna linea guida dai documenti caricati.
   * **Modifica o completa i campi delle linee guida del brand in base alle esigenze**. Le linee guida complete per il marchio costituiscono la base della comprensione del marchio dell&#39;organizzazione da parte degli addetti al marketing delle prestazioni di GenStudio. Una volta che GenStudio for Performance Marketers ha estratto le informazioni necessarie dai documenti delle linee guida del brand, ti viene richiesto di modificare manualmente o completare i campi delle informazioni estratte. Specificare singole aree di interesse per il prodotto per la creazione di contenuto aggiungendo [!DNL Product]. Le linee guida di [!DNL Personas] aiutano a personalizzare la creazione di contenuti per segmenti cliente definiti.

   Anche se l’impostazione delle linee guida per il marchio di un’organizzazione può essere un’azione da intraprendere una tantum, potrebbe essere necessario rivedere e migliorare tali linee guida in base alla volatilità, alla crescita e alle mutevoli circostanze di mercato della tua organizzazione.

1. **[Carica modelli](./content/use-templates.md)**. I modelli forniscono scelte rapide e accelerano la creazione dei contenuti. Un modello contiene funzioni approvate, come intestazioni e piè di pagina, e stabilisce protezioni per la creazione di contenuti. In genere, gli amministratori caricano e gestiscono modelli per la propria organizzazione. I creatori utilizzano i modelli per avviare rapidamente il processo di creazione dei contenuti entro i limiti stabiliti del brand organizzativo.

1. **[Carica risorse approvate](./content/manage-assets.md)**. Le risorse approvate in [!DNL Content] sono disponibili per tutti i creatori di GenStudio for Performance Marketers. È possibile eseguire il seeding di [!DNL Content] con risorse che i creatori possono utilizzare per creare nuove esperienze o risorse.

1. **[Connetti a un account Meta (Facebook)](./insights/connect-channel.md)**. Devi configurare una connessione tra GenStudio for Performance Marketers e gli account social della tua organizzazione per ricevere i dati dalle campagne di marketing, dalle risorse e dalle esperienze attive. [[!DNL Insights]](./insights/overview.md) fornisce gli strumenti per analizzare i dati derivati dal canale.
