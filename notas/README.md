# Git 

Sistema de control de versiones 

# instalacion en ubuntu 

```bash
sudo apt install git

```

# configuracion inicial

```bash
#comentario en bash

git config --system 

git config --local

git config --global user.name "nombre"

git config --global user.email "nombre@email.com"

git config --global core.editor "code --wait" # configuracion del editor

git config --global core.autocrlf input

git config --list #ver todas las configuraciones


```
## Comenzar areas de trabajo 

```bash

git init # Inicializa un repositorio Git en el directorio actual

git clone 

```

## comandos basicos 
```bash

git add [file] # Agrega un archivo al área de preparación

git status # Muestra el estado actual del repositorio Git

git commit -m "mensaje" # Crea un commit con los cambios en el área de preparación.

git commit # Crear un commit desde el editor de codigo
 
git commit -a # un git add y commit a la vez

git mv [file] [name-file-new] #cambiar de nombre
```

# Git restore, checkout 

```bash

git rm --cached [file]  #Elimina un archivo del área de preparación, pero no del directorio de trabajo

git restore [file] # restaura desde el area de preparacion

git checkout [file] #vuelve al ultimo commit

git reset [file] #

git reset  --hard

git reset --soft

```
## ver cambios y estados

```bash

git status -s #

git diff #diferencia entre versiones

git show [file] #

git diff --staged #

git diff [commit1] [commit2] #diferencia entre commit

git log 

git log --oneline 

git config --global core.abbrev 5 ##abreviar el id del commit

git diff --name-only [commit1] [commit2]

git diff --word-diff [commit1] [commit2]
```