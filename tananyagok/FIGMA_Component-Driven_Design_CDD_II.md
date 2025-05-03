[Design System Figma Template](https://old.sermitsiaq.ag/en/design-system-figma-template.html)

Kiváló döntés, hogy szeretnél egy **Component-Driven Design (CDD)** alapú mini design system sablont Figma-ban. Ez a megközelítés lehetővé teszi a felhasználói felületek moduláris, újrahasználható és könnyen karbantartható komponensekbe szervezését. Az alábbiakban bemutatok egy részletes útmutatót a sablon felépítéséhez, valamint hasznos forrásokat és példákat a gyakorlati megvalósításhoz.

---

## 🧱 **Component-Driven Design alapú mini design system sablon Figma-ban**

### 1. **Atoms (Atomok)**

Az atomok a legkisebb, önállóan nem bontható UI-elemek, mint például:

* **Gombok**: Alapértelmezett, hover és inaktív állapotokkal.
* **Űrlapmezők**: Szövegmezők, jelölőnégyzetek, rádiógombok.
* **Tipográfiai elemek**: Címsorok, bekezdések, címkék.
* **Ikonok**: Navigációs és műveleti ikonok.([Figma Vezérlőpult, Sablon és UI Készletek - UI Kits][1])

Használj **Variants**-ot az állapotok és méretek kezelésére, valamint **Auto Layout**-ot a dinamikus elrendezéshez.

### 2. **Molecules (Molekulák)**

A molekulák olyan összetett elemek, amelyek több atomot kombinálnak egy funkcionális egységbe:

* **Űrlapmező címkével**: Szövegmező és hozzá tartozó címke.
* **Keresősáv**: Szövegmező és keresés ikon kombinációja.
* **Kártya komponens**: Kép, cím és leírás együttese.

Ezeket is alakítsd komponensekké, és alkalmazz **Auto Layout**-ot a belső elrendezéshez.

### 3. **Organisms (Organizmusok)**

Az organizmusok nagyobb, összetett UI-szekciók, amelyek több molekulát és atomot tartalmaznak:

* **Fejléc**: Logó, navigációs menü és keresősáv.
* **Lábléc**: Kapcsolati információk, hivatkozások és közösségi média ikonok.
* **Termékkártya lista**: Több kártya komponens egymás mellett.

Ezeket a komponenseket is szervezd logikusan, és alkalmazz **Auto Layout**-ot a rugalmas elrendezés érdekében.

### 4. **Templates (Sablonok)**

A sablonok meghatározzák az oldalak szerkezetét, elrendezését, és tartalmazzák az organizmusokat:

* **Főoldal sablon**: Fejléc, fő tartalom és lábléc.
* **Termékoldal sablon**: Termékkép, leírás, ár és vásárlási lehetőségek.
* **Kapcsolat oldal sablon**: Űrlap, térkép és elérhetőségek.

A sablonok segítségével gyorsan létrehozhatók az oldalak, miközben biztosítják a konzisztens elrendezést.

### 5. **Pages (Oldalak)**

Az oldalak a sablonok konkrét példányai, valós tartalommal feltöltve:

* **Főoldal**: Aktuális promóciókkal és kiemelt termékekkel.
* **Termékoldal**: Egy adott termék részletes bemutatása.
* **Kapcsolat oldal**: Kapcsolati űrlap és céginformációk.

Az oldalak segítségével tesztelheted a design rendszer működését valós környezetben.

---

## 📂 **Figma fájlstruktúra javaslat**

Javasolt a következő struktúra alkalmazása a Figma fájlban:

```
📁 Design System/
├── Atoms/
│   ├── Buttons
│   ├── Inputs
│   └── Typography
├── Molecules/
│   ├── Form Fields
│   └── Cards
├── Organisms/
│   ├── Header
│   └── Footer
├── Templates/
│   ├── Home Page
│   └── Product Page
└── Pages/
    ├── Home
    └── Product
```

Ez a struktúra segít a komponensek logikus szervezésében és könnyű megtalálásában.

---

## 🔗 **Hasznos források és példák**

* **Figma Atomic Design Systems példa**: Részletes útmutató és példák az atomi design rendszer kialakításához Figma-ban.&#x20;

* **Atomic Design rendszer Figma-ban**: Gyakorlati példák és sablonok az atomi design rendszer megvalósításához.&#x20;

* **Figma sablonok és UI készletek**: Számos ingyenes sablon és UI készlet a Figma közösségétől. ([Figma Sablon Galéria][2])

---

[1]: https://www.setproduct.com/?utm_source=chatgpt.com "Figma templates, design systems and UI kits"
[2]: https://www.figma.com/templates/?utm_source=chatgpt.com "Explore 300+ free design and white board templates - Figma"

---
