#  Clase 02 - 2021-11-25 de 10 a 12

# Crear repositorio GIT
Se ejecuta dentro de la raíz del proyecto que quiero versionar

```bash
git init
```
# Primera vez que inicio con git

Un usuario y un correo

GLOBAL: Al colocar global, todos los repos se van crear con este usuario y correo
La cuenta de correo deberia coincidir con la cuenta del repositorio externo (GitHub, GitLab, etc)

```bash
git config --global user.name "Maximilano" 
```

```bash
git config --global user.email "mlapeducacion@gmail.com" 
```

LOCAL: Que su respositorio se haga con este usuario y esta correo

```bash
git config --local user.name "Maximilano Principe" 
```

```bash
git config --local user.email "mlapeducacion@gmail.com" 
```

# Como verfico la configuración del usuario y el email

```bash
git config --local --get-regexp user
```

# Que pasa con el repo

git status

# Como paso del working directory al staging area

git add README.md < un solo archivo

## Todos los archivos

git add .

## para tambien los subdirectorios

git add ./. 

## Para hacer un commit 

git commit 
Te abre nano y vos le pones la descripción al commit
1. Abre el nano, colocan la descripción
2. hacen Ctrl + O, guardan los cambios
3. Y para salir Ctrl + X

```bash
git commit -m "mensaje"
```

**IMPORTANTE**: Git no versiona carpetas vacias.

Para que versione la carpeta tengo que crear un archivo llamado **.gitkeep**

# Programas con interfaz grafica para versionado

GitKraken - https://www.gitkraken.com/ < Gratis/Paga
Github Desktop - https://desktop.github.com/ < Gratis
Sourcetree - https://www.sourcetreeapp.com/

# Crear cuenta de GitHub

Van a Github y hacen click en Sign Up

Siguen los pasos

https://docs.google.com/document/d/1MubmU3zNOg_mqu5swVWb-GG0lyeTXKal-h2GVJduvZI/edit

# Creación de repos

## 2 nombres mágicos

El de su cuenta de git, el nombre de usuario

mlapeducacionit/mlapeducacionit

Y el que permite crear un hosting (Configura el GitHub Pages)

mlapeducacionit/mlapeducacionit.github.io

# PASOS BÁSICOS Iniciales

1. git init
2. git add README.md || git add .
3. git commit -m "descripción del commit"
4. git remote add origin https://github.com/suusUarioGIT/suRepositorio.git
5. git push -u origin master

NOTA CPS: En Win 7 tuve un problema con el git push, no me tomaba las credenciales. 
            Tuve que reinstalar git, sacando la git credential manager
            Tambien tuve que generar un token en GitHub y en lugar de password poner ese codigo

# Luego de los pasos básicos

1. git status
2. git add .
3. git commit -m "descripción del commit"
4. git push

git log --oneline (para ver el registro de cambios resumido) (si son muchos se sale con q)
git diff muestra las diferencias con el VScode permite ver los cambios realizados con vista lateral

# Para colaborar con repositorios de otra persona (En el video es el minuto 01:39)

1. Ir a GitHub al repositorio y presionar boton FORK
    Eso genera una copia del repositorio en mi cuenta GitHub
2. Traer el repositorio a mi compu
    2.a no creo directorio y git clone URL
    2.b creo un directorio y  git clone URL . (el punto evita crearme otro subdir)
3. Hago los cambios necesarios en mi repo y git add / commit
4. Luego en GitHub hago un Pull Request al dueño
