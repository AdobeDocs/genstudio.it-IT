---
title: Personalizzare i modelli
description: Scopri come creare un modello personalizzato per GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: 423956d6fdbf5b31041d44eb434f90d55a87d7c0
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---


# Personalizzare i modelli

Puoi adattare i tuoi modelli di HTML per GenStudio utilizzando il linguaggio di modelli _Handlebars_. La sintassi Handlebars utilizza testo normale con doppie parentesi graffe come segnaposto di contenuto. Per informazioni su come preparare il modello, consulta [`What is Handlebars?`](https://handlebarsjs.com/guide/#what-is-handlebars) nella _Guida del linguaggio Handlebars_.

## Struttura del modello

<!-- This is for email. In the future, maybe use tabs to provide guidance for other template types.
-->

Se non disponi di un modello di HTML pronto per l&#39;uso in GenStudio, puoi iniziare definendo la struttura dell&#39;e-mail utilizzando i tag di HTML: `DOCTYPE`, `html`, `head` e `body`. Puoi includere stili CSS per personalizzare l’aspetto del messaggio e-mail.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Title</title>
    <style>
    </style>
</head>
<body>
</body>
</html>
```

>[!TIP]
>
>Nelle sezioni successive, aggiungi segnaposto di contenuto per i campi e-mail, nascondi gli elementi non necessari dall’anteprima e gestisci i collegamenti al contenuto statico. Quando il modello è pronto, puoi [caricarlo in GenStudio](use-templates.md#upload-a-template) e iniziare a generare e-mail personalizzate in base al modello personalizzato.

## Segnaposto di contenuto

All’interno dell’intestazione o del corpo del modello, puoi utilizzare la sintassi Handlebars per inserire segnaposto di contenuto in cui è necessario che GenStudio compili l’e-mail con il contenuto effettivo. GenStudio riconosce e interpreta automaticamente i segnaposto di contenuto in base al nome del campo.

Ad esempio, puoi utilizzare `{{ headline }}` per indicare dove deve essere posizionato il titolo dell&#39;e-mail:

```handlebars
<div>{{ headline }}</div>
```

Il numero massimo di campi consentiti in un modello personalizzato è venti.

**Nomi di campi riconosciuti**:

| Campo | Ruolo | Modello canale |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | Pre header | email |
| `headline` | Titolo | e-mail<br>annuncio social |
| `body` | Corpo del testo | e-mail<br>annuncio social |
| `cta` | Invito all’azione | e-mail<br>annuncio social |
| `on_image_text` | Su testo immagine | annuncio social |
| `image` | Immagine | e-mail<br>annuncio social |
| `brand_logo` | Logo del marchio selezionato | annuncio social |

>[!IMPORTANT]
>
>GenStudio fornisce automaticamente al modello di posta elettronica un campo `subject` durante il processo [!DNL Create], pertanto non è necessario includere il campo oggetto nel modello di posta elettronica.

+++Esempio: modello di base

Di seguito è riportato un esempio di base di un modello HTML per l’e-mail. L’intestazione contiene CSS semplice e in linea per lo stile. Il corpo contiene un segnaposto `pre-header`, `headline` e `image` per l&#39;inserimento di contenuto da parte di GenStudio durante il processo di generazione dell&#39;e-mail.

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

### Immagine di sfondo

Durante la progettazione di un annuncio per Meta, è importante utilizzare un’immagine di sfondo integrata da testo e una sovrapposizione con il logo del brand. Per garantire il ridimensionamento corretto dell&#39;immagine, i modelli di annunci multimediali richiedono di specificare un `aspect ratio`. In questo contesto, puoi fornire un solo campo immagine.

## Sezioni o gruppi

_Le sezioni_ consentono di informare GenStudio che i campi appartenenti a una sezione richiedono un elevato grado di coerenza. Stabilire questa relazione aiuta l’intelligenza artificiale a generare contenuti che corrispondono agli elementi creativi della sezione. Un modello può includere fino a tre sezioni.

Utilizzare il prefisso desiderato nel nome del campo per indicare che il campo fa parte di una sezione o di un gruppo. Ad esempio, potrebbe essere utile evidenziare il contenuto visualizzato in un&#39;area evidenziata. Puoi scegliere di identificare il contenuto di quest’area con un prefisso comune:

- `spotlight_headline`
- `spotlight_body`

Ogni sezione può avere un solo tipo di campo. Ad esempio, il gruppo dell&#39;esempio precedente con il prefisso `spotlight` può avere un solo campo `spotlight_headline`.

Se sono presenti più sezioni (tre al massimo):

- `headline`
- `body`
- `spotlight_headline`
- `spotlight_body`
- `news_headline`
- `news_body`

GenStudio è consapevole che `spotlight_headline` è più strettamente correlato a `spotlight_body` che a `news_body`.

+++Esempio: modello con più sezioni

Di seguito è riportato lo stesso modello di HTML nell&#39;esempio precedente, ma con altre due sezioni. L’intestazione contiene CSS in linea per la formattazione di un pod. Il corpo utilizza due pod con segnaposto di contenuto che utilizzano un prefisso.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
        <div class="pod">
            <h2>{{ pod1_headline }}</h2>
            <p>This is Pod 1 content.</p>
        </div>
        <div class="pod">
            <h2>{{ pod2_headline }}</h2>
            <p>This is Pod 2 content.</p>
        </div>
    </div>
</body>
</html>
```

+++

## Anteprima modello

I modelli e-mail a volte contengono contenuto speciale che non è necessario visualizzare in anteprima in GenStudio. È possibile controllare la visibilità di questo contenuto utilizzando Helper incorporati, ovvero espressioni speciali nel linguaggio dei modelli Handlebars che consentono di eseguire determinate azioni.

Il valore `_genStudio.browser` viene impostato durante il rendering di un modello e il valore `genStudio.export` viene impostato durante l&#39;esportazione di un modello. Puoi decidere di includere un determinato contenuto nella parte superiore delle e-mail utilizzando un wrapper condizionale, ad esempio, quando il modello viene utilizzato per l’esportazione:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Un altro esempio può essere quello di impedire l’utilizzo dei codici di tracciamento durante l’anteprima di un modello e-mail in GenStudio. Questo esempio mostra come aggiungere parametri di tracciamento ai collegamenti nel modello esportato, mantenendo allo stesso tempo puliti i collegamenti di anteprima:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Contenuto statico

I modelli e-mail e metadati spesso si collegano a immagini e file CSS ospitati al di fuori di GenStudio. Quando GenStudio genera le miniature per questi modelli o le esperienze da essi derivate, queste risorse esterne possono essere ignorate se non dispongono delle intestazioni CORS (Cross-Origin Resource Sharing) corrette.

Per garantire che queste risorse siano disponibili durante il processo di generazione delle miniature, considera due opzioni:

1. **Usa intestazioni CORS**: il server host deve inviare risposte con un&#39;intestazione `Access-Control-Allow-Origin` impostata sul valore `https://experience.adobe.com` per gli ambienti di produzione. Questo metodo consente a GenStudio di accedere alle risorse e di includerle.
1. **Usa URL dati**: incorpora le risorse esterne direttamente nel modello utilizzando URL dati. Questo metodo bypassa le restrizioni CORS e garantisce che le risorse siano disponibili durante la generazione delle miniature.
