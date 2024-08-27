---
title: Introduzione ad Adobe GenStudio per gli esperti di marketing delle prestazioni
description: Scopri come impostare GenStudio per gli esperti di marketing delle prestazioni per generare nuovi contenuti di marketing allineati al brand.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 869a70c2ccfb965a52f93b4868994188d4d33c24
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 1%

---


# Introduzione ad Adobe GenStudio per gli esperti di marketing delle prestazioni

GenStudio for Performance Marketers è una piattaforma completa per la creazione, la valutazione e la gestione di esperienze di marketing che riflettono e aderiscono alla tua identità del brand.

L&#39;accesso delle parti interessate alle sue numerose funzionalità è controllato da _ruoli utente assegnati_. Il ruolo utente assegnato determina le attività che è possibile eseguire in GenStudio per gli addetti al marketing delle prestazioni. Un amministratore di Adobe assegna le autorizzazioni nel profilo di prodotto GenStudio for Performance Marketers in Adobe Admin Console. L&#39;e-mail di benvenuto identifica il ruolo assegnato.

Se sei un nuovo utente di strumenti generativi basati sull&#39;intelligenza artificiale o sei semplicemente curioso dei principi di base di GenStudio for Performance Marketers, consulta [Concetti](concepts.md) e [Scrivi prompt validi](effective-prompts.md).

## Ruoli utente

La creazione e l’implementazione di campagne di marketing moderne richiede la collaborazione tra le parti interessate con responsabilità e competenze diverse.

Tre tipi di ruoli utente di GenStudio for Performance Marketers supportano questa diversità di ruoli organizzativi. Le autorizzazioni sono personalizzate per ciascuno di questi tipi di utenti e supportano le responsabilità di ogni utente nell’organizzazione di marketing.

**I tre tipi di ruolo utente sono**:

* **Gli editor** utilizzano le funzionalità di intelligenza artificiale generativa di GenStudio for Performance Marketers per creare risorse di campagne di marketing, richiedere la revisione e l&#39;approvazione del contenuto e pubblicare bozze approvate di questo contenuto. Tutti gli utenti di GenStudio possono accedere a una risorsa e utilizzarla dopo che il suo creatore l’ha salvata in Contenuto.

* **I collaboratori** sono la gamma più ampia di utenti di GenStudio per Performance Marketer. I collaboratori possono visualizzare e approvare i contenuti e sono una parte essenziale del flusso di lavoro per garantire che i contenuti generati corrispondano alle esigenze e agli standard della tua organizzazione.

* I **System Manager** dispongono del set più ampio di autorizzazioni in GenStudio per gli esperti di marketing delle prestazioni. I responsabili di sistema eseguono il compito essenziale di onboarding, ovvero stabilire i guardrail fondamentali per la creazione e la distribuzione delle risorse delle campagne. I responsabili di sistema implementano questi guardrail caricando informazioni specifiche per il marchio e l&#39;organizzazione come [linee guida per il marchio](/help/user-guide/guidelines/overview.md). I responsabili di sistema di GenStudio dispongono dell’autorizzazione per la creazione e la pubblicazione di brand, ma non dispongono dei privilegi di amministrazione degli utenti.

>[!NOTE]
>Prima di assegnare questi ruoli a qualsiasi utente, è necessario designare un amministratore di Adobe in Adobe Admin Console per eseguire attività di configurazione una tantum. Questo Adobe di ruolo di amministratore funziona solo nel contesto di Adobe Admin Console. Non ha alcun ruolo nell’interfaccia della piattaforma GenStudio for Performance Marketers.

### Editor GenStudio

**Gli editor** dispongono delle autorizzazioni di base necessarie per creare risorse GenStudio per gli esperti di marketing delle prestazioni [!DNL Brands], [!DNL Campaigns] e [!DNL Content]. Possono anche modificare ed eliminare le risorse create. GenStudio per gli esperti di marketing delle prestazioni supporta la creazione rapida di centinaia di contenuti. Questi utenti possono generare frammenti di contenuto o intere esperienze che orchestrano parti discrete di contenuti approvati per soddisfare le esigenze di specifiche campagne di marketing.

Gli editor interagiscono con le tecnologie di intelligenza artificiale generative di GenStudio for Performance Marketers tramite _prompt_. L’area dei prompt nell’area di lavoro fornisce gli strumenti per inserire i prompt nel contesto delle linee guida di una campagna specifica. Di conseguenza, la qualità e il successo dei contenuti generati dipendono in parte dalla qualità delle linee guida del brand caricate dalla tua organizzazione e dalla specificità del prompt.

Vedere [Scrivi prompt effettivi](effective-prompts.md).

Nella tabella seguente vengono visualizzate le autorizzazioni dell’editor predefinito:

| Funzione obsoleta | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | sì |
| [!DNL Campaigns] | sì | sì | sì | sì |
| [!DNL Content] | sì | sì | sì | sì |
| [!DNL Insights] | può configurare solo ad connectors |    |     | sì |
| [!DNL Personas] | sì | sì | sì | sì |
| [!DNL Products] | sì | sì | sì | sì |
| [!DNL Reviews and approvals] | sì | sì | sì | sì |

