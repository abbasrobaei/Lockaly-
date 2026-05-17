# Lockaly — Technologie-Stack

> Detaillierte Übersicht der eingesetzten Technologien, ihrer Rolle in der Architektur und der Gründe für unsere Auswahl.

Unser Stack folgt klaren Prinzipien: **DSGVO by Design**, **Open-Source-First**, **Skalierbarkeit** und **Developer Experience**. Jede Technologieentscheidung unterstützt unseren Kernfokus — hyperlokale Event-Discovery mit maximaler Datenschutzkonformität.

---

## 🖥️ Frontend

| Technologie | Layer | Begründung |
|:---|:---|:---|
| **Nuxt 3** (Vue.js) | Rendering-Framework | SSR für exzellente SEO & Core Web Vitals; File-based Routing; Auto-Imports für hohe Produktivität |
| **TypeScript** | Sprache | Typsicherheit reduziert Laufzeitfehler und macht den Code wartbarer und skalierbarer |
| **Tailwind CSS** | Styling | Utility-First CSS ermöglicht schnelle, konsistente UI-Entwicklung ohne CSS-Chaos |
| **Pinia** | State Management | Offizielles, leichtgewichtiges State Management für Vue 3 mit DevTools-Support |
| **Leaflet + OpenStreetMap** | Kartenintegration | Open-Source-Lösung ohne Google-Abhängigkeit — datenschutzkonform und kosteneffizient |

**Warum Nuxt 3?**
Nuxt 3 kombiniert erstklassiges Server-Side Rendering mit der Flexibilität eines modernen JavaScript-Frameworks. Das Ergebnis: hervorragende SEO-Performance (entscheidend für Event-Discovery), schnelle Time-to-Interactive durch Hydration und eine exzellente Developer Experience durch automatische Imports und File-based Routing.

---

## 🔧 Backend

| Technologie | Layer | Begründung |
|:---|:---|:---|
| **Laravel 11** (PHP 8.3) | API-Framework | Ausgereiftes Ökosystem, starke Community, schnelle Entwicklung durch Konventionen |
| **PostgreSQL 16** | Primärdatenbank | Leistungsfähigstes Open-Source-RDBMS — ideal für komplexe Geo-Abfragen und Volltextsuche |
| **PostGIS** | Geo-Erweiterung | **Schlüsseltechnologie** für hyperlokale Suche: Radius-Abfragen, Polygon-Matching, Stadtteilfilterung |
| **Redis** | Cache & Queues | High-Performance In-Memory-Datenspeicher für Caching und asynchrone Job-Verarbeitung |
| **Laravel Sanctum** | Authentifizierung | Einfache, sichere Token-basierte API-Authentifizierung — optimal für SPAs und Mobile Apps |
| **Laravel Horizon** | Queue-Management | Echtzeit-Monitoring und -Verwaltung unserer KI-Verarbeitungs-Queues |

**Warum Laravel + PostgreSQL + PostGIS?**
Diese Kombination ist für uns keine Kompromisslösung — sie ist die optimale Wahl für eine Event-Discovery-Plattform. Laravel liefert schnelle API-Entwicklung mit einem starken Ökosystem. PostgreSQL ist das leistungsfähigste Open-Source-RDBMS. **PostGIS ist der entscheidende Baustein**: Es ermöglicht präzise geografische Abfragen (Radius-Suche auf 500 m, Stadtteil-Polygone, Distanzberechnungen) — das Herzstück unserer hyperlocal Technologie.

---

## 📱 Mobile

| Technologie | Layer | Begründung |
|:---|:---|:---|
| **Capacitor 6** | Cross-Platform-Bridge | Native iOS- & Android-Apps aus einer einzigen Codebase — kein Framework-Split |
| **iOS 16+** | Apple-Plattform | Vollständige native Integration via Capacitor-Plugins |
| **Android 10+** | Google-Plattform | Breite Gerätabdeckung durch niedrigen Mindest-API-Level |

**Warum Capacitor statt React Native / Flutter?**
Capacitor nutzt unsere bestehende Nuxt 3 Codebase direkt — ohne ein separates Framework, separate Entwickler oder separate Codebases. Nativer Zugriff auf GPS, Push-Notifications und Kamera ist über Capacitor-Plugins möglich. Das Ergebnis: **eine Codebase für Web, iOS und Android** mit minimalem Mehraufwand.

---

## 🤖 KI & Automatisierung

