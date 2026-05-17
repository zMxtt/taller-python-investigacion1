## 1. Working Directory

-Es el área donde el programador trabaja directamente en los archivos del proyecto. Aquí se crean, modifican o eliminan archivos antes de guardarlos en Git.

Staging Area (Índice)

Es una zona intermedia de Git donde se preparan los archivos y cambios que serán incluidos en el próximo commit.

Repository

Es el lugar donde Git almacena el historial completo del proyecto mediante commits, guardando todas las versiones y cambios realizados.

-Es útil tener esta área intermedia porque permite organizar y seleccionar los cambios antes de guardarlos definitivamente en el repositorio. Gracias al staging area, el programador puede decidir qué archivos incluir en un commit y cuáles dejar para después, manteniendo un historial más limpio, ordenado y fácil de entender.


## 2. 
-El comando git status muestra el estado actual del repositorio. Permite ver qué archivos han sido modificados, cuáles están en el staging area, cuáles no han sido agregados y si existen conflictos o cambios pendientes por confirmar.

-El comando git status proporciona información como:

Los archivos modificados en el proyecto.
Los archivos que están en el staging area listos para el commit.
Los archivos que aún no están siendo rastreados por Git (untracked files).
Conflictos de fusión o cambios pendientes de resolver.
La rama actual en la que se está trabajando.

## 3. 
-git fetch:
Descarga los cambios del repositorio remoto, pero no los mezcla automáticamente con la rama actual. Solo actualiza la información para que el usuario revise los cambios antes de fusionarlos.
git pull:
Descarga los cambios del repositorio remoto y además los fusiona automáticamente con la rama actual mediante un merge.

-Usaría git fetch cuando quiero revisar primero los cambios del repositorio remoto antes de mezclarlos con mi trabajo local. Es útil para evitar conflictos o verificar qué cambios hicieron otros colaboradores.
Usaría git pull cuando quiero actualizar rápidamente mi rama local con los cambios del repositorio remoto y estoy seguro de que puedo fusionarlos directamente sin problemas.

-git fetch es más seguro porque solo descarga los cambios del repositorio remoto sin aplicarlos automáticamente al proyecto local. Esto permite revisar los cambios antes de fusionarlos y reduce el riesgo de conflictos o errores inesperados.

En cambio, git pull descarga y fusiona los cambios automáticamente, lo que puede generar conflictos si existen modificaciones incompatibles en la rama local.

## 4.
-Un merge conflict o conflicto de fusión ocurre cuando Git no puede combinar automáticamente los cambios de dos ramas porque modificaron la misma parte de un archivo o realizaron cambios incompatibles.

Para resolverlo:

1-Git marca los archivos con conflicto.
2-Se abren los archivos y aparecen marcas
3-El programador debe decidir qué cambios conservar o cómo combinarlos.
4-Después de corregir el archivo, se guarda y se agrega con: git add nombre-del-archivo
5-Finalmente se completa la fusión con: git commit
