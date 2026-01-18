# AI Obchodní Analytik — Showcase

Toto je veřejná prezentační část projektu **AI Obchodní Analytik**.
Obsahuje popis řešení, architekturu a ukázkovou API dokumentaci.
Kompletní zdrojový kód a infrastruktura jsou v privátním repozitáři.

---

## Co projekt dělá
AI Obchodní Analytik je full-stack aplikace pro obchodní a marketingovou analytiku nad prodejní databází.

Umožňuje:
- KPI přehled (celkové tržby, počet objednávek, průměrný košík)
- analytické grafy a časové přehledy
- detailní tabulku prodejů s paginací
- AI analytiku: dotaz v přirozeném jazyce → SQL → výsledek z databáze + shrnutí v češtině

---

## Architektura (high-level)

Aplikace je navržena jako oddělené části:

### Frontend
- Angular
- interaktivní dashboard, grafy, tabulky
- rozhraní pro AI analytické dotazy

### Backend
- NestJS (TypeScript, běžící na Node.js runtime)
- aplikační logika, práce s daty
- API pro frontend

### AI microservice
- samostatná služba v **Pythonu**
- FastAPI
- zpracování dotazů v přirozeném jazyce (CZ)
- generování SQL dotazů
- analýza dat a tvorba business shrnutí

---

## Jak funguje AI část (zjednodušeně)
1) Uživatel položí analytickou otázku v přirozeném jazyce  
2) Python AI microservice vygeneruje odpovídající SQL dotaz  
3) SQL se provede nad databází  
4) Výstupem jsou strukturovaná data a srozumitelné shrnutí

---

## Technologie
- **Frontend:** Angular, ApexCharts
- **Backend:** NestJS (TypeScript)
- **AI microservice:** Python, FastAPI
- **Databáze:** MySQL
- **Architektura:** oddělené služby (frontend / backend / AI)

---

## Screenshoty
Screenshoty aplikace a dashboardů jsou součástí této showcase
a slouží jako vizuální ukázka funkčnosti projektu.

---

## API dokumentace (prezentační kopie)
Součástí showcase je statická prezentační kopie API dokumentace
Python AI microservice.

V runtime režimu je dokumentace plně interaktivní
a napojená na běžící AI službu.

---

## Účel projektu
Portfolio a demonstrační projekt zaměřený na:
- full-stack vývoj
- obchodní a datovou analytiku
- praktickou integraci AI do reálné aplikace
- návrh a realizaci oddělených služeb
