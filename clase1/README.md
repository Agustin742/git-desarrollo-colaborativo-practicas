# Clase 01 - GIT Desarrollo Colaborativo

## Configuracion Inicial 
Esta configuracion se hace una unica vez, y es para indicar al git con que nombre u correo se van a firmar los commits creados

```sh
git config --global user.name "Agustin Tabarcache"
git config --global user.email email@gmail.com
```

## Mostrar la configuaracion de usuario

```sh
git config --get-regexp user 
```

## Listar las configuraciones

```sh
git config --list
```

## Para editar las configuraciones

```sh
git config --global -e
```

## Para crear un repo de git

```sh
git init
```

## Para borrar el repo

```sh
rm -rf .git
```

## Para ver el estado de los archivos

```sh
git status
```

## Para pasar los archivos del working directory al staging area

```sh
git add .
```

## Para pasar los archivos del staging area al repo local

```sh
git commit -m "mensaje"
```

## para ver el historial de commits completo

```sh
git log
```

## para ver un resumen del historial de commits

```sh
git log --oneline
```

## Para ver la diferencia y poder comparar entre el working directory y el repo local

```sh
git diff
```

## Para agregagr el repo remoto

```sh
git remote add origin URL
```

## Para ver las rutas del repo remoto

```sh
git remote -v
```

## Para subir todos los comits  la primera vez

```sh
git push -u origin main
```

## Ayuda Comandos

```sh
git <comando> --help
git status --help
```

## Status recortado
```sh
git status -s
```