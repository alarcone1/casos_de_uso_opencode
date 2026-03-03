# Caso de Uso: Investigación de Ideas de Negocio con Chrome DevTools MCP

## Objetivo

Proponer 3 prompts generales para investigar una idea de negocio utilizando Chrome DevTools MCP, permitiendo explorar mercados, competidores y clientes potenciales de manera automatizada.

## Herramientas Utilizadas

- **WebSearch**: Búsqueda inicial de información general
- **Chrome DevTools MCP**: Navegación y extracción de información desde sitios web

## Antecedentes

Se tenían 100 ideas de negocio categorizadas en 9 clusters temáticos:
- Salud y Medicina (10 ideas)
- Arquitectura y Construcción (10 ideas)
- Agricultura - AgriTech (10 ideas)
- Industria Alimentaria - FoodTech (10 ideas)
- Ingeniería Civil (10 ideas)
- Ingeniería Mecánica (10 ideas)
- Ingeniería Industrial y Logística (10 ideas)
- Salud Mental y Psicología (20 ideas)
- Educación - EdTech (10 ideas)

Adicionalmente, se identificó el patrón "Evals-as-a-Service" como solución transversal en 8 de las ideas.

## Propuestas de Prompts

### Prompt 1: Exploración de Mercado y Competidores

> "Investiga el mercado de **[idea de negocio]** en **[ubicación/geografía]**. Usa Chrome DevTools MCP para navegar los sitios web de las 5 empresas competidoras más importantes, extrae información sobre: modelo de negocio, precios, características principales, testimonios de clientes y datos de contacto. Presenta los hallazgos en una tabla comparativa."

**Usos recomendados:**
- Validar que existe demanda real para la idea
- Identificar gaps en el mercado
- Definir propuesta de valor diferenciada
- Conocer precios del mercado

---

### Prompt 2: Descubrimiento de Clientes Objetivo

> "Identifica empresas o profesionales que podrían ser clientes potenciales para un **[tipo de solución]** en **[sector/industria]**. Utiliza Chrome DevTools MCP para visitar directorios empresariales, perfiles de LinkedIn y sitios de asociaciones del sector. Extrae: nombres de empresas, datos de contacto, servicios que ofrecen y posibles puntos de dolor relacionados con **[problema que resuelve]**."

**Usos recomendados:**
- Generar lista de prospectos cualificados
- Entender las necesidades reales del público objetivo
- Identificar tomadores de decisión en empresas
- Preparar estrategias de venta

---

### Prompt 3: Análisis de Productos/Servicios Existentes

> "Analiza 3-5 soluciones similares a **[idea de negocio]** que existan actualmente en el mercado. Usa Chrome DevTools MCP para navegar sus sitios web oficiales y obtener: funcionalidades descritas, planes de precios, formularios de contacto, tecnologías utilizadas (stack), posicionamiento de marca y cualquier información sobre la empresa. Genera un informe de ventajas y debilidades de cada competidor."

**Usos recomendados:**
- Análisis competitivo exhaustivo
- Definir diferenciadores estratégicos
- Conocer mejores prácticas del mercado
- Identificar oportunidades de innovación

---

## Aplicación Práctica

### Ejemplo de Uso: Idea #1 - Infraestructura de Evaluación para IA (B2B)

**Prompt 1 aplicado:**
> "Investiga el mercado de plataformas SaaS de evaluación de modelos de IA (Evals) en Estados Unidos y Europa. Usa Chrome DevTools MCP para navegar los sitios web de las 5 empresas competidoras más importantes como Aporia, Fiddler, Giskard, etc., extrae información sobre: modelo de negocio, precios, características principales, testimonios de clientes y datos de contacto. Presenta los hallazgos en una tabla comparativa."

**Prompt 2 aplicado:**
> "Identifica empresas de IA en Colombia y Latinoamérica que podrían ser clientes potenciales para una plataforma de evaluación de modelos de IA. Utiliza Chrome DevTools MCP para visitar directorios de startups, perfiles de LinkedIn y sitios de asociaciones como Colombia.dev, ANDICOM. Extrae: nombres de empresas, datos de contacto, servicios que ofrecen y posibles puntos de dolor relacionados con la validación de sus modelos."

**Prompt 3 aplicado:**
> "Analiza 3-5 soluciones de MLOps y evaluación de modelos de IA que existan actualmente como Weights & Biases, MLflow, Neptune.ai. Usa Chrome DevTools MCP para navegar sus sitios web oficiales y obtener: funcionalidades descritas, planes de precios, tecnologías utilizadas, posicionamiento de marca y información sobre la empresa. Genera un informe de ventajas y debilidades de cada competidor."

---

## Beneficios del Chrome DevTools MCP para Investigación

1. **Automatización de recolección de datos**: Elimina la necesidad de visitas manuales repetitivas
2. **Datos actualizados**: Extrae información en tiempo real directamente de las fuentes
3. **Consistencia**: Permite replicar la investigación múltiples veces
4. **Profundidad**: Acceso a información que no aparece en búsquedas estáticas
5. **Eficiencia**: Reducesignificativamente el tiempo de investigación

## Comandos Utilizados

```bash
# Abrir nueva página web
chrome-devtools_new_page { "url": "https://ejemplo.com" }

# Tomar snapshot de la página actual
chrome-devtools_take_snapshot { }

# Cerrar página
chrome-devtools_close_page { "pageId": 1 }

# Tomar captura de pantalla
chrome-devtools_take_screenshot { 
  "filePath": "ruta/imagen.png",
  "fullPage": true 
}
```

## Conclusión

Estas 3 propuestas de prompts proporcionan un marco estructurado para investigar cualquier idea de negocio utilizando Chrome DevTools MCP. Permiten:

1. **Validar** la viabilidad del mercado
2. **Identificar** clientes potenciales
3. **Analizar** la competencia

La combinación de estos tres enfoques proporciona una visión completa del panorama competitivo y de mercado necesaria para tomar decisiones informadas sobre el desarrollo de un producto o servicio.

---
*Documento creado: Marzo 2026*
*Proyecto: Investigación de ideas de negocio con Chrome DevTools MCP*
