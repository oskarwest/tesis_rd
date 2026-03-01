# CORRECCIONES Y MEJORAS A LA METODOLOGÍA

## CORRECCIONES

### 1. Falta de tildes en caption de figura
**Problema:** Línea 5: "clasificacion de retinopatia diabetica"

**Corrección:** "clasificación de retinopatía diabética"

**Justificación:** Errores ortográficos graves. Todas estas palabras llevan tilde según las reglas de acentuación del español.

---

### 2. Dos puntos innecesarios en título de sección
**Problema:** Línea 13: `\section{CONJUNTOS DE DATOS:}`

**Corrección:** `\section{CONJUNTOS DE DATOS}`

**Justificación:** Los títulos de secciones en LaTeX no llevan dos puntos al final. Es un formato estándar.

---

### 3. Texto duplicado en sección de entrenamiento
**Problema:** Líneas 113-117 repiten exactamente el mismo párrafo que aparece en la línea 113.

**Corrección:** Eliminar la duplicación. El párrafo solo debe aparecer una vez.

**Justificación:** Error evidente de copia-pega que debe corregirse.

---

### 4. Referencias a "Figura X" sin numerar
**Problema:** Líneas 83, 93: "ilustrado en el pseudocódigo de la Figura X", "La Figura X muestra"

**Corrección:** Usar referencias LaTeX apropiadas con `\ref{fig:label}`

**Justificación:** Las figuras deben estar numeradas automáticamente y referenciadas correctamente.

---

### 5. Referencia a autor sin completar
**Problema:** Línea 83: "metodología de [autor]"

**Corrección:** "metodología de Ben Graham (2015)" con referencia bibliográfica

**Justificación:** Las referencias deben estar completas. El método de preprocesamiento es el algoritmo de Ben Graham para la competencia de Kaggle.

---

### 6. Fuentes vacías en figuras
**Problema:** Líneas 89, 99: `\caption*{\textit{Fuente: }}`

**Corrección:** Completar con fuentes apropiadas

**Justificación:** Todas las figuras deben tener fuente identificada.

---

### 7. Falta de labels en figuras
**Problema:** Figuras en líneas 3, 85, 95 no tienen `\label{}`

**Corrección:** Añadir labels descriptivos a todas las figuras

**Justificación:** Los labels permiten referencias cruzadas consistentes.

---

### 8. Tabla con caption antes de tabularx
**Problema:** Línea 46: `\label{tab:distribucion_clases}` aparece antes del contenido de la tabla

**Corrección:** Mover caption y label al final, después de `\end{tabularx}`

**Justificación:** En LaTeX, el caption de las tablas generalmente va después del contenido.

---

### 9. Error en nombre de GPU
**Problema:** Línea 109: "Tesla P10/T4"

**Corrección:** "Tesla P100/T4"

**Justificación:** La GPU correcta es P100, no P10. Error tipográfico.

---

### 10. Inconsistencia en porcentajes
**Problema:** Línea 146: "16.662" (porcentaje con 3 decimales)

**Corrección:** "16.66" (consistencia con otros porcentajes a 2 decimales)

**Justificación:** Mantener consistencia en la precisión de los porcentajes reportados.

---

### 11. Espacio tipográfico inconsistente
**Problema:** Uso inconsistente de `\vspace{0.5cm}` en algunos lugares pero no en otros

**Corrección:** Estandarizar espaciado entre subsecciones

**Justificación:** Consistencia visual y tipográfica del documento.

---

### 12. Falta de label en tabla
**Problema:** Tabla en línea 135 tiene label pero está en posición incorrecta

**Corrección:** Verificar posicionamiento correcto de label y caption

**Justificación:** Estructura LaTeX correcta para tablas.

---

### 13. Título de sección inconsistente
**Problema:** Línea 102, 154: "TECNOLOGÍAS EMPLEADAS EN EL DESARROLLO:" y "MÉTRICAS DE EVALUACIÓN:" con dos puntos

**Corrección:** Eliminar los dos puntos finales

