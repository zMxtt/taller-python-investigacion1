# Investigación sobre GitHub

## 1. ¿Qué es un Pull Request (PR) y cuál es su propósito?

Un Pull Request (PR) es una solicitud para fusionar los cambios realizados en una rama hacia otra rama dentro de un repositorio de GitHub. Su propósito es permitir que otros desarrolladores revisen, comenten y aprueben los cambios antes de integrarlos al proyecto principal.

---

## 2. ¿En qué se diferencia de un merge directo?

La diferencia es que un merge directo fusiona los cambios inmediatamente desde una rama a otra sin revisión previa. En cambio, un Pull Request agrega una etapa de revisión y discusión antes de realizar la fusión.

---

## 3. ¿Cuáles son las ventajas de usar PRs en proyectos colaborativos?

Las ventajas de usar Pull Requests son:

- Permiten revisar el código antes de integrarlo.
- Ayudan a detectar errores o conflictos.
- Facilitan la colaboración entre desarrolladores.
- Mantienen un historial más organizado.
- Mejoran la calidad y seguridad del proyecto.
# 2. ¿Qué es un fork en GitHub y cuándo se usa?

Un fork en GitHub es una copia de un repositorio que se crea en la cuenta de otro usuario. Se usa principalmente para trabajar en proyectos sin modificar el repositorio original.

## Diferencia entre fork y clone

- Fork: crea una copia del repositorio en GitHub dentro de otra cuenta.
- Clone: descarga una copia del repositorio desde GitHub al computador local.

## ¿Cómo contribuirías a un proyecto open source usando fork?

1. Hacer un fork del proyecto.
2. Clonar el fork al computador.
3. Crear una nueva rama.
4. Realizar los cambios necesarios.
5. Hacer commit y push.
6. Crear un Pull Request hacia el repositorio original.

---

# 3. ¿Qué es el archivo .gitignore y por qué es importante?

El archivo .gitignore sirve para indicarle a Git qué archivos o carpetas no deben subirse al repositorio.

Es importante porque evita subir archivos innecesarios, temporales o sensibles.

## 5 tipos de archivos que no deberían subirse a un repositorio Python

- __pycache__/
- *.pyc
- venv/
- .env
- archivos de configuración del sistema

## ¿Qué problemas podrían ocurrir si no usas .gitignore?

- Subir archivos innecesarios al repositorio.
- Exponer información privada o contraseñas.
- Aumentar el tamaño del proyecto.
- Generar conflictos entre desarrolladores.
- Subir dependencias o archivos temporales por error.

---

# 4. ¿Qué son los issues en GitHub y para qué sirven?

Los issues son herramientas de GitHub utilizadas para reportar errores, sugerir mejoras, hacer preguntas o registrar tareas dentro de un proyecto.

## ¿Qué información debería contener un buen issue?

- Título claro.
- Descripción detallada.
- Pasos para reproducir el problema.
- Resultado esperado.
- Evidencia o capturas si es necesario.

## ¿Cómo se pueden relacionar issues con commits?

Los commits pueden incluir el número del issue usando palabras clave como:

```txt id="n8mpk6"
Fixes #10
Closes #5

# 5. ¿Qué es GitHub Actions?

GitHub Actions es una herramienta de automatización integrada en GitHub que permite ejecutar tareas automáticamente dentro de un repositorio.

## ¿Para qué se utiliza?

Se utiliza para automatizar procesos de desarrollo como pruebas, compilación, integración continua y despliegue de aplicaciones.

## 2 ejemplos de tareas que se pueden automatizar

1. Ejecutar pruebas automáticas cada vez que se hace un push o un Pull Request.
2. Desplegar automáticamente una aplicación o página web después de actualizar el repositorio.


