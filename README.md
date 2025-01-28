# Apuntes de Git y GitHub

## Cómo agregar un repositorio local a GitHub

1. Crea un nuevo repositorio en GitHub.(*no lo inicialices ni con readme ni con .gitignore* agregaras despues los archivos).

2. Copia la url del repositorio que creaste.

3. Abre el terminal.

4. Ve al directorio de trabajo de tu proyecto local.

5. Agrega la url de tu repositorio remoto con el siguiente codigo.

```shell
    git remote add origin tuUrl.com
```

6. Para verificar que la url se haya configurado correctamente ejecutamos:

```shell
    git remote -v
```

7. Para enviar los cambios de su repositorio local a GitHub, ejecutamos:

```shell
     git push origin main
```

Si su rama predeterminada no se llama "main", reemplace con el nombre de su rama predeterminada.

## Casos de Uso

1. Tengo mi proyecto ya en local:

    1. Creo mi repositorio remoto sin inicializar.
    2. Copio la url de mi repositorio remoto.
    3. Abro una terminal y me dirijo a donde se encuentre mi proyecto en local.
    4. (**si no esta inicializado hacer `git ini`**).
    5. Ejecutar `git remote add origin tuUrl.com`.
    6. Ejecutar `git remote -v` para corroborar la configuración.
    7. Ejecutar `git push origin main`.

2. Tengo mi proyecto en GitHub:
    1. Voy a mi repositorio.
    2. Copio la Url de mi repositorio.
    3. Abro la terminal y me dirijo a la carpeta en la que quiera crear mi repositorio.
    4. Ejecutamos `git clone tuUrl.com`.
    5. Si nuestro proyecto tiene dependencias, debemos ejecutar la instalacion de los paquetes requeridos con el gestor de paquetes.

3. Tengo versión en GitHub y en Local:
    1.Siempre que tenga un proyecto en local y en la nube debemos actualizar los cambios que se hayan realizado.
    2. Abrimos nuestro proyecto en local.
    3. En la terminal ejecutamos `git pull`.
    4. Con esto ya tendremos los cambios que poseamos en el repositorio de la nube.

## Comandos Más Usados en git.

1. **`git init`**  
   Inicializa un nuevo repositorio Git vacío en el directorio actual.

2. **`git clone <url>`**  
   Clona un repositorio remoto en tu máquina local.

3. **`git status`**  
   Muestra el estado de los archivos en el directorio de trabajo (modificados, añadidos, etc.).

4. **`git add <archivo>`**  
   Agrega archivos específicos al área de preparación (staging area) para ser comprometidos.

5. **`git commit -m "<mensaje>"`**  
   Realiza un commit con un mensaje que describe los cambios.

6. **`git log`**  
   Muestra el historial de commits en el repositorio.

7. **`git diff`**  
   Muestra las diferencias entre los archivos modificados y el último commit.

8. **`git branch`**  
   Lista todas las ramas en el repositorio actual.

9. **`git checkout <rama>`**  
   Cambia a la rama especificada.

10. **`git merge <rama>`**  
   Fusiona los cambios de la rama especificada a la rama actual.

11. **`git pull`**  
   Descarga los cambios del repositorio remoto y los fusiona con tu rama local.

12. **`git push`**  
   Envía tus commits locales al repositorio remoto.

13. **`git remote -v`**  
   Muestra las URL de los repositorios remotos asociados.

14. **`git fetch`**  
   Descarga los cambios del repositorio remoto sin fusionarlos con tu rama actual.

15. **`git reset`**  
   Deshace cambios en el área de preparación o en los commits anteriores (cuidado con este comando).

16. **`git stash`**  
   Guarda temporalmente los cambios no comprometidos para que puedas trabajar en otra cosa.

17. **`git tag <nombre>`**  
   Crea una etiqueta en un commit específico.

18. **`git rm <archivo>`**  
   Elimina archivos del repositorio y prepara la eliminación para el próximo commit.

19. **`git config`**  
   Configura opciones de Git, como el nombre de usuario o correo electrónico.

20. **`git rebase`**  
   Reaplica los commits de una rama sobre otra base, útil para mantener un historial limpio.
