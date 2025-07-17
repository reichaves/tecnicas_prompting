# 02 - Elementos de un Buen Prompt

Un prompt efectivo está compuesto por cuatro elementos fundamentales que trabajan juntos para producir resultados óptimos.

## 🎯 1. Claridad

### Definición
El prompt debe ser inequívoco y específico. Evitar términos vagos o preguntas demasiado generales que lleven a respuestas amplias y poco útiles.

### Ejemplos

❌ **Ambiguo:**
```
"Explícame tecnología"
```

✅ **Claro:**
```
"Como experto en ciberseguridad, explica brevemente tres medidas para 
proteger una red corporativa contra ataques de ransomware"
```

### Técnicas para mejorar la claridad:
- Usa verbos de acción específicos (analiza, compara, resume, lista)
- Define términos técnicos si son necesarios
- Evita pronombres sin referente claro
- Estructura las instrucciones en pasos numerados cuando sea apropiado

## 🌍 2. Contexto

### Definición
Proporcionar información de fondo o situacional para guiar a la IA. Esto incluye establecer un rol o audiencia y detalles relevantes del tema.

### Componentes del contexto:
- **Rol**: "Eres un periodista deportivo..."
- **Audiencia**: "...escribiendo para lectores jóvenes..."
- **Situación**: "...cubriendo el Mundial de Fútbol 2026..."
- **Restricciones**: "...con un límite de 500 palabras"

### Ejemplo completo:
```
"Eres un periodista deportivo escribiendo para un público general no 
especializado. El contexto es la final de la Copa América 2024. 
Necesito que expliques las reglas básicas del VAR de manera simple."
```

## 📋 3. Instrucciones Precisas (Tarea)

### Definición
Indicar claramente qué se quiere que haga la IA. La tarea es el núcleo de la orden y nunca debe faltar en el prompt.

### Frases de acción útiles:
- **Para análisis**: "Analiza...", "Compara...", "Evalúa..."
- **Para síntesis**: "Resume...", "Sintetiza...", "Condensa..."
- **Para creación**: "Genera...", "Crea...", "Diseña..."
- **Para organización**: "Lista...", "Categoriza...", "Prioriza..."

### Ejemplo estructurado:
```
"Analiza los siguientes datos de criminalidad:
1. Identifica las tres tendencias principales
2. Compara con el año anterior
3. Sugiere posibles causas para los cambios observados"
```

## 📐 4. Formato de Salida

### Definición
Especificar el formato o estilo esperado en la respuesta asegura que el modelo entregue el contenido ya estructurado según la necesidad.

### Opciones de formato:
- **Estructura**: Párrafo, lista numerada, viñetas, tabla
- **Longitud**: Número de palabras, oraciones o párrafos
- **Tono**: Formal, informal, académico, conversacional
- **Estilo**: Periodístico, técnico, creativo, informativo

### Ejemplo detallado:
```
"Formato de salida:
- Un párrafo introductorio de 2-3 oraciones
- Lista de 5 puntos principales con viñetas
- Cada punto debe tener máximo 50 palabras
- Tono: profesional pero accesible
- Incluir al menos dos estadísticas relevantes"
```

## 🔧 Combinando todos los elementos

### Prompt completo ejemplar:
```
[CONTEXTO] Eres un editor de política en un diario nacional.

[TAREA] Resume los puntos clave del informe adjunto sobre transparencia 
gubernamental, enfocándote en los datos de 2023.

[CLARIDAD] Identifica específicamente:
- Los tres hallazgos más importantes
- Cambios respecto al año anterior
- Implicaciones para la política pública

[FORMATO] Responde con:
- Un párrafo inicial de contexto (máximo 3 oraciones)
- 3-5 puntos clave en lista numerada
- Tono formal y objetivo
- Extensión total: máximo 300 palabras
```

## 📝 Ejercicio Práctico

Crea un prompt que incluya los cuatro elementos para las siguientes situaciones:

1. **Situación**: Necesitas un análisis de las redes sociales de un político
   **Tu prompt**: _______________

2. **Situación**: Quieres generar preguntas para una entrevista con un CEO
   **Tu prompt**: _______________

3. **Situación**: Necesitas un resumen de un documento legal complejo
   **Tu prompt**: _______________

## ✅ Lista de verificación

Antes de enviar tu prompt, verifica:
- [ ] ¿Es claro y específico?
- [ ] ¿Incluye contexto relevante?
- [ ] ¿La tarea está bien definida?
- [ ] ¿Especifica el formato deseado?
- [ ] ¿Evita ambigüedades?

## 🚀 Próximos pasos

Una vez que domines estos elementos, explora cómo aplicarlos en [casos de uso específicos del periodismo](03-casos-uso.md).

---

[← Fundamentos](01-fundamentos.md) | [Inicio](../README.md) | [Casos de Uso →](03-casos-uso.md)