| Technologie | Layer | Begründung |
|:---|:---|:---|
| **NLP-Modelle** | Klassifikation | Semantische Event-Kategorisierung und Tagging für präzise Suchergebnisse |
| **AI-OCR** | Bilderkennung | Extraktion von Event-Daten aus Flyern und Instagram-Storys — vollautomatisch |
| **Multi-Model-Fallback** | Resilienz | Ausfallsicherheit durch automatischen Wechsel zwischen Modellen bei Störungen |
| **Custom Scraper** | Aggregation | Tägliche automatisierte Aggregation aus 11+ Event-Quellen und Plattformen |
| **Duplikat-Engine** | Datenqualität | KI-gestützte Erkennung und Zusammenführung identischer Events aus verschiedenen Quellen |

Unsere KI-Pipeline arbeitet vollständig **automatisiert und asynchron** — Events werden täglich aggregiert, klassifiziert, verifiziert und dedupliziert, ohne manuellen Eingriff. Das Ergebnis: ein stets aktueller, qualitätsgeprüfter Event-Katalog für Düsseldorf.

---

## 🏗️ Infrastruktur & Hosting

| Service | Anbieter | Layer | Begründung |
|:---|:---|:---|:---|
| **App-Server** | Hetzner Cloud (DE) | Compute | DSGVO-konformes Hosting in deutschen Rechenzentren |
| **Datenbank** | Hetzner (DE) | Persistenz | PostgreSQL + PostGIS — EU-Datenhaltung garantiert |
| **Cache / Queues** | Redis on Hetzner | Performance | Asynchrone KI-Jobs und Hochleistungs-Caching |
| **Frontend-CDN** | Vercel Edge | Delivery | Globale Auslieferung mit minimaler Latenz |

**Warum Hetzner?**
Hetzner ist ein europäisches Unternehmen mit Rechenzentren **ausschließlich in Deutschland** (Frankfurt, Nürnberg, Falkenstein). Das bedeutet: vollständige DSGVO-Konformität ohne Kompromisse, kein Datentransfer in Drittländer und ein exzellentes Preis-Leistungsverhältnis. Für eine DSGVO-first Plattform wie Lockaly ist das keine Option — es ist Pflicht.

---

## 📊 Analytics & Monitoring

| Tool | Layer | Begründung |
|:---|:---|:---|
| **Plausible Analytics** | Web-Analytics | Cookiefreie, DSGVO-konforme Webanalyse — kein Cookie-Banner nötig |
| **Laravel Telescope** | Debugging | Internes Debugging & Request-Monitoring (nicht öffentlich) |
| **Laravel Horizon** | Queue-Monitoring | Echtzeit-Einblick in KI-Verarbeitungs-Queues und Job-Status |
| **Uptime-Monitoring** | Verfügbarkeit | Automatische Alerts bei Ausfällen oder Performance-Problemen |

**Warum Plausible statt Google Analytics?**
Plausible ist die einzig konsequente Wahl für eine DSGVO-first Plattform. Es erfordert **keinen Cookie-Consent-Banner**, gibt keine Daten an Google weiter, ist Open Source und kann in der EU gehostet werden. Wir erhalten alle wesentlichen Metriken — ohne Datenschutz-Kompromisse.

---

## 🛠️ Entwicklungs-Tools

| Tool | Layer | Zweck |
|:---|:---|:---|
| **Git / GitHub** | Versionskontrolle | Source Control, CI/CD und Collaboration |
| **Docker + Laravel Sail** | Lokale Entwicklung | Reproduzierbare Entwicklungsumgebung für das gesamte Team |
| **Pest** | Backend-Tests | Modernes, expressives PHP-Testing-Framework |
| **Vitest** | Frontend-Tests | Schnelles Unit-Testing für Vue/Nuxt-Komponenten |
| **ESLint + Prettier** | Code-Qualität (FE) | Einheitlicher Code-Style und automatische Formatierung im Frontend |
| **PHP CS Fixer** | Code-Qualität (BE) | PSR-konforme Code-Style-Durchsetzung im Backend |

---

## 🏆 Zusammenfassung: Warum dieser Stack?

Unser Stack ist kein Zufall — er ist das Ergebnis bewusster Entscheidungen für:

- ✅ **DSGVO by Design** — EU-Hosting, Open-Source-Karten, cookiefreie Analytics
- ✅ **Hyperlokale Präzision** — PostGIS als Fundament für geografische Abfragen
- ✅ **Skalierbarkeit** — Stateless API, horizontales Scaling, Queue-basierte KI-Verarbeitung
- ✅ **One-Codebase-Strategie** — Nuxt 3 + Capacitor für Web, iOS und Android
- ✅ **Entwicklerproduktivität** — Laravel + Nuxt 3 mit starken Ökosystemen und TypeScript

---

*Zuletzt aktualisiert: Mai 2026*