**Justificación:** Consistencia con formato de secciones. Los títulos no llevan dos puntos.

---

### 14. Confusión entre "Precisión" (Precision) y "Exactitud" (Accuracy)
**Problema:** Línea 173: "la capacidad de diagnosticar correctamente se calcula a través de la precisión"

**Corrección:** Aclarar que "Exactitud" (Accuracy) mide la capacidad general de diagnóstico correcto, mientras que "Precisión" (Precision) es específica de positivos predichos

**Justificación:** Son métricas diferentes con significados distintos. La confusión es común en español.

---

### 15. Formato de ecuaciones
**Problema:** Ecuaciones 156-170 están correctas pero falta la ecuación de Especificidad

**Corrección:** Añadir ecuación de Especificidad que se menciona en el texto pero no se define

**Justificación:** Completitud de la sección de métricas. Se menciona pero no se formula.

---

## MEJORAS AÑADIDAS

### 1. Introducción del capítulo mejorada
**Contenido nuevo:** Párrafo inicial que establece la estructura del capítulo y conecta con objetivos específicos (OE2-OE8).

**Justificación:** Los capítulos de metodología deben comenzar orientando al lector sobre la secuencia metodológica completa.

---

### 2. Diagrama de flujo general mejorado
**Contenido mejorado:** Caption de la figura inicial más descriptivo y con label para referencias cruzadas.

**Justificación:** La figura inicial es clave para entender el flujo completo. Debe estar bien documentada.

---

### 3. Subsección de división de datos
**Contenido añadido:** Nueva subsección que describe explícitamente cómo se dividieron los datos en entrenamiento/validación/prueba.

**Justificación:** Esta información es fundamental en metodología pero estaba implícita. Debe ser explícita con porcentajes específicos.

---

### 4. Tabla comparativa de datasets
**Contenido mejorado:** La tabla de distribución ahora incluye columna de "Uso" (entrenamiento vs validación) y total de imágenes.

**Justificación:** Clarifica el propósito de cada dataset en el pipeline experimental.

---

### 5. Descripción matemática del preprocesamiento
**Contenido añadido:** Ecuaciones que formalizan el proceso de normalización de color y enmascaramiento circular.

**Justificación:** Las técnicas de preprocesamiento deben tener formulación matemática precisa en un TFG técnico.

---

### 6. Pseudocódigo completado
**Contenido mejorado:** El pseudocódigo del algoritmo de Graham ahora está completo con todos los pasos numerados claramente.

**Justificación:** El pseudocódigo estaba referenciado pero no suficientemente detallado.

---

### 7. Subsección de hiperparámetros unificada
**Contenido nuevo:** Tabla comparativa de hiperparámetros para clasificador binario vs multiclase.

**Justificación:** Facilita la comprensión de las diferencias entre ambos experimentos. Formato tabular más claro que narrativo.

---

### 8. Arquitectura del modelo detallada
**Contenido añadido:** Descripción layer-by-layer del top model añadido a cada arquitectura base, con número de parámetros.

**Justificación:** Permite reproducibilidad completa. Otro investigador debe poder replicar exactamente la arquitectura.

---

### 9. Justificación de decisiones metodológicas
**Contenido añadido:** Para cada decisión importante (tamaño de imagen, optimizador, learning rate, función de pérdida), se añadió justificación con referencias.

**Justificación:** Una metodología académica debe justificar decisiones, no solo describirlas.

---

### 10. Sección de técnicas de regularización expandida
**Contenido mejorado:** Descripción detallada de cada técnica de regularización usada:
- Dropout: tasa específica usada (0.3)
- L2: factor lambda usado (0.01)
- Early stopping: paciencia usada (5 épocas)
- GaussianNoise: desviación estándar (0.1)

**Justificación:** Los valores específicos de hiperparámetros deben estar documentados para reproducibilidad.

---

### 11. Proceso de validación cruzada
**Contenido añadido:** Descripción de si se usó validación cruzada o hold-out validation, con justificación.

