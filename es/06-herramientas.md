# 06 - Herramientas y Recursos

Guía completa de herramientas de IA útiles para periodistas, con ejemplos prácticos y mejores prácticas.

## 🤖 Principales Plataformas de IA

### Google Gemini
**URL**: https://gemini.google.com/

**Características**:
- Acceso a Gemini Pro y modelos avanzados
- Integración con búsqueda de Google
- Generación de imágenes con Imagen 3
- Análisis de documentos y PDFs

**Mejor para**:
- Investigación con datos actuales
- Verificación de hechos
- Análisis multimodal

**Prompt ejemplo**:
```
"@Gmail busca correos sobre el proyecto X en los últimos 30 días
@Drive encuentra documentos relacionados con presupuesto 2024
Resume los hallazgos principales"
```

### Google AI Studio
**URL**: https://aistudio.google.com/

**Características**:
- Entorno profesional de desarrollo
- Control fino de parámetros
- Exportación de código
- Análisis con Python integrado

**Configuración periodística recomendada**:
```
Temperature: 0.2
Top-p: 0.8
Safety: Máximo
Grounding: Activado
```

### NotebookLM
**URL**: https://notebooklm.google.com/

**Características**:
- Análisis de múltiples documentos
- Creación de resúmenes automáticos
- Generación de FAQs
- Audio resúmenes (experimental)

**Flujo de trabajo**:
1. Sube hasta 50 fuentes (PDFs, docs, links)
2. Genera notebook con puntos clave
3. Haz preguntas específicas
4. Crea guías de estudio o briefings

## 🔍 Herramientas Especializadas para Periodismo

### Google Pinpoint
**URL**: https://journaliststudio.google.com/pinpoint

**Capacidades**:
- Búsqueda en miles de documentos
- Transcripción de audio/video
- OCR para documentos escaneados
- Detección de entidades

**Caso de uso**:
```
Investigando caso de corrupción:
1. Sube todos los contratos PDF
2. Busca: "sobreprecio" OR "adjudicación directa"
3. Identifica personas mencionadas frecuentemente
4. Crea timeline con fechas clave
```

### Fact Check Explorer
**URL**: https://toolbox.google.com/factcheck/explorer

**Función**: Buscar verificaciones existentes de claims

**Ejemplo de búsqueda**:
```
Claim: "El desempleo está en mínimos históricos"
Filtros: 
- Idioma: Español
- Fecha: Últimos 30 días
- Rating: Falso/Verdadero/Parcial
```

## 🖼️ Generación de Contenido Visual

### Imagen 3 (via Gemini)
**Acceso**: Dentro de Gemini o AI Studio

**Mejores prácticas para periodismo**:
```
"Genera una imagen fotorrealista de [escena] con las siguientes 
especificaciones:
- Estilo: Fotografía periodística
- Composición: [detalles]
- Iluminación: [tipo]
- Elementos importantes: [lista]
- Evitar: Rostros identificables, violencia gráfica
- Incluir marca de agua: 'Generado por IA'"
```

### Google Vids
**URL**: https://vids.google.com/

**Capacidades**:
- Creación de videos desde texto
- Integración con Workspace
- Templates periodísticos
- Narración automática

**Template para noticieros**:
```
Escena 1: [Titular - 3 segundos]
Escena 2: [Contexto con b-roll - 10 segundos]
Escena 3: [Declaraciones clave - 15 segundos]
Escena 4: [Cierre con CTA - 5 segundos]
```

## 📊 Análisis de Datos

### Herramientas Integradas en AI Studio

**Code Execution para periodismo de datos**:
```python
# Prompt ejemplo:
"Analiza el CSV adjunto de presupuesto municipal:
1. Calcula el cambio porcentual año a año
2. Identifica los 5 departamentos con mayor aumento
3. Crea visualización de tendencias
4. Detecta anomalías estadísticas"
```

### Combinación con Sheets
```
"Toma estos datos de criminalidad:
1. Límpielos (elimina duplicados, corrige formatos)
2. Agrupa por distrito y tipo de delito
3. Calcula tasas per cápita
4. Genera fórmulas para Sheets
5. Sugiere gráficos apropiados"
```

