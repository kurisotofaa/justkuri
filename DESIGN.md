---
name: JustKuri Design System
colors:
  surface: '#fcf8f8'
  surface-dim: '#ddd9d9'
  surface-bright: '#fcf8f8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f3f2'
  surface-container: '#f1edec'
  surface-container-high: '#ebe7e7'
  surface-container-highest: '#e5e2e1'
  on-surface: '#1c1b1b'
  on-surface-variant: '#444748'
  inverse-surface: '#313030'
  inverse-on-surface: '#f4f0ef'
  outline: '#747878'
  outline-variant: '#c4c7c8'
  surface-tint: '#5d5f5f'
  primary: '#5d5f5f'
  on-primary: '#ffffff'
  primary-container: '#ffffff'
  on-primary-container: '#747676'
  inverse-primary: '#c6c6c7'
  secondary: '#005ab7'
  on-secondary: '#ffffff'
  secondary-container: '#0372e4'
  on-secondary-container: '#fefcff'
  tertiary: '#5f5e60'
  on-tertiary: '#ffffff'
  tertiary-container: '#ffffff'
  on-tertiary-container: '#767578'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c7'
  on-primary-fixed: '#1a1c1c'
  on-primary-fixed-variant: '#454747'
  secondary-fixed: '#d7e2ff'
  secondary-fixed-dim: '#abc7ff'
  on-secondary-fixed: '#001b3f'
  on-secondary-fixed-variant: '#00458f'
  tertiary-fixed: '#e4e2e4'
  tertiary-fixed-dim: '#c8c6c8'
  on-tertiary-fixed: '#1b1b1d'
  on-tertiary-fixed-variant: '#474649'
  background: '#fcf8f8'
  on-background: '#1c1b1b'
  surface-variant: '#e5e2e1'
  slate-gray: '#86868B'
  surface-soft: '#F5F5F7'
  border-subtle: '#F2F2F2'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '300'
    lineHeight: '1.2'
    letterSpacing: -0.5px
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '400'
    lineHeight: '1.3'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 1px
  quote-fact:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '500'
    lineHeight: '1.5'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-margin: 40px
  section-gap: 64px
  element-gap: 24px
  inner-padding: 20px
  white-space-ratio: '0.9'
---

from weasyprint import HTML

# Design-Inhalt für die Markdown/Design-Datei
design_content = """
# JustKuri | Brand Design Guidelines (2026)
**Concept:** Clean White / Apple Minimalist
**Mission:** High-End Content & IT Integration

---

## 1. Das LinkedIn-Profil (Apple-Style)

### A. Das Banner (Header Image)
* **Farbe:** Absolutes Weiß (`#FFFFFF`).
* **Elemente:** Nur ein Element in der Mitte oder rechts unten.
* **Text:** * *Schriftart:* Inter oder SF Pro (Dünn/Light).
    * *Inhalt:* "Consistent. Technical. International."
* **Vibe:** 90% des Bildes müssen leer bleiben (White Space).

### B. Profilbild
* **Hintergrund:** Neutraler, heller Hintergrund (Hellgrau oder Weiß).
* **Outfit:** Einfarbiges Shirt (Schwarz, Weiß oder Dunkelblau). Keine Logos.
* **Licht:** Weiches Licht von vorne (Fensterlicht).

### C. Info-Bereich (About)
*Keine langen Texte. Nur Fakten.*

> **JustKuri.**
> 180-Day Content Challenge.
>
> **Focus:**
> + High-End Video Production (DaVinci Resolve / CapCut)
> + Digital Infrastructure & IT
> + Personal Discipline
>
> **Status:**
> Building a global media brand from Lübeck.

---

## 2. Die "JustKuri" E-Mail Vorlage (Clean White)

**Betreff:** Partnership / Digital Content Production - [Firmenname]

Sehr geehrte(r) [Name],

mein Name ist Kristupas Grigas. Ich baue derzeit von Lübeck aus eine internationale Medienmarke auf. Mein Fokus liegt auf technischer Präzision und konsistenter Qualität.

Ich habe Ihr Unternehmen analysiert und sehe Potenzial, Ihre digitale Präsenz durch professionellen Kurz-Content (Reels/Shorts) auf ein neues Level zu heben.

**Mein Angebot:**
* Studio-Tonqualität (OK Lübeck Standard)
* Datengesteuertes Storytelling
* Minimalistisches, modernes Design

Gerne erstelle ich Ihnen ein kostenloses Test-Video, um meinen Standard zu demonstrieren.

Beste Grüße,

**Kristupas Grigas**
*Content Strategist | JustKuri*
[Link zu LinkedIn]

---

## 3. Strategische Roadmap (5k Ziel)

1. **Juli - August:** Fokus auf Café-Job + 180-Day Challenge (Handy + OK Studio).
2. **September:** Investition in **Sony ZV-E10 II**.
3. **Oktober - Dezember:** Erste bezahlte Kundenaufträge in Lübeck (50€ - 150€ pro Video).
4. **Januar - Juni 2027:** Skalierung. Ziel: 4.000€ für den Führerschein auf dem Sparkonto.

---
*Stay disciplined. The empire is built in the silence.*
"""

