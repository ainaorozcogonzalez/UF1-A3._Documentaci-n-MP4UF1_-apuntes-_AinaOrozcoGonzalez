# UF1-A3._Documentaci-n-MP4UF1_-apuntes-_AinaOrozcoGonzalez

# GitHub

## Como crear un repositorio
 1. Crear un repositorio nuevo
![Imagen de como crear un repositorio](https://github.com/ainaorozcogonzalez/UF1-A3._Documentaci-n-MP4UF1_-apuntes-_AinaOrozcoGonzalez/blob/main/img/rep1.png?raw=true)
 2. Como configurar un repositorio nuevo.

    En “repository name” ponemos el nombre que queremos que tenga nuestro nuevo repositorio.

    Hemos de elegir si queremos que el repositorio sea público o privado. Si queremos activar GitHub pages tenemos que tener el repositorio en público para poder publicar el repositorio.

    Marcamos la opción de creación del archivo README o no, dependiendo de:
* __Si creamos el archivo README, el repositorio se crea e inicializa automáticamente en GitHub__.
* __En caso de que no se marque el archivo README.md, el repositorio en GitHub se creará vacío y no inicializado__. Eso se usará sobre todo para crear un repositorio nuevo desde cero en local (GIT) y luego sincronizarlo o importar un repositorio local que tengamos creado. Una vez creado, nos aparecerán los comandos que hemos de utilizar dependiendo de lo que queramos hacer con él mediante comandos de CLI:
    
    a) **Clonado y trabajo en local (GIT) de un repositorio de GitHub inicializado (activo).**
    
    **Para clonar en el disco duro local un repositorio ya creado e inicializado de GitHub y poder trabajar en local, tendremos que tener instalado GIT en el disco duro:**
    
    Usaremos una estructura base C:\GIT a partir de la cual construiremos los repositorios que queramos trabajar en local y tener sincronizados con GitHub.
    
    Situados en esta carpeta “raíz” de GIT, y conociendo la URL del repositorio Gigit tHub a clonar, usaremos la orden **git clone https://github.com/Usuario/repositorioRemoto.git**  para que se cree el clon local (crea también la carpeta).
    
    Una vez creada, para trabajar con el repositorio local, nos desplazamos a la raíz del repositorio clonado y que será idéntico al remoto de GitHub para trabajar con él, realizar modificaciones y finalmente sincronizar los cambios con GitHub cada vez que queramos actualizar el repositorio de GitHub de forma que se implementen los cambios:

    - **git init** 
    
    Inicializamos el repositorio GIT en la carpeta donde estamos situados.
    
    - **git add "archivo” o  git add .** (punto: contracción de *.*) 
    
    Elementos que van a incluirse en la nueva versión  Si se incluye el wildcard “.” se incluirán todos los archivos del repositorio.
    
    - **git commit -m "añadir título"**

    Descripción de la versión o fecha, o cualquier indicador que defina qué cambios se han hecho en la versión
    
    - **git push origin main** (“main” o el nombre de la rama a sincronizar)
    
    Se sincronizan los elementos incluidos en el anterior commit al repositorio remoto y rama indicadas en los puntos anteriores..

    c) **Sincronizar un repositorio local local ya existente desde línea de comandos:**

    Navegamos en local hasta la carpeta raíz del repositorio local a vincular con el repositorio vacío recién creado en GitHub.

    - **git init**
    
    Inicializamos el repositorio dentro de la carpeta raiz del mismo

    - **git remote add origin https://github.com/AinaOrozcoGonzalez/BORRAR.git.**
    
    Una vez situados en la carpeta, añadimos como origen de ese repositorio al repositorio vacío de GitHub.
   
    - **git add .** 
    
    Añadimos todos los archivos al repositorio local
    
    - **git commit -m "first commit"** 

    Commit es un conjunto de cambios que se realizan en los archivos del repositorio (modificar, añadir, eliminar, mover, renombrar, etc). Creamos el paquete de archivos a sincronizar con el repositorio remoto (se incluirán los archivos que hayamos hecho “add” anteriormente (en esta primera ocasión TODOS) y le ponemos nombre identificativo a la nueva versión con el parámetro -m.

    - **git branch -M main**
    
    Asociamos la versión a la rama de desarrollo que queramos. La rama por defecto es “main”. 

    - **git push -u origin main**

    Subimos los cambios al repositorio remoto y rama indicadas en los puntos anteriores.

El comando git pull hará la inversa de **git push**, es decir, “bajará” los cambios que hayamos hecho directamente en el repositorio GutHub (en la web)

3. Importar repositorio ya existente en GitHub.

    Vamos al repositorio a importar (Code) y copiamos su URL:

    ![](https://github.com/ainaorozcogonzalez/UF1-A3._Documentaci-n-MP4UF1_-apuntes-_AinaOrozcoGonzalez/blob/main/img/rep2.png?raw=true)

    En repositorios, vamos a crear un repositorio nuevo:

    Y vamos a la opción “import a repository” de la cabecera:

    ![](https://github.com/ainaorozcogonzalez/UF1-A3._Documentaci-n-MP4UF1_-apuntes-_AinaOrozcoGonzalez/blob/main/img/rep3.PNG?raw=true)

    En “old repository’s clone URL” pegamos la URL del repositorio a importar mientras que en “Repository Name” ponemos el nombre que queremos que tenga nuestro repositorio clonado.

    Después elegimos si queremos que el repositorio sea público o privado. En caso de que queramos activar GitHub pages para poder publicar el repositorio (sólo HTML + CSS básico, no CSS) ha de ser público.

4. Cómo activar GitHub pages para un repositorio.

    Ir al apartado SETTINGS

    Ir a la opción “PAGES”. El repositorio ha de ser público para que pueda activarse “GitHub pages”. Si el repositorio es privado, GitHub solicita hacer un upgrade para poder hacerlo.

    Escogemos a qué rama asociar “pages” (por defecto “main”) y a qué carpeta (por defecto “root”) y aplicamos configuración con “Save”. Una vez procesado, nos muestra la URL del repositorio.

    ![](https://github.com/ainaorozcogonzalez/UF1-A3._Documentaci-n-MP4UF1_-apuntes-_AinaOrozcoGonzalez/blob/main/img/REP4.png?raw=true)


# Markdown

Introducción a lenguaje de marcas “Markdown”, usado por GitHub

 1. Recursos

    Recurso: Adam Pritchard: GitHub. Explicación básica sintaxis Markdown 
    Recurso: Página oficial Markdown - Sintaxis Markdown
    Recurso: w3schools - markdown introduction 
    Recurso: IONOS - tutorial de Markdown
    Recurso: Extensión markdown Visual Studio Code (Markdown All in One)

 2. Etiquetas básicas de Markdown

    * **Encabezados**. Llevan ya asociado un estilo por defecto cada uno.

     # H1
     ## H2
     ### H3
     #### H4
     ##### H5
     ###### H6

    * **Estilos de letra:**
        Itálica o cursiva: *texto* o _texto_
        Negrita: **texto** o __texto__
        : ~~palabra~~ (ALT+126)
        Anidar estilos: **palabra1  _palabra2_** (itálicas pero la segunda además negrita).

    * Listas:

        * ORDENADAS
         1. Primer elemento de lista

         2. Segundo elemento de lista

         (El número de orden no ha de ser necesariamente consecutivo)
         
         Tabulación→ 1. Elemento de sublista ordenado
        
        * DESORDENADAS

            *  Elemento de lista desordenada

            -  Otro elemento de lista desordenada
            
            + Otro elemento de lista desordenada
            
            (Se puede elegir cualquiera de los tres símbolos para crear una lista desordenada)
            
            Tabulación→ * Elemento de sublista desordenado

    * Párrafos:

        Para crear un bloque de texto nuevo (etiqueta), se introduce una línea en blanco.

    * Código:

        El código se ha de incluir entre acentos graves (`). Si en el código aparece un acento grave, se ha de introducir el carácter dos veces al principio de la sección del código.

        ``Todo esto es `código`.``

        También se puede marcar el área correspondiente al código insertando tres acentos graves al principio y al final. Junto a los tres iniciales se puede indicar el lenguaje (HTML, JavaScript) para que incluso se muestre con los colores adecuados:

        ```html
        <html>
            <head>
            </head>
        </html>
        ``` 

    * Enlaces:
        
        [Link](https://github.com/ "Título opcional del enlace")

        a) Primero se incluye el texto del link entre corchetes y posteriormente el link entre paréntesis).    
        
        b) El “título opcional del enlace” es el texto alternativo al pasar el ratón por encima.

    * Imágenes:
        
        Inline-style: 
        
        ![alt text](https://github.com/ainaorozcogonzalez/UF1-A3._Documentaci-n-MP4UF1_-apuntes-_AinaOrozcoGonzalez/blob/main/img/icono.png?raw=true "Título opcional de la imagen")

        Reference-style: 
        
        ![alt text][logo]

        [logo]: https://github.com/ainaorozcogonzalez/UF1-A3._Documentaci-n-MP4UF1_-apuntes-_AinaOrozcoGonzalez/blob/main/img/icono.png?raw=true "Logo Title Text 2"

    * Tablas:

        | Encabezado1        | Encabezado2         | Encabezado2  |
        | ------------------ |:-------------------:| ------------:|
        | Item1              | boligrafos          | $20          |
        | Item2              | Grapadoras          | $1000        |
        | Item3              | Lapices             | $150         |

        a) Los dos puntos se usan para alinear las columnas (izquierda, centrado, derecha).
        
        b) No es necesario que estén alineadas verticalmente. Solo a nivel visual para claridad del código.
        
        c) Se han de poner al menos tres guiones para separar cada encabezado

    * Notas al pie de página:

        Texto con enlace a nota de pie de página [^1]

        [^1]: Aquí encuentras el texto de la nota al pie de página.

    * Listas de verificación:
        - [x] A
        - [ ] B
        - [ ] C
        
# HTML

## Introducción a HTML

1. Recursos
        
    Recurso: Documento Fonaments d’HTML

    Recurso:  Mozilla Developer- HTML básico

    Recurso: Conversor PNG a ICO online convertICO

    Recurso: Insertar icono de pestaña en HTML

    Servicio: fontawesome

2. Características HTML

    Las siglas de HTML corresponden con “HyperText Markup Language”, que tiene el siguiente significado:

     - __HyperText__, cuyo significado es hipertexto, que no es más que un texto que enlaza con otros contenidos, que pueden ser otro texto u otro archivo. Esto es la base del funcionamiento de la web tal y como la conocemos, que no es más que páginas y recursos interconectados.

     - __Markup__, que significa marca o etiqueta, ya que todas las páginas web están construidas en base a etiquetas, desde las primeras versiones hasta las últimas etiquetas de HTML5. Un ejemplo de una etiqueta HTML es la que identifica a un párrafo, que se compone de la etiqueta, el contenido de la etiqueta y el cierre del párrafo: <p>HOLA</p>.

     - __Language__, cuyo significado es lenguaje, porque HTML es un lenguaje, es decir, tiene sus normas, tiene su estructura y una serie de convenciones que nos sirven para definir tanto la estructura como el contenido de una web. Algo importante a tener en cuenta y con lo que no hay que confundirse, es que porque HTML sea un lenguaje no quiere decir que sea un lenguaje programación. HTML no lo es, ya que no tiene estructuras de lenguaje de programación, como los bucles, las condiciones, las funciones, etcétera.

    Es decir, que HTML no es un lenguaje de programación; es un lenguaje de marcado que define la estructura de su contenido. HTML consiste en una serie de elementos que usarás para encerrar diferentes partes del contenido para que se vean o comporten de una determinada manera.

    Esto implica que la información a mostrar ha de ir “etiquetados” para formar elementos que el navegador web sepa interpretar de qué tipo de información se trata y como tal sepa como representarlos.

    Las partes principales del elemento son:

     - __La etiqueta de apertura__: consiste en el nombre del elemento (en este caso, p), encerrado por paréntesis angulares (< >) de apertura y cierre. Establece dónde comienza o empieza a tener efecto el elemento —en este caso, dónde es el comienzo del párrafo-.


     - __La etiqueta de cierre__: es igual que la etiqueta de apertura, excepto que incluye una barra de cierre (/) antes del nombre de la etiqueta. Establece dónde termina el elemento —en este caso dónde termina el párrafo—.


     - __El contenido__: este es el contenido del elemento, que en este caso es sólo texto.


     - __El elemento__: la etiqueta de apertura, más la etiqueta de cierre, más el contenido equivale al elemento.

    Los elementos pueden también tener atributos, que se ven así:

    Los atributos contienen información adicional acerca del elemento, la cual no quieres que aparezca en el contenido real del elemento. Aquí class es el nombre del atributo y editor-note el valor del atributo. En este caso, el atributo class permite darle al elemento un nombre identificativo, que se puede utilizar luego para apuntarle al elemento información de estilo y demás cosas.

    Los atributos contienen información adicional acerca del elemento, la cual no quieres que aparezca en el contenido real del elemento. Aquí class es el nombre del atributo y editor-note el valor del atributo. En este caso, el atributo class permite darle al elemento un nombre identificativo, que se puede utilizar luego para apuntarle al elemento información de estilo y demás cosas.

    Los atributos siempre se incluyen en la etiqueta de apertura de un elemento y deben tener siempre:

     - Un espacio entre este y el nombre del elemento (o del atributo previo, si el elemento ya posee uno o más atributos).
    
     - El nombre del atributo, seguido por un signo de igual (=).
    
     - Comillas de apertura y de cierre, encerrando el valor del atributo.

    Puedes también colocar elementos dentro de otros elementos. Esto se llama anidamiento.


3. Estructura documento HTML

    Un documento HTML tiene la siguiente estructura básica:

        <!DOCTYPE html>
        <html>
        <head>
            <meta charset="utf-8">
            <title>Mi pagina de prueba</title>
            <link rel="icon" href="favicon.png">
        </head>
        <body>
            <img src="images/firefox-icon.png" alt="Mi imagen de prueba">
        </body>
        </html>

    Donde:

     - < !DOCTYPE html> — el tipo de documento. Es un preámbulo requerido. Anteriormente, cuando HTML era joven (cerca de 1991/2), los tipos de documento actuaban como vínculos a un conjunto de reglas que el código HTML de la página debía seguir para ser considerado bueno, lo que podía significar la verificación automática de errores y algunas otras cosas de utilidad. Sin embargo, hoy día es simplemente un artefacto antiguo que a nadie le importa, pero que debe ser incluido para que todo funcione correctamente. Por ahora, eso es todo lo que necesitas saber.


     - < html></ html> — el elemento < html>. Este elemento encierra todo el contenido de la página entera y, a veces, se le conoce como el elemento raíz (root element). 

     - < head></ head> — el elemento < head>. Este elemento actúa como un contenedor de todo aquello que quieres incluir en la página HTML que no es contenido visible por los visitantes de la página. 
        
        Incluye cosas como:

        - Palabras clave (keywords)

        - Una descripción de la página que quieres que aparezca en resultados de búsquedas

        - Código CSS para dar estilo al contenido

        - Declaraciones del juego de caracteres: < meta />— < meta>. Añade metainformación a la página. Podemos poner varias marcas < meta> que dan información no visible del documento. En el caso del ejemplo, este elemento establece el juego de caracteres que tu documento usará en utf-8, que incluye casi todos los caracteres de todos los idiomas humanos. Básicamente, puede manejar cualquier contenido de texto que puedas incluir. No hay razón para no establecerlo, y puede evitar problemas en el futuro. 

        - El título de la página: < title></ title> — el elemento < title> establece el título de tu página, que es el título que aparece en la pestaña o en la barra de título del navegador cuando la página es cargada, y se usa para describir la página cuando es añadida a los marcadores o como favorita.

        - El icono (llamado favicon) de la página. Podemos usar la etiqueta < link> y el atributo rel="icon" para agregar un favicon de navegador en HTML. El tamaño más común para crear un favicon es 16x16 píxeles. Sin embargo, también pueden aparecer en dimensiones un poco más grandes (32x32). Casi todos los navegadores modernos admiten imágenes PNG pero si nos encontramos con problemas, por ejemplo con navegadores como IE10 y sus versiones anteriores, podemos utilizar imágenes ICO.

        - El enlace con otros ficheros relacionados con el documento (hojas de estilo, codigo Javascrip…), etc.
    
    - < body>< /body> — el elemento < body>. Encierra todo el contenido que deseas mostrar a los usuarios web que visiten tu página, ya sea texto, imágenes, videos, juegos, pistas de audio reproducibles, y demás. Los elementos HTML descendientes de < body> se pueden clasificar en:

        - Elementos de bloque (block elements). Son grandes estructuras que contienen otros elementos de bloque, elementos de línea o texto. Normalmente el navegador los muestra como bloques independientes y separa un bloque de otro con una línea en blanco. Son por ejemplo los títulos, los párrafos, las listas o las tablas.


        - Elementos de línea (inline elements). Son pequeñas estructuras que representan o describen pequeños trozos de texto o datos. Pueden contener solo texto u otros elementos de línea. Normalmente el navegador los muestra en línea uno tras otro dentro del bloque que los contiene. Son un ejemplo los hiperenlaces, las citas o las imágenes.

    Si lo comparamos con un procesador de textos, podemos pensar en un párrafo como un elemento de bloque y una palabra enfatizada en negrita como un elemento de línea.

4. Etiquetas básicas HTML
    
    - Encabezados (<h1>...<h6>) Permiten especificar que ciertas partes del contenido son encabezados, o subencabezados del contenido. Son elementos de bloque.


    - Párrafos (<p>). Se utilizan para encerrar párrafos de texto, entendiendo como párrafo un conjunto de frases relacionadas entre sí. Son elementos de bloque.

    - Listas:

        - Las listas desordenadas son aquellas en las que el orden de los ítems no es relevante, como en una lista de compras. Estas son encerradas en un elemento <ul> (unordered list).

        - Las listas ordenadas son aquellas en las que el orden sí es relevante, como en una receta. Estas son encerradas en un elemento <ol> (ordered list).

    Cada elemento de la lista se coloca dentro de un elemento <li> (list item).

    - Enlaces (<a>). Para convertir algún texto dentro de un párrafo en un víncu.

    - Salto de línea (<br/>) Inserta un “intro” en un párrafo.

    - Línea separadora (<hr/>). Muestra una línea horizontal.

    - Cita (<blockquote>) Formatea el texto como una cita. Es de tipo bloque.

    - Más elementos en el documento “Fonaments d’HTML”

5. Organización del código

    Es fundamental que el código fuente HTML que generemos sea legible dado que normalmente no trabajaremos solos y que lo que hemos desarrollado sea legible puede ayudar a los que trabajan con nosotros a entender qué hemos hecho y por qué lo hacemos. Hay varias técnicas para que el código sea legible y esté bien organizado:

    
     - Comentarios. En un documento HTML podemos poner anotaciones que no se visualizarán cuando la página web se vea en el navegador pero que son útiles para desarrollar la web. La sintaxis es <!-- comentario --> 

     - Sangrado del código. Las etiquetas HTML se abren y se cierran. El navegador web no interpreta ni saltos de página ni tabuladores pero para nuestro análisis del código necesitamos ver una estructura coherente.

        <div>
        <p>Contenido del párrafo <a href="http://web.org">enlace externo</a></p>
        </div>

        Como se puede ver, los elementos de línea (<a> en el ejemplo) no se sangran

     - Organización de ficheros. Cuando la aplicación web es muy grande tendrá archivos de muchos formatos (.html, .css, imágenes, videos, etc..). Hemos de organizar nuestra aplicación en directorios para que todos esos ficheros estén bien ordenados.

6. Fontawesome

    1. Darse de alta en la página web https://fontawesome.com/


    2. Añadir tu Kit’s code al proyecto:

	    <script src="https://kit.fontawesome.com/09f87768b9.js" crossorigin="anonymous"></script>

        Copia tu “kit's code” dentro de la sección <head> de cada página en tu proyecto donde quieras usar fontawrsome mediante ese kit. La parte subrayada dependerá del ID de tu kit’s code.


    3. Encuentra y añade cualquiera de los iconos GRATUITOS al proyecto

    Busca entre los iconos de la web de Fontawesome los que necesites y añade el nombre de icono y estilo con sus clases CSS dengro una etiqueta HTML <i> que ya te proporciona directamente la web.

## 3. CSS ##

El CSS, nos ayudará a dar forma a nuestros documentos HTML, se encargará de la parte estética.

### UBICACIÓN DE LAS PROPIEDADES CSS ###

1. EN LA ETIQUETA

Usando el atributo _style_ de la siguiente manera
\<p style="text-align: center; color: ">


2. EN LA CABECERA DEL DOCUMENTO HMTL

Usaremos el mismo atributo que antes, pero en el _head_. Esto nos servirá cuando queramos que más de un elemento tenga la misma estética, como por ejemplo que todos los titulos sean rosas y esten alineados en el centro.


3. EN UN DOCUMENTO EXTERNO

Crearemos un nuevo documento con la extensión _.css_
En el head de nuestro documento HTML pondremos <link rel="stylesheet" href="estils.css" type="text/css"> y en nuestro fichero estils.css p{ text.align:center; color:blue; }.
Usando esta última forma podemos reutilizar nuestro fichero CSS para diferentes documentos HTML.

### SINTAXIS BÁSICA ###

__1. SINTAXIS GENÉRICA__

selector {
    declaración1
    declaración2
}


__2. AGRUPAR SELECTORES__

 Por ejemplo, si queremos aplicar el mismo color a los titulos y subtitulos podemos escribir:
 h1,h2 {color:azul}

__3. TIPOS DE SELECTORES__

+ SELECTOR DE CLASE

    Dentro de cada etiqueta que queramos que tengan el mismo estilo escribiremos class="NombreClase", y en el head escribiremos _.NombreClase_ 
    

+ SELECTOR DE ID

    Es parecido al selector de clase, solo tenemos que escribir id="NombreID", dentro de la etiqueta, y en head escribiremos _#NombreID_


+ SELECTOR UNIVERSAL

    Este tipo de selector selecciona todos los elementos de la página para aplicar estilos.
    Por ejemplo:
    * { border: 1px solid #000000}, para poner que toda la pagina tenga un borde negro liso de 1 píxel.
 
+ SELECTOR DE ATRIBUTOS

    Selecciona elementos en función del atributo, por ejemplo si queremos que todas las fotos con el atributo _alt_ tenga un borde negro escribiremos:
    img [alt] {border: 1px solid }

+ SELECTOR DE HIJOS

    Sirve para seleccionar elementos concretos y aplicarles un estilo especifico. Por ejemplo: 
    h1>strong { color:rosa }, hará que solo los títulos _h1_ que tengan el selector de strong sean rosas.

+ SELECTOR DE DESCENDIENTES

    Hace que los selectores de descendientes seleccionen los elementos pertinentes en cualquier punto de la jerarquía del elemento


+ PSEUDOCLASES

    Sirve para definir estilos a los diversos estados de los elementos, como por ejemplo, indicar que es un link.
    Para ello escribiremos: 
    a:link {color:green}

### MÁRGENES, BORDES Y RELLENO ###

+ MARGIN

Para definir los márgenes, escribiremos _margin-_, y dependiendo cual queramos definir: -top, -right, -bottom, -left.

+ BORDER

Al borde, le podemos cambiar, la anchura, el estilo y el color.
Podemos definirlo todo junto

O por separado
border-right: [anchura, color, estilo]
border-top: [anchura, color, estilo]
...

+ PADDING

Es el relleno de nuestro documento y es para definir cuanto ocupará el contenido de nuestro documento. Funciona igual que el margin: padding-top, padding-bottom,...


### GOOGLE FONTS ###
Con CSS, podemos cambiar la tipografía a nuestro texto, para ellos usaremos la web de google fonts.
Seleccionaremos la tipografía que deseemos
Copiaremos el <link> en el head, encima de style
Y el _CSS rules to specify families_ en style donde queramos que se aplique ese estilo
