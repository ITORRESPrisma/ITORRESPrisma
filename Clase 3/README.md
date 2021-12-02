# GIT STASH
El git stash guarda lo que está en el working directory en un area temporal.

## Crea un stash

```bash
git stash
```

## Lista los stash 
```bash
git stash list
```

# .gitignore
Este archivo es un blacklist de archivo. Todos archivos que coloque dentro de el archivo .gitignore, van ser descartados

# GIT Log
Cuando estoy dentro del comando para salir tengo presionar la tecla **q** del teclado

### Para lista un solo commit

```bash
git log --oneline -1
```

### De una fecha en particular

```bash
git log --since="2021-10-01"
git log --after="2021-10-01"
git log --before="2021-10-01"
git log --after="2021-10-01" --before="2021-10-21" --oneline
```

```bash
git log --oneline --decorate --all --graph
```


# Corregir el última descripción del commit
Si me equivoco en el última descripción del commit puedo corregirlo con git amend

```bash
git commit --amend -m "Agrego lo de git log"
```
# ADD y COMMIT todo junto
**IMPORTANTE:** Tengo que tener en el Staging AREA.

```bash
git commit -am "Nombre del commit"
```

# GIT remote

Ver si tengo el repo remoto configura

```bash
git remote -v
```
### Agregar un remoto a mi repo local
```bash
git remote {alias del remoto } https://github.com/{usuarioGit}/{nombreRepo}
```
### Cambio de nombre del repo remoto
```bash
git remote rename {origin} {it} https://github.com/{usuarioGit}/{nombreRepo}
```
### Borro repositorio remoto del local
```bash
git remote rm {origin} https://github.com/{usuarioGit}/{nombreRepo}
```

# BRANCH

## Creo una rama

```bash
git branch {nombre rama}
```

### Ejemplo
```bash
git branch dev
```

## Cambio de Rama

```bash
git switch dev
```

## Otra forma de cambiar de rama

```bash
git checkout <rama>
```

# AYUDA DE GIT en LOCAL

```bash
git help <nombreComando>
```

## Borro la rama

```bash
git branch -d <rama>
```

## Borro la rama de forma forzada

```bash
git branch -d <rama> -f
git branch -D <rama>
```