---
title: Personalizzare i modelli
description: Scopri come creare un modello personalizzato, ad Adobe GenStudio per gli esperti di marketing delle prestazioni.
level: Intermediate
feature: Templates, Content
source-git-commit: 44390d551e638fcff47cff5844fcfda4ed9f98f3
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---


# Personalizzare i modelli

Adattare i modelli di HTML per Adobe GenStudio per gli esperti di marketing delle prestazioni utilizzando il linguaggio di modelli _Handlebars_. La sintassi Handlebars utilizza testo normale con doppie parentesi graffe come segnaposto di contenuto. Per informazioni su come preparare il modello, consulta [`What is Handlebars?`](https://handlebarsjs.com/guide/#what-is-handlebars) nella _Guida del linguaggio Handlebars_.

Se non si dispone di un modello di HTML pronto per l&#39;utilizzo in GenStudio per gli addetti al marketing delle prestazioni, è possibile iniziare definendo la struttura del modello utilizzando i tag di HTML: `DOCTYPE`, `html`, `head` e `body`. Di seguito è riportato un modello e-mail di base che include stili CSS per personalizzare l’aspetto:

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
>Nelle sezioni successive, aggiungi segnaposto di contenuto per i campi e-mail, vedi modelli di esempio, nascondi elementi non necessari dall’anteprima e gestisci collegamenti a contenuto statico. Quando il modello è pronto, puoi [caricarlo in GenStudio per gli esperti di marketing delle prestazioni](use-templates.md#upload-a-template) e iniziare a generare e-mail personalizzate in base al modello personalizzato.

## Segnaposto di contenuto

All&#39;interno dell&#39;intestazione o del corpo di un modello, è possibile utilizzare la sintassi Handlebars per inserire segnaposto di contenuto in cui è necessario che GenStudio for Performance Marketers compili il modello con il contenuto effettivo. GenStudio for Performance Marketers riconosce e interpreta automaticamente i segnaposto di contenuto in base al nome del campo.

Ad esempio, puoi utilizzare `{{ headline }}` per indicare dove deve essere posizionato il titolo dell&#39;e-mail:

```handlebars
<div>{{ headline }}</div>
```

### Nomi di campi riconosciuti

Il numero massimo di campi consentiti in un modello personalizzato è venti.

Nella tabella seguente sono elencati i nomi dei campi riconosciuti da GenStudio per gli addetti al marketing delle prestazioni per la compilazione in modelli.

| Campo | Ruolo | Modello canale |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | Pre header | e-mail (consigliato) |
| `headline` | Titolo | e-mail (consigliato)<br>Annuncio metadati |
| `body` | Corpo del testo | e-mail (consigliato)<br>Annuncio metadati |
| `cta` | Invito all’azione | e-mail (consigliato)<br>Annuncio metadati |
| `on_image_text` | Su testo immagine | Meta annuncio (consigliato) |
| `image` | Immagine | e-mail (consigliato)<br>Annuncio metadati (consigliato) |
| `brand_logo` | Logo del marchio selezionato<br>Per informazioni sull&#39;utilizzo consigliato, vedere il [nome campo](#brand-logo-field-name). | e-mail<br>Meta annuncio |

GenStudio for Performance Marketers compila automaticamente alcuni campi nei modelli, pertanto non è necessario includerli nelle progettazioni dei modelli:

- Campo `subject` (modello e-mail)
- Campi `headline`, `body` e `CTA` (modello di annunci multimediali)

>[!WARNING]
>
>Per gli annunci Instagram, il titolo generato non viene visualizzato nell’esperienza finale.

#### Nome campo logo marchio

Negli esempi seguenti vengono illustrati due metodi che eseguono il rendering condizionale del logo del marchio, verificano l’origine, forniscono un logo predefinito o alternativo nel caso in cui il logo del marchio non sia disponibile e applicano uno stile:

_Esempio_: nella definizione HTML `img src`

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;"> 
```

_Esempio_: in una condizione Handlebars

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### Nomi di campi manuali

Tutti gli altri nomi di campo vengono trattati come campi popolati manualmente. Per creare una sezione modificabile, aggiungere parentesi doppie attorno al nome della sezione:

```handlebars
{{customVariable}}
```

## Sezioni o gruppi

_Le sezioni_ informano GenStudio per gli addetti al marketing delle prestazioni che i campi in questa sezione richiedono un elevato grado di coerenza. Stabilire questa relazione aiuta l’intelligenza artificiale a generare contenuti che corrispondono agli elementi creativi della sezione.

Utilizzare un prefisso scelto nel nome del campo per indicare che un campo fa parte di una sezione o di un gruppo.

Ad esempio, potrebbe essere utile evidenziare il contenuto visualizzato in un&#39;area evidenziata:

- `spotlight_headline`
- `spotlight_body`

Ogni sezione può avere un solo tipo di campo. Nell&#39;esempio precedente, il prefisso `spotlight` può avere un solo campo `spotlight_headline`.

Un modello può includere fino a tre sezioni:

- `headline`
- `body`
- `spotlight_headline`
- `spotlight_body`
- `news_headline`
- `news_body`

GenStudio for Performance Marketers è consapevole del fatto che `spotlight_headline` è più strettamente correlato a `spotlight_body` che a `news_body`.

## Esempi di modelli

+++Esempio: modello e-mail con una sezione

Di seguito è riportato un esempio di base di un modello HTML per un messaggio e-mail che contiene una sezione. L’intestazione contiene CSS semplice e in linea per lo stile. Il corpo contiene un `pre-header`, `headline` e `image` [segnaposto](#content-placeholders) per l&#39;utilizzo da parte di GenStudio per gli esperti di marketing delle prestazioni per inserire contenuto durante il processo di generazione dell&#39;e-mail.

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

+++Esempio: modello e-mail con più sezioni

Di seguito è riportato lo stesso modello di HTML nell&#39;esempio precedente, ma con altre due sezioni. L’intestazione contiene CSS in linea per la formattazione di un gruppo. Il corpo utilizza due gruppi con [segnaposto contenuto](#content-placeholders) utilizzando un prefisso.

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

+++Esempio: Meta ad template

Di seguito è riportato un esempio di base di un modello di annunci Meta. L’intestazione contiene CSS in linea per lo stile. Il corpo utilizza [segnaposto contenuto](#content-placeholders) utilizzando un prefisso.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>
</body>
</html>
```

+++

## Anteprima modello

Controlla la visibilità dei contenuti speciali utilizzando Helper incorporati (espressioni speciali nel linguaggio dei modelli Handlebars che eseguono determinate azioni). Ad esempio, puoi aggiungere parametri di tracciamento ai collegamenti nel modello esportato mantenendo puliti i collegamenti di anteprima.

Il valore `_genStudio.browser` viene impostato durante il rendering di un modello e il valore `genStudio.export` viene impostato durante l&#39;esportazione di un modello. Puoi decidere di includere un determinato contenuto nella parte superiore di un’e-mail utilizzando un wrapper condizionale, ad esempio, quando il modello viene utilizzato per l’esportazione:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Un altro esempio può essere quello di impedire l’utilizzo dei codici di tracciamento durante l’anteprima di un modello in GenStudio. Questo esempio mostra come aggiungere parametri di tracciamento ai collegamenti nel modello esportato, mantenendo allo stesso tempo puliti i collegamenti di anteprima:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Contenuto statico

I modelli e-mail e metadati spesso si collegano a immagini e file CSS ospitati al di fuori di GenStudio per gli esperti di marketing delle prestazioni. Quando GenStudio for Performance Marketers genera le miniature per questi modelli o le esperienze da essi derivate, potrebbe ignorare queste risorse esterne se non dispongono delle intestazioni CORS (Cross-Origin Resource Sharing) corrette.

Per garantire che queste risorse siano disponibili durante il processo di generazione delle miniature, considera due opzioni:

1. **Usa intestazioni CORS**: il server host deve inviare risposte con un&#39;intestazione `Access-Control-Allow-Origin` impostata sul valore `https://experience.adobe.com` per gli ambienti di produzione. Questo metodo consente a GenStudio per gli esperti di marketing delle prestazioni di accedere alle risorse e di includerle.
1. **Usa URL dati**: incorpora le risorse esterne direttamente nel modello utilizzando URL dati. Questo metodo bypassa le restrizioni CORS e garantisce che le risorse siano disponibili durante la generazione delle miniature.
