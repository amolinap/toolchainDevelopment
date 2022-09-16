# PostgreSQL

Comandos SQL para Base de Datos PostgreSQL

&nbsp;
## Descargar Git de Toolchain

Inicialmente descargamos Git. [Página principal de Descargas](Toolchain.html)

## Comandos básicos
**`update [tabla] set [columna1] = [columna2]`** Copiar columna2 a columna1

**`Alter table [tabla] add column [columna] Varchar(100);`** Agregar columna a tabla

**`git commit -a -m "Descripcion del commit"`** Hacer commit

**`git remote -v`** Ver lista de repositorios

**`git remote add nombre_repositorio "http://ruta_del_repositorio"`** Agregar repositorio

**`git push nombre_repositorio nombre_rama`** Empujar a repositorio

**`git pull nombre_repositorio nombre_rama`** Jalar de repositorio

**`git branch nombre_rama`** Crear rama

**`git checkout nombre_rama`** Cambiar rama

**`git log`** Ver lista de commits básica

**`git log --oneline --graph --all`** Ver lista de commits mejorada

**`git diff`** Ver cambios en repositorio

**`git branch -a`** Ver ramas remotas

**`git log -p nombre_archivo`** Ver historia de un archivo

&nbsp;
## Comandos avanzados

**`git branch -D nombre_rama`** Borrar rama local

**`git push origin :nombre_rama`** Borrar rama remota

**`git pull . nombre_rama`** Hacer pull en equipo local

Borrar credenciales almacenadas
> 1.  git credential-osxkeychain erase ⏎
> 2.  host=github.com  ⏎
> 3.  protocol=https   ⏎

&nbsp;
## Hacer una nueva rama master

**`git checkout [nombre_rama | sha1_id]`** Pasar a la rama que se va hacer master

**`git branch -D master`** Borrar rama master

**`git checkout -b master`** Hacer la rama actual master

&nbsp;
## Hacer una nueva rama master

**`git push origin :nombre-rama`** Eliminar rama de repositorio remoto

&nbsp;
## Deshacer cambios

**`git reset --hard`** Deshace todos los cambios no guardados

&nbsp;
## Creando etiquetas

**`git tag -a v1.4 -m "Descripcion de la etiqueta"`** Crear una etiqueta anotada

**`git tag`** Listando etiquetas

**`git show v1.4`** Ver información de la etiqueta

**`git tag -l "v1.4.2.*"`** Buscar etiquetas de acuerdo a un patrón en particular

**`git push origin v1.4`** Compartiendo etiquetas

**`git tag -d tag_name`** Borrando Tag local

**`git push --delete origin tagname`** Borrando Tag remoto