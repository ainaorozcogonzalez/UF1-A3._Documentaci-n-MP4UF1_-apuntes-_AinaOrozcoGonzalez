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
        
        [Link](https://ejemplo.com/ "Título opcional del enlace")

        a) Primero se incluye el texto del link entre corchetes y posteriormente el link entre paréntesis).    
        
        b) El “título opcional del enlace” es el texto alternativo al pasar el ratón por encima.

    * Imágenes:
        
        Inline-style: 
        
        ![alt text](https://github.com/img/icon48.png "Título opcional de la imagen")

        Reference-style: 
        
        ![alt text][logo]

        [logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"

    * Tablas:

        | Tables        | Are           | Cool  |
        | ------------- |:-------------:| -----:|
        | col 3 is      | right-aligned | $1600 |
        | col 2 is      | centered      |   $12 |
        | zebra stripes | are neat      |    $1 |

        a) Los dos puntos se usan para alinear las columnas (izquierda, centrado, derecha).
        
        b) No es necesario que estén alineadas verticalmente. Solo a nivel visual para claridad del código.
        
        c) Se han de poner al menos tres guiones para separar cada encabezado

    * Notas al pie de página:

        Texto con enlace a nota de pie de página [^1]

        [^1]: Aquí encuentras el texto de la nota al pie de página.

    * Listas de verificación:
        - [ ] A
        - [x] B
        - [ ] C
        
        (Dejar un espacio en blanco entre los dos corchetes en las que aparezcan vacias)




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

        Algunos elementos no poseen contenido, y son llamados elementos vacíos. Por ejemplo, el elemento <img>: <img src="images/firefox-icon.png" alt="Mi imagen de prueba"> posee dos atributos, pero no hay etiqueta de cierre </img> ni contenido encerrado.

    
    2. Características HTML