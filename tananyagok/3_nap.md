Rendben, elkészítem a **3. nap** részletes tananyagát a **Design Rendszerek és Skálázhatóság** témában. Ez a nap alapozza meg azt a szemléletet, amellyel **nagyvállalati szintű, fenntartható, újrahasznosítható és dokumentálható** UI rendszereket tudsz építeni. Ez kulcskompetencia minden erős UX/UI pályázatban.

---

# ✅ **3. Nap – Design Rendszerek és Skálázhatóság a Figma-ban**

## 🎯 **Napi célkitűzések**

* Megérted a design rendszer alapelemeit és működését.
* Elsajátítod, hogyan építhetsz újrahasznosítható, hierarchikus rendszereket Figma-ban.
* Képes leszel egy mini design system struktúra felépítésére (tipográfia, színek, komponensek, layout).
* Megtanulod a token-alapú tervezés gondolkodásmódját.

---

## 🧠 **I. Elmélet: Mi az a design rendszer?**

### 🔹 A design rendszer (Design System) összetevői:

1. **Visual Style Guide** – színek, betűk, térközök
2. **Komponens könyvtár (Component Library)** – újrahasználható UI elemek
3. **Dokumentáció** – használati szabályok, példák, UX szövegek
4. **Design Tokens** – centralizált változók, exportálhatók fejlesztéshez

### 🔹 Struktúra Figma-ban:

* **Page** szint: Külön oldalak dokumentációra, UI screenekre, komponensekre.
* **Frame** szint: Egyes layout vagy logikai egységek (pl. gombtípusok).
* **Component + Instance**: Öröklés és újrahasználás alapja.
* **Style-k**: Színek, szövegek, térközök központosított szabályozása.

👉 *Figma alapjaiban nem „layer-first” (mint a Photoshop), hanem **component- és style-first.*** Ez teszi lehetővé a robusztus, skálázható design rendszereket.

---

## 🧪 **II. Gyakorlat: Mini design system készítése**

> ⏱️ **Időkeret:** 2-3 óra | 🎯 *Cél: saját token-vezérelt design system létrehozása*

### 1. **Alap style-ok létrehozása**

* **Színek (Color Styles)**: `Primary / Secondary / Accent / Warning / Surface / Text`
* **Tipográfia (Text Styles)**: `Heading 1–4`, `Body`, `Caption`
* **Spacing scale (nem explicit style, de dokumentálva legyen)**: `4 / 8 / 16 / 24 / 32 px`

### 2. **Token-szerű dokumentáció**

* Frame-ben vizualizáld: színsémák, tipók, layout méretek – mint egy **UI inventory**
* Használj [Tokens Studio](https://tokens.studio/plugin) plugint a tokens JSON exporthoz

### 3. **Komponens könyvtár felépítése**

* **Buttons** (Component + Variants): `Primary`, `Secondary`, állapot: `Default`, `Hover`, `Disabled`
* **Input fields**: `Text`, `Search`, `Textarea`
* **Cards**: Header + content + footer layoutban, Auto Layout + nesting

> 🔄 Mindent komponensként hozz létre, ne egyszeri layerként – ezt várják el a vállalati rendszerekben.

### 4. **Komponens névkonvenció**

Használj **BEM-szerű** vagy fájlrendszer-alapú elnevezést:

* `btn/primary/large`
* `input/text/default`
* `card/with-image`

---

## 🧭 **III. Deep Dive: Hierarchia és öröklődés**

### 🔹 Öröklés logikája:

* Egy **Instance** örökli a **Component** összes tulajdonságát, de lokálisan testreszabható (pl. felirat, ikon).
* Ha frissíted az alap komponenst, minden Instance is automatikusan frissül.

### 🔹 Komponensek egymásba ágyazása:

* Gomb komponens = tartalmazhat egy **Icon** komponenst
* Kártya = tartalmazhat `btn/primary` vagy `btn/link` komponenseket

Ez a **kompozíciós modell** megfelel az objektumorientált rendszerarchitektúra gondolkodásmódjának.

---

## 🔎 **IV. Inspiráció & Iparági példák**

### 🔗 Ipari design system-ek:

* [IBM Carbon](https://carbondesignsystem.com/)
* [Shopify Polaris](https://polaris.shopify.com/)
* [Atlassian Design System](https://atlassian.design/)

### 🎨 Figmában tanulmányozható rendszerek:

* [Material 3 UI Kit (official)](https://www.figma.com/community/file/1035203688168086460/)
* [Ant Design System for Figma](https://www.figma.com/design/dpZfImYKfEEBd42o8nfO4h/Preview---Ant-Design-System-for-Figma-5.24?t=cJHK0Tb3NduEsWjh-0)

---

## 🛠️ **Plugin ajánlások a rendszerépítéshez**

* [Tokens Studio](https://www.figma.com/community/plugin/843461159747178978) – Tokenek kezelése, export
* [Design Lint](https://www.figma.com/community/plugin/801195587640428208/design-lint) – Konzisztencia ellenőrzés
* [Style Organizer](https://www.figma.com/community/plugin/816627069580757929/styles-variables-organizer) – Globális style-ok rendbetétele

---

## 📋 **Zárógyakorlat (30–45 perc)**

**Feladat:** Készíts el egy "Design System Starter" Figma fájlt az alábbi elemekkel:

* 4 szín style
* 3 tipográfia style
* 1 komponens (gomb) 3 variánssal
* 1 kártya Auto Layout-al

**+ Dokumentálás:**

* Szöveges leírás `Description` mezőkben
* Komponens nevek: logikus, skálázható

---

## 🔮 **Továbbfejlődési javaslatok, következő lépések**

* 💡 **Design system dokumentációval** kombinálva: [Zeroheight](https://zeroheight.com/)
* 🎥 **Videók a koncepcióról**:

  * [Build a Design System (1:25)](https://www.youtube.com/watch?v=HNJmWKndUA4)
  * [Learn Figma Auto Layout in 10 Minutes ](https://www.youtube.com/watch?v=To_ADCVSg5g)

---