### Collaboratori GenStudio

**I collaboratori** possono visualizzare le risorse in GenStudio per gli addetti al marketing delle prestazioni, ma non crearle, modificarle o eliminarle. I collaboratori includono le parti interessate che sono essenziali per il successo del processo di revisione e approvazione dei contenuti, ma che non devono creare o modificare direttamente i contenuti. Esperti legali e manager dei creatori sono esempi di potenziali collaboratori. I collaboratori di GenStudio for Performance Marketers potrebbero disporre delle autorizzazioni necessarie per creare e visualizzare le risorse in altri prodotti Creative Cloud.

Nella tabella seguente vengono visualizzate le autorizzazioni di collaborazione predefinite:

| Funzione obsoleta | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | sì |
| [!DNL Campaigns] | no | no | no | sì |
| [!DNL Content] | no | no | no | sì |
| [!DNL Insights] | no | no | no | sì |
| [!DNL Personas] | no | no | no | sì |
| [!DNL Products] | no | no | no | sì |
| [!DNL Reviews and approvals] | no | no | no | sì |

### Responsabili di sistema GenStudio

**I responsabili di sistema di GenStudio** hanno completato le attività iniziali che preparano l&#39;organizzazione a distribuire GenStudio per gli addetti al marketing delle prestazioni.

Nella tabella seguente vengono visualizzate le autorizzazioni predefinite di GenStudio System Manager:

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

I responsabili di sistema GenStudio preparano l’ambiente GenStudio for Performance Marketers della propria organizzazione affinché gli editor e i collaboratori possano creare le risorse delle campagne. Tali compiti preliminari di configurazione comprendono:

1. [Aggiungi linee guida](./guidelines/overview.md) per [!DNL Brands], [!DNL Products] e [!DNL Personas]. Impostare gli elementi costitutivi chiave dell’identità del marchio della tua organizzazione è un prerequisito essenziale per il lavoro di creatori e collaboratori. Puoi caricare i documenti sulle linee guida del brand o inserire manualmente le informazioni sul brand.
   * **Prepara i documenti sulle linee guida**. Più le linee guida del tuo marchio sono descrittive e complete, migliore sarà l’output. Includi brevi esempi di funzioni ritenute essenziali per il tuo marchio e aggiungi descrizioni di comportamenti che desideri escludere dalla creazione di contenuti. GenStudio for Performance Marketers estrae informazioni da questi documenti caricati e inizia a creare il tuo marchio. Informazioni quali la voce del brand, il canale e le linee guida per le immagini vengono compilate quando GenStudio for Performance Marketers assembla ciascuna linea guida dai documenti caricati.
   * **Modifica o completa i campi delle linee guida del brand in base alle esigenze**. Le linee guida complete per il marchio costituiscono la base della comprensione del marchio dell&#39;organizzazione da parte degli addetti al marketing delle prestazioni di GenStudio. Una volta che GenStudio for Performance Marketers ha estratto le informazioni necessarie dai documenti delle linee guida del brand, ti viene richiesto di modificare manualmente o completare i campi delle informazioni estratte. Specificare singole aree di interesse per il prodotto per la creazione di contenuto aggiungendo [!DNL Product]. Le linee guida di [!DNL Personas] aiutano a personalizzare la creazione di contenuti per segmenti cliente definiti.

   Anche se l’impostazione delle linee guida per il marchio di un’organizzazione può essere un’azione da intraprendere una tantum, potrebbe essere necessario rivedere e migliorare tali linee guida in base alla volatilità, alla crescita e alle mutevoli circostanze di mercato della tua organizzazione.

1. **[Carica modelli](./content/use-templates.md)**. I modelli forniscono scelte rapide e accelerano la creazione dei contenuti. Un modello contiene funzioni approvate, come intestazioni e piè di pagina, e stabilisce protezioni per la creazione di contenuti. In genere, i responsabili di sistema caricano e gestiscono i modelli per la propria organizzazione. I creatori utilizzano i modelli per avviare rapidamente il processo di creazione dei contenuti entro i limiti stabiliti del brand organizzativo.

1. **[Carica risorse approvate](./content/manage-assets.md)**. Le risorse approvate in [!DNL Content] sono disponibili per tutti i creatori di GenStudio for Performance Marketers. È possibile eseguire il seeding di [!DNL Content] con risorse che i creatori possono utilizzare per creare nuove esperienze o risorse.

1. **[Connetti a un account Meta (Facebook)](./insights/connect-channel.md)**. Configura una connessione tra GenStudio for Performance Marketers e gli account social della tua organizzazione per ricevere dati da campagne di marketing, risorse ed esperienze attive. [[!DNL Insights]](./insights/overview.md) fornisce gli strumenti per analizzare i dati derivati dal canale.
