---
name: git-commit-formatter
description: Formatea los mensajes de confirmación de Git según la especificación de confirmaciones convencionales. Úselo cuando el usuario solicite confirmar cambios o escribir un mensaje de confirmación.
---

# Git Commit Formatter Skill

Cuando se escribe un mensaje de confirmación de Git, debes seguir la especificación de confirmaciones convencionales.

## Formato
`<tipo>[ámbito opcional]: <descripción>`

## Tipos Permitidos
- **feat**: Nueva característica
- **fix**: Corrección de error
- **docs**: Cambios solo en la documentación
- **style**: Cambios que no afectan el significado del código (espaciado, formato, etc)
- **refactor**: Cambio de código que ni corrige un error ni añade una característica
- **perf**: Cambio de código que mejora el rendimiento
- **test**: Añadir pruebas faltantes o corregir pruebas existentes
- **chore**: Cambios en el proceso de construcción o herramientas auxiliares y bibliotecas como la generación de documentación

## Instrucciones
1. Analiza los cambios para determinar el tipo principal.
2. Identifica el `ámbito` si es aplicable (por ejemplo, un componente o archivo específico).
3. Escribe una descripción concisa en modo imperativo (por ejemplo, "añadir función" no "función añadida").
4. Si hay cambios que rompen la compatibilidad, agrega un pie de página que comience con `BREAKING CHANGE:`.

## Ejemplo
`feat(auth): implementar el inicio de sesión con Google`

## Contexto Específico del Proyecto: SisuLine

Este asistente y los comandos Git ejecutados pertenecen al proyecto **SisuLine** (Historial Clínico en Lienzo Infinito).

- **Repositorio Remoto (GitHub):** [https://github.com/alarcone1/SisuLine](https://github.com/alarcone1/SisuLine)
- Usa este contexto si debes referenciar issues o generar comandos relacionados con el origen remoto de este proyecto específico.

## Comandos Especiales

Si el usuario indica instrucciones como **"actualiza el repositorio"**, **"actualice repositorio"** o similares, debes entender que el usuario desea que se agreguen y confirmen los cambios locales (`git add .`, `git commit -m "..."`) y posteriormente realizar un `git push` hacia la rama principal en el remoto (`https://github.com/alarcone1/SisuLine`). 

Asegúrate siempre de proponer el mensaje de confirmación siguiendo el formato de esta guía antes del *push*.

**Nota importante**: El repositorio en GitHub para este proyecto de documentación es: https://github.com/alarcone1/casos_de_uso_opencode

Si el usuario está trabajando en este proyecto específico (mi-memoria-web), usa el repositorio: https://github.com/alarcone1/casos_de_uso_opencode
