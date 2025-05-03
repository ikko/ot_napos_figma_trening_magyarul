# Fejlesztői Handoff-ready Layout

Remek választás! Egy **handoff-ready layout** elkészítése kiváló gyakorlat a CDD, a design system használat, az Auto Layout és a fejlesztői átadás (Inspect) készségek integrálására. Végigvezetlek egy **konkrét példán**, miközben közösen építjük fel a struktúrát.

---

## 🎯 **Példa: Bejelentkezési képernyő (Login UI) – fejlesztői handoff-ready layout**

Ez a UI a következő elemekből áll:

* App logó
* Címsor („Jelentkezz be”)
* E-mail input mező
* Jelszó input mező
* „Elfelejtetted a jelszavad?” link
* Bejelentkezés gomb
* Választó komponens (pl. „Vagy jelentkezz be Google-lel”)

---

## 🧱 **1. lépés: Atomi komponensek elkészítése**

📂 Figma `Design System/Atoms` page

### ① `btn/primary`

* Variants: `default`, `hover`, `disabled`
* Méretek: `small`, `medium`, `large`
* Auto Layout: vertical padding + text center

### ② `input/text`

* Label (Text Style)
* Input mező (rectangle + placeholder text)
* Hibaüzenet (opcionális text below)

### ③ `typography`

* H1: 32px bold
* Body: 16px regular
* Caption: 12px, grey600

---

## 🧩 **2. lépés: Molekulák kombinálása**

📂 Figma `Design System/Molecules` page

### `input/with-label`

* Label + Input mező vertikálisan
* Auto Layout vertical, spacing 8px
* Property: `error: true/false`

---

## 🧩 **3. lépés: Organismus komponens**

📂 Figma `Design System/Organisms` page

### `form/login`

* Címsor (`H1`)
* 2 db input/with-label komponens
* „Elfelejtetted?” szöveg, jobbra igazítva
* `btn/primary` komponens
* Divider + 3rd party login gomb

Auto Layout → vertical flow, spacing 24px

---

## 🧰 **4. lépés: Template és Page**

📂 Figma `Templates/Login Page Template`

* Fejléc nélkül
* Középre igazított login blokk (form/login organism)
* 375px (mobile), 768px (tablet), 1440px (desktop)

📂 Figma `Pages/Login Page`

* Végleges példányokból összeállított mockup
* Ne tartalmazzon `Detach`-elt példányokat!

---

## 🔄 **5. lépés: Handoff előkészítés**

✅ **Inspect-ready layout ellenőrzőlista:**

* Minden szöveg `Text Style`-hoz kötött?
* Minden szín `Color Style`-ból jön?
* Minden komponens `Instance`?
* `Auto Layout` használat minden groupban?
* Minden elemen `Constraints` beállítva (responsive)?

✅ **Előnézet:**

* Váltás `Prototype` módra → interakció hozzáadása: `login btn → success screen`

✅ **Kommentek fejlesztőknek:**

* „Ez a mező validálható inputot tartalmaz, regex: email format”
* „A bejelentkezés gomb disabled állapotban inaktív”

---

## 📦 **Export és fejlesztői átadás:**

1. Nyisd meg a végleges UI page-et
2. Válaszd ki a fő `Frame`-et (pl. LoginPage/Desktop)
3. Jobb oldalon válaszd az `Inspect` panelt
4. A fejlesztők látják a:

   * CSS értékeket
   * Padding, margin, font, színstílus
   * Exportálható ikonokat SVG-ben

---


