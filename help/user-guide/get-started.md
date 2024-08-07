---
title: Introduzione a GenStudio
description: Scopri come configurare il GenStudio per generare nuovi contenuti di marketing allineati al brand.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 2501d1e36f76d1534a735b9147fb42f762a665e8
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 1%

---


# Introduzione a GenStudio

GenStudio è una piattaforma completa per la creazione, la valutazione e la gestione di esperienze di marketing che riflettono e aderiscono alla tua brand identity.

L’accesso delle parti interessate alle sue numerose funzionalità è controllato da ruoli utente assegnati. Il ruolo utente assegnato determina le attività eseguibili in GenStudio. Un amministratore di GenStudio imposta le tue autorizzazioni, che sono definite nel messaggio e-mail di benvenuto.

Se sei nuovo a strumenti generativi basati sull&#39;intelligenza artificiale o semplicemente curioso dei principi di base di GenStudio, consulta [Concetti di GenStudio](concepts.md) e [Scrivi prompt efficaci](effective-prompts.md).

## Ruoli utente di GenStudio

La creazione e l’implementazione di campagne di marketing moderne richiede la collaborazione tra le parti interessate con responsabilità e competenze diverse.

Tre tipi di ruoli utente di GenStudio supportano questa diversità di ruoli organizzativi. Le autorizzazioni sono personalizzate per ciascuno di questi tipi di utenti e supportano le responsabilità di ogni utente nell’organizzazione di marketing.

**I tre tipi di ruolo utente sono**:

* **I creatori** utilizzano le funzionalità di intelligenza artificiale generativa di GenStudio per creare risorse di campagne di marketing, richiedere la revisione e l&#39;approvazione del contenuto e pubblicare bozze approvate di questo contenuto. Tutti gli utenti GensStudio possono accedere e utilizzare una risorsa una volta che il suo creatore l’ha salvata in Content (Contenuto).

* **I collaboratori** sono la gamma più ampia di utenti di GenStudio. I collaboratori possono visualizzare e approvare i contenuti GenStudio e sono una parte essenziale del flusso di lavoro per garantire che i contenuti generati corrispondano alle esigenze e agli standard della tua organizzazione.

* **Gli amministratori di sistema** dispongono del set più ampio di autorizzazioni in GenStudio. Gli amministratori di sistema possono aggiungere ed eliminare utenti e contenuti da Genstudio. Gli amministratori eseguono l’attività di onboarding essenziale per stabilire i guardrail fondamentali per la creazione e la distribuzione delle risorse della campagna. Gli amministratori implementano questi guardrail caricando informazioni specifiche per il brand e l&#39;organizzazione come [linee guida per il brand](/help/user-guide/guidelines/overview.md).

>[!NOTE]
>Adobe Prima che a qualsiasi utente vengano assegnati questi ruoli, è necessario designare un amministratore come utente avanzato in Admin Console per eseguire attività di configurazione una tantum. Questo ruolo utente avanzato funziona solo nel contesto di Adobe Admin Console. Non ha alcun ruolo nell’interfaccia della piattaforma GenStudio. Non esiste alcun concetto di utente avanzato nelle assegnazioni dei ruoli di GenStudio.

### Creatori

**I creatori** dispongono delle autorizzazioni di base necessarie per creare risorse GenStudio [!DNL Brands], [!DNL Campaigns] e [!DNL Content]. Possono anche modificare ed eliminare le risorse create. GenStudio supporta la creazione rapida di centinaia di contenuti. Questi utenti possono generare frammenti di contenuto o intere esperienze che orchestrano parti discrete di contenuti approvati per soddisfare le esigenze di specifiche campagne di marketing.

I creatori interagiscono con le tecnologie di intelligenza artificiale generative di GenStudio tramite _prompt_. L’area dei prompt di GenStudio nell’area di lavoro offre gli strumenti per inserire i prompt nel contesto delle linee guida di una campagna specifica. Di conseguenza, la qualità e il successo dei contenuti generati dipendono in parte dalla qualità delle linee guida del brand caricate dalla tua organizzazione e dalla specificità del prompt.

Vedere [Scrivi prompt effettivi](effective-prompts.md).

Nella tabella seguente vengono visualizzate le autorizzazioni predefinite di GenStudio Creator:

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

**I collaboratori** possono visualizzare le risorse in GenStudio ma non crearle, modificarle o eliminarle. I collaboratori includono le parti interessate che sono essenziali per il successo del processo di revisione e approvazione dei contenuti GenStudio, ma che non devono creare o modificare direttamente i contenuti. Esperti legali e manager dei creatori sono esempi di potenziali collaboratori. I collaboratori GenStudio potrebbero disporre delle autorizzazioni per creare e visualizzare le risorse in altri prodotti Creative Cloud.

