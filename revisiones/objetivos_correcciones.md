# CORRECCIONES Y MEJORAS A LOS OBJETIVOS

## CORRECCIONES

### 1. Formato incorrecto del objetivo general
**Problema:** El objetivo general está dentro de un entorno `\begin{itemize}...\end{itemize}` con un solo elemento.

**Corrección:** Eliminar el entorno de lista y presentar el objetivo general como texto directo después del título de subsección.

**Justificación:** Los objetivos generales, al ser únicos, no deben presentarse como listas. Solo debe usarse itemize cuando hay múltiples elementos del mismo nivel.

---

### 2. Falta de especificidad en el alcance
**Problema:** El objetivo general dice "desarrollar un algoritmo de clasificación" sin especificar si es binaria, multiclase o ambas.

**Corrección:** Especificar "desarrollar algoritmos de clasificación binaria y multiclase"

**Justificación:** El trabajo desarrolla ambos tipos de clasificadores, por lo que el objetivo debe reflejarlo claramente.

---

### 3. Redundancia entre objetivo general y específico
**Problema:** El objetivo específico 3 ("Desarrollar un algoritmo para la clasificación...") es casi idéntico al objetivo general.

**Corrección:** Reemplazar por objetivos más específicos sobre las arquitecturas concretas, técnicas de regularización y análisis de canales de color.

**Justificación:** Los objetivos específicos deben desglosar el objetivo general en tareas concretas, no repetirlo con otras palabras.

---

### 4. Objetivo específico 2 demasiado vago
**Problema:** "Recopilar y organizar un conjunto de datos" no especifica qué datos, de dónde, ni para qué propósito específico.

**Corrección:** Dividir en dos objetivos más específicos: uno sobre recopilación de datasets públicos y privados con tamaños específicos, y otro sobre preprocesamiento.

**Justificación:** La recopilación y el preprocesamiento son actividades distintas y fundamentales que merecen objetivos separados.

---

### 5. Falta de objetivos medibles
**Problema:** Los objetivos actuales son difíciles de medir objetivamente (¿cuándo se ha "desarrollado" un algoritmo?, ¿qué significa "efectividad"?).

**Corrección:** Añadir métricas específicas o entregables concretos (ej: "alcanzar sensibilidad superior al 90%", "validar en al menos 3 datasets externos").

**Justificación:** Los objetivos deben seguir el criterio SMART (Específicos, Medibles, Alcanzables, Relevantes, Temporales). La medibilidad es fundamental.

---

### 6. Falta objetivo sobre contribución original
**Problema:** No hay objetivo específico sobre el análisis por canales de color RGB, que es una de las contribuciones originales del trabajo.

**Corrección:** Añadir objetivo específico sobre análisis comparativo de canales de color.

**Justificación:** Las contribuciones originales del trabajo deben estar reflejadas en los objetivos específicos.

---

### 7. Falta objetivo sobre validación externa
**Problema:** El objetivo 4 menciona "evaluar y validar" pero no específica que se usarán datasets externos diferentes al de entrenamiento.

**Corrección:** Separar evaluación interna de validación externa en objetivos distintos, especificando los datasets externos.

**Justificación:** La validación externa es crítica para demostrar generalización y debe estar explícitamente mencionada como objetivo.

---

## MEJORAS AÑADIDAS

### 1. Objetivo general más completo y específico
**Contenido nuevo:** "Desarrollar e implementar algoritmos de clasificación automática basados en aprendizaje profundo para la detección y gradación de severidad de retinopatía diabética en imágenes del fondo del ojo, mediante redes neuronales convolucionales con aprendizaje por transferencia."

**Justificación:** Un objetivo general debe ser comprehensivo pero específico. Debe indicar QUÉ se va a hacer, CÓMO se va a hacer, y PARA QUÉ.

---

### 2. Objetivo específico sobre revisión del estado del arte
**Contenido mejorado:** Se especificó que la revisión debe identificar "arquitecturas preentrenadas más efectivas, técnicas de preprocesamiento y métricas de evaluación estándar en el dominio".

**Justificación:** Un objetivo de revisión bibliográfica debe especificar qué se busca obtener de esa revisión, no solo que se va a realizar.

---

### 3. Objetivo específico sobre recopilación de datos
**Contenido nuevo:** "Recopilar y consolidar conjuntos de datos de imágenes de fondo de ojo etiquetadas, integrando datasets públicos (Kaggle, MESSIDOR-2, IDRiD) y privados (FOSCAL), alcanzando un mínimo de 35,000 imágenes para entrenamiento y 3 datasets externos para validación."

**Justificación:** Especifica CUÁNTAS imágenes, de DÓNDE provienen, y PARA QUÉ se usarán (entrenamiento vs validación). Es medible y verificable.

---

### 4. Objetivo específico sobre preprocesamiento
**Contenido nuevo:** "Implementar y evaluar técnicas de preprocesamiento de imágenes (normalización de color, enmascaramiento periférico, balanceo de clases) y aumento de datos para optimizar la calidad del conjunto de entrenamiento y mitigar el desbalance entre clases."

**Justificación:** El preprocesamiento es una parte fundamental del trabajo que merece un objetivo específico. Además, el desbalance de clases fue un problema importante abordado en el trabajo.

---

