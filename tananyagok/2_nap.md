Nagyszerű, merüljünk el a **második nap** teljes tananyagában, amelynek középpontjában a **komponens-alapú gondolkodás, a variánsok kezelése és az „öröklődés-szerű” viselkedések** állnak. Ez a nap képezi az alapját a **design rendszerek** megértésének és skálázásának.

---

# 📘 **2. nap – Komponensek, Variánsok és Strukturált UI újrahasznosítás Figma-ban**

### 🎯 **A nap célja:**

Megérteni és tudatosan alkalmazni a Figma egyik legerősebb funkcióját: **komponensek (components), példányok (instances) és variánsok (variants)** használatát úgy, hogy képes legyél egy UI-építőelemet többféle állapotban és kontextusban **karbantarthatóan és örökölhető módon** felhasználni.

---

## 📖 **1. Elméleti bevezetés – Figma komponensek filozófiája**

### 🔹 1.1. Mi az a **Component**?

* Egy UI-elem „forrásmintája” (master/origin), amelyből példányok (instance-ek) készülnek.
* Úgy viselkedik, mint egy **OOP osztály**, amelyből példányosítani lehet – változtathatsz rajta lokálisan, de örökli az alap logikát.

### 🔹 1.2. Mi az az **Instance**?

* Egy adott komponens példánya, amelyet egy konkrét UI képernyőre helyezel ki.
* Megváltoztathatsz benne bizonyos értékeket (szöveg, ikon), de az alapszerkezet a fő komponenshez kötött.

### 🔹 1.3. Mi az a **Variant**?

* Egy komponens többféle **állapotának vagy konfigurációjának strukturált egyesítése**.
* Pl. egy gomb: `primary`, `secondary`, `disabled` → egy `Button` komponens három variánssal.

---

## 🧠 **2. Koncepcionális modellek, amik a Figma-t kiemelik:**

| Fogalom           | Rövid leírás           | Analógia         |
| ----------------- | ---------------------- | ---------------- |
| Component         | Alap UI egység         | OOP osztály      |
| Instance          | Példányosított elem    | Objektum         |
| Nested Component  | Beágyazott komponens   | Kompozíció       |
| Variant           | Állapot, opció gyűjtés | Enum / paraméter |
| Property override | Lokális módosítás      | Argumentum       |

📌 **Tipp**: Ezek együtt képezik a Figma **öröklődés-szerű rendszerét**, amely hasonlít az Adobe Smart Object-hez, de **sokkal mélyebben szabályozható, struktúrált és skálázható**.

---

## 🧪 **3. Gyakorlati rész – Feladatok**

### ⚙️ **3.1. Button-rendszer építése (Variants)**

**Feladat:**
Készíts egy `Button` komponenst a következő tulajdonságokkal:

* **3 méret**: `Small`, `Medium`, `Large`
* **2 szín**: `Primary`, `Secondary`
* **3 állapot**: `Default`, `Hover`, `Disabled`

#### Lépések:

1. Hozd létre az első `Button` komponenst egy Auto Layout-tal (padding, spacing, szöveg).
2. Duplikáld és alakítsd ki a többi állapotot.
3. Jelöld ki az összes változatot, és alakítsd őket egy `Component Set`-té (jobbkatt > Combine as Variants).
4. Nevezd el a variánsokat így:
   `Size=Small`, `Type=Primary`, `State=Hover` stb.
5. Használj **Property controls**-t: állítható dropdown a UI-ban.

📎 [Figma Tutorial: Variants](https://help.figma.com/hc/en-us/articles/360056440594-Create-and-use-variants)

---

### ⚙️ **3.2. Input mező család (Nested Components)**

**Feladat:**
Készíts egy `Input Field` családot a következő logikával:

* Tartalmazzon:

  * Label (felirat)
  * Input mező
  * Hibaüzenet (hiba állapot esetén)
  * Ikon (opcionális, jobb oldalt)
* Legyen két változat: `Standard` és `Error`

#### Lépések:

1. Készíts külön komponenseket a `Label`, `Input`, `Error Message`, `Icon` elemekből.
2. Kombináld ezeket egy **Parent Component**-be `Auto Layout`-tal.
3. Készíts `Variant`-okat: pl. `State=Default` és `State=Error`.
4. Mutasd/eltüntesd az `Error Message` elemet conditional visibility-vel.

📎 TIPP: A `Component inside Component` = **"Nested Component"**, ami örökli a belső viselkedéseket.

---

## 🧩 **4. Plugin és haladó tippek**

### 🔌 Ajánlott pluginok:

* [**Instance Finder**](https://www.figma.com/community/plugin/1111463131251015674/Instance-Finder): Mutatja, hol használtad fel a komponens példányokat
* [**Similayer**](https://www.figma.com/community/plugin/738454987945972471/Similayer): Rétegek kiválasztása stílus/név alapján
* [**Design Lint**](https://www.figma.com/community/plugin/801175210412417057/Design-Lint): Hibák keresése design token szinten

---

## 🎓 **5. Összefoglalás & kérdések önellenőrzéshez**

### ❓ Kérdések:

* Mi a különbség egy component és egy instance között?
* Milyen eszközöket kínál a Figma a komponensvariációk kezelésére?
* Milyen módon érdemes strukturálni egy input mező komponenscsaládot?
* Milyen esetekben célszerű nested komponenseket használni?

### ✅ Mini recap feladat:

* Készíts egy új UI elemet (pl. kártya komponens) 2 variánssal: `With Image` és `Without Image`
* Használd `Boolean property`-t az image megjelenítésének vezérléséhez

---

## 📌 **Másnapi előkészület (3. nap):**

* Készülj fel egy teljes **mini design system** felépítésére az eddigi komponensekből
* Vezess be színsémát, betűtípus rendszert, spacing skálát

---

