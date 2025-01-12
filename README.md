<p align="center"><img alt="Laraflash" src="logo.png" width="450"></p>

<p align="center">This package provides the language support for <b>Laravel Nova</b>.</p>

Feel free to submit your language or update an existing one by sending a PR to help other people.  
If you want to contribute, please ensure you read the [contributing guidelines](CONTRIBUTING.md) first.

## Installation

```bash
composer require coderello/laravel-nova-lang
```

## Usage
### Publish Command
Publish translations for one language:
```bash
php artisan nova-lang:publish de
```

Publish translations for multiple languages:
```bash
php artisan nova-lang:publish de,ru
```

Publish translations for all languages:
```bash
php artisan nova-lang:publish --all
```

Publish translations and override existing files:
```bash
php artisan nova-lang:publish de,ru --force
```

### Development Commands (debug mode only)

You must have the `app.debug` config option set to true for these commands to be available:

#### Missing Command

This command is to assist contributors to find any untranslated keys for their chosen language.

A stub JSON file will be created at `storage_path('app/nova-lang/missing/{locale}.json')`. You can copy those keys into the `resources/lang/{locale}.json` language file in your own fork of the repository, translate them and create a pull request.

Output missing translation keys for one or more languages:
```bash
php artisan nova-lang:missing de,ru
```

Output missing translation keys for all languages:
```bash
php artisan nova-lang:missing --all
```

#### Stats Command

This command is to assist maintainers to update the completeness of each language and list of contributors in this README file.

A `README.excerpt.md` and `contributors.json` file will be created at `storage_path('app/nova-lang')`. You can copy those files into your own fork of the repository and create a pull request.

Output list of languages, lines translated and contributors:
```bash
php artisan nova-lang:stats
```

Ensure you have created a GitHub personal access token and saved it as a `GITHUB_TOKEN_NOVALANG` env variable in your master Laravel application in order to download the most recent contributions.

## Available Languages

