# 01 - Fundamentos del Prompting

## ¿Qué es un Prompt?

Un **prompt** es la instrucción o entrada que le damos a un modelo de IA para que genere una respuesta o resultado. El modelo responde en lenguaje natural basándose en esa indicación.

> 💡 **Concepto clave**: Los modelos generativos no "entienden" intenciones ocultas, solo siguen las instrucciones provistas. Por eso, es responsabilidad del usuario formular bien la petición.

## La Importancia de un Buen Prompt

La calidad del prompt influye directamente en la calidad de la respuesta del modelo. Piensa en el prompting como una habilidad similar a hacer las preguntas correctas en una entrevista periodística.

## Prompt Genérico vs. Específico

### Ejemplo de Comparación

**Prompt Genérico:**
```
"¿Qué me puedes decir sobre el cambio climático?"
```

**Prompt Específico:**
```
"Eres un periodista científico. Resume en 3 frases claras los efectos del 
cambio climático en América Latina, citando un dato reciente."
```

### ¿Por qué la diferencia importa?

- El prompt genérico puede generar respuestas muy amplias y poco útiles
- El prompt específico:
  - Define un rol (periodista científico)
  - Establece una tarea clara (resumir)
  - Limita el alcance (3 frases)
  - Especifica el contexto geográfico (América Latina)
  - Requiere evidencia (dato reciente)

## Principios Básicos del Prompting Efectivo

### 1. Sé Específico
En lugar de preguntas abiertas, proporciona instrucciones claras sobre lo que necesitas.

### 2. Proporciona Contexto
Ayuda al modelo a entender el marco de referencia de tu solicitud.

### 3. Define el Formato
Especifica cómo quieres que se estructure la respuesta.

### 4. Establece Limitaciones
Indica restricciones como longitud, tono o estilo.

## Ejercicio Práctico

Transforma estos prompts genéricos en específicos:

1. **Genérico**: "Escribe sobre la economía"
   **Específico**: Tu versión aquí

2. **Genérico**: "Dame información sobre elecciones"
   **Específico**: Tu versión aquí

3. **Genérico**: "Habla sobre tecnología"
   **Específico**: Tu versión aquí

## Errores Comunes a Evitar

1. **Ser demasiado vago**: "Dime algo interesante"
2. **No especificar el formato**: Olvidar indicar si quieres lista, párrafo, tabla, etc.
3. **Asumir conocimiento implícito**: El modelo no sabe tu contexto específico
4. **Prompts muy largos sin estructura**: Dificultan la comprensión

## Mejores Prácticas

- **Itera y refina**: Si la primera respuesta no es ideal, ajusta tu prompt
- **Guarda prompts exitosos**: Crea tu biblioteca personal
- **Experimenta con variaciones**: Pequeños cambios pueden mejorar mucho los resultados
- **Incluye ejemplos**: Si es posible, muestra el tipo de respuesta que esperas

## Próximos Pasos

Una vez que comprendas estos fundamentos, estarás listo para explorar los [elementos específicos de un buen prompt](02-elementos.md).

---

[← Volver al inicio](../README.md) | [Siguiente: Elementos de un Buen Prompt →](02-elementos.md)
