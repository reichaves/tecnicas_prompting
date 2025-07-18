# Guía Completa de Google AI Studio para Periodistas

Google AI Studio es una plataforma poderosa para prototipar y probar prompts con los modelos Gemini. Esta guía detalla las configuraciones esenciales para periodistas.

## 🚀 Configuraciones Esenciales

### 1. System Instructions (Instrucciones del Sistema)
**Qué es**: Define la personalidad, rol y estilo de las respuestas de la IA.

**Cómo usar para periodismo**:
```
"Eres un periodista investigativo escéptico, siempre verificando hechos y 
cuestionando fuentes. Tus respuestas deben ser objetivas, basadas en 
evidencias y seguir el estándar de pirámide invertida."
```

### 2. Temperature (Temperatura)
**Qué es**: Controla la aleatoriedad y creatividad de las respuestas (0 a 1).

**Configuraciones recomendadas**:
- `0.0 - 0.3`: Fact-checking, resúmenes, análisis de datos
- `0.4 - 0.7`: Redacción de noticias, preguntas para entrevistas
- `0.8 - 1.0`: Brainstorming, titulares creativos, pautas

### 3. Token Count (Conteo de Tokens)
**Qué es**: Cantidad de texto que el modelo puede procesar.

**Límites importantes**:
- Gemini 1.5 Pro: hasta 2 millones de tokens de entrada
- Gemini 1.5 Flash: hasta 1 millón de tokens
- 1 token ≈ 0.75 palabras en español

### 4. Thinking Mode (Modo Pensamiento)
**Qué es**: Muestra el razonamiento del modelo antes de la respuesta final.

**Cuándo activar**:
- Investigaciones complejas
- Análisis que requieren múltiples perspectivas
- Verificación de lógica en argumentos

### 5. Grounding with Google Search
**Qué es**: Conecta el modelo a información actualizada de la web.

**Esencial para**:
- Verificación de hechos recientes
- Cobertura de eventos actuales
- Confirmación de datos y estadísticas

## 📊 Configuración Recomendada para Periodismo

### Para Reportaje Factual:
```
Temperature: 0.1
Thinking Mode: Activado
Grounding: Activado
Safety Settings: Máximo
System Instructions: "Eres un periodista factual. Siempre cita fuentes 
e indica cuando la información no puede ser verificada."
```

### Para Contenido Creativo:
```
Temperature: 0.7
Thinking Mode: Desactivado
Top P: 0.9
System Instructions: "Eres un redactor creativo pero responsable. 
Mantén precisión factual mientras exploras ángulos interesantes."
```

## 🔧 Otras Configuraciones Útiles

### Top P
- Controla diversidad vocabular
- Usa valores bajos (0.1-0.5) para textos técnicos
- Usa valores altos (0.8-0.95) para textos creativos

### Safety Settings
Configura filtros para:
- Discurso de odio
- Contenido dañino
- Desinformación
- Importante: Mantener al máximo para periodismo

### Code Execution
Permite análisis de datos con Python:
- Útil para periodismo de datos
- Procesamiento de hojas de cálculo
- Creación de visualizaciones

## 💰 Límites de la Cuenta Gratuita

### Solicitudes por Minuto (RPM):
- Gemini 1.5 Pro: 2 RPM
- Gemini 1.5 Flash: 15 RPM

### Solicitudes por Día (RPD):
- Gemini 1.5 Pro: 50 RPD
- Gemini 1.5 Flash: 1,500 RPD
- Grounding with Search: 1,000-1,500 RPD

## 🎯 Flujo de Trabajo Optimizado

### 1. Investigación Inicial
```
1. Usa Gemini Flash con Temperature 0.5
2. Activa Grounding para datos actuales
3. Haz preguntas exploratorias
```

### 2. Profundización
```
1. Cambia a Gemini Pro
2. Reduce Temperature a 0.1
3. Activa Thinking Mode
4. Realiza análisis detallados
```

### 3. Redacción Final
```
1. Usa configuración equilibrada (Temperature 0.3)
2. Define System Instructions para tono deseado
3. Revisa y verifica todos los hechos
```

## ⚡ Atajos de Productividad

### Plantillas Guardadas
Crea y guarda prompts para:
- Resúmenes de conferencias
- Análisis de documentos
- Generación de pautas
- Fact-checking

### Uso de Contexto
- Adjunta múltiples documentos
- Usa hasta 10 archivos por vez
- Formatos soportados: PDF, TXT, DOC, imágenes

### Exportación
- Copia código para API
- Exporta a Vertex AI
- Guarda historial de conversaciones

## 🚨 Avisos Importantes

1. **Siempre verificar**: La información puede ser incorrecta
2. **Citar el uso de IA**: Mantener transparencia
3. **Proteger fuentes**: No incluir información sensible
4. **Respetar límites**: Monitorear uso de tokens y solicitudes

## 📚 Recursos Adicionales

- [Documentación Oficial](https://ai.google.dev/docs)
- [Mejores Prácticas](https://ai.google.dev/docs/prompting_guide)
- [Foro de la Comunidad](https://discuss.ai.google.dev/)

---

[← Volver al inicio](README.md)