Nella tabella seguente vengono visualizzate le autorizzazioni predefinite di GenStudio Collaborator:

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

Gli utenti amministratori creano e assegnano gli utenti a uno qualsiasi dei ruoli supportati da GenStudio. Se necessario, possono assegnare nuove autorizzazioni a singoli creatori o collaboratori. Il loro compito più importante è quello di completare le attività iniziali di onboarding che preparano la tua organizzazione all’implementazione di GenStudio.

Nella tabella seguente vengono visualizzate le autorizzazioni predefinite per l&#39;amministratore di sistema di GenStudio:

| Funzione obsoleta | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | sì | sì | sì | sì |
| [!DNL Campaigns] | sì | sì | sì | sì |
| [!DNL Content] | sì | sì | sì | sì |
| [!DNL Insights] | sì | sì | sì | sì |
| [!DNL Personas] | sì | sì | sì | sì |
| [!DNL Products] | sì | sì | sì | sì |
| [!DNL Reviews and approvals] | sì | sì | sì | sì |


## Preparare GenStudio per generare il contenuto

Gli amministratori di sistema preparano l’ambiente GenStudio della propria organizzazione affinché i creatori e i collaboratori creino risorse per le campagne. Tali compiti preliminari di configurazione comprendono:

1. [Imposta linee guida](./guidelines/overview.md) per [!DNL Brands], [!DNL Products] e [!DNL Personas]. Impostazione dei blocchi predefiniti chiave del marchio **[Aggiungi linee guida](./guidelines/overview.md)** ([!DNL Brands], [!DNL Products] e [!DNL Personas]) a GenStudio. Impostare gli elementi costitutivi chiave dell&#39;identità del marchio dell&#39;organizzazione è un prerequisito essenziale per il lavoro dei creatori e dei collaboratori di GenStudio. Puoi caricare i documenti sulle linee guida del brand o inserire manualmente le informazioni sul brand.
   * **Prepara i documenti sulle linee guida**. Maggiore è la descrizione e la completezza delle linee guida per il marchio, migliore sarà l&#39;output di GenStudio. Includi brevi esempi di funzioni che ritieni essenziali per il tuo marchio e aggiungi descrizioni di comportamenti che desideri escludere dalla creazione di contenuti GenStudio. GenStudio estrae informazioni da questi documenti caricati e inizia a creare il tuo marchio. Informazioni quali la voce del brand, il canale e le linee guida per le immagini vengono compilate man mano che GenStudio assembla ciascuna linea guida dai documenti caricati.
   * **Modifica o completa i campi delle linee guida del brand in base alle esigenze**. Le linee guida complete per il marchio sono alla base della conoscenza che GenStudio ha del marchio della tua organizzazione. Dopo aver estratto le informazioni necessarie dai documenti delle linee guida per il brand, GenStudio ti chiede di modificare manualmente o completare i campi delle informazioni estratte. Specificare singole aree di interesse per il prodotto per la creazione di contenuto aggiungendo [!DNL Product]. Le linee guida di [!DNL Personas] aiutano a personalizzare la creazione di contenuti per segmenti cliente definiti.

   Anche se l’impostazione delle linee guida per il marchio di un’organizzazione può essere un’azione da intraprendere una tantum, potrebbe essere necessario rivedere e migliorare tali linee guida in base alla volatilità, alla crescita e alle mutevoli circostanze di mercato della tua organizzazione.

1. **[Carica modelli](./content/use-templates.md)**. I modelli forniscono scelte rapide e accelerano la creazione dei contenuti. Un modello contiene funzioni approvate, come intestazioni e piè di pagina, e stabilisce protezioni per la creazione di contenuti. In genere, gli amministratori caricano e gestiscono modelli per la propria organizzazione. I creatori utilizzano i modelli per avviare rapidamente il processo di creazione dei contenuti entro i limiti stabiliti del brand organizzativo.

1. **[Carica risorse approvate](./content/manage-assets.md)**. Le risorse approvate in GenStudio [!DNL Content] sono disponibili per tutti i creatori di GenStudio. È possibile eseguire il seeding di [!DNL Content] con risorse che i creatori possono utilizzare per creare nuove esperienze o risorse.

1. **[Connetti a un account Meta (Facebook)](./insights/connect-channel.md)**. Devi configurare una connessione tra GenStudio e gli account social della tua organizzazione per ricevere dati dalle campagne di marketing, dalle risorse e dalle esperienze attive. In GenStudio [Insights](./insights/overview.md) sono disponibili strumenti per l&#39;analisi dei dati derivati dal canale.
