# KépMozaik

Reszponzív, teljesen böngészőben futó alkalmazás, amellyel több képből rendezett és testreszabható képmozaik készíthető.

A képek átrendezhetők, kivághatók, nagyíthatók és feliratozhatók, majd az elkészült mozaik veszteségmentes PNG-ként vagy kisebb fájlméretre optimalizált JPG-ként exportálható.

## Online változat

**[KépMozaik megnyitása](https://lkristof.github.io/kepmozaik/)**

![KépMozaik előnézet](./assets/images/screenshot-light.jpg)

## Főbb funkciók

* Több kép egyidejű betöltése
* Képek hozzáadása fájlválasztóval vagy drag and drop módszerrel
* Képek sorrendjének átrendezése
* Képek pozicionálása és nagyítása a kivágási területen
* Érintőképernyős mozgatás és nagyítás
* Előre definiált és egyéni képarányok
* 1–10 oszlopos elrendezés
* Többsoros képfeliratok
* Feliratszín, feliratháttér és mozaikháttér beállítása
* Állítható rácsköz
* Több exportminőség
* Veszteségmentes PNG-export
* Optimalizált JPG-export kisebb fájlmérethez
* Projekt mentése és visszatöltése JSON-fájlból
* Automatikus helyreállítás véletlen oldalfrissítés után
* Magyar és angol kezelőfelület
* Világos és sötét megjelenés
* Reszponzív asztali és mobil felület
* Billentyűzettel is használható kezelőelemek

## Adatvédelem

A képek feldolgozása helyben, közvetlenül a böngészőben történik.

Az alkalmazás nem tölti fel a kiválasztott képeket külső szerverre. Projekt mentésekor a böngésző helyi JSON-fájlt készít, exportáláskor pedig a kiválasztott formátumtól függően PNG- vagy JPG-fájlt generál.

## Használat

1. Nyisd meg az [online alkalmazást](https://lkristof.github.io/kepmozaik/).
2. Kattints a **Képek tallózása** gombra, vagy húzd a képeket a feltöltési területre.
3. Állítsd be a képarányt és az oszlopok számát.
4. Mozgasd és nagyítsd a képeket a kívánt kivágás eléréséhez.
5. Rendezd át a képeket a kívánt sorrendbe.
6. Adj meg feliratokat, és állítsd be a megjelenésüket.
7. Válaszd ki az exportálási minőséget, a rácsközt és a kívánt háttérbeállításokat.
8. Kattints a **PNG** vagy **JPG** exportgombra a kívánt formátum letöltéséhez.

## Projekt mentése

A **Projekt mentése** gombbal az aktuális munka JSON-fájlba menthető, így később ugyanonnan folytatható.

A projektfájl többek között tartalmazza:

* a képeket optimalizált formában;
* a képek sorrendjét;
* a kivágási pozíciókat;
* a nagyítási értékeket;
* a képfeliratokat;
* az elrendezési beállításokat;
* az exportálási beállításokat.

A mentett projekt a **Projekt betöltése** gombbal tölthető vissza.

### Automatikus helyreállítás

A folyamatban lévő projekt állapota automatikusan mentésre kerül a böngésző helyi tárhelyére. Ennek köszönhetően egy véletlen oldalfrissítés után a munka visszaállítható.

Az automatikus helyreállítás az adott böngészőhöz és eszközhöz kötődik, ezért nem helyettesíti a **Projekt mentése** funkcióval letölthető JSON-fájlt.

> A projektfájl a beágyazott képek miatt nagy méretű lehet.

## Technológiák

* HTML5
* CSS3
* Vanilla JavaScript
* Canvas API
* File API és Blob API
* Pointer Events
* Local Storage és IndexedDB
* GitHub Pages

A projekt nem használ JavaScript frameworköt, csomagkezelőt vagy külső buildrendszert.

## Projektstruktúra

```text
kepmozaik/
├── assets/
│   └── images/
│       ├── apple-touch-icon.png
│       ├── favicon-96x96.png
│       ├── favicon.ico
│       ├── favicon.svg
│       ├── og-image.jpg
│       ├── screenshot-dark.jpg
│       ├── screenshot-light.jpg
│       ├── web-app-manifest-192x192.png
│       └── web-app-manifest-512x512.png
├── index.html
├── LICENSE
├── README.md
└── site.webmanifest
```

Az alkalmazás HTML-, CSS- és JavaScript-kódja jelenleg az `index.html` fájlban található.

## Böngészőtámogatás

Modern asztali vagy mobil böngésző használata ajánlott, például:

* Google Chrome
* Microsoft Edge
* Mozilla Firefox
* Safari

Nagyméretű projektek esetén a memóriahasználat a képek számától, felbontásától és a választott exportminőségtől függ.

## Felhasznált ikonok

A kezelőfelület a [Lucide Icons](https://lucide.dev/) ikonjait használja, amelyek az ISC licenc alatt érhetők el.

## Licenc

A projekt az MIT licenc alatt érhető el. További információ a [LICENSE](./LICENSE) fájlban található.
