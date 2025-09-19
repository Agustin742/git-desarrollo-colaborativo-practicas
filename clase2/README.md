# Clase 2 - GIT Desarrollo colaborativo

## .gitkeep
es un archivo que me permite hacer un commit para guardar una carpeta, que no es detectada por git cuando esta vacia.

## .gitignore
Es un archivo que me permite ignorar archivos o carpetas completas que no quiero que se guarden dentor del repositorio. Dentro del archivo menciono los archivos que quiero que git ignore y no guarde dentro del repositorio.

## Repaso de comandos basicos

### Marcar archivos que quiero que sean parte del proximo commit
O sea marcar archivos que estan en el working directory terminados y quiero llevarlos al area de configuracion para que sean parte del proximo commit

```sh
git add <nombre-archivo1> <nombre-archivo2>
git add <nombre-archivo1>
git add README.md
```