# 05 - Limitaciones y Consideraciones Éticas

El uso de IA en el periodismo presenta oportunidades y desafíos. Este capítulo aborda las principales limitaciones técnicas y consideraciones éticas que todo periodista debe conocer.

## ⚠️ 1. Precisión y Verificación

### El Problema de las "Alucinaciones"
Los modelos de IA pueden generar información falsa con aparente confianza. Esto incluye:
- Citas inventadas
- Estadísticas falsas
- Eventos que nunca ocurrieron
- Atribuciones incorrectas

### Mejores Prácticas
```
✅ SIEMPRE verificar:
- Nombres y cargos
- Fechas y lugares
- Cifras y porcentajes
- Citas y declaraciones
- Enlaces y referencias

❌ NUNCA publicar:
- Información no verificada de la IA
- Datos sin contrastar con fuentes
- Contenido generado sin revisión
```

### Estrategias de Verificación
1. **Triangulación**: Confirma con al menos 2 fuentes independientes
2. **Prompt de verificación**: "¿Puedes mostrar la fuente exacta de esta información?"
3. **Búsqueda inversa**: Googlea citas y datos para confirmar
4. **Escepticismo profesional**: Si suena demasiado perfecto, probablemente es falso

## 📅 2. Actualidad de los Datos

### Limitaciones Temporales
- Los modelos tienen fechas de corte de conocimiento
- No acceden a información en tiempo real (salvo con herramientas específicas)
- Pueden mezclar información de diferentes períodos

### Soluciones
```
Para información actual:
1. Activa "Grounding with Google Search" en AI Studio
2. Proporciona contexto temporal explícito
3. Incluye fechas en tus prompts
4. Verifica con fuentes actualizadas
```

## ⚖️ 3. Sesgos y Neutralidad

### Tipos de Sesgos Comunes
- **Geográficos**: Sobrerrepresentación de ciertas regiones
- **Culturales**: Perspectivas dominantes en los datos de entrenamiento
- **Lingüísticos**: Mejor rendimiento en inglés que en otros idiomas
- **Demográficos**: Estereotipos sobre grupos sociales

### Cómo Mitigar Sesgos
```
Prompt anti-sesgo:
"Analiza este tema desde múltiples perspectivas, incluyendo voces 
minoritarias y puntos de vista diversos. Evita estereotipos y 
generalizaciones. Si detectas posibles sesgos en tu respuesta, 
señálalos explícitamente."
```

### Checklist de Revisión
- [ ] ¿La respuesta incluye diversas perspectivas?
- [ ] ¿Hay generalizaciones sobre grupos?
- [ ] ¿Se perpetúan estereotipos?
- [ ] ¿Falta contexto cultural importante?

## 🔒 4. Protección de Datos Confidenciales

### Qué NO Compartir con IA
```
❌ NUNCA incluir:
- Nombres de fuentes protegidas
- Información off the record
- Datos personales sensibles
- Documentos clasificados
- Información de menores
- Material bajo embargo
```

### Técnicas de Anonimización
1. **Reemplazar nombres**: Usa [FUENTE A], [EMPRESA X]
2. **Generalizar datos**: "Una ciudad del norte" vs nombre específico
3. **Omitir identificadores**: Elimina números de documento, direcciones
4. **Usar herramientas locales**: Para información muy sensible

## 👥 5. Transparencia con la Audiencia

### Cuándo Revelar el Uso de IA
- Cuando la IA contribuyó significativamente al contenido
- En visualizaciones o imágenes generadas
- Para análisis de datos complejos
- En traducciones o transcripciones

### Ejemplos de Declaraciones
```
"Este análisis fue asistido por herramientas de inteligencia artificial, 
con verificación humana de todos los datos."

"La visualización fue creada con IA basándose en datos oficiales del 
[fuente]."

"Utilizamos IA para procesar [número] documentos. Todos los hallazgos 
fueron verificados independientemente."
```

## 🧠 6. Evitar la Dependencia

### Riesgos de la Sobre-dependencia
- Pérdida de habilidades periodísticas básicas
- Disminución del pensamiento crítico
- Homogenización del contenido
- Reducción de la creatividad

### Uso Equilibrado
```
✅ USA IA para:
- Acelerar tareas mecánicas
- Explorar ángulos adicionales
- Procesar grandes volúmenes de datos
- Superar bloqueos creativos

❌ NO uses IA para:
- Reemplazar el reporteo directo
- Evitar el contacto con fuentes
- Sustituir el análisis crítico
- Eludir la responsabilidad editorial
```

## 📋 7. Marco Ético para la Redacción

### Política Editorial Sugerida

```markdown
POLÍTICA DE USO DE IA - [Nombre del Medio]

1. PRINCIPIOS GENERALES
   - La IA es una herramienta, no un reemplazo del periodismo humano
   - Toda información debe ser verificada antes de publicación
   - La transparencia con la audiencia es fundamental

2. USOS PERMITIDOS
   - Investigación preliminar
   - Análisis de datos
   - Generación de ideas
   - Traducciones (con revisión)
   - Transcripciones (con corrección)

3. USOS PROHIBIDOS
   - Publicación directa sin edición
   - Creación de citas falsas
   - Suplantación de fuentes
   - Generación de imágenes engañosas

4. REQUISITOS DE TRANSPARENCIA
   - Indicar cuando la IA fue usada significativamente
   - Mantener registro de prompts utilizados
   - Documentar proceso de verificación

5. RESPONSABILIDAD
   - El periodista es responsable del contenido final
   - Editores deben conocer cuándo se usó IA
   - Errores de IA son responsabilidad del medio
```

## 🎯 Guía de Decisión Ética

### Antes de Usar IA, Pregúntate:

1. **¿Es necesario?** ¿O puedo hacerlo sin IA?
2. **¿Es apropiado?** ¿Para este tipo de contenido?
3. **¿Es transparente?** ¿Debo informar a la audiencia?
4. **¿Es seguro?** ¿Protejo la información sensible?
5. **¿Es verificable?** ¿Puedo confirmar los resultados?

## 📚 Recursos Éticos Adicionales

### Guías y Códigos
- [Ethical Guidelines for AI in Journalism - AP](https://www.ap.org/)
- [Reuters Institute Digital News Report](https://reutersinstitute.politics.ox.ac.uk/)
- [SPJ Code of Ethics](https://www.spj.org/ethicscode.asp)

### Herramientas de Verificación
- [Google Fact Check Explorer](https://toolbox.google.com/factcheck/explorer)
- [Verification Handbook](https://verificationhandbook.com/)
- [First Draft Verification Toolkit](https://firstdraftnews.org/)

## ✅ Checklist Final

Antes de publicar contenido asistido por IA:

- [ ] ¿Verifiqué todos los hechos?
- [ ] ¿Eliminé posibles sesgos?
- [ ] ¿Protegí información confidencial?
- [ ] ¿Soy transparente sobre el uso de IA?
- [ ] ¿Mantuve mi criterio periodístico?
- [ ] ¿El contenido cumple estándares éticos?

---

[← Técnicas Avanzadas](04-tecnicas-avanzadas.md) | [Inicio](../README.md) | [Herramientas →](06-herramientas.md)
