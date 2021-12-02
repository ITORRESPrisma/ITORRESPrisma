# GIT ADD

## Agregar todo lo de working directory al Staging Area o Index

```bash
git add .
```

## Si borre el archivo físico del WD, para quitarlo tengo que hacer lo siguiente

```bash
git rm <nombreArchivo>
```

## Si quiero agregar archivos por separado

```bash
git add <nombreArchivo>
```

# ALIAS

```bash
git config alias.lg "log --oneline --decorate --all --graph"
git config alias.s "status"
```

## Listar Alias disponibles

```bash
git config --get-regexp alias
```

## Para quitar un alias o cualquier configuración que hice

```bash
git config --unset alias.s
```

```bash
git config --unset alias.s
```
## Modifico manualmente la configuración de git

```
git config --global -e // Abre el editor configurado por defecto en git
```

# Para moverme entre los commit
** IMPORTANTE **: No es recomendable salvo casos muy especificos moverme entre los commits

```bash
git checkout <hashDeCommit>
```

Ejemplo
```bash
git checkout d1d74f4
```

# Subir rama local al remoto

```bash
git push --set-upstream <urlDelRemoto> <rama>
```

# Quito el seguimiento de esa rama en el remoto

```bash
git push --unset-upstream <urlDelRemoto> <rama>
```

# Para subir todas las ramas al remoto

```bash
git push --all 
```

# Para listar todas las ramas local y del remote

```bash
git branch -av
```