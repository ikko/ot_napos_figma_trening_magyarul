Nagyszerű célkitűzés, és a korábbi Illustrator és Photoshop tapasztalataid szilárd alapot adnak a Figma professzionális szintű elsajátításához. A Figma nemcsak vizuális tervezőeszköz, hanem **strukturált, kollaboratív, komponensalapú design rendszer platform**, amely a mai UX/UI pozíciók kulcseszközévé vált.

Az alábbi 5 napos tanterv **fókuszált, intenzív képzést** nyújt, amely ötvözi az elméletet, gyakorlati projekteket, koncepcionális mélymerülést és ipari szintű módszertanokat – különös figyelemmel a **hierarchikus komponenskezelésre, öröklődésre, újrahasználhatóságra és design rendszerekre**.

---

## 🧭 **5 napos Figma tanterv UI/UX tervezőknek (közép–nagyvállalati szint)**

### 🔹 **Napi struktúra (minden napra):**

* **Elméleti megalapozás** (1–1,5 óra)
* **Gyakorlati feladat/projekt** (2–3 óra)
* **Haladó koncepcionális ismeretek és inspirációk** (1 óra)
* **Reflektív kérdések + kis recap feladat**

---

## ✅ **1. nap – A Figma világképe & belépés a rendszerbe**

**🎯 Cél:** Átfogó koncepcionális kép a Figma mögötti filozófiáról, különbségek az Adobe-világhoz képest.

### 📘 Elmélet:

* Figma, mint *DesignOps* eszköz: [Multiplayer design](https://www.figma.com/blog/how-figmas-multiplayer-technology-works/)
* Különbség Photoshop/Illustrator rétegalapú rendszere és Figma **frame/page/component** alapú rendszere között.
* Hogyan működik a **real-time kollaboráció, verziókövetés, komponens szinkronizálás**.
* Figma alapvető fogalmai: Frame, Group, Component, Variant, Styles, Auto Layout

### 🧪 Gyakorlat:

* Készíts egy mobil app vázlatát (3 képernyő) frame-ek és layout grid segítségével
* Használj **reusable components** gombokhoz, input mezőkhöz

### 🧠 Koncepcionális mélymerülés:

* **Auto Layout** = Figma „dinamikus dobozolási” rendszere, hasonló mint CSS Flexbox – segít responsív UI komponensek készítésében.
* **Nested Components** – mint az OOP „öröklődés”: egyik komponens beágyazva egy másikba.
* **Variánsok**: több állapot (pl. hover, disabled) egy komponenshez, logikusan kezelhető.

---

## ✅ **2. nap – Komponensek, Variánsok, Öröklés mint design eszköz**

**🎯 Cél:** Megérteni és implementálni újrahasznosítható komponenseket.

### 📘 Elmélet:

* **Components vs Instances**: Hogyan öröklik az "Instance"-ek a fő komponens tulajdonságait
* **Variants** – állapotok (pl. hover, active), méretváltozatok (S, M, L)
* **Component Set-ek** és komponenskönyvtárak felépítése

### 🧪 Gyakorlat:

* Készíts saját **Button rendszer**-t: 3 méret, 2 szín, 3 állapot (normal, hover, disabled)
* Készíts egy **Reusable Input field** family-t (text, textarea, search box)

### 🧠 Deep Dive:

* **Design tokens koncepciója**: A színek, betűméretek, spaciok központi kezelése (mint SCSS változók, de designra)
* Figma + [Tokens Studio plugin](https://tokens.studio/plugin) – design tokenek exportálása CSS-be, JSON-be

---

## ✅ **3. nap – Design rendszerek és skálázhatóság**

**🎯 Cél:** Megérteni és építeni design rendszert vállalati szinten.

### 📘 Elmélet:

* **Design System** fogalma: komponens, stílus, dokumentáció, szabályrendszer együttesen
* Figma könyvtárak (Libraries): megosztható komponensek és stílusok
* Naming conventions & struktúra (pl. `btn/primary/small`)

### 🧪 Gyakorlat:

* Készíts egy mini design system-et (4-5 komponens + színséma + typográfia + spacing scale)
* Használd a [Figma styles](https://help.figma.com/hc/en-us/articles/360039238753-Styles-in-Figma) lehetőséget: Color, Text, Effects, Grid

### 🧠 Inspiráció:

* Nézd meg a [IBM Carbon Design System](https://carbondesignsystem.com/) vagy [Shopify Polaris](https://polaris.shopify.com/) rendszerét
* Építs hasonlót kicsiben

---

## ✅ **4. nap – Prototípusok és user flow modellezés**

**🎯 Cél:** Dinamikus prototípus és felhasználói útvonalak modellezése

### 📘 Elmélet:

* **Interaction model** Figma-ban: click, hover, open overlay, navigate to, swap variant
* **User Flow diagram** készítése frame-ekkel és panellinkekkel
* Prototípus animációk, átmenetek, delayed interaction

### 🧪 Gyakorlat:

* Készíts egy **mobil checkout flow-t** 4 képernyővel, interakciókkal
* Építs user flow diagramot külön frame-ekkel

### 🧠 Tipp:

* Használj [FigJam](https://www.figma.com/figjam/) a user journey-k, wireframe-k gyorsabb feldolgozásához – sticky notes, flow arrows, feedback sessionök

---

## ✅ **5. nap – Kollaboráció, dokumentáció, skálázás**

**🎯 Cél:** Csapatmunkára, dokumentációra és prezentációra való felkészülés

### 📘 Elmélet:

* Figma-csapatstruktúrák (Team, Project, File, Page)
* Verziókövetés, megjegyzések, Review módszerek
* Dokumentálás: *Component Description*, *Usage Guides*, *UX Copy*

### 🧪 Gyakorlat:

* Dokumentáld a gomb-komponens rendszered használatát
* Készíts **handoff-ready** UI tervet fejlesztőknek (Inspect panel, CSS export)
* Használj [Zeroheight](https://zeroheight.com/) vagy [Notion](https://www.notion.so/) Figma-integrációt dokumentációhoz

### 🧠 Továbbfejlesztés:

* Figma → code export: [Anima](https://www.animaapp.com/), [Locofy](https://www.locofy.ai/), [Builder.io](https://www.builder.io/)
* Pluginok: [Design Lint](https://www.figma.com/community/plugin/801195587640428208/design-lint), [Content Reel](https://www.figma.com/community/plugin/731627216655469013/Content-Reel)

---

## 📍 **Kiemelt koncepcionális alapelvek, amelyek a Figma előnyeit adják:**

| Fogalom                 | Adobe megfelelő             | Figma előnye                        |
| ----------------------- | --------------------------- | ----------------------------------- |
| `Component`             | Smart Object                | Öröklődés, Variánsok                |
| `Auto Layout`           | Nincs igazán                | Responsív design, mint CSS Flexbox  |
| `Design Token`          | Custom styles               | JSON export, platformfüggetlenség   |
| `Library`               | Shared Assets               | Live sync, frissítés push           |
| `Instance`              | Layer Copy                  | Linkelt, módosítható példány        |
| `Prototype`             | Photoshop animation vagy XD | Komplett flow, UX demo              |
| `Interactive Component` | Nincs                       | Állapotváltás egy komponensen belül |

---

## 🎓 Továbblépési javaslatok:

* 🌱 [Figma’s Learn Hub](https://help.figma.com/hc/en-us/categories/23557013073047-Courses-tutorials-projects) (ingyenes képzések)
* 💡 [Design Course on Design Systems](https://www.designsystems.com/)
* 🧩 Plugin fejlesztés: [Figma Plugin API](https://www.figma.com/plugin-docs/intro/)

---
