# Dokumentation: Webseite „Raubvögel der Schweiz“

---

## 🦅 Übersicht

Diese Dokumentation erklärt den Aufbau und die Funktionsweise der statischen Webseite **„Raubvögel der Schweiz“**. Die Seite wurde als praktische Arbeit im Rahmen einer Ausbildung erstellt und bietet eine übersichtliche, barrierefreundliche und responsive Darstellung von Informationen zu heimischen Raubvögeln – insbesondere **Adlern** und **Falken**.

Die Webseite richtet sich an naturinteressierte Besucher:innen, Schüler:innen oder alle, die mehr über die faszinierende Welt der Schweizer Raubvögel erfahren möchten.

---

## 📁 Projektstruktur

Die Dateien sind wie folgt organisiert:

```
/
├── index.html                 ← Startseite
├── css/
│   └── styles.css             ← Globales Stylesheet
├── pages/
│   ├── adler.html             ← Informationsseite zu Adlern
│   └── falken.html            ← Informationsseite zu Falken
├── kontakt/
│   └── impressum.html         ← Kontakt- und Impressumsseite
└── assets/
    ├── adler.webp
    ├── falke.webp
    ├── wanderfalke.webp
    ├── sturzflug.webp
    ├── ruettelflug.jpg
    ├── baumfalke.webp
    └── falkenPortait.jpg      ← Alle Bilder für die Webseite
```

---

## 🌐 Seiten im Detail

### 1. **Startseite (`index.html`)**

**Zweck**: Begrüßt Besucher:innen und bietet einen Überblick über die Themen der Webseite.

**Inhalte**:
- Einleitungstext: „Willkommen in der Welt der Könige der Lüfte“
- Zwei Teaser-Karten:
  - **Adler**: Verlinkt zur Seite `pages/adler.html`
  - **Falken**: Verlinkt zur Seite `pages/falken.html`
- Navigation im Header mit aktiver Markierung der aktuellen Seite (`class="active"`)

**Besonderheiten**:
- Responsive Design durch `<meta name="viewport">`
- Barrierefreundliche Bildbeschreibungen (`alt`-Attribute)

---

### 2. **Seite „Adler“ (`pages/adler.html`)**

**Zweck**: Informiert über Adler, insbesondere den **Steinadler** in der Schweiz.

**Inhalte**:
- Beschreibung des Steinadlers als „König der Alpen“
- **Vergleichstabelle** mit drei Adlerarten (Steinadler, Seeadler, Weisskopfseeadler)
- **Interaktive Google Maps-Einbettung**, die das Verbreitungsgebiet in den Schweizer Alpen zeigt

**Technische Details**:
- Bilder werden aus dem `assets/`-Ordner geladen (z. B. `steinadler.webp`)
- Die Karte ist mit `loading="lazy"` optimiert, um die Ladezeit zu verbessern

---

### 3. **Seite „Falken“ (`pages/falken.html`)**

**Zweck**: Stellt verschiedene Falkenarten und ihre Jagdtechniken vor.

**Inhalte**:
- Fokus auf den **Wanderfalken** als schnellstes Tier der Welt (>300 km/h im Sturzflug)
- **Bildergalerie** mit vier Bildern und aussagekräftigen Bildunterschriften (`<figcaption>`)
- **Aufzählung** der besonderen Merkmale:
  - Spitze Flügel
  - „Falkenzahn“ am Schnabel
  - Verschiedene Jagdmethoden (Sturzflug, Rüttelflug, Luftjagd)

**Barrierefreundlichkeit**:
- Alle Bilder haben aussagekräftige `alt`-Texte
- Klare Gliederung mit Überschriften (`<h2>`, `<h3>`)

---

### 4. **Kontakt & Impressum (`kontakt/impressum.html`)**

**Zweck**: Erfüllt rechtliche Anforderungen und bietet eine Kontaktmöglichkeit.

**Inhalte**:
- **Kontaktabschnitt**: E-Mail-Adresse (verlinkt mit `mailto:`)
- **Impressum**: Name, Adresse und Ort gemäß Schweizer Recht

**Hinweis**:  
Die E-Mail-Adresse in der Vorlage (`max.mustermann@beispiel.com`) sollte vor der Veröffentlichung durch eine echte Adresse ersetzt werden.

---

## 🎨 Design & Styling

- Das Styling erfolgt über **`css/styles.css`** (nicht im Code enthalten, aber eingebunden).
- Die Webseite nutzt eine **Container-basierte Layoutstruktur** für konsistente Abstände.
- Klassen wie `.card`, `.button`, `.gallery` und `.content-image` deuten auf ein **modulares CSS-Design** hin.
- Die Navigation zeigt mit der Klasse `.active` an, auf welcher Seite man sich befindet.

---

## ✅ Best Practices

Die Webseite folgt mehreren modernen Webstandards:

| Merkmal | Umsetzung |
|--------|-----------|
| **Sprachangabe** | `<html lang="de">` für bessere Zugänglichkeit |
| **Responsive** | `<meta name="viewport">` für mobile Geräte |
| **Semantisches HTML** | Nutzung von `<header>`, `<main>`, `<footer>`, `<nav>`, `<figure>` |
| **Barrierefreiheit** | `alt`-Texte bei allen Bildern |
| **SEO-freundlich** | Klare Titel (`<title>`) und Überschriftenstruktur |

---

*Erstellt im Rahmen einer praktischen Arbeit – 2025*  
*© Max Mustermann*