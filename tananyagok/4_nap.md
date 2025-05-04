Rendben, az alábbiakban megtalálod a **4. nap** részletes, oktatási célú tananyagát, fókuszálva a **Figma prototípus-készítés**, **user flow modellezés**, valamint az **interaktív viselkedések** gyakorlati alkalmazására. Az anyag úgy épül fel, hogy:

1. Bevezet az elméleti alapokba
2. Lépésről lépésre halad a gyakorlati példán
3. Kiemel advanced koncepciókat (animáció, overlay, variant-interakciók)
4. Részletes példán mutatja be a **felhasználói útvonalak vizualizálását**

---

# 🎯 **4. nap: Prototípus készítés & User Flow Modellezés Figmában**

---

## 🧠 **Célkitűzés**

* Megérteni, hogyan lehet egy alkalmazás vagy weboldal **felhasználói élményét (UX)** prototípus formájában tesztelhetővé és bejárhatóvá tenni Figma segítségével.
* Megtanulni az **interakciók, állapotváltások, modális megjelenések**, és navigációs útvonalak vizualizálását.
* Létrehozni egy **kattintható UX prototípust**, amely képes modellezni a felhasználói útvonalakat (user journey).

---

## 📘 **1. Elméleti megalapozás – Figma prototípus alapfogalmak**

### 🔹 **Alapfogalmak**

| Fogalom                 | Jelentés                                                                                |
| ----------------------- | --------------------------------------------------------------------------------------- |
| **Prototype mode**      | A Figma felső paneljében váltható mód, amely lehetővé teszi az interakciók definiálását |
| **Interaction**         | A komponens vagy frame viselkedése kattintásra, hover-re, stb.                          |
| **Flow Starting Point** | A kezdőképernyő (→ prototípus futtatás innen indul)                                     |
| **Overlay**             | Olyan panel vagy modal, ami a meglévő képernyő fölött jelenik meg (pl. beállítások)     |
| **Swap Variant**        | Variáns cseréje adott interakció hatására                                               |
| **Smart Animate**       | Intelligens animáció a változások között (ha van közös layer/név)                       |

### 🧩 **Interakció típusok példákkal**

| Esemény (Trigger) | Viselkedés (Action) | Példa                                  |
| ----------------- | ------------------- | -------------------------------------- |
| On Click          | Navigate to frame   | "Tovább" gomb → Következő képernyő     |
| On Click          | Open overlay        | "Profil ikon" → Popup panel            |
| On Hover          | Change to variant   | Hover állapot gomboknál                |
| After Delay       | Auto navigate       | Splash screen automatikus továbblépése |
| While Pressing    | Smart animate       | Gomb lenyomása alatt animáció          |

---

## 🧪 **2. Gyakorlati projekt – Mobilos Checkout Flow prototípus**

### 🎯 **Cél:** Készíts egy 4 képernyős mobil prototípust:

1. **Product list**
2. **Product detail**
3. **Cart**
4. **Checkout confirmation**

### 🛠️ **Lépések**

#### 1. **Frame-ek elkészítése** (`Frame Tool` `F`)

* Használj `iPhone 13 Pro` méretet (390x844px)
* Adj minden képernyőnek nevet (`Product List`, `Detail`, stb.)
* Helyezz el UI elemeket: title, card, gomb, ár, ikon

#### 2. **Komponensek alkalmazása**

* Használj meglévő vagy saját gomb-komponenseket
* Használj `Variants`-et: pl. gomb: `default`, `hover`, `disabled`

#### 3. **Prototype kapcsolatok beállítása**

* Váltás `Prototype mode`-ba (felső panel `Design` → `Prototype`)
* Húzz nyilakat a gombokról a megfelelő képernyőre
* Beállítások:

  * **On Click → Navigate To → Destination Frame**
  * `Smart Animate` animáció típusként

#### 4. **Overlay használata**

* Készíts egy `Cart overlay` Frame-et (pl. mini kosár)
* Beállítás:

  * `On Click → Open Overlay`
  * Pozíció: `Center` vagy `Manual`
  * Animáció: `Move in`, `Slide in`, vagy `Instant`

#### 5. **Interaktív komponens**

* Változtasd meg a "Buy" gombot `On Hover` esetén (`Change to variant`)

#### 6. **Start point beállítása**

* Válaszd ki az első frame-et (Product list)
* Kattints a kis „play” ikonra `Set as starting frame`

---

## 🧭 **3. User Flow vizualizálása FigJam vagy Figma segítségével**

### 🧩 **Figma User Flow modellezési módszerek**

* Hozz létre külön frame-eket, amelyek csak ikonokat, lépéseket, döntéseket tartalmaznak
* Használj nyilakat (`Shift + Arrow`) és `Flow starting point`-okat
* Adj hozzá szövegdobozokat: "User clicks", "System response"

### ✍️ **Alternatíva: FigJam**

* Használj [FigJam](https://www.figma.com/figjam/) rajztáblát a journey vizualizálására:

  * Sticky notes = felhasználói cél
  * Arrows = lépések
  * Sections = képernyők
  * Emojik, kommentek = feedback fázis

---

## 🧠 **4. Haladó: Állapotváltás komponensen belül – Interaktív komponensek**

Az **Interactive Components** lehetővé teszi, hogy **egy komponensen belül definiálj interakciókat** (pl. toggle switch, accordion, checkbox viselkedés).

### 🔧 Példa: Checkbox

* Hozz létre egy `Checkbox` komponenst
* Készíts két `variant`-ot: `unchecked`, `checked`
* Válts `Prototype` módba, állítsd be:

  * `On Click → Change to → Checked`
  * `Smart Animate` → 200ms

Ezzel nem kell minden képernyőn külön prototípus nyilat húzni – a viselkedés önmagában hordozódik.

---

## 🧰 **Eszközök és Pluginok**

| Eszköz                                                                                    | Mire jó                                           |
| ----------------------------------------------------------------------------------------- | ------------------------------------------------- |
| [Smart Animate](https://help.figma.com/hc/en-us/articles/360039818874-Smart-animate-layers-between-frames)                    | Animált frame váltás komponensnév egyezés alapján |
| [Figmotion](https://www.figma.com/community/plugin/733025261168520714/Figmotion)          | Haladó animáció (mint After Effects)              |
| [Flowkit](https://useflowkit.com/)                        | Előre gyártott user flow ikonok, sablonok         |
| [User Flows plugin](https://www.figma.com/community/diagramming/flowcharts?resource_type=mixed&editor_type=figjam&price=all&sort_by=all_time&creators=all) | Flow modellezés gyors nyilazással                 |

---

## 📈 **Feladat: Mobil Checkout Prototípus**

### 📋 Követelmények:

* Legalább 4 képernyő
* Minden gombnak interaktív funkciója legyen
* Legalább 1 overlay
* 1 interaktív komponens (pl. checkbox, switch)

### 🎥 Tesztelés:

* Kattints a „Present” gombra (felső jobb sarok)
* Nézd meg, hogy a flow logikusan működik-e
* Oszd meg URL-en: teszteléshez, stakeholder review-hoz

---

## 📚 **Végszó – Mit tanultunk ma**

✅ Dinamikus prototípus készítés alapjait
✅ Interakció típusokat és azok UX jelentőségét
✅ Overlay használatot és user journey vizualizálást
✅ Interaktív komponensek elvét, öröklés-szerű viselkedést
✅ Prezentációs és dokumentációs lépéseket fejlesztői Handoff-hoz

---

