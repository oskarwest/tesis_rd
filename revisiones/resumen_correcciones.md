# CORRECCIONES Y MEJORAS AL RESUMEN

## CORRECCIONES

### 1. Errores de precisión en los resultados
**Problema:** El resumen original menciona "el mejor modelo para la clasificación multiclase es 62.8%" sin especificar qué métrica es ese valor.

**Corrección:** Según los resultados experimentales (Tabla en resultados.tex), el mejor modelo multiclase (MobileNetV2 con canal verde) alcanzó una sensibilidad de 65%, exactitud de 55%, y F1-score de 54%. Se corrigió para reflejar exactitud de 55% y se añadió la sensibilidad de 65%.

**Justificación:** La precisión en los resultados es fundamental en un resumen científico. Los lectores deben poder verificar las cifras exactas reportadas.

---

### 2. Inconsistencia gramatical
**Problema:** "Este trabajo propone dos modelos basados en redes neuronales convolucionales (CNN) que, ayuden a detectar la enfermedad y permita clasificar"

**Corrección:** Se eliminó la coma incorrecta y se corrigió la concordancia: "Este trabajo desarrolla modelos basados en redes neuronales convolucionales (CNN) para detectar la enfermedad y clasificar"

**Justificación:** Error gramatical que afecta la legibilidad profesional del documento.

---

### 3. Imprecisión en la descripción del dataset
**Problema:** Solo menciona "dataset de Kaggle" sin especificar el tamaño ni las fuentes de validación.

**Corrección:** Se especificó "35,121 imágenes del dataset público de Kaggle" y se agregaron los datasets de validación externa (MESSIDOR-2, IDRiD y FOSCAL).

**Justificación:** El tamaño del dataset es información crítica para evaluar la robustez del estudio. La validación externa es un elemento de calidad que debe destacarse.

---

### 4. Falta de especificación de arquitecturas
**Problema:** Dice "redes preentrenadas" sin especificar cuáles.

**Corrección:** Se añadió explícitamente: "MobileNetV2, ResNet50V2, InceptionV3 y VGG19"

**Justificación:** Las arquitecturas específicas son información relevante que permite reproducibilidad y comparación con otros trabajos.

---

### 5. Ambigüedad en "dos modelos"
**Problema:** "Este trabajo propone dos modelos" sugiere solo dos modelos cuando en realidad se evaluaron múltiples configuraciones.

**Corrección:** Se reescribió como "desarrolla modelos" y se aclaró que se implementaron "clasificadores binarios y multiclase".

**Justificación:** Mayor precisión en la descripción del alcance del trabajo.

---

### 6. Descripción incompleta del preprocesamiento
**Problema:** Solo menciona "técnicas de preprocesamiento" sin especificar cuáles.

**Corrección:** Se añadió: "normalización de color, enmascaramiento periférico, balanceo de clases mediante submuestreo y aumento de datos"

**Justificación:** Las técnicas de preprocesamiento son contribuciones metodológicas importantes del trabajo.

---

## MEJORAS AÑADIDAS

### 1. Motivación clínica con datos específicos de Colombia
**Contenido agregado:** "En Colombia, con una proporción de 1.56 oftalmólogos por cada 100,000 habitantes y aproximadamente 1.2 millones de personas con retinopatía diabética, la detección automatizada representa una solución crítica para ampliar la cobertura del tamizaje."

**Justificación:** Los resúmenes científicos en medicina deben contextualizar el problema con datos epidemiológicos específicos. Este dato está en la introducción y es relevante para justificar el trabajo.

---

### 2. Prevalencia global de la enfermedad
**Contenido agregado:** "afectando a 145 millones de personas a nivel mundial"

**Justificación:** Dimensionar el problema a nivel global es una práctica estándar en resúmenes de trabajos médicos. El dato está disponible en la introducción.

---

### 3. Especificación de arquitecturas y métodos
**Contenido agregado:** Mención explícita de las cuatro arquitecturas evaluadas y el uso de aprendizaje por transferencia.

**Justificación:** En trabajos de deep learning aplicado, especificar las arquitecturas exactas es estándar en resúmenes científicos.

---

### 4. Técnicas de regularización
**Contenido agregado:** "incorporando bloques Multi-Head Attention, capas GaussianNoise y técnicas de regularización (Dropout, L2, early stopping)"

**Justificación:** Las técnicas de regularización son contribuciones metodológicas específicas del trabajo que lo diferencian de implementaciones básicas.

---

### 5. Hallazgo sobre el canal verde
**Contenido agregado:** "identificando el canal verde como el más efectivo para la clasificación multiclase debido a su mejor contraste para lesiones hemorrágicas"

**Justificación:** Este es un hallazgo original y relevante del trabajo que debe destacarse en el resumen. Es una contribución específica al conocimiento del área.

---

### 6. Validación externa con resultados
**Contenido agregado:** "La validación externa en datasets MESSIDOR-2, IDRiD y FOSCAL confirmó la capacidad de generalización del modelo"

**Justificación:** La validación externa es un indicador de calidad metodológica fundamental en estudios de machine learning médico. Debe mencionarse explícitamente.

---

### 7. Métricas de evaluación completas
**Contenido agregado:** Especificación de que se usaron "sensibilidad, precisión, F1-score y AUC-ROC" como métricas.

**Justificación:** Enumerar las métricas específicas es estándar en resúmenes de trabajos de clasificación médica.

---

### 8. Mejor modelo específico
**Contenido agregado:** "siendo MobileNetV2 con preprocesamiento mediante filtrado y umbral optimizado (0.4826) el modelo de mejor desempeño"

**Justificación:** Identificar el modelo específico ganador y su configuración es información crítica para reproducibilidad y comparación.

---

### 9. Intervalos de confianza
**Contenido agregado:** "con intervalos de confianza bootstrap (IC95%: AUC-ROC 0.9636–0.9936)"

**Justificación:** Los intervalos de confianza demuestran rigor estadístico y son cada vez más requeridos en publicaciones científicas médicas.

---

### 10. Estructura y flujo mejorados
**Mejora general:** Se reorganizó el texto siguiendo la estructura típica de resúmenes científicos:
1. Contexto y problema (RD como causa de ceguera + datos epidemiológicos)
2. Limitaciones actuales (escasez de especialistas)
3. Objetivo del trabajo
4. Metodología (datasets, arquitecturas, técnicas)
5. Resultados principales (binario y multiclase)
6. Validación externa
7. Conclusión/Aportación

**Justificación:** Esta estructura facilita la lectura rápida y permite encontrar información específica de manera eficiente, siguiendo estándares de publicaciones científicas en el área.

---

## RESUMEN DE CAMBIOS

**Total de correcciones:** 6 errores/imprecisiones corregidos
**Total de mejoras:** 10 elementos añadidos para completar estándares científicos
**Extensión:** De 162 palabras a 221 palabras (aumento de ~36%, manteniéndose dentro del rango típico 200-250 palabras para resúmenes de TFG)

**Palabras clave:** No se modificaron (son adecuadas y completas)
