# Školní projekt pro předmět XWEB

## Úvaha

Webové stránky jsou jen tak dobré, jak dobrý je jejich obsah, proto jsem se řídil přístupem _CONTENT-FIRST_ a nedříve napsal text ve formátu markdown,
který jsem nakonec zkompiloval do HTML a po minimálním zpracování vložil do layout šablony.

## Stránka obsahuje

-   navigaci + javascript dropdown menu pro mobilní zařízení
-   kompletní hlavičku
    -   metadata (description, keywords, viewport)
    -   title
    -   favicon
-   atributu \[lang="en"\]
-   responzivní layout pomocí css flex a grid, který zabírá vždy alespoň 100% viewportu
-   sémantické rozdělení stránky pomocí tagů header, main, footer
-   sémantické tagy strong em a dfn
-   přístupnost pro lidi se zrakovou vadou (Google chrome Lighthouse audit)

## Prostředky/jazyky použité na stránku

-   HTML, CSS, JS
-   Adobe Illustrator na SVG ikony/ilustrace
-   Markdown pro rychlejší a jednodušší psaní obsahu
-   SASS na jednodušší generaci CSS (media queries, dělení kódu)
-   Visual studio code jako textový editor
-   Node http-server

## Průvodce systémem v adresářích

-   **css** - obsahuje zkompilované css soubory
-   **sass** - obsahuje neprocesované scss/sass soubory
-   **audio** - obsahuje zvukové soubory
-   **music, sound**
    -   **content.md** - markdown verze obsahu
    -   **content.html** - zkompilovaný soubor content.md
    -   **index.html** - prozatím finální verze stránky
-   **index.html** - landing page webové stránky
-   **README.md** - popisuje projekt na repozitáři git
-   **package.json** - obsahuje npm skripty na jednodušší development
-   **package-lock.json** - popisuje stromovou strukturu node_modules po instalaci
-   **.gitignore** - zaručí, že se soubory nebudou trackovat v gitu

## How to run

Ke spuštění stránky stačí mít nainstalovaný node.js a do terminállu zkopírovat `npm install && npm run serve`
nebo použít libovolný server a nasměrovat ho na kořenový adresář repozitáře
