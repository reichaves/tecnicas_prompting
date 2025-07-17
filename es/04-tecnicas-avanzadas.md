# 04 - Técnicas Avanzadas de Prompting

Este capítulo explora métodos sofisticados para obtener resultados superiores de los modelos de IA, especialmente útiles para investigaciones complejas y proyectos periodísticos ambiciosos.

## 🌳 Tree-of-Thoughts (Árbol de Pensamientos)

### ¿Qué es?
Una técnica que hace que la IA explore múltiples ramas de pensamiento antes de decidir una respuesta, similar a cómo un periodista evalúa diferentes ángulos de una historia.

### Estructura Básica
```
"Explora este tema considerando múltiples perspectivas:

1. Primero, identifica 3-4 enfoques posibles
2. Para cada enfoque, desarrolla los argumentos principales
3. Evalúa pros y contras de cada perspectiva
4. Sintetiza una conclusión balanceada

Tema: [Tu tema aquí]"
```

### Ejemplo Periodístico
```
"Como editor investigativo, analiza la propuesta de ley sobre privacidad 
digital:

1. Identifica 4 perspectivas clave:
   - Defensores de privacidad
   - Empresas tecnológicas
   - Gobierno/seguridad
   - Ciudadanos comunes

2. Para cada perspectiva, desarrolla:
   - Argumentos principales
   - Intereses en juego
   - Posibles consecuencias

3. Evalúa conflictos entre perspectivas

4. Propón ángulos periodísticos para cubrir el tema"
```

### Cuándo Usar Tree-of-Thoughts
- Investigaciones con múltiples stakeholders
- Análisis de políticas públicas
- Cobertura de temas controversiales
- Planificación de series investigativas

## 🔄 ReAct (Reasoning and Acting)

### ¿Qué es?
Combina razonamiento paso a paso con acciones específicas, permitiendo que el modelo "piense en voz alta" antes de responder.

### Estructura ReAct
```
"Paso 1 - Razonamiento: [Analiza la situación]
Paso 2 - Acción: [Qué hacer basado en el análisis]
Paso 3 - Observación: [Qué resultó de la acción]
Paso 4 - Conclusión: [Síntesis final]"
```

### Aplicación en Fact-Checking
```
"Verifica esta afirmación usando el método ReAct:
'El desempleo juvenil aumentó 50% en el último año'

Razonamiento: Primero debo identificar qué período específico se 
menciona y qué fuentes oficiales reportan desempleo juvenil.

Acción: Buscar datos del Instituto Nacional de Estadística para el 
último año disponible.

Observación: [Incluir datos encontrados]

Razonamiento: Comparar con el año anterior y calcular el porcentaje 
real de cambio.

Conclusión: La afirmación es [verificada/falsa/parcialmente correcta] 
porque..."
```

## 📚 Bibliotecas y Templates

### Creando tu Biblioteca Personal

#### Template: Investigación de Antecedentes
```
PROMPT: Perfil de Investigación

Eres un periodista investigativo preparando un perfil sobre [SUJETO].

Recopila y organiza:
1. Información biográfica básica
2. Trayectoria profesional
3. Conexiones empresariales/políticas
4. Declaraciones públicas relevantes
5. Controversias o investigaciones previas
6. Patrimonio declarado (si es público)

Fuentes a considerar:
- Registros públicos
- Declaraciones juradas
- Noticias previas
- Redes sociales profesionales

Formato: Informe ejecutivo con secciones claramente marcadas
Advertencias: Señala información no verificada o rumores
```

#### Template: Análisis de Datos
```
PROMPT: Análisis Periodístico de Datos

Contexto: Tengo un dataset sobre [TEMA] con las siguientes variables:
[LISTA DE VARIABLES]

Tareas:
1. Identifica las 3 tendencias más significativas
2. Busca correlaciones relevantes
3. Detecta anomalías o outliers
4. Sugiere visualizaciones apropiadas
5. Formula preguntas para investigación adicional

Consideraciones:
- Tamaño de muestra
- Posibles sesgos en los datos
- Limitaciones del dataset
- Contexto socioeconómico

Entrega: Bullet points con hallazgos clave + párrafo narrativo
```

## 🔗 Prompting en Cadena

### ¿Qué es?
Técnica de usar múltiples prompts secuenciales donde cada uno construye sobre el anterior.

### Ejemplo: Investigación en 4 Pasos

**Prompt 1 - Exploración**
```
"Lista los 10 principales actores involucrados en el caso de 
corrupción en [empresa/institución]"
```

