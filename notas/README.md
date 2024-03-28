# Git 

Sistema de control de versiones 

# instalacion en ubuntu 

```bash
sudo apt install git

```

# configuracion inicial (Herramientas)

```bash
#comentario en bash

git config --system 

git config --local

git config --global user.name "nombre" 

git config --global user.email "nombre@email.com"

git config --global core.editor "code --wait" # configuracion del editor

git config --global core.autocrlf input

git config --global color.ui auto

git config --list #ver todas las configuraciones

git config --global core.abbrev 5 ##abreviar el id del commit


```
## Crear repositorios

```bash

git init # Inicializa un repositorio Git en el directorio actual

git clone  #Descarga un proyecto 

```

## comandos basicos 
```bash

git add [file] # Agrega un archivo al área de preparación

git status # Muestra el estado actual del repositorio Git

git commit -m "mensaje" # Crea un commit con los cambios en el área de preparación.

git commit # Crear un commit desde el editor de codigo
 
git commit -a # un git add y commit a la vez

```
## Visualizar Cambios

```bash

git status # Muestra el estado actual del repositorio Git

git status -s #

git diff #diferencia entre archivos 

git show [file] #

git diff --staged # Muestra las diferencias del archivo entre el área de espera y la última versión del archivo

```

## Ver historial de archivos

```bash
git log 

git log --oneline 

git diff [commit1] [commit2] #diferencia entre commit

git diff --name-only [commit1] [commit2] #nombre de los archivos cambiados

git diff --word-diff [commit1] [commit2] #en que cambiaron

git show [commit]
```

## Rehacer y modificar Commits 

```bash

git reset [commit] #

git reset  --hard  [commit] 

git reset --soft [commit]

git commit --amend 

git reset --soft head~1 

git reset --mixed [commit] 

git checkout [file] #vuelve al ultimo commit

git restore [file] # restaura desde el area de preparacion

```

# Nombre de archivos y borrados

```bash

git rm --cached [file]  #Elimina un archivo del área de preparación, pero no del directorio de trabajo


git rm [file] #borra el archivo 

git mv [archivo-original] [archivo-renombrado] #cambiar nombre de archivo

```

# Ramas

```bash

git branch [nombre] #crear una rama

git branch  # ver las ramas creadas

git checkout [rama] #cambiamos a esa ramaa

git branch -d [rama] # eliminar una rama

git switch [rama]  # cambiarnos entre ramas (recomendada)

git checkout -b [rama-nueva] # crear una rama y cambiarnos de una a ella

git switch -c [rama-nueva] # crear una rama y cambiarnos de una a ella

git branch -m [rama] [nuevo-nombre-rama]

git branch -m [nuevo-nombre-rama]

git merge [rama] #fusionar

```