### 5. Objetivo específico sobre arquitecturas CNN
**Contenido nuevo:** "Implementar y comparar cuatro arquitecturas de redes neuronales convolucionales preentrenadas (MobileNetV2, ResNet50V2, InceptionV3, VGG19) mediante aprendizaje por transferencia, incorporando técnicas de regularización (Dropout, L2, GaussianNoise, Multi-Head Attention) para prevenir sobreajuste."

**Justificación:** Especifica CUÁLES arquitecturas, CUÁNTAS, y QUÉ técnicas adicionales se usarán. Es el núcleo del trabajo experimental.

---

### 6. Objetivo específico sobre clasificación binaria
**Contenido nuevo:** "Desarrollar un clasificador binario optimizado para detección de presencia/ausencia de retinopatía diabética, alcanzando una sensibilidad mínima del 90% con optimización del umbral de decisión."

**Justificación:** La clasificación binaria y multiclase son objetivos separados con desafíos distintos. Cada uno merece su propio objetivo específico con meta medible.

---

### 7. Objetivo específico sobre clasificación multiclase
**Contenido nuevo:** "Desarrollar un clasificador multiclase para gradación de severidad de retinopatía diabética en cinco niveles (0: sin RD, 1: leve, 2: moderada, 3: severa, 4: proliferativa), analizando el desempeño diferencial de los canales de color RGB procesados independientemente."

**Justificación:** Especifica los 5 niveles exactos y menciona la contribución original del análisis por canales de color.

---

### 8. Objetivo específico sobre análisis de canales de color
**Contenido nuevo:** "Analizar comparativamente el desempeño de los modelos al procesar imágenes RGB completas versus canales de color individuales (rojo, verde, azul), identificando el canal más efectivo para la detección de lesiones específicas de retinopatía diabética."

**Justificación:** Este es un aporte original del trabajo que debe estar explícitamente en los objetivos. Es medible comparando métricas de desempeño.

---

### 9. Objetivo específico sobre evaluación con métricas estándar
**Contenido nuevo:** "Evaluar el desempeño de los modelos desarrollados utilizando métricas clínicas estándar (sensibilidad, especificidad, precisión, F1-score, AUC-ROC) con intervalos de confianza bootstrap, asegurando rigor estadístico en la presentación de resultados."

**Justificación:** Las métricas de evaluación deben estar especificadas como objetivo. La mención de intervalos de confianza demuestra rigor estadístico.

---

### 10. Objetivo específico sobre validación externa
**Contenido nuevo:** "Validar la capacidad de generalización de los modelos mediante evaluación en datasets externos independientes (MESSIDOR-2, IDRiD, FOSCAL) con diferentes características de adquisición y distribución de clases."

**Justificación:** La validación externa es crítica para demostrar que el modelo no está sobreajustado al dataset de entrenamiento. Es un objetivo específico distinto de la evaluación interna.

---

### 11. Objetivo específico sobre comparación con estado del arte
**Contenido nuevo:** "Comparar el desempeño de los modelos desarrollados con trabajos previos reportados en la literatura, posicionando los resultados dentro del contexto del estado del arte en detección automatizada de retinopatía diabética."

**Justificación:** La comparación con trabajos previos es fundamental para validar la contribución del trabajo. Debe ser un objetivo explícito.

---

### 12. Numeración de objetivos específicos
**Contenido añadido:** Se numeraron los objetivos específicos (OE1, OE2, etc.) para facilitar referencias cruzadas en el documento.

**Justificación:** La numeración permite referenciar objetivos específicos desde otras secciones (metodología, resultados, conclusiones) de forma clara.

---

## RESUMEN DE CAMBIOS

**Total de correcciones:** 7 problemas estructurales y de contenido corregidos
**Total de mejoras:** 12 elementos añadidos para elevar la calidad y especificidad

**Cambios estructurales:**
- Objetivo general: De vago a específico y completo
- Objetivos específicos: De 4 genéricos a 8 específicos, medibles y alineados con el trabajo realizado

**Antes:** 1 objetivo general + 4 objetivos específicos vagos
**Después:** 1 objetivo general completo + 8 objetivos específicos SMART (Específicos, Medibles, Alcanzables, Relevantes)

**Extensión:** De ~80 palabras a ~350 palabras (aumento de ~340%)

**Impacto:** Los objetivos ahora:
1. Son medibles y verificables
2. Reflejan fielmente el trabajo realizado
3. Incluyen las contribuciones originales
4. Están alineados con la metodología y resultados
5. Permiten verificar el cumplimiento en las conclusiones

**Alineación con el trabajo:**
- ✅ OE1: Revisión bibliográfica (Capítulo 2)
- ✅ OE2: Recopilación de datos (Sección 4.1)
- ✅ OE3: Preprocesamiento (Sección 4.2)
- ✅ OE4: Implementación de CNNs (Sección 4.3)
- ✅ OE5: Clasificador binario (Sección 6.1)
- ✅ OE6: Clasificador multiclase (Sección 6.2)
- ✅ OE7: Análisis de canales (Sección 6.2, Tablas)
- ✅ OE8: Evaluación con métricas (Sección 4.4, Capítulo 6)
- ✅ OE9: Validación externa (Sección 6.1.4)
- ✅ OE10: Comparación con estado del arte (Sección 6.1.5, Discusión)
