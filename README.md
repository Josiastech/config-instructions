Python, Django y entornos virtuales
=======

Cuando trabajamos en Django cada proyecto puede necesitar diferentes especificaciones, desde la versión hasta dependencias muy puntuales. Para solucionarlo tenemos los entornos virtuales. Estos se encargan de crear un entorno apartado del sistema, basado en Python, con el objetivo de tener distintos proyectos al mismo tiempo y con distintas características (en dependencias y versiones). Uno de ellos es virtualenv.

Instalando Python, pip y virtualenv
En Mac OS:
* Primero debemos instalar Hombrew. Este es un gestor de paquetes de UNIX decente para Mac OS. Abrimos terminal y digitamos el siguiente comando:

$ ruby -e "$ (curl-FSSL https://raw.github.com/mxcl/homebrew/go)"

* Después debemos pasar Hombrew a nuestra ruta del sistema para asegurarnos de darle prioridad al Hombrewinstalado sobre cualquier otra versión que hayamos tenido. Así que en terminal ejecutamos:

$ export PATH = / usr / local / bin: $ PATH

* Ahora deberás reiniciar tu terminal. Procedemos a instalar Python, pip  y virtualenv.

* Para instalar Python en terminal:

$ brew install python -- framework

* Luego de esto instalas pip con easy_install:

$ easy_install pip

* Ya con pip instalado instalas virtualenv:

$ pip virtualenv

En Linux:
En Linux ya tienes instalado Python así que solo queda instalar easy_install, pip y virtualenv. Ten en cuenta sersuperusuario para cada uno de los comandos a ejecutar.

* Para easy_install (si no lo tienes instalado):

$ sudo apt-get install python-setuptools python-dev build-essential

* Ahora instalamos pip y virtualenv:

$ easy_install pip
$ pip virtualenv

En Windows: 
- Descargas Active Python, con este instalarás Python, pip y easy_install.
* Ahora solo queda abrir un cmd y ejecutar:

$ pip virtualenv

Crear un entorno virtual

Para crear un entorno virtual basta con determinar la carpeta en la que se ubicará y luego ejecutar:

$ virtualenv __nombre__

Siendo __nombre__ el nombre del entorno que deseas crear.  Para acceder a él deberás colocar:

$ cd __nombre__
$ source bin/activate

Listo.

* Por último, dentro del entorno virtual para instalar Django en cualquier sistema operativo solo basta con ejecutar:

$ pip django -U

* "U" lo colocamos para obtener la última versión.

* Ahora todo se instalará y ejecutará dentro del entorno virtual.  Si deseas colocar algo de manera global la instalación deberá ser fuera de este.