## 🔗 Integraciones y APIs

### Gemini API para Redacciones
```python
# Configuración básica
import google.generativeai as genai

genai.configure(api_key="TU_API_KEY")
model = genai.GenerativeModel('gemini-1.5-pro')

# Prompt para automatización
prompt = """
Eres un editor de noticias. 
Convierte este comunicado de prensa en noticia:
- Lead de 50 palabras
- Cuerpo de 200 palabras
- Tono objetivo
- Incluye contexto relevante
"""
```

### Webhooks y Automatización
- Conectar con CMS
- Alertas de breaking news
- Resúmenes automáticos de ruedas de prensa
- Monitoreo de menciones

## 🛡️ Herramientas de Verificación

### Conjunto de Verificación Essential
1. **Google Images inversa**: Verificar origen de fotos
2. **InVID**: Verificación de videos
3. **Wayback Machine**: Versiones anteriores de websites
4. **WHOIS**: Información de dominios
5. **TinEye**: Búsqueda inversa especializada

### Prompt para verificación cruzada
```
"Verifica estas afirmaciones usando múltiples fuentes:
[Lista de claims]

Para cada una indica:
- Fuente original
- Fuentes que la confirman
- Fuentes que la contradicen
- Nivel de confianza (Alto/Medio/Bajo)
- Contexto faltante"
```

## 📚 Recursos de Aprendizaje

### Cursos Recomendados
1. **Google News Initiative Training**: Herramientas digitales para periodistas
2. **Knight Center**: IA para periodistas
3. **Coursera**: Periodismo de datos con Python
4. **DataCamp**: Análisis de datos para medios

### Documentación Esencial
- [Guía de Prompting de Google](https://ai.google.dev/docs/prompting_guide)
- [Mejores prácticas de Gemini](https://ai.google.dev/gemini-api/docs/get-started/tutorial)
- [Ética en IA - UNESCO](https://www.unesco.org/es/artificial-intelligence/recommendation-ethics)

## 🎯 Flujos de Trabajo Completos

### Investigación Rápida (30 minutos)
```
1. Gemini: Contexto general + búsqueda web (5 min)
2. NotebookLM: Análisis de documentos clave (10 min)
3. Pinpoint: Búsqueda en archivo propio (10 min)
4. AI Studio: Síntesis y generación de ángulos (5 min)
```

### Preparación para Entrevista (1 hora)
```
1. Gemini: Perfil del entrevistado + noticias recientes
2. NotebookLM: Análisis de declaraciones previas
3. AI Studio: Generación de 20 preguntas categorizadas
4. Revisión manual y personalización
```

### Fact-Checking Completo (2 horas)
```
1. Identificar claims principales
2. Fact Check Explorer: Verificaciones existentes
3. Gemini + Grounding: Búsqueda de fuentes
4. AI Studio: Análisis de consistencia
5. Documentación de fuentes
```

## 💡 Tips de Productividad

### Atajos y Comandos
- **Gemini**: @ para mencionar Google apps
- **AI Studio**: Ctrl+Enter para ejecutar
- **NotebookLM**: Cmd+K para búsqueda rápida

### Templates Guardados
Crea una biblioteca de prompts en:
- Google Docs compartido del equipo
- GitHub del medio
- Base de datos de Notion
- Herramienta de gestión interna

### Métricas de Efectividad
Rastrea:
- Tiempo ahorrado por tarea
- Precisión de información generada
- Número de verificaciones necesarias
- Satisfacción del equipo

## 🚀 Próximas Herramientas

### En Desarrollo
- **Gemini 2.0**: Capacidades multimodales mejoradas
- **Veo 2**: Generación de video avanzada
- **Project Astra**: Asistente universal

### Tendencias a Seguir
- Agentes autónomos para investigación
- Verificación automática en tiempo real
- Traducción y localización instantánea
- Análisis de sentimiento en redes

---

[← Limitaciones y Ética](05-limitaciones-etica.md) | [Inicio](../README.md) | [Ejemplos →](ejemplos/)
