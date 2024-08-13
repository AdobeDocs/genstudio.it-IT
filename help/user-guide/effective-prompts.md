---
title: Scrivi prompt effettivi
description: Scopri come scrivere prompt efficaci per GenStudio.
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
source-git-commit: 5e17996ee3a86cf664ee468d6b9cf178c8853992
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# Scrivi prompt effettivi

Comunicare con l’intelligenza artificiale generativa è essenziale per lavorare efficacemente in GenStudio.

GenStudio fornisce un prompt di IA generativo ogni volta che è possibile modificare una risorsa. I componenti di un prompt efficace devono includere un linguaggio descrittivo, esempi e informazioni non fornite dalle linee guida configurate.

Come best practice, fornisci a GenStudio le tue informazioni sul brand utilizzando [linee guida](/help/user-guide/guidelines/overview.md), quindi puoi sfruttare appieno l’intelligenza artificiale generativa per produrre esperienze di contenuti allineati al brand.

## Lingua descrittiva

Puoi usare il linguaggio naturale per articolare le tue idee e creare esperienze. Il prompt guida l’intelligenza artificiale nella generazione di contenuti di canale personalizzati e immagini complementari alla tua visione. Maggiore è il numero di dettagli forniti, maggiori sono le possibilità di produrre un&#39;immagine o un&#39;esperienza che soddisfi le tue esigenze. Utilizza un linguaggio chiaro e descrittivo per fornire il maggior numero di dettagli possibile:

- Per **immagini**, utilizza parole che descrivono atmosfera, umore, colore, composizione e stile.
- Per **copia**, utilizza parole che descrivono il pubblico, lo scopo, le descrizioni delle nuove funzionalità, gli esempi e le azioni.

Di seguito è riportato un prompt di esempio che articola le informazioni relative all’intento, al pubblico di destinazione e allo stile.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++Vedi i risultati di esempio

![tre e-mail generate](/help/assets/sample-email.png)

+++

## Criteri di richiesta

In GenStudio [[!DNL Create]](/help/user-guide/create/overview.md) è possibile utilizzare **[!UICONTROL Criteri prompt]** ([_Parametri_](/help/user-guide/create/overview.md#parameters) e un prompt) nell&#39;area dei prompt per aggiungere dettagli tramite la selezione per migliorare l&#39;interpretazione di IA.

Per [e-mail](/help/tutorials/create-email-experience.md), i criteri di richiesta potrebbero includere l&#39;aggiunta di [linee guida](/help/user-guide/guidelines/overview.md) in _Parametri_, il caricamento di una risorsa da utilizzare nelle varianti di e-mail e un prompt descrittivo. Per un [Meta ad](/help/tutorials/create-meta-ad.md), i criteri di richiesta potrebbero includere una linea guida del brand in _Parametri_, la selezione o il caricamento di una risorsa esistente, impostazioni relative a immagini o risorse quali proporzioni e un prompt. La potenza effettiva inizia con [la configurazione delle linee guida di GenStudio](/help/user-guide/guidelines/add-guidelines.md).

>[!NOTE]
>
>Se vengono aggiunte linee guida in _Parametri_ nell&#39;area prompt, non è necessario includere un riferimento a tali linee guida nel prompt. GenStudio sfrutterà questi [!DNL Brands], [!DNL Products] e [!DNL Personas] nella generazione dei contenuti.

### Linee guida

Le linee guida di GenStudio aiutano l’intelligenza artificiale generativa a personalizzare la composizione delle risorse GenStudio. Quando viene visualizzato un criterio di richiesta, è possibile scegliere [[!DNL Brand]](/help/user-guide/guidelines/brands.md), [[!DNL Persona]](/help/user-guide/guidelines/personas.md) e [[!DNL Product]](/help/user-guide/guidelines/products.md) dalle linee guida configurate.

>[!TIP]
>
>Puoi controllare come e quando GenStudio utilizza le linee guida di [!DNL Brand]. Consulta [Linee guida](/help/user-guide/guidelines/overview.md) per scoprire come configurare e gestire le linee guida per il brand.

## Riprova

La richiesta è un processo iterativo. Se i risultati non soddisfano le aspettative, rivedere la richiesta e apportare alcune modifiche o aggiungere ulteriori dettagli. Per perfezionare la richiesta, fornisci un URL come esempio o come origine per ulteriori informazioni.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.

Use information from https://www.adobe.com/products/photoshop.html to inspire users with the latest features.
```

In alternativa, puoi incollare le sezioni da una descrizione della campagna. Puoi anche richiedere che GenStudio eviti determinate parole, elementi o temi.

## Best practice

Alcune semplici best practice per creare prompt efficaci in GenStudio:

- Sii specifico e fornisci dettagli su cosa fare e non fare.
- Fornisci contesto utilizzando riferimenti esterni.
- Utilizzare le linee guida di GenStudio.
- Rivedi e adegua regolarmente le linee guida.
- Iterare e perfezionare.
- Imparare attraverso la sperimentazione.
