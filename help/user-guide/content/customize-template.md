---
title: Personalizzare i modelli
description: Scopri come creare un modello personalizzato per GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: 1b5b12615c52823aa2f1c10ad704e3fc0dabb1e9
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---


# Personalizzare i modelli

Puoi adattare i tuoi modelli di HTML per GenStudio utilizzando il linguaggio di modelli _Handlebars_. La sintassi Handlebars utilizza testo normale con doppie parentesi graffe come segnaposto di contenuto. Per informazioni su come preparare il modello, consulta [`What is Handlebars?`](https://handlebarsjs.com/guide/#what-is-handlebars) nella _Guida del linguaggio Handlebars_.

<!-- This is for email. In the future, maybe use tabs to provide guidance for other template types.
-->If you do not have an HTML template ready to use in GenStudio, you can start by defining the structure of your email using HTML tags: `DOCTYPE`, `html`, `head`, and `body`. You can include CSS styles to customize the appearance of your email.

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

Vedi [Esempi di modelli](#template-examples).

>[!TIP]
>
>Nelle sezioni successive, aggiungi segnaposto di contenuto per i campi e-mail, vedi modelli di esempio, nascondi elementi non necessari dall’anteprima e gestisci collegamenti a contenuto statico. Quando il modello è pronto, puoi [caricarlo in GenStudio](use-templates.md#upload-a-template) e iniziare a generare e-mail personalizzate in base al modello personalizzato.

## Segnaposto di contenuto

All’interno dell’intestazione o del corpo di un modello, puoi utilizzare la sintassi Handlebars per inserire segnaposto di contenuto in cui è necessario che GenStudio compili il modello con il contenuto effettivo. GenStudio riconosce e interpreta automaticamente i segnaposto di contenuto in base al nome del campo.

Ad esempio, puoi utilizzare `{{ headline }}` per indicare dove deve essere posizionato il titolo dell&#39;e-mail:

```handlebars
<div>{{ headline }}</div>
```

### Nomi di campo

Il numero massimo di campi consentiti in un modello personalizzato è venti.

#### Nomi di campi riconosciuti

Nella tabella seguente sono elencati i nomi dei campi riconosciuti da GenStudio per il popolamento in modelli.

| Campo | Ruolo | Modello canale |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | Pre header | e-mail (consigliato) |
| `headline` | Titolo | e-mail (consigliato)<br>Annuncio metadati |
| `body` | Corpo del testo | e-mail (consigliato)<br>Annuncio metadati |
| `cta` | Invito all’azione | e-mail (consigliato)<br>Annuncio metadati |
| `on_image_text` | Su testo immagine | Meta annuncio (consigliato) |
| `image` | Immagine | e-mail (consigliato)<br>Annuncio metadati (consigliato) |
| `brand_logo` | Logo del marchio selezionato | Meta annuncio |

GenStudio compila automaticamente alcuni campi nei modelli, pertanto non è necessario includerli nelle progettazioni dei modelli:

* Campo `subject` (modello e-mail)
* Campi `headline`, `body` e `CTA` (modello di annunci multimediali)

>[!WARNING]
>
>Per gli annunci Instagram, il titolo generato non viene visualizzato nell’esperienza finale.

#### Nome campo logo marchio

Per aggiungere un logo del brand al modello, utilizza il seguente codice per eseguire il rendering del logo predefinito:

```{{#if brand_logo}}{{brand_logo}}{{else}} encoded inline logo {{/if}}```

#### Nomi di campi manuali

Tutti gli altri nomi di campo vengono trattati come campi popolati manualmente. Se si desidera che una sezione sia modificabile, aggiungere parentesi doppie intorno alla sezione che si desidera modificare.

> Esempio: ``{{customVariable}}`` (customVariable è la sezione modificabile manualmente)

## Sezioni o gruppi

_Sezioni_ informano GenStudio che i campi in questa sezione richiedono un elevato grado di coerenza. Stabilire questa relazione aiuta l’intelligenza artificiale a generare contenuti che corrispondono agli elementi creativi della sezione.

Utilizzare il prefisso desiderato nel nome del campo per indicare che un campo fa parte di una sezione o di un gruppo.

Ad esempio, potrebbe essere utile evidenziare il contenuto visualizzato in un&#39;area evidenziata:

* `spotlight_headline`
* `spotlight_body`

Ogni sezione può avere un solo tipo di campo. Nell&#39;esempio precedente, il prefisso `spotlight` può avere un solo campo `spotlight_headline`.

Un modello può includere fino a tre sezioni:

* `headline`
* `body`
* `spotlight_headline`
* `spotlight_body`
* `news_headline`
* `news_body`

GenStudio è consapevole che `spotlight_headline` è più strettamente correlato a `spotlight_body` che a `news_body`.

## Esempi di modelli

+++Esempio: modello e-mail con una sezione

Di seguito è riportato un esempio di base di un modello HTML per un messaggio e-mail che contiene una sezione. L’intestazione contiene CSS semplice e in linea per lo stile. Il corpo contiene `pre-header`, `headline` e `image` [segnaposto](#content-placeholders) per l&#39;inserimento di contenuto da parte di GenStudio durante il processo di generazione dell&#39;e-mail.

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

I modelli e-mail e metadati spesso si collegano a immagini e file CSS ospitati al di fuori di GenStudio. Quando GenStudio genera le miniature per questi modelli o le esperienze da essi derivate, queste risorse esterne possono essere ignorate se non dispongono delle intestazioni CORS (Cross-Origin Resource Sharing) corrette.

Per garantire che queste risorse siano disponibili durante il processo di generazione delle miniature, considera due opzioni:

1. **Usa intestazioni CORS**: il server host deve inviare risposte con un&#39;intestazione `Access-Control-Allow-Origin` impostata sul valore `https://experience.adobe.com` per gli ambienti di produzione. Questo metodo consente a GenStudio di accedere alle risorse e di includerle.
1. **Usa URL dati**: incorpora le risorse esterne direttamente nel modello utilizzando URL dati. Questo metodo bypassa le restrizioni CORS e garantisce che le risorse siano disponibili durante la generazione delle miniature.
