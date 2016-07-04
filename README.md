#GIT

Un **Repositorio** es un almacén de cambios registrados en nuestro proyecto. 
**Commit** es el registro de cambios (adición, modificación o eliminación) de uno o varios ficheros.  
**Snapshot** instantánea.

Ficheros                
- Trackeados
- No trackeados

Pasos para usar git

1. Crear nueva carpeta para el repo
2. Entrar
3. Crear nuevo fichero
4. Inicializar el repositorio (`git ini`)
5. Trackear fichero (`git add nombrefichero.ext`)
6. Hacer cambios en el fichero y salvarlo (**Working área**)
7. Pasar los cambios al **Staging Área** (`git add nombrefichero.ext`)
8. Añadir los cambios al **Repositorio Local** (`git commit -m "mensaje"`)

 
Comandos:
- `git --version` --> para saber si tenemos instalado git y qué nº de versión
- `git init nombrefichero.ext` --> Trackea un fichero
- `git init -all` --> Trackea todos los ficheros del directorio
- `git reset HEAD nombrefichero.ext` --> para quitar un fichero del trackeo de nuestro repo
- `git status` --> nos muestra el estado de nuestro repositorio
- `git commit -m "mensaje"` --> Comitea al repositorio local los cambios que hay pendientes en el staging área
- `git log` --> Nos muestra el listado de comiteos del repositorio en el que estamos con su hash, autor, fecha, mensaje,  etc.
- `git diff nombrefichero.ext` --> para ver los cambios que hay en un fichero de nuestro **Working Área** comparado con el **Local Repository** (commit)