**Prompt 2 - Profundización**
```
"Para los 3 actores más importantes de la lista anterior, detalla:
- Rol específico
- Conexiones entre ellos
- Beneficios obtenidos"
```

**Prompt 3 - Verificación**
```
"Identifica qué afirmaciones del análisis anterior necesitan 
verificación adicional y sugiere fuentes para confirmarlas"
```

**Prompt 4 - Narrativa**
```
"Construye un lead de 100 palabras que capture la esencia de 
esta investigación, comenzando con el hallazgo más impactante"
```

## 🎯 Few-Shot Prompting

### ¿Qué es?
Proporcionar ejemplos específicos del tipo de respuesta que buscas.

### Estructura
```
"Quiero titulares en este estilo:

Ejemplo 1: 'Revelan red de sobornos: 15 funcionarios implicados'
Ejemplo 2: 'Exclusiva: Documentos muestran desvío millonario'
Ejemplo 3: 'Investigan a ministro por conflicto de interés'

Ahora crea 5 titulares similares para esta noticia: [NOTICIA]"
```

### Cuándo es Más Efectivo
- Cuando necesitas consistencia de estilo
- Para formatos específicos del medio
- Al entrenar nuevos colaboradores
- Para mantener tono editorial

## 🧩 Combinación de Técnicas

### Super-Prompt Investigativo
```
[CONTEXTO - System Instructions]
Eres un periodista investigativo senior del Washington Post 
especializado en seguir el dinero en casos de corrupción.

[TREE-OF-THOUGHTS]
Analiza el siguiente caso desde 3 perspectivas:
1. Flujo financiero
2. Red de contactos
3. Timeline de eventos

[REACT]
Para cada perspectiva:
- Razona qué buscar
- Identifica fuentes necesarias
- Anticipa obstáculos

[FEW-SHOT]
Formato de salida como estos ejemplos:
- "HALLAZGO: [descripción] | FUENTE: [tipo] | VERIFICACIÓN: [método]"

[CHAIN]
Finalmente, propón los próximos 5 pasos de investigación en orden 
de prioridad.
```

## 💡 Técnicas Específicas por Tipo de Cobertura

### Para Investigación Financiera
```
"Modo: Análisis forense financiero
1. Rastrea flujos de dinero entre entidades
2. Identifica patrones sospechosos
3. Marca transacciones que requieren scrutinio
4. Sugiere expertos para consultar"
```

### Para Cobertura Electoral
```
"Modo: Análisis electoral multidimensional
1. Tendencias demográficas
2. Comparación histórica
3. Factores externos influyentes
4. Escenarios probables con porcentajes"
```

### Para Periodismo de Datos
```
"Modo: Data journalist
1. Limpieza de datos - qué eliminar/corregir
2. Variables clave para story
3. Correlaciones vs causaciones
4. Visualización más impactante"
```

## 📈 Optimización de Resultados

### Técnica de Refinamiento Iterativo
1. **Prompt inicial**: Amplio y exploratorio
2. **Refinamiento 1**: Enfoca en hallazgos interesantes
3. **Refinamiento 2**: Profundiza en detalles específicos
4. **Pulido final**: Ajusta tono y formato

### Ejemplo Práctico
```
Iteración 1: "Analiza tendencias en educación pública"
Iteración 2: "Enfócate en la brecha rural-urbana identificada"
Iteración 3: "Detalla casos específicos de 3 municipios"
Iteración 4: "Redacta con tono humano, incluyendo testimonios"
```

## 🛠️ Herramientas Complementarias

### Prompts para Diferentes Herramientas

**Para NotebookLM**
```
"Analiza estos 10 documentos y crea:
1. Resumen ejecutivo de hallazgos comunes
2. Contradicciones entre documentos
3. Línea temporal unificada
4. Personas mencionadas con frecuencia"
```

**Para Google AI Studio con Code Execution**
```
"Analiza este CSV de gastos gubernamentales:
1. Calcula totales por departamento
2. Identifica aumentos superiores al 50%
3. Crea gráfico de tendencias
4. Marca anomalías estadísticas"
```

## ✅ Mejores Prácticas Avanzadas

1. **Documenta tus prompts exitosos**: Crea un repositorio personal
2. **Combina técnicas según necesidad**: No todas sirven para todo
3. **Ajusta por modelo**: Gemini vs GPT vs Claude responden diferente
4. **Mide efectividad**: Tiempo ahorrado vs calidad obtenida
5. **Comparte con el equipo**: Estandariza prompts en la redacción

---

[← Casos de Uso](03-casos-uso.md) | [Inicio](../README.md) | [Limitaciones y Ética →](05-limitaciones-etica.md)
