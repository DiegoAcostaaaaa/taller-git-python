Creación del Repositorio en GitHub
Vamos a ir a el primer link en el apartado de herramientas e iniciaremos sesión en github,
despues vamos a crear un nuevo repositorio de nombre “taller-git-python”, este mismo
deberá ser público y no inicializamos con README, para hacerlo después de manera
manual. Finalmente copiamos el URL del repositorio porque lo usaremos más adelante.

Clonación del Repositorio y Creación de Archivos
Ahora dentro la terminal, en mi caso, en la terminal de VS Code vamos a clonar el
repositorio usando “git clone URL”, en el cual el URL es el que ya copiamos de nuestro
repositorio en el paso anterior, ahora dentro del repositorio clonado creamos un directorio
con nombre “app” y dentro de ese directorio creamos tres archivos Python.

Seguimiento y Confirmación de Cambios (Commits)
Primero vamos a ver el estado del repositorio y deberíamos ver que los archivos de este, no
tienen seguimiento, entonces vamos a darle seguimiento con el comando “git add *.py” así
vamos a darle seguimiento a todos los archivos que tengamos de Python.
Seguido a eso vamos a hacerle un commit a estos archivos con el comando “git commit -m
‘Confirmamos estos archivos para que se guarden’”, el “-m” es para poner un mensaje que
describa lo que estamos haciendo.
Por último, vamos a subir estos cambios al repositorio remoto en GitHub con el comando
“git push origin main”, después de esto puedes ver que tu repositorio en GitHub ya no está
vacío y contiene la carpeta “app”.

Creación y Uso de Ramas
En este paso lo primero que haremos será crear una rama llamada “nueva-funcionalidad”, lo
haremos con el comando “git branch nueva-funcionalidad”, ahora nos moveremos a esa
rama con “git checkout nueva-funcionalidad” y una vez dentro de ella vamos a modificar dos
de los archivos Python que ya teníamos.
Es entonces cuando procedemos a confirmar los cambios con el comando “git commit -a -m
‘Confirmamos los cambios hechos en la rama nueva-funcionalidad’”, lo que hicimos con el
“-a” fue ahorrarnos escribir el comando “add”, pero al final pasa por el mismo procedimiento.
Después de todo vamos a subir los archivos al repositorio en GitHub, lo anterior con el
comando “git push origin nueva-funcionalidad”

Fusionar Ramas y Mantener el Repositorio Sincronizado
Antes de cualquier cosa vamos a regresar a la rama “main” para después fusionar la rama
“nueva-funcionalidad” con la rama “main”, lo anterior se logra con el comando “git merge
nueva-funcionalidad”, para confirmar la fusión lo vemos con el comando “git log”, lo que
abrirá un historial de los cambios hechos y ahi aparecera la fusión. Ya una vez hecho todo
lo anterior, actualizaremos el repositorio en GitHub con el comando “git push origin main”

Cambios en GitHub y Sincronización Local
Dentro de nuestro repositorio dentro de GitHub vamos a dirigirnos a uno de los tres archivos
y lo vamos a modificar, después confirmamos los cambios hechos en el archivo con el botón
que dice Commit Changes.
Ahora desde la terminal con la que estábamos trabajando vamos a actualizar los cambios
que se hicieron en el repositorio de GitHub a nuestra computadora, esto con el comando “git
pull origin main”. Por último, podremos ver los cambios hechos en el repositorio de GitHub
dentro del archivo en nuestra computadora.
