---
title: Preparare un modello di metadati per GenStudio
description: Scopri come creare un modello di Meta Ad personalizzato per GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: 31f02218e02b1400ca9f32472acdecae03dbd304
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---


# Preparazione del modello di metadati per GenStudio

La creazione di un modello di metadati implica un approccio strutturato personalizzato per i social media. Dopo aver progettato e testato un modello di Meta Ad, puoi prepararlo per il caricamento e l’utilizzo in GenStudio.

## Aggiungi linee guida

Prima di preparare un Meta Ad Template, assicurati di aver aggiunto [linee guida](/help/user-guide/guidelines/overview.md) al tuo GenStudio e di averle compilate con informazioni complete per i brand rilevanti. Le [linee guida per il brand](/help/user-guide/guidelines/brands.md) influenzano direttamente i contenuti generati.

**Esempio**: se desideri che il corpo di un modello di annunci multimediali non superi i 500 caratteri, aggiungi tale requisito alle [linee guida per i canali](/help/user-guide/guidelines/brands.md#channel-guidelines) per il campo &quot;body&quot;.

Se non si aggiungono linee guida a GenStudio, vengono utilizzati i valori predefiniti.

## Progettare un modello

In genere, una finestra di progettazione crea la progettazione visiva di un modello in un programma di progettazione come Adobe XD.

Consulta [Anatomia di un modello](/help/user-guide/content/use-templates.md#anatomy-of-a-template) e [Esempi di modelli](/help/user-guide/content/customize-template.md#template-examples).

### Specifiche dell’annuncio

GenStudio supporta le seguenti proporzioni per gli annunci Meta:

* Quadrato (1:1): 1080 x 1080 pixel
* Verticale (4:5): 1080 x 1350 pixel
* Storia (9:16): 1080 x 1920 pixel

Se l’annuncio non è progettato in uno di questi rapporti di formato, GenStudio ritaglia automaticamente l’immagine nelle dimensioni appropriate.

## Testare un modello di metadati

Prova il modello utilizzando il Creative Hub di Meta per vedere come si presenta l’annuncio in posizionamenti diversi, ad esempio in un feed o come una storia.

Utilizza la piattaforma di consegna e-mail o di verifica per testare l’e-mail e verificare che venga riprodotta correttamente tra client e dispositivi e-mail diversi.

## Definire le aree di contenuto generato

Definisci le aree nel modello e-mail che devono essere compilate dinamicamente con il contenuto di GenStudio.

Per definire le aree di contenuto generato:

* Identifica gli elementi di testo nel modello che GenStudio deve generare automaticamente, ad esempio il titolo o CTA.
* Adatta il modello di HTML inserendo segnaposto al suo interno utilizzando la sintassi Handblebars.

Vedi [Segnaposto contenuto](/help/user-guide/content/customize-template.md#content-placeholders).

## Visualizzare l’anteprima del modello

Controlla la visibilità di aree di contenuto specifiche utilizzando gli Helper integrati. Ad esempio, puoi includere parametri di tracciamento per i collegamenti in un modello esportato mantenendo collegamenti di anteprima puliti.

Vedi [Anteprima modello](/help/user-guide/content/customize-template.md#template-preview).

## Caricare e utilizzare il modello

Dopo aver progettato, codificato, testato e visualizzato in anteprima il modello, puoi caricarlo in GenStudio per utilizzarlo nella generazione di nuovi contenuti di marketing.

Vedi [Utilizzo dei modelli](use-templates.md).
