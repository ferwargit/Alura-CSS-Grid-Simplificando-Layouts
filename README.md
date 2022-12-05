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