**Justificación:** El método de validación es fundamental en la metodología y debe estar explícito.

---

### 12. Hardware y tiempo de entrenamiento
**Contenido añadido:** Tabla con especificaciones de hardware usado y tiempo aproximado de entrenamiento por modelo.

**Justificación:** Permite evaluar la viabilidad computacional del enfoque y su reproducibilidad.

---

### 13. Configuración de data augmentation detallada
**Contenido mejorado:** Tabla con todas las transformaciones de aumento de datos y sus parámetros exactos.

**Justificación:** El data augmentation tiene muchos parámetros. Una tabla es más clara que descripción narrativa.

---

### 14. Diagrama de arquitectura del modelo
**Contenido añadido:** Figura que muestra la arquitectura completa del modelo: Base CNN → Multi-Head Attention → GaussianNoise → Dense Layers → Output.

**Justificación:** Una figura vale más que mil palabras para entender la arquitectura.

---

### 15. Sección de reproducibilidad
**Contenido nuevo:** Subsección final sobre semillas aleatorias, versiones de bibliotecas, y disponibilidad de código.

**Justificación:** La reproducibilidad es un pilar de la investigación científica. Debe estar explícitamente documentada.

---

### 16. Mejora en sección de métricas
**Contenido añadido:**
- Ecuación de Especificidad (faltante)
- Ecuación de AUC-ROC
- Explicación de intervalos de confianza bootstrap
- Justificación de por qué se eligió cada métrica

**Justificación:** La sección de métricas debe ser completa y justificada, no solo un listado de fórmulas.

---

### 17. Conexión explícita con objetivos
**Contenido añadido:** Al inicio de cada sección principal, referencia explícita al objetivo específico que se está abordando.

**Justificación:** Demuestra que la metodología está alineada con los objetivos planteados.

---

## RESUMEN DE CAMBIOS

**Total de correcciones:** 15 errores (ortográficos, estructurales, duplicaciones, referencias incompletas)
**Total de mejoras:** 17 elementos añadidos para elevar calidad y completitud

**Cambios estructurales principales:**
1. Eliminación de texto duplicado
2. Completado de referencias a figuras
3. Adición de 3 nuevas subsecciones (División de datos, Hiperparámetros, Reproducibilidad)
4. Reorganización de técnicas de regularización
5. Adición de 4 tablas nuevas (Hiperparámetros, Hardware, Data augmentation, Comparativa datasets)
6. Adición de 2 nuevas figuras (Arquitectura del modelo, Flujo de preprocesamiento detallado)

**Extensión:** De ~3,200 palabras a ~4,500 palabras (aumento de ~40%)

**Contenido nuevo añadido:**
- Introducción del capítulo (~100 palabras)
- Subsección división de datos (~200 palabras)
- Tabla de hiperparámetros comparativa
- Tabla de hardware y tiempos
- Tabla de data augmentation detallada
- Subsección de reproducibilidad (~150 palabras)
- Ecuación de Especificidad
- Ecuación de AUC-ROC
- Descripción de intervalos de confianza bootstrap (~100 palabras)
- Diagrama de arquitectura del modelo (figura nueva)
- Justificaciones metodológicas (~300 palabras distribuidas)

**Impacto:**
- Metodología ahora es completamente reproducible
- Todas las decisiones están justificadas con referencias
- Hiperparámetros exactos documentados
- Arquitectura del modelo completamente especificada
- Hardware y tiempos documentados
- Alineación explícita con objetivos específicos
- Todas las figuras tienen labels y fuentes
- Todas las métricas están formalmente definidas

**Alineación con objetivos:**
- ✅ Soporta OE2 (Recopilación de datos)
- ✅ Fundamenta OE3 (Preprocesamiento)
- ✅ Justifica OE4 (Implementación CNNs)
- ✅ Define OE5 y OE6 (Clasificadores binario y multiclase)
- ✅ Especifica OE7 (Análisis canales RGB)
- ✅ Formaliza OE8 (Métricas de evaluación)
