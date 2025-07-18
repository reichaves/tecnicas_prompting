# 03 - Casos de Uso en Periodismo

Esta sección explora aplicaciones prácticas de prompting en tareas periodísticas cotidianas, con ejemplos y plantillas listas para usar.

## 📰 1. Generación de Titulares

### ¿Por qué usar IA para titulares?
- Generar múltiples opciones rápidamente
- Explorar diferentes ángulos
- Optimizar para diferentes plataformas
- Superar bloqueos creativos

### Plantilla Básica
```
"Eres un editor de [tipo de publicación]. Crea [número] titulares para 
la siguiente noticia: [resumen o lead de la noticia]. 

Requisitos:
- Máximo [X] caracteres
- Tono: [informativo/llamativo/neutro]
- Evitar: [clickbait/sensacionalismo/jerga]
- Incluir: [palabra clave si es necesaria]"
```

### Ejemplo Práctico
```
"Eres un editor de un portal de noticias online. Crea 5 titulares para la 
siguiente noticia: 'Investigación revela que 67% de los mexicanos cambiaron 
hábitos de consumo después de la pandemia, priorizando compras en línea y 
productos locales.'

Requisitos:
- Máximo 60 caracteres
- Tono informativo pero atractivo
- Incluir el dato porcentual
- Enfocarse en el impacto post-pandemia"
```

### Variaciones por Plataforma
- **Web**: Titulares SEO-friendly con palabras clave
- **Redes Sociales**: Más conversacionales y directos
- **Impreso**: Pueden ser más largos y descriptivos

## 📋 2. Resúmenes Automáticos

### Aplicaciones
- Condensar reportes extensos
- Crear briefs de noticias
- Preparar newsletters
- Resumir transcripciones de entrevistas

### Plantilla para Resumen
```
"Como periodista, resume el siguiente [tipo de documento] en [número] 
[frases/párrafos], destacando:
- [Aspecto 1]
- [Aspecto 2]
- [Aspecto 3]

Mantener: [datos específicos/citas/números]
Tono: [objetivo/analítico/informativo]
Audiencia: [especializada/general]"
```

### Ejemplo Real
```
"Como periodista económico, resume este informe del Banco de México en 
3 párrafos, destacando:
- Tasa de interés actual y proyección
- Principales riesgos inflacionarios
- Cambios respecto al informe anterior

Mantener todos los porcentajes exactos
Tono: objetivo y técnico
Audiencia: lectores con conocimiento básico de economía"
```

## 🗂️ 3. Organización de Pautas

### Usos Prácticos
- Priorizar coberturas
- Organizar reuniones de pauta
- Distribuir tareas en la redacción
- Planear coberturas especiales

### Plantilla de Organización
```
"Eres un jefe de redacción. Organiza las siguientes pautas:
[Lista de pautas]

Criterios:
1. Agrupar por sección (política, economía, cultura, etc.)
2. Clasificar por urgencia (urgente, hoy, esta semana)
3. Indicar recursos necesarios (reportero, fotógrafo, tiempo)
4. Sugerir orden de prioridad basado en [criterio]"
```

### Ejemplo Aplicado
```
"Eres un jefe de redacción de un periódico regional. Organiza estas pautas:
- Aumento de casos de dengue en la ciudad
- Nuevo centro comercial será inaugurado
- Alcalde anuncia cambios en el tránsito
- Festival de música el fin de semana
- Escándalo de corrupción en el cabildo

Criterios:
1. Agrupar por relevancia periodística
2. Considerar impacto en la comunidad
3. Sugerir deadline para cada pauta
4. Indicar si necesita seguimiento"
```

## 🔍 4. Análisis de Documentos

### Escenarios de Uso
- Investigaciones con muchos documentos
- Análisis de datos públicos
- Revisión de procesos judiciales
- Fact-checking de declaraciones

### Plantilla para Análisis
```
"Eres un periodista investigativo. Analiza el documento adjunto y:

1. Identifica los principales actores mencionados
2. Extrae todas las fechas y crea una línea de tiempo
3. Destaca valores monetarios y sus contextos
4. Señala inconsistencias o información contradictoria
5. Lista preguntas para investigación adicional

Formato: informe estructurado con subtítulos
Enfoque: [aspecto específico de la investigación]"
```

### Tips para Documentos Largos
- Dividir en secciones si excede el límite de tokens
- Pedir primero un resumen general
- Después profundizar en secciones específicas
- Usar prompts encadenados para análisis completo

## 🎨 5. Creación de Imágenes

### Cuándo Usar
- Ilustrar notas sin fotos
- Crear infografías conceptuales
- Visualizar datos o estadísticas
- Producir contenido para redes sociales

### Plantilla para Imágenes
```
"Crea una [tipo de imagen] mostrando [descripción de la escena].

Estilo: [fotorrealista/ilustración/infográfico]
Composición: [descripción de elementos y posicionamiento]
Colores: [paleta o mood]
Iluminación: [tipo y dirección]
Detalles importantes: [elementos que no pueden faltar]
Evitar: [elementos no deseados]
Formato: [proporción y resolución]"
```

### Ejemplo Práctico
```
"Crea una ilustración fotorrealista mostrando el impacto de la sequía en 
una ciudad del interior de México.

Estilo: fotoperiodístico, realista
Composición: calle principal con comercio local, personas caminando
Colores: tonos terrosos, cielo sin nubes, sensación árida
Iluminación: sol fuerte del mediodía creando sombras duras
Detalles importantes: 
- Vegetación seca
- Suelo agrietado visible
- Personas con expresiones de cansancio
- Comercio con aspecto de poco movimiento
Evitar: dramatización excesiva
Formato: 16:9, alta resolución"
```

## 💡 Mejores Prácticas por Caso

### Para Todos los Casos:
1. **Siempre revisar**: IA es herramienta, no sustituto
2. **Verificar hechos**: Especialmente fechas y números
3. **Mantener ética**: Transparencia sobre uso de IA
4. **Personalizar**: Adaptar plantillas a tu contexto
5. **Iterar**: Refinar prompts basándose en resultados

### Errores Comunes a Evitar:
- Aceptar primera respuesta sin revisión
- No verificar información generada
- Usar tono inadecuado para el medio
- Olvidar contexto local/cultural
- No acreditar uso de IA cuando es apropiado

## 📚 Próximos Pasos

Explora [técnicas avanzadas](04-tecnicas-avanzadas.md) para maximizar resultados o revisa [limitaciones éticas](05-limitaciones-etica.md) del uso de IA en periodismo.

---

[← Elementos](02-elementos.md) | [Inicio](../README.md) | [Técnicas Avanzadas →](04-tecnicas-avanzadas.md)