| Language | Code | Lines translated | Thanks to |
| --- | --- | --- | --- |
| Arabic | [ar](resources/lang/ar.json) | 392 (100%) | [saleem-hadad](https://github.com/saleem-hadad), [danyelkeddah](https://github.com/danyelkeddah), [Arryan](https://github.com/Arryan) |
| Brazilian Portuguese | [pt-BR](resources/lang/pt-BR.json) | 392 (100%) | [henryavila](https://github.com/henryavila), [pedrofurtado](https://github.com/pedrofurtado), [eduardokum](https://github.com/eduardokum), [saulo-silva](https://github.com/saulo-silva), [chbbc](https://github.com/chbbc), [IgorDePaula](https://github.com/IgorDePaula) |
| English | [en](resources/lang/en.json) | 392 (100%) | [taylorotwell](https://github.com/taylorotwell), [bonzai](https://github.com/bonzai), [davidhemphill](https://github.com/davidhemphill), [themsaid](https://github.com/themsaid), [mziraki](https://github.com/mziraki), [kitbs](https://github.com/kitbs) |
| German | [de](resources/lang/de.json) | 392 (100%) | [pille1842](https://github.com/pille1842), [shieraki](https://github.com/shieraki), [kitbs](https://github.com/kitbs), [dakira](https://github.com/dakira) |
| Chinese (Simplified) | [zh-CN](resources/lang/zh-CN.json) | 387 (98.7%) | [jcc](https://github.com/jcc), [zacksleo](https://github.com/zacksleo) |
| Chinese (Traditional) | [zh-TW](resources/lang/zh-TW.json) | 387 (98.7%) | [CasperLaiTW](https://github.com/CasperLaiTW), [zacksleo](https://github.com/zacksleo) |
| French | [fr](resources/lang/fr.json) | 387 (98.7%) | [MarceauKa](https://github.com/MarceauKa), [InfinityWebMe](https://github.com/InfinityWebMe), [Arryan](https://github.com/Arryan), [KillianH](https://github.com/KillianH) |
| Spanish | [es](resources/lang/es.json) | 382 (97.4%) | [joebordes](https://github.com/joebordes), [ajmariduena](https://github.com/ajmariduena), [Arryan](https://github.com/Arryan), [xcodinas](https://github.com/xcodinas), [dgtal](https://github.com/dgtal), [rodrigore](https://github.com/rodrigore) |
| Farsi | [fa](resources/lang/fa.json) | 374 (95.4%) | [alirezamirsepassi](https://github.com/alirezamirsepassi), [mziraki](https://github.com/mziraki) |
| Russian | [ru](resources/lang/ru.json) | 371 (94.6%) | [hivokas](https://github.com/hivokas), [S-anasol](https://github.com/S-anasol), [deadem](https://github.com/deadem), [estim](https://github.com/estim) |
| Portuguese | [pt](resources/lang/pt.json) | 370 (94.4%) | [Pedrocssg](https://github.com/Pedrocssg) |
| Italian | [it](resources/lang/it.json) | 350 (89.3%) | (deleted), [manuelcoppotelli](https://github.com/manuelcoppotelli), [dejdav](https://github.com/dejdav) |
| Catalan | [ca](resources/lang/ca.json) | 349 (89%) | [joebordes](https://github.com/joebordes) |
| Basque | [eu](resources/lang/eu.json) | 348 (88.8%) | [JonPaternain](https://github.com/JonPaternain) |
| Swedish | [sv](resources/lang/sv.json) | 347 (88.5%) | [tanjemark](https://github.com/tanjemark) |
| Croatian | [hr](resources/lang/hr.json) | 346 (88.3%) | [defart](https://github.com/defart), [walaski](https://github.com/walaski) |
| Czech | [cs](resources/lang/cs.json) | 346 (88.3%) | [walaskir](https://github.com/walaskir), [walaski](https://github.com/walaski) |
| Danish | [da](resources/lang/da.json) | 346 (88.3%) | [olivernybroe](https://github.com/olivernybroe) |
| Dutch | [nl](resources/lang/nl.json) | 346 (88.3%) | [happyDemon](https://github.com/happyDemon), [jschram](https://github.com/jschram), [sebastiaanspeck](https://github.com/sebastiaanspeck), [daniel-de-wit](https://github.com/daniel-de-wit) |
| Filipino | [fil](resources/lang/fil.json) | 346 (88.3%) | [granaderos](https://github.com/granaderos) |
| Finnish | [fi](resources/lang/fi.json) | 346 (88.3%) | [Krisseck](https://github.com/Krisseck) |
| Georgian | [ka](resources/lang/ka.json) | 346 (88.3%) | [akalongman](https://github.com/akalongman) |
| Hindi | [hi](resources/lang/hi.json) | 346 (88.3%) | [bantya](https://github.com/bantya) |
| Hungarian | [hu](resources/lang/hu.json) | 346 (88.3%) | [milli05](https://github.com/milli05) |
| Indonesian | [id](resources/lang/id.json) | 346 (88.3%) | [dvlwj](https://github.com/dvlwj) |
| Serbian (Cyrillic) | [sr](resources/lang/sr.json) | 346 (88.3%) | [marjanovicsteva](https://github.com/marjanovicsteva) |
| Serbian (Latin) | [sr-Latn](resources/lang/sr-Latn.json) | 346 (88.3%) | [marjanovicsteva](https://github.com/marjanovicsteva) |
| Slovak | [sk](resources/lang/sk.json) | 346 (88.3%) | [hejty](https://github.com/hejty) |
| Slovenian | [sl](resources/lang/sl.json) | 346 (88.3%) | [morpheus7CS](https://github.com/morpheus7CS) |
| Turkish | [tr](resources/lang/tr.json) | 346 (88.3%) | [bureken](https://github.com/bureken), [sineld](https://github.com/sineld), [dilekuzulmez](https://github.com/dilekuzulmez) |
| Ukrainian | [uk](resources/lang/uk.json) | 346 (88.3%) | [hivokas](https://github.com/hivokas), [Ostap34JS](https://github.com/Ostap34JS), [coderello](https://github.com/coderello) |
| Bulgarian | [bg](resources/lang/bg.json) | 345 (88%) | [BKirev](https://github.com/BKirev) |
| Lithuanian | [lt](resources/lang/lt.json) | 345 (88%) | [minved](https://github.com/minved) |
| Polish | [pl](resources/lang/pl.json) | 345 (88%) | [Strus](https://github.com/Strus), [marekfilip](https://github.com/marekfilip), [wiktor-k](https://github.com/wiktor-k) |
| Romanian | [ro](resources/lang/ro.json) | 344 (87.8%) | [BTeodorWork](https://github.com/BTeodorWork), [alexgiuvara](https://github.com/alexgiuvara) |
| Tagalog | [tl](resources/lang/tl.json) | 344 (87.8%) | [rcjavier](https://github.com/rcjavier) |
