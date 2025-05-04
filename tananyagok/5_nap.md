Nagyszerű — az ötödik nap kulcsfontosságú, mert itt találkozik a **professzionális workflow** a **csapatmunkával, dokumentációval és skálázhatósággal**. Ezt a tudást keresik a közép- és nagyvállalati UX/UI állásoknál, különösen akkor, ha design system-mel vagy más csapattagokkal (pl. fejlesztőkkel, product ownerrel) dolgozol együtt.

---

# ✅ **5. nap – Kollaboráció, dokumentáció és skálázható munkafolyamatok Figma-ban**

---

## 🎯 **Napi célkitűzések:**

* Megtanulni, hogyan lehet a design munkát hatékonyan dokumentálni, verziózni és fejlesztőkkel átadni
* Elsajátítani a **komponensszintű dokumentációt**
* Felkészülni **design system** dokumentációra és karbantartásra
* Megismerni a **csapatmunkát támogató Figma-struktúrákat és workflow-kat**

---

## 📘 **1. Elmélet: kollaboráció és workflow alapok**

### 🔹 **Figma struktúra:**

* **Team → Project → File → Page** – hasonló mint GitHub → Repo → Branch → Commit
* Minden entitás megosztható különböző permission szintekkel: view, edit, comment
* **Comment mode**: stakeholder review, issue tracking designban
* **Version history**: minden mentés időbélyeggel visszanézhető, összehasonlítható

### 🔹 **Dev handoff (fejlesztői átadás):**

* `Inspect` panel: CSS, iOS, Android értékek automatikusan generálva
* Tokenek és gridek is átvihetők fejlesztésre (ha jól strukturált a fájl!)
* Exportálható SVG, PNG, PDF + rendkívül pontos layout méretek

---

## 🧪 **2. Gyakorlat: egy design rendszer dokumentálása**

### 🎯 Feladat:

Dokumentálj egy meglévő UI komponenst (pl. `Primary Button`) a következő elemekkel:

#### 📌 **Dokumentációs tartalom** (komponens saját `page`-én vagy külön file-ban):

* **Leírás**: mikor használandó (pl. primer akciókhoz)
* **Állapotok**: default, hover, disabled (→ Variants használata)
* **Méretek**: small, medium, large
* **Használati példák**: valós layoutban
* **Do & Don't példák** (pl. színválasztás, elhelyezés)
* **Design tokenek**: `btn-primary-bg`, `btn-primary-text`, stb.

### ➕ Haladó:

* Készíts külön `Page`-et: `Documentation`
* Adj hozzá `Text` és `Annotation` blokkokat a frame-eken belül
* Használj `Section`-öket a logikai elválasztáshoz (új Figma feature!)

---

## 🔧 **3. Automatizált dokumentációs eszközök**

### ✨ **Zeroheight**

* Cél: Figma file-ból automatikusan generált web-alapú design system dokumentáció
* Fő előny: nem designerek is könnyen olvassák

🔗 [Zeroheight integráció](https://zeroheight.com/help/figma/)

### ✨ **Notion + Figma Embed**

* Notion oldalon embed-eld a Figma komponensfile-okat `Public link` használatával
* Kombinálható UX copy, user journey, A/B teszteredményekkel

---

## 🔄 **4. Verziózás és fájlstruktúra stratégiák**

### 💼 **Projektstruktúra javaslat**:

```
Design System/
  ├─ Colors & Typography
  ├─ Buttons
  ├─ Forms
  ├─ Layout
  └─ Components Documentation

Projects/
  ├─ Mobile App
  ├─ Marketing Website
  └─ Admin Dashboard
```

### 💡 **Naming konvenció**:

* `btn/primary/small/default`
* `form/input/text/active`
* Segíti a keresést és tokenizálást

---

## 🤝 **5. Developer handoff workflow (demo)**

1. Készítsd el a `Frame`-et komponensekkel és stílusokkal
2. Jelöld ki a `Frame`-et → Inspect panel (Jobb oldal)
3. `Export` → PNG/SVG vagy fejlesztői tool által olvasott metaadatok
4. Adj hozzá **megjegyzéseket** → `C` billentyű (Comment tool)
5. Készíts egy `handoff-ready` oldalt (csak fejlesztőknek) → csak véglegesített UI-kkal

📦 **Pro Tipp**:

* A Figma `Inspect` panel automatikusan konvertál:

  * színt: HEX, RGB, HSL
  * szöveget: font-family, weight, line-height
  * box modelt: padding, margin

---

## 🧠 **Koncepcionális reflektív zárás (Deep Thinking)**

### ❓ Mit tanultál?

* A Figma nem csak design eszköz, hanem *strukturált dokumentációs és kollaborációs platform*
* A komponensek és design tokenek révén **öröklődő és skálázható** rendszerek építhetők
* A csapatmunkához szükséges minden eszköz és workflow natívan elérhető

---

## 🚀 **Haladó tanulási útvonal innen tovább:**

* 🔄 **DesignOps gondolkodásmód**: [DesignOps Handbook (InVision)](https://www.scribd.com/document/429768921/InVision-DesignOperationsHandbook-pdf)
* ⚙️ **Component Driven Design**: [Atomic Design – Brad Frost](https://bradfrost.com/blog/post/atomic-web-design/)
* 📚 **Figma plugin fejlesztés**: [Plugin API Docs](https://www.figma.com/plugin-docs/intro/)
* 📡 **Figma → Code Bridge**:

  * [Locofy.ai](https://www.locofy.ai/) – React export
  * [Anima](https://www.animaapp.com/) – Tailwind export
  * [Figma Tokens plugin](https://www.figma.com/community/plugin/843461159747178978/Tokens-Studio-for-Figma)

---

