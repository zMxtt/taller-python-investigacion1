# Investigación Avanzada de Git y Buenas Prácticas

# 1. ¿Qué es Git Rebase y en qué se diferencia de Git Merge?

Git Rebase es un comando que permite mover o reaplicar commits de una rama sobre otra rama base.

## Diferencia entre Rebase y Merge

- Git Merge une el historial de dos ramas creando un commit de fusión.
- Git Rebase reorganiza los commits para crear un historial más lineal y limpio.

## ¿Cuándo es apropiado usar rebase?

Es apropiado usar rebase cuando se quiere mantener un historial organizado y evitar commits de merge innecesarios.

## ¿Qué significa "reescribir la historia" en Git?

Significa modificar el historial de commits existente, cambiando el orden o recreando commits anteriores.

---

# 2. ¿Qué hace el comando git stash y cuándo lo usarías?

El comando `git stash` guarda temporalmente cambios no confirmados para limpiar el área de trabajo sin perder información.

## Ejemplo de uso

Sería útil cuando estás trabajando en una funcionalidad y necesitas cambiar rápidamente de rama para solucionar otro problema.

```bash
git stash
```

## ¿Cómo recuperas cambios guardados con stash?

```bash
git stash apply
```

o

```bash
git stash pop
```

---

# 3. ¿Qué es un "commit convencional" (Conventional Commits)?

Es una convención para escribir mensajes de commit de forma organizada y estandarizada.

## ¿Por qué es importante?

- Facilita entender los cambios realizados.
- Mejora la organización del historial.
- Ayuda en proyectos colaborativos.
- Facilita la automatización y generación de changelogs.

## Otros prefijos además de feat:, fix:, docs:

- test: cambios relacionados con pruebas.
- refactor: mejoras internas del código sin cambiar funcionalidad.
- style: cambios de formato o estilo del código.

---

# 4. ¿Qué es Git Flow?

Git Flow es un modelo de trabajo basado en ramas que organiza el desarrollo de proyectos usando diferentes tipos de ramas.

## Modelo de branching de Git Flow

Se basa en separar el desarrollo, producción y nuevas funcionalidades en ramas independientes.

## Tipos de ramas en Git Flow

- main: versión estable del proyecto.
- develop: rama principal de desarrollo.
- feature: nuevas funcionalidades.
- release: preparación de versiones.
- hotfix: corrección rápida de errores en producción.

---

# 5. ¿Qué es un "HEAD detached" en Git?

Un HEAD detached ocurre cuando Git apunta directamente a un commit y no a una rama.

## ¿Cómo ocurre?

Sucede al cambiar a un commit específico usando:

```bash
git checkout ID_DEL_COMMIT
```

## ¿Cómo sales de un HEAD detached?

Debes cambiar nuevamente a una rama:

```bash
git checkout main
```

o crear una nueva rama:

```bash
git checkout -b nueva-rama
```

---

# 6. ¿Qué hace el comando git log y qué opciones útiles tiene?

El comando `git log` muestra el historial de commits del repositorio.

## Flags útiles

### --oneline

Muestra cada commit en una sola línea.

```bash
git log --oneline
```

### --graph

Muestra un gráfico del historial de ramas y merges.

```bash
git log --graph
```

### --all

Muestra commits de todas las ramas.

```bash
git log --all
```

## Ejemplo de uso

```bash
git log --oneline --graph --all
```