# LaboratorioGit

---
## Crear un repositorio en local.

### Abre tu terminal y navega hasta el directorio donde deseas crear el repositorio. 
 
Utilizaremos los comandos de ls y cd.
    Ls para revisar las carpetas y ficheros que tenemos.
    Cd para abrir una carpeta que tengamos.
Podemos utilizar code . para abrir en VisualStudioCode la carpeta.

### Crea una carpeta con el nombre del repositorio.
```
mkdir LaboratorioGit
```
### Ingresa a la carpeta que acabas de crear.
```
cd LaboratorioGit
```
### Inicializa el repositorio de Git
```
git init
```
---
## Subir el repositorio a GitHub.

### Crea un nuevo repositorio en GitHub

Entramos en GitHub y en el apartado de New podemos crear un nuevo repositorio.
Tendremos Owner que será el dueño y en Repositorio name será el nombre del repositorio que le daremos.
Ahí podremos crear el README, o crearlo manualmente en nuestra carpeta local.

### Copia el URL del repositorio que acabas de crear en GitHub.

Una vez dentro del repositorio que hemos creado en el apartado anterior, pulsamos  <> Code. 
Dentro de local vamos a HTTPS y copiamos la URL. (También podríamos usar SSH.)

### Conecta tu repositorio local con el repositorio en GitHub.

Para conectar nuestro repositorio local con el repositorio en la nube, vamos a nuestra terminal y ejecutamos:

```
git remote add origin https://github.com/Mandarina28/LaboratorioGit.git
```
Si es con SSH simplemente si lo tenemos configurado copiamos la URL y la copiamos donde hemos pegado esa.

### Verifica que la conexión se haya establecido correctamente 
Con este codigo podemos ver si la configuración de git está apuntando correctamente al repositorio en la nube: 
```
git remote -v
```
---
## Hacer un commit y un push.
### Crea un archivo en la carpeta del repositorio
Creamos un archivo HTML (index.html) y hacemos un pequeño código. Guardamos el código.

### Añade el archivo a Staging
En la terminal escribimos si queremos añadir todos los cambios de los diferentes archivos
```
git add .
```
o si queremos que sea solo un archivo espedífico:
```
git add ./index.html
```

### Crea un commit con un mensaje descriptivo
Después de que los archivos hayan pasado a Staging escribimos en la terminal:
```
git commit -m "Aádir index.html con mensaje"
```

### Sube los cambios al repositorio en GitHub.
```
git push
```
---
## Crear una rama.
### Crea una rama llamada "development"
### Cambia a la nueva rama
### Realiza algunos cambios en el archivo que creaste
### Añade y haz commit con los cambios en la rama "development"
### Sube los cambios a GitHub.
---
## Hacer un merge.
### Vuelve a la rama "main"
### Haz un merge de la rama "development" a la rama "main"
### Si no hay conflictos los cambios realizados en la rama "development" se incorporarán a la rama "main"
### Haz un push de los cambios al repositorio en GitHub.

