#EjercicioGit2#

<!-- TODO: Ir completando cada punto con capturas y código -->

1. Creación de repositorio en GitHub, inicializándolo con un README.md y el .gitignore que GitHub ofrece para JAVA.
2. Modificación de este README.md desde GitHub para indicar los dos primeros pasos.
3. Clono el repo.
4. Creo un proyecto en ese directorio
5. ¡Ups! el proyecto se creó en una subcarpeta. Muevo su contenido al directorio raiz del repo.
6. Quiero volver al paso 3 para hacerlo bien. Hago un log
```
a21pablosp@W10N-I8E05 MINGW64 /c/Users/a21pablosp/Desktop/Ejercicios Git/EjercicioGit2 (main)
$git log --oneline
abd3bdd (Head -> main, origin/main) moviendo el proyecto a la carpeta raiz del repo
cf9723d Creacion de proyecto con IntelliJ
40d29d0 Update README.md
d93e588 Initial commit
```
Como quiero volver a antes de crear el proyecto, tengo que hace un reset al comit previo. Al hacerlo, predería los comits posteriores, asique creo una rama nueva para ello
```
a21pablosp@W10N-I8E05 MINGW64 /c/Users/a21pablosp/Desktop/Ejercicios Git/EjercicioGit2 (main)
$git branch rama2
a21pablosp@W10N-I8E05 MINGW64 /c/Users/a21pablosp/Desktop/Ejercicios Git/EjercicioGit2 (main)
$git checkout rama2
Switched to branch 'rama2'
```
(para crear una rama y pasar directamente a ella se podria tambien hacer en un paso con "git checkout -b rama2").
Ahora ya puedo hacer el resert
```a21pablosp@W10N-I8E05 MINGW64 /c/Users/a21pablosp/Desktop/Ejercicios Git/EjercicioGit2 (main)
$git reset --hard 40d29d0
HEAD is now at 40d29d0 Update README.md
```
y crear el proyecto directamente en el directorio donde ya esta el repo.
![Creacion de Proyecto](./img/Captura%20de%20pantalla%202022-11-28%20214640.png)

