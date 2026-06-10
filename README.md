# Kaya decomposition: rozklad emisí CO₂ pro vybrané státy

Interaktivní analýza rozkladu emisí CO₂ metodou Kaya identity pro vybrané státy světa za období 1990–2024. Projekt byl zpracován v R a Quarto.

**Autoři:** Romana Pejcalová, Jakub Pejcal  
**Datum:** červen 2026  
**Interaktivní report:** https://ropej.github.io/kaya-decomposition-2026/

## Obsah analýzy

- Kaya dekompozice emisí CO₂ pro vybrané státy (trendy příspěvků faktorů)
- Souhrnné trendy podle příjmové skupiny a role v obchodu s fosilními palivy
- Mapa emisí CO₂ na obyvatele
- Decoupling – odpojení ekonomiky od emisí
- Korelogram Kaya faktorů
- Clusterová analýza zemí (k-means, k = 5)
- Kulturní dimenze – vzdělání a emise CO₂

## Metoda

Kaya identita rozkládá změnu emisí CO₂ na čtyři faktory:

**Δ CO₂ ≈ Δ Populace + Δ HDP/obyvatele + Δ Energie/HDP + Δ CO₂/Energie**

Faktory jsou vyjádřeny jako meziroční procentuální změny (logaritmická aproximace).

## Zdroje dat

| Dataset | Zdroj | Popis |
|---|---|---|
| Our World in Data – CO₂ and GHG emissions | [owid/co2-data](https://github.com/owid/co2-data) | Emise CO₂, HDP, populace, energetická a uhlíková intenzita |
| Our World in Data – Energy data | [owid/energy-data](https://github.com/owid/energy-data) | Produkce a spotřeba ropy, plynu a uhlí (klasifikace exportérů) |
| World Bank – Education Statistics | [data.worldbank.org](https://data.worldbank.org) | Hrubá míra terciárního vzdělání |
| ISO 3166 – Countries with Regional Codes | [lukes/ISO-3166](https://github.com/lukes/ISO-3166-Countries-with-Regional-Codes) | Kontinenty dle ISO kódu |

Data jsou stahována přímo z veřejných zdrojů a nejsou součástí repozitáře.

## Soubory

| Soubor | Popis |
|---|---|
| `kaya_decomposition.qmd` | Zdrojový Quarto dokument |
| `docs/index.html` | Publikovaný interaktivní report |
