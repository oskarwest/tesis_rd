# CORRECCIONES Y MEJORAS A LA INTRODUCCIÓN

## CORRECCIONES

### 1. Error de sintaxis LaTeX
**Problema:** Línea 3: `\nnchapter{INTRODUCCIÓN}`

**Corrección:** `\chapter{INTRODUCCIÓN}`

**Justificación:** Error tipográfico que impide la correcta compilación del documento LaTeX. El comando correcto es `\chapter`.

---

### 2. Error de concordancia gramatical
**Problema:** Línea 58: "Este tipo de problemáticas requieren herramientas capaz de procesar"

**Corrección:** "Este tipo de problemáticas requiere herramientas capaces de procesar"

**Justificación:** "Tipo" es singular, por lo que requiere verbo singular. Además, "herramientas" es plural y requiere "capaces" en plural.

---

### 3. Espaciado inconsistente
**Problema:** Línea 58: "para este tipo de problemas ," (espacio antes de la coma)

**Corrección:** "para este tipo de problemas," (sin espacio antes de la coma)

**Justificación:** Las normas tipográficas del español requieren que no haya espacio antes de los signos de puntuación.

---

### 4. Espaciado en rangos numéricos
**Problema:** Línea 34: "65- 69 años"

**Corrección:** "65-69 años"

**Justificación:** Los rangos numéricos no llevan espacios alrededor del guion.

---

### 5. Redundancia innecesaria
**Problema:** Primer párrafo repite "(DM)" tres veces: "diabetes mellitus (DM)... diabetes mellitus (DM)... diabetes mellitus (DM)"

**Corrección:** Primera mención "diabetes mellitus (DM)", luego usar solo "DM" o "diabetes"

**Justificación:** Una vez definida la abreviatura, debe usarse consistentemente para evitar redundancia.

---

### 6. Falta de especificación de arquitecturas
**Problema:** Línea 63: "experimentación con diferentes configuraciones de redes neuronales" sin especificar cuáles

**Corrección:** Añadir "MobileNetV2, ResNet50V2, InceptionV3 y VGG19"

**Justificación:** La introducción debe dar contexto completo del trabajo. Las arquitecturas específicas son información relevante.

---

### 7. Mayúscula incorrecta
**Problema:** Línea 58: "investigaciones previas" después de punto

**Corrección:** "Investigaciones previas"

**Justificación:** Después de punto siempre va mayúscula.

---

### 8. Inconsistencia en números
**Problema:** Mezcla de números escritos en palabras y cifras sin criterio claro

**Corrección:** Aplicar regla estándar: números menores a 10 en palabras, mayores en cifras; excepto cuando son datos estadísticos específicos que siempre van en cifras

**Justificación:** Consistencia editorial y claridad en la presentación de datos científicos.

---

## MEJORAS AÑADIDAS

### 1. Estructura del primer párrafo mejorada
**Contenido modificado:** Se dividió el primer párrafo excesivamente largo en dos párrafos más digeribles, separando la definición de diabetes de la descripción de la retinopatía diabética.

**Justificación:** Párrafos más cortos mejoran la legibilidad y permiten mejor procesamiento de la información. Cada párrafo debe contener una idea principal.

---

### 2. Transición mejorada entre secciones estadísticas
**Contenido añadido:** Frases de transición entre las secciones de datos globales, latinoamericanos y colombianos.

**Justificación:** Las transiciones suaves mejoran el flujo narrativo y ayudan al lector a seguir la progresión de lo general a lo específico.

---

### 3. Contextualización de figuras mejorada
**Contenido modificado:** Mejorada la integración de las referencias a figuras en el texto narrativo, evitando interrupciones abruptas.

**Justificación:** Las figuras deben estar perfectamente integradas en el texto, no parecer agregadas posteriormente.

---

### 4. Párrafo de contribuciones específicas expandido
**Contenido añadido:** Se especificaron las cuatro arquitecturas CNN utilizadas (MobileNetV2, ResNet50V2, InceptionV3, VGG19) y se mencionó el hallazgo del canal verde.

