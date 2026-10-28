# Exemple d'Estructura XML i Visualització

Aquest document serveix com a guia pràctica per entendre com s'estructura un fitxer XML utilitzant un exemple de catàleg de llibres.

## 1. El Codi XML

Aquest és el fitxer de dades XML original ben formatat, amb elements, subelements i atributs:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<cataleg>
  <llibre id="bk101">
    <autor>García, María</autor>
    <titol>Guia del Desenvolupador</titol>
    <genere>Informàtica</genere>
    <preu currency="EUR">44.95</preu>
    <publicacio>2026-10-01</publicacio>
    <descripcio>Una mirada profunda a la creació d'aplicacions.</descripcio>
  </llibre>
  <llibre id="bk102">
    <autor>Martí, Joan</autor>
    <titol>Pluja de Mitjanit</titol>
    <genere>Fantasia</genere>
    <preu currency="EUR">9.95</preu>
    <publicacio>2025-12-16</publicacio>
    <descripcio>Una història sobre mags medievals i dracs.</descripcio>
  </llibre>
</cataleg>
```

## 2. Diagrama de l'Estructura (Mermaid)

A continuació es mostra com s'organitzen les dades de manera jeràrquica en forma d'arbre. GitHub renderitzarà aquest bloc automàticament en un gràfic visual:

```mermaid
graph TD
    %% Element Arrel
    Cataleg[cataleg]
    
    %% Primer Llibre
    Cataleg --> Llibre1[llibre id="bk101"]
    Llibre1 --> Autor1[autor: García, María]
    Llibre1 --> Titol1[titol: Guia del Desenvolupador]
    Llibre1 --> Genere1[genere: Informàtica]
    Llibre1 --> Preu1[preu currency="EUR": 44.95]
    Llibre1 --> Pub1[publicacio: 2026-10-01]
    Llibre1 --> Desc1[descripcio: ...]

    %% Segon Llibre
    Cataleg --> Llibre2[llibre id="bk102"]
    Llibre2 --> Autor2[autor: Martí, Joan]
    Llibre2 --> Titol2[titol: Pluja de Mitjanit]
    Llibre2 --> Genere2[genere: Fantasia]
    Llibre2 --> Preu2[preu currency="EUR": 9.95]
    Llibre2 --> Pub2[publicacio: 2025-12-16]
    Llibre2 --> Desc2[descripcio: ...]
    
    %% Estils visuals per diferenciar nivells
    style Cataleg fill:#f9f,stroke:#333,stroke-width:2px
    style Llibre1 fill:#bbf,stroke:#333,stroke-width:1px
    style Llibre2 fill:#bbf,stroke:#333,stroke-width:1px
```

## 3. Elements clau de la jerarquia

* **`cataleg`**: És l'element arrel (*root*), el contenidor principal.
* **`llibre`**: Subelements directes que utilitzen un atribut identificador (`id`).
* **Fulles de dades**: Etiquetes finals (`autor`, `titol`, `preu`, etc.) que contenen la informació textual real.

