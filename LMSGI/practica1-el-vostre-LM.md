# El vostre propi llenguatge de marques 
Esta hecho con un fitxero XML, que va sobre un catalogo de diferentes libros que tienen la siguiente información:
> - 
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

## 2. Elements clau de la jerarquia

* **`cataleg`**: És l'element arrel (*root*), el contenidor principal.
* **`llibre`**: Subelements directes que utilitzen un atribut identificador (`id`).
* **Fulles de dades**: Etiquetes finals (`autor`, `titol`, `preu`, etc.) que contenen la informació textual real.