**Justificación:** La introducción debe dar una visión completa del trabajo, incluyendo las herramientas específicas utilizadas y los hallazgos principales.

---

### 5. Mención de resultados principales
**Contenido añadido:** "Este trabajo logró una sensibilidad de 96.5% en clasificación binaria y 55% de exactitud en clasificación multiclase, demostrando la viabilidad de estas tecnologías para tamizaje automatizado."

**Justificación:** La introducción debe anticipar los resultados principales para dar contexto completo al lector sobre el alcance y éxito del trabajo.

---

### 6. Enlace explícito con la estructura del documento
**Contenido añadido:** Oración final que conecta con la estructura del resto del documento: "El presente documento se estructura de la siguiente manera: en el Capítulo 2 se presentan los fundamentos teóricos y el estado del arte; el Capítulo 3 detalla los objetivos; el Capítulo 4 describe la metodología implementada; los Capítulos 5 y 6 exponen la configuración experimental y los resultados obtenidos; y finalmente, los Capítulos 7, 8 y 9 presentan la discusión, conclusiones y trabajo futuro."

**Justificación:** Es una práctica estándar en tesis y TFG proporcionar al lector un mapa claro de la estructura del documento al final de la introducción.

---

### 7. Conexión explícita entre problema y solución
**Contenido mejorado:** Se reforzó el vínculo entre la escasez de oftalmólogos y la necesidad de soluciones automatizadas, haciendo más explícita la motivación del trabajo.

**Justificación:** La introducción debe establecer claramente el problema y por qué la solución propuesta es relevante.

---

### 8. Especificación de datasets utilizados
**Contenido añadido:** Mención explícita de los datasets: "utilizando 35,121 imágenes del dataset de Kaggle para entrenamiento y datasets externos (MESSIDOR-2, IDRiD, FOSCAL) para validación"

**Justificación:** Los datos son el fundamento del trabajo de machine learning; deben mencionarse en la introducción para dar contexto completo.

---

### 9. Aclaración del aporte original
**Contenido mejorado:** Se clarificó qué es aporte original vs. lo que ya existe en la literatura, particularmente el análisis por canales de color y la comparación de arquitecturas.

**Justificación:** Es fundamental que el lector entienda cuál es la contribución específica de este trabajo respecto al estado del arte.

---

### 10. Mejora en la redacción del párrafo sobre CNNs
**Contenido modificado:** Se dividió el párrafo extremadamente largo sobre soluciones digitales y CNNs en dos párrafos más manejables, uno sobre la evolución histórica y otro sobre la aplicación específica.

**Justificación:** Párrafos muy largos (más de 150 palabras) dificultan la comprensión. La división temática mejora la claridad.

---

### 11. Actualización de datos temporales
**Contenido añadido:** Se agregó nota sobre la vigencia de los datos: "Es importante notar que estos datos corresponden a 2016-2018 y la situación puede haber evolucionado."

**Justificación:** Transparencia sobre la vigencia de los datos epidemiológicos utilizados para contextualizar el trabajo.

---

### 12. Mejora en la conclusión de la introducción
**Contenido mejorado:** Se fortaleció el párrafo final para que sirva como puente efectivo hacia el resto del documento, enfatizando el impacto potencial y la estructura del trabajo.

**Justificación:** La conclusión de la introducción debe motivar la lectura del resto del documento y dar un sentido de cierre a esta sección inicial.

---

## RESUMEN DE CAMBIOS

**Total de correcciones:** 8 errores corregidos (tipográficos, gramaticales, de formato)
**Total de mejoras:** 12 elementos mejorados para elevar la calidad académica
**Cambios estructurales:** División de 3 párrafos excesivamente largos para mejorar legibilidad
**Adiciones de contenido:** ~200 palabras de contenido nuevo (mención de arquitecturas, resultados, estructura del documento)

**Extensión:** De ~1,050 palabras a ~1,250 palabras (aumento de ~19%, apropiado para una introducción de TFG)

**Impacto:** La introducción ahora proporciona una visión completa y autocontenida del trabajo, con mejor flujo narrativo y conexión clara entre problema, solución y resultados.
