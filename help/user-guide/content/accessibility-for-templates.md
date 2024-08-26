---
title: Creare modelli accessibili
description: Crea modelli in grado di raggiungere tutti i tipi di pubblico da utilizzare in Adobe GenStudio per gli esperti di marketing delle prestazioni.
feature: Templates, Content
source-git-commit: 26d1b9c7b392e93e87ffcd9444f391c2980d1c3c
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---


# Creare modelli accessibili

Adobe si impegna a fornire un’esperienza ottimale per tutti i tipi di pubblico. Consulta [Iniziative per l&#39;accessibilità all&#39;Adobe](https://www.adobe.com/trust/accessibility/initiatives.html) per ulteriori informazioni.

In GenStudio for Performance Marketers, puoi caricare risorse e modelli che consentono la creazione di contenuti per una varietà di esperienze. Il rispetto degli standard di accessibilità consente ai contenuti di raggiungere il pubblico desiderato.

Utilizza i consigli seguenti per preparare i modelli utilizzando standard di accessibilità ottimali.

## Testo alternativo

Fornisci alternative testuali per il contenuto non testuale, ad esempio le immagini.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![Collage di idee, libri, uomo con matita gigante, computer](../../assets/card-create-assets.png){width="400"}

## Scopo collegamento (solo collegamento)

Crea un testo di collegamento chiaro che descriva lo scopo e la posizione del collegamento.

Ad esempio, l’utilizzo di testo di collegamento come &quot;Fai clic qui&quot; o &quot;Ulteriori informazioni&quot; non descrive chiaramente lo scopo del collegamento:

```html
<a href="product-site.html">Click here</a>
```

Come best practice, utilizza un testo che descriva chiaramente dove va il collegamento. Un esempio migliore potrebbe utilizzare il titolo della sorgente del collegamento e lo scopo:

```html
<a href="product-site.html">Explore Product Site</a>
```

## Lingua

Molti prodotti e servizi utilizzano il linguaggio in modo creativo o univoco. Evita il gergo, le frasi lunghe e le frasi complesse. Utilizza un linguaggio chiaro, conciso e di facile lettura compatibile con il tuo pubblico di destinazione.

- Se possibile, utilizza descrizioni chiare, definizioni in linea o esempi correlati. Può essere difficile tradurre un vernacolo unico.

- Scrivi o collega a una definizione per le prime istanze di un acronimo o di un’abbreviazione. Può essere difficile tradurre le abbreviazioni.

- Se possibile, utilizza elementi visivi per integrare il testo o le idee complesse.