# HTML Template für die PDF-Version des Designs
html_template = f"""
<!DOCTYPE html>
<html>
<head>
<style>
    @page {{
        size: A4;
        margin: 20mm;
        background-color: #ffffff;
    }}
    body {{
        font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
        color: #1d1d1f;
        line-height: 1.6;
        background-color: #ffffff;
    }}
    h1 {{
        font-weight: 300;
        font-size: 28pt;
        letter-spacing: -0.5px;
        border-bottom: 1px solid #f2f2f2;
        padding-bottom: 10px;
    }}
    h2 {{
        font-weight: 400;
        font-size: 18pt;
        color: #0071e3;
        margin-top: 30px;
    }}
    h3 {{
        font-weight: 600;
        font-size: 12pt;
        text-transform: uppercase;
        letter-spacing: 1px;
        color: #86868b;
    }}
    .box {{
        background-color: #f5f5f7;
        padding: 20px;
        border-radius: 12px;
        margin-top: 10px;
    }}
    .footer {{
        margin-top: 50px;
        font-style: italic;
        color: #86868b;
        text-align: center;
    }}
    li {{
        margin-bottom: 8px;
    }}
</style>
</head>
<body>
    <h1>JustKuri Design System</h1>
    <p>Version 1.0 | April 2026</p>

    <h2>1. Visual Identity</h2>
    <h3>Farbe</h3>
    <p>Primär: Weiß (#FFFFFF) | Sekundär: Apple Blue (#0071e3) | Akzent: Slate (#1d1d1f)</p>
    
    <div class="box">
        <strong>Core Philosophy:</strong> "Simple is harder than complex." - Wenn dein Profil zu voll aussieht, lösche Dinge. Je weniger Text, desto mehr Power hat jedes Wort.
    </div>

    <h2>2. LinkedIn Strategy</h2>
    <h3>Der Post-Stil</h3>
    <p>Nutze bei Fotos immer den "High-Key" Look (hell, klar, sauber). Poste keine Selfies im Schlafzimmer. Wenn du kein Studio hast, geh nach draußen bei bewölktem Himmel (bestes Softbox-Licht der Welt).</p>

    <h2>3. Revenue Stream</h2>
    <ul>
        <li><strong>Stufe 1:</strong> Minijob Café (Sicheres Basis-Einkommen).</li>
        <li><strong>Stufe 2:</strong> Video-Freelancing Lübeck (Equipment-Finanzierung).</li>
        <li><strong>Stufe 3:</strong> Eigener Kanal (Long-term Empire).</li>
    </ul>

    <div class="footer">
        Generated for Kristupas Grigas. Build your future.
    </div>
</body>
</html>
"""

# Datei speichern
with open("design_justkuri.md", "w") as f:
    f.write(design_content)

HTML(string=html_template).write_pdf("JustKuri_Brand_Design.pdf")
