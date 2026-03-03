# Índice de Casos de Uso

Este documento lista todos los casos de uso documentados en el proyecto, con resúmenes y propósitos.

---

## 📋 Lista de Casos de Uso

### Caso de Uso 1: Investigación de Empresas Tech
**Archivo:** `caso-uso-1-investigacion-empresas.md`

**Objetivo:** Investigar empresas de tecnología en Cartagena de Indias para identificar prospectos potenciales para un curso de inteligencia artificial.

**Herramientas:**
- WebSearch
- Chrome DevTools MCP

**Resultado:** Lista de empresas con información de contacto

---

### Caso de Uso 2: Análisis de Archivos Locales
**Archivo:** `caso-uso-2-analisis-archivos-locales.md`

**Objetivo:** Analizar la carpeta de Descargas para identificar los 5 archivos más antiguos y los 5 más pesados.

**Herramientas:**
- Bash (comandos del sistema)
- Glob
- Grep

**Resultado:** 
- Archivos más antiguos: Logos de 2023
- Archivos más pesados: Imagenes.zip (86MB), OpenCode Desktop.dmg (79MB)

---

### Caso de Uso 3: Análisis y Visualización de Ideas de Negocio
**Archivo:** `caso-uso-3-analisis-ideas-negocio.md`

**Objetivo:** Analizar el repositorio de 100 ideas de negocio, organizarlas en categorías y generar un mapa de nodos visual.

**Herramientas:**
- Read
- Write
- Chrome DevTools MCP (para captura de pantalla)

**Resultado:**
- 9 clusters temáticos identificados
- Mapa de nodos en formato PNG
- 3 prompts propuestos para investigación

---

### Caso de Uso 4: Diagnóstico y Optimización de Macbook
**Archivo:** `caso-uso-4-diagnostico-macbook.md`

**Objetivo:** Diagnosticar por qué la computadora está funcionando lenta, identificando causas raíz.

**Herramientas:**
- top
- vm_stat
- df
- ps
- du

**Resultado:** 
- 5 causas identificadas
- 31GB de espacio liberado
- Mejora significativa de rendimiento

---

### Caso de Uso 5: Investigación y Publicación de Artículo AEO
**Archivo:** `caso-uso-5-investigacion-publicacion-aeo.md`

**Objetivo:** Investigar sobre Answer Engine Optimization (AEO), crear contenido y publicarlo en un sitio web.

**Herramientas:**
- CodeSearch
- Write
- Chrome DevTools MCP

**Resultado:**
- Artículo: "Cómo crear contenido que ChatGPT cite en 2026"
- Sitio web profesional en HTML

---

### Caso de Uso 6: Análisis y Documentación del Proyecto
**Archivo:** `caso-uso-6-analisis-documentacion.md`

**Objetivo:** Analizar la estructura del proyecto para identificar áreas sin documentación y crear la estructura necesaria.

**Herramientas:**
- Bash (comandos del sistema)
- Glob
- Write

**Resultado:**
- README.md principal creado
- Carpeta /docs/ creada con 3 archivos
- Índice de casos de uso actualizado

---

### Caso de Uso 7: Configuración de Skill Frontend-Design
**Archivo:** `caso-uso-7-configuracion-skill.md`

**Objetivo:** Configurar el skill de frontend-design de Anthropic en el proyecto.

**Herramientas:**
- WebFetch
- WebSearch
- Bash
- Write
- Edit

**Resultado:**
- Skill frontend-design creado en `skills/frontend-design/SKILL.md`
- Documentación actualizada

---

## 📊 Resumen por Tipo de Herramienta

| Tipo de Herramienta | Casos de Uso |
|---------------------|--------------|
| Chrome DevTools MCP | 1, 3, 5 |
| Bash/Sistema | 2, 4, 6, 7 |
| Búsqueda (Web/Code) | 1, 5, 7 |
| Write/Archivos | 3, 5, 6, 7 |
| Glob | 6 |
| WebFetch | 7 |
| Edit | 7 |

---

## 🎯 Propósito de los Casos de Uso

Los casos de uso demuestran las capacidades de OpenCode y sus herramientas MCP para:

1. **Investigación de mercado**: Web scraping, análisis de empresas
2. **Administración del sistema**: Gestión de archivos, diagnóstico de rendimiento
3. **Análisis de datos**: Organización, categorización, visualización
4. **Creación de contenido**: Artículos, documentación, sitios web
5. **Documentación de proyectos**: Análisis de estructura, creación de índices
6. **Configuración de herramientas**: Skills, integraciones, personalización

---

*Última actualización: Marzo 2026*
