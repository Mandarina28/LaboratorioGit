# LaboratorioGit

[Visita el index](https://mandarina28.github.io/LaboratorioGit/)
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

Para conectar nuestro repositorio local con el repositorio remoto en GitHub, vamos a nuestra terminal y ejecutamos:

```
git remote add origin https://github.com/Mandarina28/LaboratorioGit.git
```
Si es con SSH simplemente si lo tenemos configurado, copiamos la URL y la usamos en el comando.

### Verifica que la conexión se haya establecido correctamente 
Con este código podemos ver si la configuración de git está apuntando correctamente al repositorio en la nube: 
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
o si queremos que sea solo un archivo en concreto:
```
git add ./index.html
```

### Crea un commit con un mensaje descriptivo
Después de que los archivos hayan pasado a Staging escribimos en la terminal:
```
git commit -m "Añadir index.html con mensaje"
```

### Sube los cambios al repositorio en GitHub.
En este caso hacemos push a secas porque no tenemos mas ramas así que indudablemente será main, si no especificamos.
```
git push
```
---
## Crear una rama.

### Crea una rama llamada "development"
```
git branch development
```
podemos revisar las ramas con: 
```
git branch -a
```
### Cambia a la nueva rama
Con este código solo cambiamos la nueva rama en local.
```
git checkout development 
```
### Realiza algunos cambios en el archivo que creaste
Realiza cambios en index.html

### Añade y haz commit con los cambios en la rama "development"
```
git add ./index.html
git commit -m "Añadir cambios en index.html"
```

### Sube los cambios a GitHub.

Si queremos que cuando se suban sea en la rama development como aun no la hemos creado hacemos:
```
git push origin development
```
Si queremos además fijarla como predeterminada hacemos:
```
git push --set-upstream origin development 
```
Este código hará 3 cosas: crear development en remoto si no existe, subir los commits de tu rama local a la remota y además configurar que tu rama local siga a la rama remota.

Podemos revisar la rama activa y cambios tenemos, podemos hacer:
```
git status
```
---
## Hacer un merge.

### Vuelve a la rama "main"

```
git checkout main
```
### Haz un merge de la rama "development" a la rama "main"
Antes de mergear tenemos que salir de la rama que vamos a mergear.
```
git merge development
```
### Si no hay conflictos los cambios realizados en la rama "development" se incorporarán a la rama "main"

```
LaboratorioGit % git merge development
Actualizando 65a6a23..9e8fcf5
Fast-forward
 index.html | 5 ++++-
 1 file changed, 4 insertions(+), 1 deletion(-)
```
Mergeado sin conflictos.

### Haz un push de los cambios al repositorio en GitHub.

```
git push
```

[Visita el index](https://mandarina28.github.io/LaboratorioGit/)