# Clase 03 - GIT Desarrollo Colborativo

## Repaso

### Estado de los archivos

```sh
git status
```

### Agregar a la zona de Staging Area (SA) o index (area de confirmacion)

```sh
git add <archivo>
git add . # todos los archivos
```

### Persistir los archivos que coloque en SA (Hacer un commit)

```sh
git commit -m "Mensaje"
git commit # abre un editor de texto y me permite escribir el mensaje
```

### Ver los commits

```sh
git log # forma larga
git log --oneline # forma corta
git log -5 # cantidad de commits que quiero que muestre
```

### Como veo la diferencia entre lo que tengo en WD y LR

```sh
git diff
```

### Ver la diferencia entre 2 ramas, la rama main y al rama dev

```sh
git diff <nombre-rama
# ejemplo
git switch main
fit diff dev
```

### Como arreglo el mensaje de un commit (Elm ultimo)

```sh
git commit --amend
```

**IMPORTANTE**: Ademas de corregir el mensaje puedo agregar archivos que olvide dentro del commit

```sh
git add <archivo-olvidado>
git commit --amend
```

### Crear una rama

```sh
git branch <nombre-rama>
```

### Cambiarse de rama

```sh
git switch <nombre-rama>
```

### Fusionar 2 ramas

```sh
git merge <nombre-rama>
# si me quiero traer los cambios que estan en dev a la rama main
git switch main
git merge dev
```


## Hacer un commit sin cammbiar el mensaje pero agregando archvios o lineas de codigo que nos faltaron guardar

```sh
git add . # agrego archivos o lineas que faltaron
git commit --amend --no-edit # evito cambiar el mensaje
```

## Agregar  modificacciones de archvios granularmente (agregar partes del codigo agregado en un archivo)

```sh
git add --patch
```

## GIT alias

### Crear un alias

```sh
git config --global alias.s "status"
git config --global alias.ll "log"
git config --global alias.l "log --oneline"
git config --global alias.amend "--amend -no-edit"
git config --global alias.c "commit -m"
```

### Listar los alias que tengo cargados

```sh
git config --get-regexp alias
```
