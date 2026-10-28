# El vostre propi llenguatge de marques (BookLM)
Esta hecho con un fitxero XML, que va sobre un catalogo de diferentes libros que tienen la siguiente información:
> - **Biblioteca:** Agrupa todos los libros.
> - **Libro:** Contiene los datos del libro.
> - **Titutlo:** Nombre del libro.
> - **Autor:** Nombre del escritor.
> - **Genero**: Categoria literaria.
> - **Descripción:** Resumen del libro.
> - **Precio** Coste del libro.
> - **Editorial:** Empresas que publican el libro.
> - **Isbn:** Identificador del libro.
> - **Idioma:** Idioma de publicación.
> - **Año_de_publicación:** Año de publucación
> - **Paginas:** Numero de paginas del libro.
> - **Formato:** Tapa dura, digital o blanda.
> - **Stock:** Unidades disponiles.
## 1. El Codi XML

Aquest és el fitxer de dades XML original ben formatat, amb elements, subelements i atributs:

## 2. Elements clau de la jerarquia

* **`cataleg`**: És l'element arrel (*root*), el contenidor principal.
* **`llibre`**: Subelements directes que utilitzen un atribut identificador (`id`).
* **Fulles de dades**: Etiquetes finals (`autor`, `titol`, `preu`, etc.) que contenen la informació textual real.

