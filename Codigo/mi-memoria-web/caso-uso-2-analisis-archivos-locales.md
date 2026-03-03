# Caso de Uso: Análisis de Archivos en el Sistema Local

## Prompt Original

> "Busca la carpeta de Descargas en mi dispositivo, analízala para encontrar los 5 archivos más antiguos que haya allí, así como los 5 archivos más pesados, y preséntamelos en un formato claro (NO LOS BORRES TODAVÍA), repito, NO BORRES NADA."

---

## Objetivo

Analizar la carpeta de Descargas (Downloads) del usuario para identificar los 5 archivos más antiguos y los 5 archivos más pesados, sin eliminar ningún archivo.

## Herramientas Utilizadas

- **Bash**: Comandos del sistema para listar y analizar archivos
- **Glob**: Búsqueda de patrones de archivos
- **Grep**: Búsqueda de contenido en archivos
- **Read**: Lectura de metadatos de archivos

## Proceso Realizado

### 1. Listado Inicial de la Carpeta Downloads

Se ejecutó el comando `ls -laR` para obtener una visión completa de la estructura de directorios y archivos.

```bash
ls -laR ~/Downloads/
```

### 2. Identificación de Archivos Más Antiguos

Se utilizaron comandos para ordenar archivos por fecha de modificación:

```bash
# Ordenar por fecha ascendente (más antiguos primero)
find ~/Downloads/ -type f -exec ls -lrt {} + | head -20
```

**Resultados obtenidos:**

| # | Archivo | Fecha de modificación | Tamaño |
|---|---------|---------------------|--------|
| 1 | `Logo png.png` | 22 Ago 2023 | 99 KB |
| 2 | `Logo png (1).png` | 22 Ago 2023 | 8 KB |
| 3 | `Logo Corregido.png` | 23 Ago 2023 | 37 KB |
| 4 | `Inicio marca personal.png` | 27 Ago 2023 | 426 KB |
| 5 | `logo 1.png` | 8 Sep 2023 | 34 KB |

### 3. Identificación de Archivos Más Pesados

Se utilizó el comando para ordenar por tamaño:

```bash
# Ordenar por tamaño descendente
ls -lS ~/Downloads/ | head -20
```

**Resultados obtenidos:**

| # | Archivo | Fecha de modificación | Tamaño |
|---|---------|---------------------|--------|
| 1 | `Imagenes.zip` | 17 Feb 2026 | **86 MB** |
| 2 | `OpenCode Desktop.dmg` | 23 Feb 2026 | **79 MB** |
| 3 | `WhatsApp Video 2026-02-16 at 08.29.37.mp4` | 18 Feb 2026 | **28 MB** |
| 4 | `Manual-de-Identidad-Visual-02072024.pdf` | 17 Feb 2026 | **17 MB** |
| 5 | `Pepin.mp4` | 20 Feb 2026 | **8.3 MB** |

### 4. Estadísticas Generales

- **Total en Downloads**: ~544 MB
- **Archivos más antiguos**: Del año 2023 (logos y marca personal)
- **Archivos más pesados**: Principalmente archivos comprimidos, videos y PDFs de alta calidad

## Comandos Utilizados

```bash
# Listar todos los archivos con detalles
ls -laR ~/Downloads/

# Encontrar archivos más antiguos
find ~/Downloads/ -type f -exec ls -lrt {} + | head -20

# Encontrar archivos más pesados
ls -lS ~/Downloads/ | head -20

# Filtrar solo archivos (no directorios)
ls -lt ~/Downloads/ | grep "^-"

# Obtener solo nombres de archivos ordenados por fecha
ls -l ~/Downloads/ | awk '{print $6, $7, $8, $9}' | sort -M
```

## Análisis de Contenido

### Archivos Antiguos Identificados

1. **Logos de marca personal** (Ago 2023)
   - `Logo png.png`
   - `Logo png (1).png`
   - `Logo Corregido.png`
   - `Inicio marca personal.png`

2. **Logos institucionales** (Sep 2023)
   - Serie de logos en `Logos ae1 de colores en PNG/`

### Archivos Pesados Identificados

1. **Imágenes comprimidas**
   - `Imagenes.zip`: 86 MB - Contiene imágenes varias

