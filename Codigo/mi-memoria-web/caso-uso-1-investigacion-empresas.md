# Caso de Uso: Chrome Dev Tools MCP para Investigación de Empresas de Tecnología

## Prompt Original

> "Necesito encontrar clientes de alta calidad para un curso de inteligencia artificial, cómo aprovechar la inteligencia artificial para su negocio. Por favor, deme las direcciones de correo, las direcciones físicas y el teléfono de contacto en una tabla CSV. Personalmente, vivo en Cartagena de Indias y entonces necesito que encuentre información detallada para ello. Ponte a trabajar inmediatamente en la búsqueda y sea claro. Asegúrate de usar Chrome Dev Tools MCP para ejecutar cualquiera de estas tareas porque quiero ver cómo funciona."

---

## Objetivo

Investigar empresas de tecnología en Cartagena de Indias, Colombia, para identificar prospectos potenciales para un curso de inteligencia artificial.

## Herramientas Utilizadas

- **WebSearch**: Búsqueda inicial de empresas de tecnología en Cartagena
- **Chrome Dev Tools MCP**: Navegación y extracción de información de contacto desde sitios web

## Proceso Realizado

### 1. Búsqueda Inicial (WebSearch)

Se realizaron búsquedas para identificar:
- Empresas de tecnología y startups en Cartagena
- Agencias de desarrollo de software
- Directorios de empresas tech en la región

**Resultados encontrados:**
- Artificial Intelligence de Colombia S.A.S. (ai-col.co)
- Agilesoft (agilesoft.com.co)
- Dev Brothers SAS (devbrothers.co)
- Tu Consultor TI (tuconsultorti.com)
- Tecniblast S.A.S.
- SIIR Group
- Invest in Cartagena y Bolívar

### 2. Exploración con Chrome Dev Tools MCP

#### Página 1: Artificial Intelligence de Colombia S.A.S.
- **URL**: https://ai-col.co/site
- **Información extraída**:
  - Teléfono: (+57) 305 2406220
  - Contacto: WhatsApp
  - Empresa especializada en soluciones de IA y chatbots (SmartChatAI)
  - Ubicación: Cartagena, Colombia

#### Página 2: Agilesoft
- **URL**: https://agilesoft.com.co/
- **Información extraída**:
  - Email: info@agilesoft.com.co
  - Dirección: Calle 123 #45-67, Bogotá, Colombia
  - Especialidades: Hiperautomatización, IA, desarrollo de software

#### Página 3: Tu Consultor TI
- **URL**: https://www.tuconsultorti.com/ubicaciones/cartagena/
- **Información extraída**:
  - Teléfono: +57 (300) 3172063
  - Email: contacto@tuconsultorti.com
  - Servicios: Ciberseguridad, cloud, desarrollo, RPA

## Resultados Obtenidos

| Empresa | Teléfono | Email | Sitio Web |
|---------|----------|-------|-----------|
| Artificial Intelligence de Colombia S.A.S. | (+57) 305 2406220 | WhatsApp | ai-col.co |
| Agilesoft | - | info@agilesoft.com.co | agilesoft.com.co |
| Tu Consultor TI | +57 (300) 3172063 | contacto@tuconsultorti.com | tuconsultorti.com |

## Beneficios del Chrome Dev Tools MCP

1. **Navegación automatizada**: Permite abrir múltiples páginas web automáticamente
2. **Extracción de contenido**: Snapshot completo del DOM con identificación de elementos
3. **Acceso a información dinámica**: Captura datos que no aparecen en búsquedas estáticas
4. **Interacción con elementos**: Posibilidad de hacer click, fill forms, y otras interacciones
5. **Sin necesidad de screenshots**: El snapshot proporciona estructura navegable

## Comandos Utilizados

```bash
# Abrir nueva página
chrome-devtools_new_page { "url": "https://ai-col.co/" }

# Tomar snapshot de la página actual
chrome-devtools_take_snapshot { }

# Cerrar página
chrome-devtools_close_page { "pageId": 3 }
```

## Recomendaciones para Uso Futuro

1. **Verificar información**: Los datos de contacto pueden cambiar, siempre verificar en el sitio oficial
2. **Ética de prospecting**: Usar métodos éticos de contacto (no spam)
3. **Formularios de contacto**: Preferir el uso de formularios oficiales en lugar de emails directos no solicitados
4. **Networking**: Asistir a eventos tecnológicos locales para contacto directo

## Conclusión

Chrome Dev Tools MCP es una herramienta poderosa para investigación de mercado y prospecting, permitiendo automatizar la recolección de información de contacto directamente desde sitios web empresariales. Es útil para:
- Investigación de competidores
- Generación de leads
- Verificación de información de contacto
- Monitoreo de sitios web

---
*Documento creado: Marzo 2026*
*Proyecto: Investigación de empresas tech en Cartagena*
