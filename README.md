#GIT

Un **Repositorio** es un almacén de cambios registrados en nuestro proyecto. 
**Commit** es el registro de cambios (adición, modificación o eliminación) de uno o varios ficheros.  
**Snapshot** instantánea.

##Flujo de Trabajo
Tu repositorio local esta compuesto por tres "árboles" administrados por git. El primero es tu **_Directorio de trabajo_** (Working Dir) que contiene los archivos, el segundo es el **_Index_** (Staging Area - Add) que actua como una zona intermedia, y el último es el **_HEAD_** (Local Repo - Commit) que apunta al último commit realizado.

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
8. Añadir los cambios al **Repositorio Local**, a nuestro HEAD (`git commit -m "comentario de commit"`)

 
Comandos:
- `git --version` --> para saber si tenemos instalado git y qué nº de versión
- `git init nombrefichero.ext` --> Trackea un fichero
- `git add -all` (= `git add .`) --> Trackea todos los ficheros del directorio
- `git reset HEAD nombrefichero.ext` --> para quitar un fichero del trackeo de nuestro repo. Lo quita de la zona de staging
- `git status` --> nos muestra el estado de nuestro repositorio
- `git commit -m "mensaje"` --> Comitea al repositorio local los cambios que hay pendientes en el staging área
- `git log` --> Nos muestra el listado de comiteos del repositorio en el que estamos con su hash, autor, fecha, mensaje,  etc.
- `git diff nombrefichero.ext` --> para ver los cambios que hay en un fichero de nuestro **Working Área** comparado con el **Local Repository** (commit) (Para ver todos los cambios `git diff HEAD`; y para ver cambios entre el WA y el SA --> `git diff --staged`)
- `git remote add origin https://github.com/Tsuna-mi/notes-bootcamp.git`--> para configurar nuestro repo remoto
- `git push -u origin master` --> para subir nuestros cambios del repositorio local al remoto y sincronizar los repos (pushea de los cambios desde el origen a la rama master); el resto de veces con que solo hagamos `git push`
- `git checkout -- nombrefichero.txt` --> volvemos a la última versión comiteada
- `git branch nombrenuevarama` --> Para crear una rama nueva, ésta no estará disponible para los demás a menos que subas (push) la rama a tu repositorio remoto:
-`git push origin nombrerama`
- `git checkout -b feature_x` --> Crea una nueva rama llamada feature_x y nos cambiamos a ella
- `git checkout master` --> para volver a la rama principal
- `git branch -d nombrerama` --> para borrar una rama
- `git rm '*.txt'` --> remove todos los ficheros de extensión txt
- `git clone /path/to/repository` --> para clonar un repo local
- `git clone username@host:/path/to/repository` --> para clonar un repo remoto
- `git pull` --> Para actualizar tu repositorio local al commit más nuevo. (`git fetch` + `git merge` --> Para fusionar otra rama a tu rama activa)
- `git diff <source_branch> <target_branch>` --> Antes de fusionar los cambios, puedes revisarlos usando

-----------

- cl --> clean
- clr --> clear
- ps --> password
- u / usr --> user
- rst --> reset