2. **Aplicaciones**
   - `OpenCode Desktop.dmg`: 79 MB - Instalador de aplicación

3. **Videos**
   - `WhatsApp Video 2026-02-16 at 08.29.37.mp4`: 28 MB
   - `Pepin.mp4`: 8.3 MB

4. **Documentos PDF**
   - `Manual-de-Identidad-Visual-02072024.pdf`: 17 MB

## Recomendaciones

### Para清理 (Limpieza)
- Los archivos de logos de 2023 podrían archivarse en otro lugar
- Los videos de WhatsApp podrían moverse o eliminarse si ya no son necesarios
- Los archivos .zip muy grandes podrían descomprimirse y evaluarse

### Para Mantener
- Documentos importantes como pasaportes, contratos, certificados
- Materiales de trabajo activo
- Descargas recientes necesarias

## Conclusión

Este caso de uso demuestra la capacidad de OpenCode para:
1. Navegar por el sistema de archivos local
2. Ejecutar comandos del sistema operativo
3. Analizar y filtrar información de archivos
4. Presentar resultados de manera organizada
5. Proporcionar recomendaciones basadas en el análisis

La herramienta permite realizar tareas de administración de archivos de manera eficiente sin necesidad de recordar múltiples comandos o usar diferentes aplicaciones.

---
*Documento creado: Marzo 2026*
*Proyecto: Análisis de archivos locales con OpenCode*

---

# Acciones que puedes hacer con OpenCode en tu equipo

## 📁 Gestión de Archivos

- Listar, buscar y analizar archivos en cualquier directorio
- Leer, crear, editar y eliminar archivos
- Buscar contenido dentro de archivos (grep)
- Ver tamaño y fechas de archivos
- Comprimir/descomprimir archivos zip, tar, etc.
- Mover y copiar archivos entre directorios

## 🔍 Búsqueda y Análisis

- Buscar archivos por nombre, extensión o contenido
- Analizar estructuras de directorios
- Encontrar archivos duplicados o muy pesados
- Buscar código específico en proyectos
- Filtrar y ordenar archivos por múltiples criterios

## 🖥️ Ejecución de Comandos

- Ejecutar cualquier comando de terminal
- Corregir scripts y código
- Instalar dependencias (npm, pip, etc.)
- Ejecutar tests y builds
- Compilar proyectos
- Gestionar procesos del sistema

## 🌐 Navegación Web (Chrome Dev Tools)

- Abrir páginas web automáticamente
- Extraer información de sitios web
- Rellenar formularios automáticamente
- Hacer capturas de pantalla y análisis visual
- Automatizar interacciones web
- Scraping de datos públicos
- Testing de aplicaciones web

## 🔧 Operaciones de Desarrollo

- Inicializar proyectos (git, npm, etc.)
- Crear y modificar código en cualquier lenguaje
- Ejecutar linting y typechecking
- Gestión de repositorios Git
- Debugging de aplicaciones
- Refactorización de código

## 📊 Análisis de Código

- Explicar código existente
- Encontrar bugs y sugerir correcciones
- Refactorizar código
- Escribir tests unitarios
- Documentar funciones y módulos
- Analizar dependencias

## 🤖 Integración con AI/MCP

- Usar modelos de IA locales (Ollama)
- Integrar herramientas externas via MCP
- Crear agentes automatizados
- Ejecutar prompts personalizados
- Conectar con APIs externas

## 📝 Documentación

- Generar documentación automática
- Crear y editar archivos Markdown
- Documentar código
- Crear README y guías
- Generar changelogs

## 🎨 Operaciones con Imágenes y Medios

- Ver metadatos de imágenes
- Convertir formatos de imagen
- Redimensionar imágenes
- Comprimir archivos multimedia

## 🏠 Administración del Sistema

- Gestionar paquetes (brew, npm, etc.)
- Ver procesos en ejecución
- Monitorear recursos del sistema
- Configurar entorno de desarrollo
- Gestionar servicios y demonios

## 💼 Automatización de Tareas

- Crear scripts de automatización
- Programar tareas recurrentes
- Respaldar archivos y directorios
- Sincronizar archivos entre ubicaciones
- Generar reportes automáticos
