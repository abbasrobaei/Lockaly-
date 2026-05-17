<div align="center">

<img src="https://lockaly.de/og-image.jpg" alt="Lockaly — Hyperlokale Event-Discovery-Plattform aus Düsseldorf" width="100%">

<br/>
<br/>

# Lockaly — Das digitale Herz der Stadt

### Hyperlokale, KI-gestützte Event-Discovery-Plattform · Made in Düsseldorf 🇩🇪

<br/>

[![Website](https://img.shields.io/badge/🌐%20Website-lockaly.de-0066FF?style=for-the-badge)](https://lockaly.de)
[![Status](https://img.shields.io/badge/🚀%20Status-Live%20seit%202025-22C55E?style=for-the-badge)](#aktueller-status)
[![Users](https://img.shields.io/badge/👥%20Nutzer-300%2B%20aktiv-8B5CF6?style=for-the-badge)](#aktueller-status)
[![Events](https://img.shields.io/badge/🎉%20Events-530%2B%20live-F59E0B?style=for-the-badge)](#aktueller-status)

[![DSGVO](https://img.shields.io/badge/🔒%20Datenschutz-DSGVO%20by%20Design-16A34A?style=flat-square)](https://lockaly.de/datenschutz)
[![Hosting](https://img.shields.io/badge/🏠%20Hosting-Hetzner%20Germany-E55A1B?style=flat-square)](#datenschutz--infrastruktur)
[![Stack](https://img.shields.io/badge/⚡%20Stack-Nuxt%203%20%7C%20Laravel%2011%20%7C%20PostGIS-3B82F6?style=flat-square)](#technologie-stack)
[![Made in](https://img.shields.io/badge/📍%20Made%20in-Düsseldorf%2C%20NRW-FACC15?style=flat-square)](#kontakt--links)

</div>

---

## 🏙️ Über Lockaly

**Lockaly** ist die erste hyperlokale, KI-gestützte Event-Discovery-Plattform in Deutschland — entwickelt von Düsseldorf aus, für das urbane Leben in NRW und darüber hinaus.

Wir lösen ein echtes Problem: Lokale Events — von der Kleinkunstbühne im Kiez bis zum Stadtfest um die Ecke — sind kaum auffindbar. Große Plattformen wie Eventbrite oder Facebook sind zu unübersichtlich, zu global und datenschutzrechtlich problematisch.

**Lockaly macht das anders.** Wir aggregieren Events vollautomatisch aus über **11 verschiedenen Quellen**, reichern sie mit KI an und machen sie auf **Stadtteilebene** (bis 500 m Radius) präzise auffindbar — datenschutzkonform, ohne Cookie-Banner, direkt für Menschen in ihrem Viertel.

> **Live seit Ende 2025** in Düsseldorf · **530+ Events** · **300+ aktive Nutzer** · wachsende Community

---

## ✨ Features & Alleinstellungsmerkmale

| Feature | Beschreibung |
|:---|:---|
| 📍 **Hyperlokaler Fokus** | Event-Entdeckung auf Stadtteil-Ebene — bis auf 500 m Radius präzise |
| 🤖 **KI-Vollautomatisierung** | Tägliche Aggregation aus 11+ Quellen + AI-OCR für Flyer & Instagram-Storys |
| 📱 **Intuitive Swipe-UX** | TikTok-inspirierte Oberfläche — schnell, engagierend, ohne Lernkurve |
| 🔒 **DSGVO by Design** | EU-Hosting, kein Cookie-Banner, keine Datenweitergabe an Google/Meta |
| 🚀 **Zero-Friction Onboarding** | Plattform vollständig ohne Account nutzbar |
| 👥 **Community & Social** | „Bin dabei"-Funktion, WhatsApp-Sharing, Gamification, Friends-System |
| 🎫 **Veranstalter-Dashboard** | Event-Management, Reichweiten-Statistiken, Boosts & SEO-optimierte Profile |
| 🗺️ **Interaktive Karte** | Open-Source-Karte mit PostGIS-basierten Geo-Abfragen (kein Google Maps) |
| 🔍 **Semantische Suche** | NLP-gestützte Kategorisierung und Ähnlichkeitssuche |
| 🛡️ **Duplikat-Erkennung** | Mehrstufige KI-Pipeline verhindert doppelte Events aus verschiedenen Quellen |

---

## ⚡ Technologie-Stack

<details>
<summary><strong>🖥️ Frontend</strong></summary>
<br/>

| Technologie | Zweck |
|:---|:---|
| **Nuxt 3** (Vue.js) | Full-Stack Framework mit SSR — exzellente SEO & Core Web Vitals |
| **TypeScript** | Typsichere Entwicklung für höhere Codequalität |
| **Tailwind CSS** | Utility-First Styling für schnelle, konsistente UI-Entwicklung |
| **Pinia** | Modernes State Management für Vue 3 |
| **Leaflet + OpenStreetMap** | Datenschutzfreundliche Kartenintegration (kein Google Maps) |

</details>

<details>
<summary><strong>🔧 Backend</strong></summary>
<br/>

| Technologie | Zweck |
|:---|:---|
| **Laravel 11** (PHP 8.3) | Ausgereiftes API-Framework mit starkem Ökosystem |
| **PostgreSQL 16** | Leistungsfähigstes Open-Source-RDBMS |
| **PostGIS** | Geografische Erweiterung — Schlüsseltechnologie für hyperlokale Suche |
| **Redis** | High-Performance Cache & Queue-Backend |
| **Laravel Sanctum** | Token-basierte API-Authentifizierung |
| **Laravel Horizon** | Queue-Monitoring und Verwaltung |

</details>

<details>
<summary><strong>📱 Mobile</strong></summary>
<br/>

| Technologie | Zweck |
|:---|:---|
| **Capacitor 6** | Native iOS & Android Apps aus einer Codebase |
| **iOS 16+** | Apple App Store |
| **Android 10+** | Google Play Store |

</details>

<details>
<summary><strong>🤖 KI & Automatisierung</strong></summary>
<br/>

| Technologie | Zweck |
|:---|:---|
| **NLP-Modelle** | Semantische Event-Klassifikation und Kategorisierung |
| **AI-OCR** | Extraktion von Event-Daten aus Flyern und Social-Media-Bildern |
| **Multi-Model-Fallback** | Robustheit und Ausfallsicherheit der KI-Pipeline |
| **Custom Scraper** | Automatische Aggregation aus 11+ Event-Quellen |
| **Duplikat-Engine** | KI-gestützte Erkennung identischer Events |

</details>

<details>
<summary><strong>🏗️ Infrastruktur & Datenschutz</strong></summary>
<br/>

| Service | Zweck |
|:---|:---|
| **Hetzner Cloud (DE)** | DSGVO-konformes Hosting in Deutschland |
| **Vercel Edge Network** | Globale Frontend-Auslieferung mit minimaler Latenz |
| **Plausible Analytics** | Cookiefreie, DSGVO-konforme Webanalyse — kein Banner nötig |
| **Leaflet + OpenStreetMap** | Open-Source-Karten ohne Google-Abhängigkeit |

</details>

> 📄 Vollständige technische Details: **[docs/tech-stack.md](./docs/tech-stack.md)** · **[docs/architecture.md](./docs/architecture.md)** · **[docs/about.md](./docs/about.md)**

---

## 🌍 Unsere Vision

Wir bauen die **digitale Infrastruktur für das urbane Leben** in NRW und darüber hinaus.

Lockaly schließt die Lücke zwischen Bürger:innen, lokalen Veranstaltern und Stadtmarketing — **transparent, datenschutzkonform und hochgradig nutzerzentriert**. Wir glauben, dass Technologie das Lokale stärken kann, ohne dabei Datenschutz oder Nutzerautonomie zu opfern.

**Unsere These:** In einer Welt überwältigender digitaler Reizüberflutung sehnen sich Menschen nach authentischen lokalen Erlebnissen. Lockaly ist die Plattform, die diese Erlebnisse sichtbar macht.

---

## 📊 Aktueller Status

| Bereich | Details |
|:---|:---|
| 🟢 **Produktstatus** | Voll funktionsfähig und live in Produktion |
| 📍 **Pilotmarkt** | Düsseldorf, Nordrhein-Westfalen |
| 🎉 **Events** | 530+ aggregiert und live |
| 👥 **Nutzer** | 300+ aktive Nutzer in Düsseldorf |
| 🤖 **KI-Quellen** | 11+ automatisierte Event-Datenquellen |
| 👨‍💻 **Team** | 3 Gründer — Tech, Growth, B2B-Partnerships |
| 🗺️ **Nächstes Ziel** | Skalierung NRW: Köln, Ruhrgebiet (2026/27) |
| 💡 **Langfristig** | Ausbau zur führenden hyperlocal Event-Plattform in DACH |

---

## 📁 Über dieses Repository

Dieses Repository dient als öffentliche Informations- und Dokumentationsquelle für Lockaly:

- 📖 **Für Interessierte & Partner** — Produkt-Übersicht, Vision und Technologieentscheidungen
- 📐 **Für Entwickler** — Technische Architektur und Stack-Dokumentation
- 💡 **Für Investoren** — Showcase unserer Werte: Transparenz, Datenschutz, lokale Verwurzelung

> **Hinweis:** Der vollständige Quellcode ist derzeit privat. Dokumentation, Architektur-Übersichten und öffentliche Teile werden kontinuierlich ergänzt.

---

## 📬 Kontakt & Links

| | |
|:---|:---|
| 🌐 **Website** | [lockaly.de](https://lockaly.de) |
| 📍 **Standort** | Düsseldorf, Nordrhein-Westfalen, Deutschland |
| 👤 **Abbas Robaei** | CTO & Co-Founder |
| 👤 **Anahita Daneshgarian** | Growth & Co-Founder |
| 👤 **Hossein Kawianifard** | Partnerships & Co-Founder |

---

<div align="center">

**Made with ❤️ in Düsseldorf · Hyperlocal · KI-gestützt · DSGVO-konform**

*Lockaly — Wo deine Stadt lebt.*

*© 2025–2026 Lockaly. Alle Rechte vorbehalten.*

</div>