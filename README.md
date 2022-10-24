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
