# Caso de Uso 7: Configuración de Skill Frontend-Design

## Prompt Original

> "Por favor, configura la siguiente SKILL.md aquí en este proyecto: https://github.com/anthropics/skills --skill frontend-design. Documente y actualice la documentación del proyecto."

---

## Objetivo

Configurar el skill de frontend-design de Anthropic en el proyecto, basado en el repositorio oficial de skills de Anthropic, y actualizar la documentación del proyecto.

## Herramientas Utilizadas

- **WebFetch**: Obtención del contenido del repositorio de Anthropic
- **WebSearch**: Búsqueda de información sobre skills
- **Bash**: Creación de directorios
- **Write**: Creación de archivos de skill y documentación
- **Edit**: Actualización de archivos existentes

## Proceso Realizado

### 1. Investigación del Repositorio de Skills

Se exploró el repositorio oficial de Anthropic Skills para entender:
- La estructura de los archivos SKILL.md
- El formato YAML frontmatter requerido
- El contenido de la skill frontend-design

**Fuente:** https://github.com/anthropics/skills

### 2. Estructura de un Skill

Un skill de Anthropic tiene la siguiente estructura:

```yaml
---
name: [nombre-del-skill]
description: [descripción de uso]
license: [tipo de licencia]
---

# Contenido del skill
[Instrucciones detalladas]
```

**Campos requeridos:**
- `name`: Identificador único (minúsculas, guiones para espacios)
- `description`: Descripción completa de para qué sirve

### 3. Obtención del Skill Frontend-Design

Se obtuvo el contenido completo del archivo:
- **URL**: https://github.com/anthropics/skills/blob/main/skills/frontend-design/SKILL.md
- **Contenido**: Guías para crear interfaces frontend distintivas y de grado de producción

**Características del skill:**
- Design Thinking antes de codificar
- Frontend Aesthetics Guidelines
- Directrices sobre tipografía, color, movimiento, composición espacial
- Lista de elementos a evitar (AI slop)

### 4. Creación de la Estructura

Se creó la siguiente estructura:

```
skills/
└── frontend-design/
    └── SKILL.md
```

### 5. Actualización de Documentación

Se actualizaron los siguientes archivos:

| Archivo | Cambio |
|---------|--------|
| README.md | Agregada sección de Skills |
| docs/ESTRUCTURA.md | Agregada tabla de skills |
| docs/ESTRUCTURA.md | Actualizadas estadísticas |

---

## Contenido del Skill: Frontend-Design

### Descripción

Crea interfaces frontend distintivas y de grado de producción con alta calidad de diseño. Úsalo cuando el usuario pida construir componentes web, páginas, artifacts, posters o aplicaciones.

### Enfoque Principal

1. **Design Thinking**: Antes de codificar, entender el contexto
2. **Dirección estética bold**: Minimalismo refinado o maximalismo audaz
3. **Código funcional**: HTML/CSS/JS, React, Vue, etc.

### Directrices de Aesthetic

- **Tipografía**: Fuentes distintivas y únicas
- **Color**: Paletas cohesionadas con acentos
- **Movimiento**: Animaciones y micro-interacciones
- **Composición espacial**: Layouts inesperados, asimetría
- **Detalles visuales**: Texturas, sombras, profundidad

### Elementos a Evitar

- Fuentes genéricas (Arial, Inter, Roboto)
- Esquemas de color clichés (gradientes morados)
- Layouts predecibles
- Diseño "cookie-cutter" sin carácter

---

## Resultados Obtenidos

| Archivo | Estado |
|---------|--------|
| `skills/frontend-design/SKILL.md` | ✅ Creado |
| README.md | ✅ Actualizado |
| docs/ESTRUCTURA.md | ✅ Actualizado |

---

## Cómo Usar Este Skill

Para usar el skill de frontend-design en tus proyectos:

1. OpenCode automáticamente detectará el skill cuando trabajes en código frontend
2. El skill guiará la creación de interfaces distintivas
3. Se evitarán los美学 genéricos de IA

---

## Conclusión

Este caso de uso demuestra la capacidad de OpenCode para:

1. **Investigar** repositorios oficiales de skills
2. **Extraer** contenido estructurado de fuentes confiables
3. **Configurar** skills en proyectos locales
4. **Documentar** la configuración para referencia futura
5. **Actualizar** automáticamente la documentación del proyecto

La skill configurada permite crear interfaces frontend de alta calidad con estética distintiva y profesional.

---
*Documento creado: Marzo 2026*
*Proyecto: Configuración de Skill - Caso 7*
