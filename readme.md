# PASOS PARA CREAR UN REPOSITORIO DE MANERA LOCAL DESDE 0

1. Crear un directorio en la ubicación que desees. 
   * Manera manual con la interfaz gráfica: ![Aparece una imagen de como crear una carpeta con interfaz gráfica](/Screenshot_1.png "Crear carpeta con interfaz gráfica.")
   * Usando comandos: ![Aparece una imagen de como crear una carpeta con comandos](/Screenshot_2.png "Crear carpeta con comandos.")
2. Situarse dentro de la carpeta que acabamos de crear desde Bash y ejecutar el comando `git init` que lo que hará es crear la carpeta .git invisible que nos permitirà desplazarnos por el tiempo. ![Aparece una imagen del uso de git init](/Screenshot_3.png "Crear repositorio usando git init.")
3. Ahora que ya tenemos creado un repositorio lo que hacemos es crear nuestro primer fichero que será el readme.md actual.
   - Usando la interfaz gráfica. ![Aparece una imagen de como crear un fichero readme.md con interfaz gráfica](/Screenshot_4.png "Crear fichero readme.md con interfaz gráfica.")
   - Usando comandos. ![Aparece una imagen de como crear un fichero readme.md con comandos](/Screenshot_5.png "Crear fichero readme.md con comandos.") 
4. Añadimos los ficheros que tenemos untracked a la stagin area (Área previa donde pones los ficheros que quieres commitear) usando el comando `git add`
   - Podemos usar `git add .` para añadir todos los cambios. ![Aparece una imagen de como usar git add .](/Screenshot_7.png "Uso del comando git add .")
   - Podemos usar `git add readme.md` para añadir solamente el fichero readme.md ![Aparece una imagen de como usar git add readme.md](/Screenshot_6.png "Uso del comando git add readme.md.")
5. Realizamos el commit una vez tenemos los ficheros en el staging area con el comando `git commit -m "Mensaje del commit"` ![Aparece una imagen de como usar git commit -m](/Screenshot_8.png "Uso del comando git commit -m") Ahora mismo tenemos el commit hecho en el repositorio local. 
6. Para poder juntar este repositorio local con uno de remoto lo que tenemos que hacer a continuación es crear el repositorio remoto, en este caso, crearemos uno desde GitHub. ![Aparece una imagen de como crear un repositorio remoto](/Screenshot_9.png "Creación de un repositorio remoto.")
7. Una vez creado, para sincronizar los repositorios, tendremos que ejecutar las siguientes líneas de comandos que encontraremos en la parte de abajo de la página del GitHub del repositorio creado. ![Aparece una imagen de que comandos tengo que hacer para sincronizar los repositorios](/Screenshot_10.png "Lista de comandos para sincronizar los repositorios") ![Aparece una imagen de los comandos ejecutados por mi para sincronizar los repositorios](/Screenshot_11.png "Lista de comandos ejecutados por mi para sincronizar los repositorios") 
8. Comprobación de si se han sincronizado correctamente los dos repositorios. Podemos realizarlo de dos maneras diferentes:
   - Recargando la página del GitHub y vemos si el commit ha sido actualizado de manera correcta. ![Aparece una imagen del GitHub con el commit actualizado](/Screenshot_12.png "GitHub con el commit actualizado") 
   - Usando el comando `git log` y si vemos que en último commit realizado nos aparece origin/main. ![Aparece una imagen del uso del comando git log](/Screenshot_13.png "Uso del comando git log") 