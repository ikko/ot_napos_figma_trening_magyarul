Íme az **1. nap** teljes tananyaga, amely bevezet a Figma koncepciójába, megmutatja a Photoshop/Illustrator háttérből való átállás kulcspontjait, és felkészít a haladó komponensalapú design-gondolkodásra. Az elmélethez példákat, gyakorlathoz konkrét feladatokat, végül mélystruktúrához pedig szakmai kitekintőt adok.

---

# 📘 **1. nap: A Figma alapjai – gondolkodásváltás és rendszermegértés**

## 🎯 Napi célkitűzések:

* Megérteni a Figma struktúráját és működését
* Felismerni a különbségeket az Adobe és Figma közötti koncepcionális világképben
* Elsajátítani a Frame, Auto Layout, Component, Style fogalmak működését
* Első saját Figma projekt létrehozása 3 képernyős mobilapp-vázlattal

---

## 🧠 **Elmélet: Figma mint strukturált UI gondolkodásmód**

### 🔑 Figma koncepcionális pillérei:

| Fogalom         | Jelentés                                                         | Koncepcionális analógia      |
| --------------- | ---------------------------------------------------------------- | ---------------------------- |
| **Frame**       | Tartókeret, UI nézet vagy UI elem konténere                      | Illustrator Artboard + Group |
| **Component**   | Újrafelhasználható UI egység                                     | Smart Object öröklődéssel    |
| **Instance**    | Komponens példány, amely visszavezethető az eredetire            | Linked Smart Object          |
| **Variant**     | Komponens több állapota (pl. hover, disabled, különböző méretek) | Layer state switch + logic   |
| **Auto Layout** | Dinamikus elrendezés, mint CSS Flexbox                           | Responsive Grouping          |
| **Styles**      | Központi színek, betűtípusok, effektek                           | Illustrator Graphic Styles   |

#### 🌐 Miért vált a Figma iparági standarddé?

* Multiplayer by design → **real-time kollaboráció**
* Böngészőalapú, **telepítés nélkül elérhető**
* Komponens és stílus öröklés, **skálázhatóság design rendszerben**
* Integrációs ökoszisztéma (pl. Jira, Notion, Storybook, GitHub, Zeroheight)
* Design + Prototyping + Developer handoff → egyetlen folyamat

---

## 🧪 **Gyakorlati feladat: első mobilalkalmazás vázlat**

### 📂 Projekt setup

1. Regisztrálj/nyisd meg a [https://figma.com](https://figma.com) oldalt
2. Hozz létre egy új **Design File-t**
3. Adj neki nevet: `Mobil App Vázlat – Nap 1`

---

### 🎨 1. Feladat: App képernyők keretezése

* Készíts 3 Frame-et mobil méretben (iPhone 13, 390x844)

  * *Start képernyő*
  * *Bejelentkezés*
  * *Főképernyő*

💡 *TIPP:* A Frame parancs: `F` billentyű

---

### 🧱 2. Feladat: Alapelemek elhelyezése

* Használj `Rectangle`, `Text`, `Button` elemeket (manuálisan vagy a bal panelből)
* Csoportosíts elemeket `Group`-ba, majd alakítsd őket **Component**-té (`Cmd/Ctrl + Alt + K`)
* Hozz létre `Styles`-okat (Color, Text) a bal oldali panelről → jobb klikk: `Create Style`

---

### ⚙️ 3. Feladat: Auto Layout alkalmazása

* Jelölj ki egy gombot, és alkalmazz Auto Layout-ot (`Shift + A`)
* Hozz létre dinamikusan növekvő gombokat több szöveggel (pl. „Tovább”, „Bejelentkezés”, „Mentés”)

🔁 *TIPP:* Próbáld ki a "Padding" és "Spacing" opciókat is az Auto Layout panelen

---

### 🔄 4. Feladat: Komponens újrahasznosítás

* Duplikáld a gomb-komponenst
* Módosítsd a példány szövegét
* Nézd meg, hogyan *öröklődnek* a stílusbeállítások, és mi változtatható külön

---

## 🔍 **Strukturális kitekintő: hogyan működik a Figma, mint öröklődő design rendszer**

### 1. **Komponens öröklés és változatkezelés**

* Ha készítesz egy Component-et, minden `Instance` örökli az alapbeállításokat
* Az `Instance` felülírhatja a tartalmat (pl. szöveg), de megtartja az elrendezési szabályokat
* A `Main Component` módosítása **automatikusan frissíti** az összes példányt

### 2. **Hierarchikus komponensek – Nested Components**

* Egy `Card` komponens tartalmazhat `Image`, `Title`, `Button` komponenseket → ezek egymástól függetlenül is módosíthatók
* **Composable Design**: egy összetett UI elem nem egy nagy layer-halmaz, hanem strukturált objektumfa

### 3. **Auto Layout mint dinamikus viselkedés**

* Ha növekszik a szöveg, a gomb mérete automatikusan igazodik
* Ha hozzáadsz egy új elemet egy `Frame`-hez, az pozícióját automatikusan beállítja

---

## 🧩 **Továbbfejlesztés: ajánlott sablonok, pluginek**

### 🎁 Hasznos Figma File-ok:

* [Figma Learn UI Kit (official)](https://www.figma.com/community/file/1035203688168086460/Figma-Learn-UI-Kit)
* [Apple iOS 17 UI Kit](https://www.figma.com/community/file/1347891532582509253)

### 🔌 Plugin javaslatok:

* [Wireframe Kit](https://www.figma.com/community/plugin/747985167520512094/Wireframe)
* [Auto Layout Visualizer](https://www.figma.com/community/plugin/823394012531778978/Auto-Layout-Visualizer)

---

## 📚 **Zárógyakorlat: Nap végi feladat**

**Téma:** „Bejelentkezés mobilalkalmazás képernyő”

Készíts el egy 3 képernyős UI flow-t:

1. **Start** – Logó + „Belépés” gomb
2. **Login képernyő** – e-mail, jelszó mező + gomb
3. **Főképernyő** – üdvözlő szöveg + lista

Használj:

* Min. 2 saját komponenst (pl. gomb, mező)
* Auto Layout-ot legalább 2 esetben
* 1 szín- és szövegstílust `Styles`-ként definiálva

---

## 🤔 **Reflektív kérdések estére**

1. Miben más gondolkodni Figma-ban, mint Illustratorban?
2. Hogyan segíti az Auto Layout az újrahasználhatóságot?
3. Mit jelent a komponens-öröklés a design fenntarthatósága szempontjából?

---
