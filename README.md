# Alura-CSS-Grid-Simplificando-Layouts

## Archivo normalize.css

<https://necolas.github.io/normalize.css/>

## Header

Encabezado: Contiene el menu.

## Main

Main: Contiene todo el contenido.

## Footer

Rodapie: Contiene el fin de página.

## 3 Areas definidas

En la carpeta css tenemos el archivo style.css. Dentro la clase .app que corresponde al body: en el cual indicamos un ``display: grid;``
Tenemos que definir las 3 areas con ``grid-template-areas: "encabezado" "contenido" "rodapie";``
Definimos la cantidad de columnas que en nuestro caso es 1 con ``grid-template-columns: auto;``
Luego definimos nuestras rows, en donde nuestro encabezado tendra 50px, el contenido auto y nuestro footer auto, ``grid-template-rows: 50px auto auto;``. La parte de contenido toma toda página la setear en 100vh, ``grid-template-rows: 50px 100vh auto;``
La añadimos un background para visualizar mejor las areas.  
De esta manea definimos las templates-areas.
Ahora necesito definir cuales son cada una, ``grid-area: encabezado;`` ``grid-area: contenido;`` ``grid-area: rodapie;``  

Sabemos que nuestro sitio web se divide en tres partes:

* Encabezado
* Contenido
* Rodapié  

El CSS GRID Layout se usa para diseñar sitios web de una manera simple usando templates predefinidas. Estas templates deben tener información sobre cómo se dividirán las áreas.

```css
grid-template-areas:
        "encabezado"
        "contenido"
        "rodapie";
```  

Debemos definir las áreas en el orden en que deben colocarse en la página, la definición se hizo en el orden correcto.  

## Definiendo las columnas  

Los blogs suelen estar divididos en dos columnas: la de la izquierda con la lista de publicaciones y la de la derecha con información sobre el blog.

Usando CSS Grid Layout, ¿cuáles son las formas correctas de definir dos columnas como en el ejemplo anterior?  

Estamos creando dos columnas donde su tamaño será 80vw a la izquierda y 20vw a la derecha (también podemos usar otras unidades de medida).

```css
grid-template-columns: 80vw 20vw;
```

Estamos creando dos columnas donde el tamaño de las mismas será automático según el contenido que se inserte.

```css
grid-template-columns: auto auto;
```

## Definiendo líneas / rows

¿Cómo podemos definir el tamaño de las cuatro líneas?  

Estamos creando cuatro líneas donde el tamaño de las mismas será automático según el contenido que se inserte en ellas.

```css
grid-template-rows: auto auto auto auto;
```

Estamos creando cuatro líneas donde el tamaño de ellas serán: 10% para la primera, 20px para la segunda, 50vh para la tercera y 10% para la cuarta. Podemos mezclar unidades de medida en las definiciones.

```css
grid-template-rows: 10% 20px 50vh 10%;
```  
