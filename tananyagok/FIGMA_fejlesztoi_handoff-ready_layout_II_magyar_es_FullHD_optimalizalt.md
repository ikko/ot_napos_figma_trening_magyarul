Tökéletes! Most egy **Figma-alapú, fejlesztői handoff-ready Login UI-t** fogunk közösen elkészíteni, **magyar nyelven**, **FullHD alapon**, de **teljesen reszponzív**, azaz **mobil, tablet és 4K képernyőkre optimalizált** formában.

## 🎯 Cél:

* CDD szerkezet szerint: Atoms → Molecules → Organisms → Template → Page
* Reszponzív, Auto Layout + Constraints segítségével
* Inspect-használatra kész, fejlesztők által olvasható, dokumentált komponensekkel

---

## 🧱 1. lépés: Atomi komponensek definiálása

📍 **Atoms oldal** – Hozzunk létre egy külön `Page`-et: `Atoms`

### 🧩 `btn/primary`

* **Szöveg**: „Bejelentkezés”
* **Auto Layout**: vertical padding = 16px, horizontal padding = 24px
* **States**: `default`, `hover`, `disabled`
* **Text Style**: 16px, bold, white
* **Background Color Style**: `primary/600` (#0047AB)

### 🧩 `input/base`

* **Placeholder**: „Add meg az email címed”
* **Rectangle**: 100% width, height: 48px, border-radius: 8px
* **Border Color Style**: `gray/300`, on hover: `gray/500`
* **Label text**: 14px, regular
* **Hint text**: 12px, gray600

> 📌 Ezeket Variants segítségével tedd komponenssé: `default`, `focused`, `error`.

---

## 🧪 2. lépés: Molekulák építése

📍 **Molecules oldal** – `Page`: `Molecules`

### 🧬 `input/with-label`

* Label (pl. „Email cím”)
* Base input komponens (Instance)
* Hint text vagy error message

Használj `Auto Layout` vertical spacing: 8px

### 🧬 `divider/with-text`

* Vízszintes vonal – középen szöveg: „vagy jelentkezz be Google-lel”
* Auto Layout horizontal, center

---

## 🧩 3. lépés: Organizmus komponens

📍 **Organisms oldal** – `Page`: `Organisms`

### 🧬 `form/login`

* `H1`: „Lépj be a fiókodba”
* `input/with-label` (email)
* `input/with-label` (jelszó)
* `link` (Elfelejtetted a jelszavad?)
* `btn/primary` (Bejelentkezés)
* `divider/with-text`
* `btn/secondary` (Google-gomb)

Auto Layout:

* Direction: vertical
* Spacing: 24px
* Width: 100%
* Padding: 32px

---

## 🧰 4. lépés: Template és Page

📍 **Templates** → `login-template`

* Layout frame: 1440x1024 (FullHD base), használj `Layout Grid` (12-oszlopos, 8px gutter)
* Középen elhelyezett `form/login` komponens (organism)

📍 **Pages** → `login-final-ui`

* Responsive Frames:

  * `Mobile (375x812)`
  * `Tablet (768x1024)`
  * `FullHD (1440x1024)`
  * `4K (2560x1440)`

A layoutot `Auto Layout` + `Constraints` segítségével alakítsd ki, pl.:

* Form középen
* Responsive padding (mobilon kisebb)
* Szélesség max 480px-en belül

---

## 📝 5. lépés: Dokumentáció & Dev handoff

📍 **Page**: `Documentation & Handoff`

* Minden komponenshez írd oda:

  * Mikor használandó
  * Variánsok leírása
  * Exportálható ikonok SVG-ben
* Adj meg kommenteket (`C` → comment tool)
* Ellenőrizd, hogy `Inspect` panelben:

  * minden szöveg style-hoz kötött
  * színek tokenből jönnek
  * komponensek instance-ok
  * Auto Layout mindenütt aktív

---

## ➕ Mit csinálok most?

Mivel jelenleg nem tudok közvetlen `.fig` fájlt szerkeszteni valós időben, a következőt javaslom:

- **Te készíted el a .fig sablont, én real-time vezetlek benne**

   * Megnyitod a Figma-t
   * Írom soronként, mit csinálj, hogyan állítsd be az Auto Layout-ot, Token-eket, Variánsokat
