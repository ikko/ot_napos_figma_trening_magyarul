Nagyszerű döntés – a **Component-Driven Design (CDD)** a modern UI/UX és frontend fejlesztés egyik legmeghatározóbb szemlélete. Mélységeiben átlátva nemcsak hatékonyabban fogsz tervezni Figma-ban, hanem **skálázhatóbb, újrahasználhatóbb, dokumentálhatóbb design rendszerek** kialakítására is képes leszel.

---

## 🔍 **Mi az a Component-Driven Design (CDD)?**

A Component-Driven Design egy olyan megközelítés, amelyben a felhasználói felületet **kisebb, független, újrahasználható komponensekre** bontjuk, majd ezekből építjük fel a komplex UI-t.

Ez a gondolkodásmód a **frontend fejlesztésből** (React, Vue, Angular) ered, de a **design rendszerek és Figma** világába is tökéletesen átültethető.

---

## 🧱 **CDD alapelvei (és párhuzamok Figma világában)**

| CDD fogalom              | Fejlesztői analógia          | Figma-beli megfelelő     |
| ------------------------ | ---------------------------- | ------------------------ |
| Atomok (Atoms)           | HTML elemek (pl. `<button>`) | `Component`: Button base |
| Molekulák (Molecules)    | Kombinált UI elemek          | Input field + Label      |
| Organizmusok (Organisms) | Komplett UI blokkok          | Search bar, Card list    |
| Templates                | Layout sablon                | Wireframe + Auto Layout  |
| Oldalak (Pages)          | Végső nézet                  | Mockup screen            |

> 📖 Ez az elmélet [Atomic Design](https://bradfrost.com/blog/post/atomic-web-design/) néven is ismert, és a CDD egyik legjobb gyakorlata.

---

## 📁 **CDD Figma-ban lépésről lépésre**

### 🧩 1. **Tervezd meg az alap komponenseket (Atoms)**

Pl.: Button, TextField, Label, Icon, Avatar

#### Példa:

* `btn/primary/medium`
* `icon/arrow-right`
* `typography/h1`

🎯 Használj **Variants**-ot az állapotok (pl. hover, pressed) és méretek kezelésére.

---

### 🧩 2. **Kombináld őket összetett elemekké (Molecules)**

Pl.: Labeled Input Field, Button with Icon, Dropdown Menu

#### Példa:

* `input/with-label`
* `dropdown/select/with-icon`

🎯 Használj `Auto Layout`-ot a dinamikus elrendezéshez.

---

### 🧩 3. **Szervezz UI blokkokat (Organisms)**

Pl.: Navigációs sáv, termékkártya, kosár widget

#### Példa:

* `card/product/compact`
* `header/main`
* `search-bar/with-filters`

🎯 Ezek már összetettek, de tartalmazhatnak instanciákat (molekulákból).

---

### 🧩 4. **Készíts sablonokat (Templates)**

Sablonoldalak egy adott típusú felhasználói élményhez

Pl.: Checkout page, Product detail, User profile

🎯 Használd: `Auto Layout` + `Constraints` + `Components` a dinamikus oldalszerkezethez.

---

### 🧩 5. **Alkosd meg a végleges képernyőket (Pages)**

Ez a végleges UI mockup (design delivery/hand-off célokra).

🎯 Ezek ne tartalmazzanak már kézi rajzolású UI elemeket — csak komponens példányokat (`Instance`).

---

## 🧠 **CDD előnyei**

* ✅ Könnyen karbantartható
* 🔁 Újrahasználható komponensek
* 🧪 Egységenként tesztelhető (akár UI-tesztekhez is)
* 📐 Rendszerszemléletet kényszerít ki
* 🧩 Könnyű fejlesztői átadás (strukturált Inspect panel)

---

## 🎓 **CDD gyakorlat Figma-ban – példa struktúra**

```plaintext
📁 Design System/
   ├── Atoms/
   │   ├── Button
   │   ├── Text Field
   │   └── Typography
   ├── Molecules/
   │   ├── Input + Label
   │   └── Search Bar
   ├── Organisms/
   │   ├── Product Card
   │   └── Header
   ├── Templates/
   │   └── Product Detail Template
   └── Pages/
       └── Product Detail Final UI
```

Minden elem `Component` vagy `Instance`. Variánsokat `Property` struktúrával érdemes kezelni:

```plaintext
btn/primary → size: small | medium | large
            → state: default | hover | disabled
```

---

## 🔧 **Ajánlott Pluginok és technikák**

* **[Figma Tokens](https://www.figma.com/community/plugin/843461159747178978/Tokens-Studio-for-Figma)** – tokenizált design elemek
* **[Instance Finder](https://www.figma.com/community/plugin/741895659787979282/instance-finder)** – hol van használatban egy komponens
* **Auto Layout v5** – padding, gap, direction (mint flexbox!)
* **Interactive Components** – állapotváltás interakció alapján

---


