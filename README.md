# Curso de Python: PIP y Entornos Virtuales

Repaso de comandos:

* pwd: Nos indica la ubicación actual en la consola.
* mkdir: Crear una nueva carpeta.
* ll: Visualizar el listado de archivos en la ubicación actual.
* clear: Limpiar la consola.
* git init: Inicializar un proyecto con Git.
* touch: Crear un nuevo archivo.

## Instalacion en Windows (WSL) y Linux

Si eres usuario de Windows con WSL o de Linux lo más probable es que ya tengamos Python instalado.

Podemos verificarlo de la siguiente manera:

```
python3
```

Esto inicia el intérprete interactivo de Python indicando la versión que tiene instalada.

Para salir del intérprete interactivo de Python ejecuta la siguiente instrucción:

```
exit()
```

En caso de no tener instalado Python, ejecuta los siguiente comandos:

1. Actualiza los paquetes disponibles desde los repositorios configurados:

```
sudo apt update
```

2. Actualiza todos los paquetes instalados a sus versiones más recientes disponibles:

```
sudo apt -y upgrade
```

Con esto ya deberiamos tener Python instalado. Verifica ejecutando el siguiente comando:

```
python3 -V
```

Debemos asegurarnos de tener instalado el gestor de dependencias de Python, ejecuta el siguiente comando:

```
sudo apt install -y python3-pip
```

Verifica que el paquete ha sido instalado:

```
pip3 -V
```

Por último vamos a instalar algunas dependencias útiles dentro de Python en un entorno profesional:

```
sudo apt install -y build-essential libssl-dev libffi-dev python3-dev
```

## Python con VSCode

Extensiones necesarias para un entorno profesional:

* Python: https://marketplace.visualstudio.com/items/?itemName=ms-python.python

* Si eres usuario de Windows con WSL: https://marketplace.visualstudio.com/items/?itemName=ms-vscode-remote.remote-wsl

Crear un proyecto de Python:

* Crear una carpeta:

```
mkdir py-project
```

* Cambiar a la carpeta creada:

```
cd py-project
```

* Abrir el proyecto con VSCode:

```
code .
```

* Crea un archivo `hello.py` con el siguiente contenido:

```python
print('Hola desde mi maquina')
```

* Ejecuta el archivo:

```
python3 hello.py
```

## Python con Git y GitHub

Comandos para la configuración de Python con Git y GitHub:

* Inicializar el proyecto con Git:

```
git init
```

* Enlazar nuestro proyecto con el repositorio remoto:

```
git remote add origin <url>
```

* Verificar el enlace agregado:

```
git remote -v
```

* Agregar cambios al repositorio:

```
git add *
```

* Confirmar los cambios:

```
git commit -m "Mi primer archivo"
```

* Subir los cambios al repositorio remoto:

```
git push origin master
```

Configuración para el `.gitignore`: https://www.toptal.com/developers/gitignore/api/windows,linux,macos,python