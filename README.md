# UF1-A3._Documentaci-n-MP4UF1_-apuntes-_AinaOrozcoGonzalez

# GitHub

## Como crear un repositorio
 1. Crear un repositorio nuevo
<img scr="img/rep1.png">
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

    b) **Sincronizar un repositorio local local ya existente desde línea de comandos:**

    Navegamos en local hasta la carpeta raíz del repositorio local a vincular con el repositorio vacío recién creado en GitHub.

