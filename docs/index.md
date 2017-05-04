## Bienvenido

Este sitio pretende ser una guia completa para el uso del validador para los padrones del SIPP-G, cubriremos desde la instalación hasta la ejecución de los scripts que contiene el validador.


## Que es SIPP-G Validator

SIPP-G Validator es un conjunto de scripts que analizan campos especificos de un conjunto de datos en formato csv, para validar ciertas caracteristicas que debe cumplir una CURP de un usuario, como lo es la longitud, y las claves de la entidad formadas por dos digitos.

### Guia de instalación y Requerimientos :point_down:

#### Requerimientos del sistema

Para instalar el validador asegurate de que tu equipo tenga las siguientes caracteristicas:

* GNU/Linux, Unix, or macOS
* Windows 7 or 10 
* 4GB RAM or higher

#### Instalación en Windows

SIPP-G Validator necesita de [Python](https://www.python.org/) para poder ejecutarse, instalaremos [Python](https://www.python.org/)
en su versión mas reciente la cual es **Python 3.6.1**

Si tu plataforma es Windows puedes dar click en el siguiente enlace y ejecutar el instalador :point_down:

* [Python :snake: ](https://www.python.org/downloads/)

#### Instalación en macOS

Si tu palaforma esta basa en **UNIX** como **macOS** ejecutaremos los siguientes comandos dentro de la terminal:

```markdown
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ nano ~/.bash_profile
$ export PATH=/usr/local/bin:$PATH

# guardamos los cambios presionando ctr + o y salimos de nano presionando ctr + x

$ source ~/.bash_profile

```

Ahora para estar seguros de que Homebrew esta correctamente instalado ejecutamos el comando: 
```markdown 
brew doctor 
``` 
si nos aparece el siguiente mensaje 
```markdown 
Your system is ready to brew.
``` 
Procedemos con la instalación de **Python**, usaremos Homebrew para instalar **Python** ejecutamos el siguiente comando:
```markdown 
$ brew search python
```
Una vez ejecutado en la terminal nos aparecera una lista de lo que podemos instalar algo como esto:
```markdown 
#Output
app-engine-python          micropython                python3                 
boost-python               python                     wxpython                 
gst-python                 python-markdown            zpython                  
homebrew/apache/mod_python               homebrew/versions/gst-python010        
homebrew/python/python-dbus              Caskroom/cask/kk7ds-python-runtime     
homebrew/python/vpython                  Caskroom/cask/mysql-connector-python   
```
 Instalaremos **Python 3** nos aparece en el listado:
 ```markdown
 $ brew install python3
 ```
Listo ya tenemos **Python3** instalado en nuestros equipos, para verificar que esta correctamente instalado **Python** en nuestro equipo ejecutamos el siguiente comando que nos devolvera la versión de **Python** instalada:
```markdown
 $ python --version
 ```
 Si obtenemos como la salida en la terminal la versión de **Python** instalada todo esta correcto.
 
 Para actualizar nuestro **Python3** primero actualizaremos **brew** y despues **Python**, ejecutamos los siguientes comandos dentro de la terminal:
 ```markdown
$ brew update
$ brew upgrade python3
 ```
 ¡ Bien hecho tu versión de **Python** esta actualizada !

#### Instalación en Linux

En Linux **Python3** viene preinstalado, para asegurarnos que nuestro sistema esta actualizado ejecutamos los siguientes comandos en nuestra terminal:
```markdown
$ sudo apt-get update
$ sudo apt-get -y upgrade
```
Una vez terminado el proceso ha sido completado podemos verificar la versión de **Python3** que esta instalada en nuestro sistema ejecutando el siguiente comando:
```markdown
$ python3 -V
# Output 
Python 3.x.x
```
Como salida veremos la versión de python instalada en nuestro sistema.
