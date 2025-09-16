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

### Crea un nuevo depositorio en GitHub

Entramos en Github y en el apartado de New podemos crear un nuevo repositorio.
Tendremos Owner que será el dueño y en Repositorio name será el nombre del repositorio que le daremos.
Ahí podremos crear el README, o crearlo manualmente en nuestra carpeta local.

### Copia el URL del repositorio que acabas de crear en GitHub.

Una vez dentro del Repositorio que hemos creado en el apartado anterior, pulsamos  <> Code. 
Dentro de local vamos a HTTPS y copiamos la URL. (Tambien podríamos usar SSH.)

### Conecta tu repositorio local con el repositorio en GitHub.

Para conectar nuestro repositorio local con el repositorio en la nube, vamos a nuestra terminal y ejecutamos:

```
git remote add origin https://github.com/Mandarina28/LaboratorioGit.git
```
---
## Hacer un commit y un push.
---
## Crear una rama.
---
## Hacer un merge.

