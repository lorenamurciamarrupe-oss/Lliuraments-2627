# El vostre propi llenguatge de marques (BookLM)
## 1. Introducción a los lenguajes de marcas
Los lenguajes de marcas organizan y describen información mediante etiquetas que identifican el tipo de contenido de un documento y permiten que los programas informáticos lo interpreten y procesen automáticamente. 

A partir de esta idea, se ha propuesto BookLM, un lenguaje de marcas destinado a almacenar y organizar de forma estructurada y sencilla información relacionada con los libros.

## 2. Introducción a nuestro lenguaje de marcas y sus reglas.
BookLM significa *Book Markup Language*. Es un lenguaje de marcas propio basado en **XML**, diseñado para guardar información sobre libros, como el título, autor, género, descripción, precio y editorial. 

La idea es que se pueda utilizar en una biblioteca, librería o en tiendas online para mantener todos los datos de los libros organizados y facilitar la consulta. 

## 3.Clasificación de BookLM 
BookLM es un lenguaje de marcas **descriptivo** o **semántico**, porque sus etiquetas indican qué representa cada dato. No define cómo debe mostrarse visualmente la información, sino cómo se organiza y que significado tiene cada cosa. 

## 4. Caso de uso adecuado
Sería útil para gestionar el catálogo de libros de una biblioteca o librería. Permitiría almacenar los datos de cada libro y facilitar búsquedas por título, autor o género.

También podría usarse en una tienda online para consultar información como seria el precio y las unidades disponibles mediante un programa que procese los datos. 

## 8. Información que guarda
Esta hecho con un fitxero XML, que va sobre un catalogo de diferentes libros que tienen la siguiente información:
> - **`<biblioteca>`** Agrupa todos los libros.
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

## 1. Reglas del lenguaje

Aquest és el fitxer de dades XML original, tiene diferentes datos que tienen que ver con cada libro que hay en el código:

## 2. El Codi XML

Aquest és el fitxer de dades XML original, tiene diferentes datos que tienen que ver con cada libro que hay en el código:

```xml
<biblioteca>
    <libro>
        <titulo>El nombre del viento</titulo>
        <autor>Patrick Rothfuss</autor>
        <genero>Fantasía</genero>
        <descripcion>
            Un joven relata su vida y sus aventuras
            en un mundo lleno de magia.
        </descripcion>
        <precio moneda="EUR">24.95</precio>
        <editorial>Plaza & Janés</editorial>
        <isbn>9788401337208</isbn>
        <idioma>Español</idioma>
        <anio_publicacion>2009</anio_publicacion>
        <paginas>880</paginas>
        <formato>Tapa dura</formato>
        <stock>15</stock>
    </libro>
    <libro>
        <titulo>El imperio final</titulo>
        <autor>Brandon Sanderson</autor>
        <genero>Fantasía</genero>
        <descripcion>
            Un grupo de ladrones planea derrocar a un 
            tirano inmortal en un mundo cubierto de ceniza.
        </descripcion>
        <precio moneda="EUR">21.90</precio>
        <editorial>Nova</editorial>
        <isbn>9788466658904</isbn>
        <idioma>Español</idioma>
        <anio_publicacion>2016</anio_publicacion>
        <paginas>672</paginas>
        <formato>Tapa blanda</formato>
        <stock>8</stock>
    </libro>
    <libro>
        <titulo>Dune</titulo>
        <autor>Frank Herbert</autor>
        <genero>Ciencia ficción</genero>
        <descripcion>
            Un joven noble debe sobrevivir en un peligroso 
            planeta desértico que posee la sustancia más valiosa del universo.
        </descripcion>
        <precio moneda="EUR">18.95</precio>
        <editorial>Debolsillo</editorial>
        <isbn>9788497596824</isbn>
        <idioma>Español</idioma>
        <anio_publicacion>2003</anio_publicacion>
        <paginas>704</paginas>
        <formato>Bolsillo</formato>
        <stock>22</stock>
    </libro>
    <libro>
        <titulo>El hobbit</titulo>
        <autor>J.R.R. Tolkien</autor>
        <genero>Fantasía</genero>
        <descripcion>
            Un apacible hobbit es reclutado por un mago 
            y un grupo de enanos para recuperar un tesoro custodiado por un dragón.
        </descripcion>
        <precio moneda="EUR">22.00</precio>
        <editorial>Minotauro</editorial>
        <isbn>9788445000656</isbn>
        <idioma>Español</idioma>
        <anio_publicacion>2012</anio_publicacion>
        <paginas>352</paginas>
        <formato>Tapa dura</formato>
        <stock>12</stock>
    </libro>
</biblioteca>
```


