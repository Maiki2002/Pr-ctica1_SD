## Práctica1: Introducción a Git 

### Descripción 
El programa HolaMundo.py imprime el mensaje *"Hola Git"*.

El objetivo de esta práctica es repasar los comandos básicos de Git, por lo que se hizo:
- Crear un repositorio local y conectarlo con un repositorio remoto
- Añadiendo archivos para realizar commits
- Realizar commits con mensajes 
- Uso del archivo .gitignore
- Probar comando `git stauts`
- Subir cambios al repositorio remoto
- Craer archivo README.md

### HolaMundo.py
Necesitarás ir a la ruta en donde se encuentra HolaMundo.py y ejecutar el siguiente comando en la terminal
~~~
python3 HolaMundo.py
~~~

### Comandos Git utilizados
Crear un repositorio
~~~
git init
~~~
Agregar repositorio remoto a local
~~~
git remote add origin <link del repositorio>
~~~
Preparar los archivos para ser incluidos en el commit
~~~
git add
~~~
Guardar los cambios en el área de preparación
~~~
git commit -m "Mensaje"
~~~
Envíar los cambios al repositorio remoto
~~~
git push origin main
~~~

### .gitignore
Este archivo se creó con la finalidad de ignorar los archivos que no se desean subir en el repositorio remoto.

El archivo contiene la siguiente linea
~~~
*.log
~~~
![](/images/image.png)

Al preparar archivos con `git add .`debe preparar todos los archivos excepto los que contengan la extensión `.log`.

![](/images/image-1.png)
Cuando se suban los cambios, el archivo .debug.log no debe estar en el repositorio remoto.