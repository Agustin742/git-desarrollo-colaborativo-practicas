# Clase 2 - GIT Desarrollo colaborativo

## .gitkeep
es un archivo que me permite hacer un commit para guardar una carpeta, que no es detectada por git cuando esta vacia.

## .gitignore
Es un archivo que me permite ignorar archivos o carpetas completas que no quiero que se guarden dentor del repositorio. Dentro del archivo menciono los archivos que quiero que git ignore y no guarde dentro del repositorio.

## Repaso de comandos basicos

### Marcar archivos que quiero que sean parte del proximo commit
O sea marcar archivos que estan en el working directory terminados y quiero llevarlos al area de configuracion para que sean parte del proximo commit.

```sh
git add <nombre-archivo1> <nombre-archivo2>
git add <nombre-archivo1>
git add README.md
```

### ver el contenido de un contenido hecho

```sh
git show <hash>
git show e2c3685
```

### Guardar los cambios en el repo

```sh
git commit -m "mensaje"
git commit #se abre el editor para escribir el mensaje
git commit -a # se hace un add a los archivos modificados, no se hace un add los archivos untracked y se abre el editor
git commit -am "mensaje" # se agregan los archivos modificados y no se abre el editor para escribir el mensaje
```
**NOTA**: Los mensajes idealmente pueden tener maximo 80 caracteres

### Ver los commits dentro del repo

```sh
git log # largo con detalle
git log --oneline # corto solo el mensaje
git log -2 # me muestra los ultimos 2 commits del listado
git log --oneline -2 # muestra los 2 ultimos commits cortos
```

## Ver la diferencia entre el WK(working directory) y el Local repo
```sh
git diff
```