# Notas sobre GIT+GitHub: Todo un sistema de control de versiones de cero por Fernando Herrera

## Qué es Git?

Es un sistema de control de versiones

Git no le da seguimiento a una carpeta si no tiene archivos

## Listado de Comandos

### Primeras configuraciónes

`git --version` *Muestra la versión instalada de GIT*
`git help` *Muestra la ayuda de GIT*

`git config --global -e` *Editar la configuración global, -e es abreviación de --edit*
`git config --global --edit`

`git config --global user.name "<nombre usuario>"` *Cambiar el nombre de usuario*
`git config --global user.email "<mail usuario>"` *Cambiar el mail de usuario*

`git config --global --unset-all core.editor` *Elimina el editor por defecto configurado*

>video 8

`git config --global init.defaultBranch <nombre>` *Cambia el nombre por defecto del branch principal al crear un repositorio*

`git init` *Inicializa el repositorio (crea carpeta oculta .git)*
`git status` *Muestra los archivos que se modificaron desde el último commit*

`git add .` *Añade todos los archivos untracked y modificados al stage*
`git add <archivo>` *Añade el archivo o carpeta al stage*
`git reset <archivo>` *Quita un archivo o carpeta del stage*

`git commit -m <mensaje>` *Realiza el commit del stage con la descripción del mensaje*
`git commit --message <mensaje>`

>video 10

`git checkout -- .` *Reconstruye el proyecto al último commit*

>video 12

`git branch` *Muestra las ramas existentes y en cual de ellas estoy*
`git branch -m <nombre-branch> <nombre-nuevo>` *Renombra la rama nombre-branch a nombre-nuevo*

>video 13

`git commit -am <mensaje>` *Añade al stage y commitea los archivos trackeados que hayamos modificado*

>video 15

`git add <archivo1> <archivo2>` *Añadir varios archivos al stage*
`git reset <archivo1> <archivo2>` *Quitar varios archivos del stage*
`git add *.<extension>` *Añade los archivos de la extensión indicada. Ej: git add \*.js*
`git add <dir>/*.<extension>` *Idem anterior pero para un directorio específico. Ej: git add js/\*.js*
