# CORRECCIONES Y MEJORAS A LA DISCUSIÓN

## CORRECCIONES

### 1. Referencias bibliográficas sin comando \cite{}
**Problema:** Líneas 7, 11, 17, 31, 35, 37, 39: Autores citados como texto plano (ej. "Gulshan et al.\ (2016)")

**Corrección:** Usar comando LaTeX `\cite{clave_referencia}` o `\citep{}` para todas las referencias bibliográficas

**Justificación:** Las referencias deben estar formalmente vinculadas a la bibliografía mediante comandos LaTeX para numeración automática y consistencia.

---

### 2. Subsecciones sin numeración
**Problema:** Todas las subsecciones usan `\subsection*{}` (sin numeración)

**Corrección:** Cambiar a `\subsection{}` para que se numeren automáticamente (ej. 4.1, 4.2, etc.)

**Justificación:** En una tesis académica, las subsecciones generalmente se numeran para facilitar referencias cruzadas y navegación.

---

### 3. Falta de labels en subsecciones
**Problema:** Ninguna subsección tiene `\label{}` para referencias cruzadas

**Corrección:** Añadir labels descriptivos a todas las subsecciones (ej. `\label{subsec:discusion-binario}`)

**Justificación:** Permite referencias cruzadas desde otros capítulos y dentro del mismo capítulo.

---

### 4. Ausencia de referencias a tablas y figuras previas
**Problema:** Se discuten resultados sin referenciar explícitamente las tablas/figuras del capítulo de Resultados

**Corrección:** Añadir referencias como "como se observa en la Tabla~\ref{tab:comparacion_redes}" o "según la Figura~\ref{fig:conf-matrix-original}"

**Justificación:** La discusión debe conectar explícitamente con los resultados presentados anteriormente.

---

### 5. Porcentajes inconsistentes en precisión decimal
**Problema:** Línea 7: "sensibilidad de 96.5\%" vs línea 15: "F1-score de 0.95 a 0.96"

**Corrección:** Estandarizar formato: porcentajes enteros o con 1 decimal para métricas principales

**Justificación:** Consistencia en la presentación de métricas a lo largo de todo el documento.

---

### 6. Falta de introducción del capítulo
**Problema:** El capítulo comienza directamente con discusión de resultados sin orientar sobre su estructura

**Corrección:** Añadir párrafo introductorio que establezca las secciones de la discusión y su propósito

**Justificación:** Los capítulos deben tener introducción que oriente al lector sobre la organización del contenido.

---

### 7. Párrafos excesivamente largos
**Problema:** Líneas 9, 27, 29: Párrafos de más de 10 líneas dificultan la lectura

**Corrección:** Dividir párrafos largos en unidades más pequeñas (4-7 líneas) con ideas cohesivas

**Justificación:** Mejora la legibilidad y permite al lector asimilar mejor cada idea.

---

### 8. Valores de intervalos de confianza sin unidades claras
**Problema:** Línea 51: "0.9510--1.0000" sin aclarar que son valores decimales de sensibilidad

**Corrección:** Especificar "sensibilidad: IC 95\% [0.951, 1.000]" o convertir a porcentajes

**Justificación:** Los intervalos de confianza deben presentarse con el formato estadístico estándar.

---

### 9. Formato de miles inconsistente
**Problema:** Línea 55: "100{,}000" usa separador LaTeX pero no es consistente con el resto del documento

**Corrección:** Usar `\num{100000}` con paquete siunitx o mantener "100,000" como número normal

**Justificación:** Consistencia en el formato de números a lo largo del documento.

---

### 10. Falta de conclusión del capítulo
**Problema:** El capítulo termina abruptamente sin párrafo de cierre

**Corrección:** Añadir subsección de conclusión que sintetice los puntos principales de la discusión

**Justificación:** Los capítulos deben tener cierre claro que consolide las ideas discutidas.

---

### 11. No hay transición al siguiente capítulo
**Problema:** El capítulo no menciona la conexión con el capítulo siguiente (Conclusiones)

**Corrección:** Añadir frase de transición al final que anticipe el capítulo de conclusiones

**Justificación:** La narrativa de la tesis debe ser fluida con transiciones claras entre capítulos.

---

### 12. Término ambiguo "filtrado"
**Problema:** Línea 14: "algoritmo de filtrado" puede confundirse con filtrado de datos en lugar de preprocesamiento de imágenes

**Corrección:** Especificar "algoritmo de preprocesamiento de Graham" o "filtrado de Ben Graham"

**Justificación:** Claridad terminológica para evitar ambigüedades.

---

## MEJORAS AÑADIDAS

### 1. Introducción del capítulo estructurada
**Contenido nuevo:** Párrafo inicial (~150 palabras) que establece:
- Propósito de la discusión: interpretar resultados en contexto científico
- Estructura del capítulo: análisis por modelo, preprocesamiento, validación, limitaciones, implicaciones
- Conexión con objetivos específicos OE5-OE10

**Justificación:** Orienta al lector sobre qué esperar en el capítulo y cómo se organiza la discusión.

---

### 2. Tabla comparativa ampliada con literatura
**Contenido añadido:** Tabla que compara el modelo propuesto con 6-8 trabajos previos en múltiples dimensiones:
- Año de publicación
- Arquitectura utilizada
- Tamaño del dataset
- Métricas de desempeño (Sensibilidad, Especificidad, AUC-ROC)
- Estrategia de validación (interna vs externa)
- Innovación principal

**Justificación:** Permite visualizar claramente cómo se posiciona este trabajo en el contexto del estado del arte.

---

### 3. Análisis de trade-off sensibilidad-especificidad
**Contenido añadido:** Subsección (~250 palabras) que discute explícitamente:
- El trade-off entre sensibilidad (maximizar detección) y especificidad (minimizar falsos positivos)
- Por qué en contexto de tamizaje se prioriza sensibilidad
- Implicaciones de falsos positivos vs falsos negativos en salud pública
- Análisis de la curva ROC y selección del punto de corte óptimo

**Justificación:** Este análisis es crítico en aplicaciones médicas donde los errores tienen costos diferentes.

---

### 4. Subsección de interpretabilidad y explicabilidad
**Contenido añadido:** Nueva subsección (~300 palabras) sobre:
- Importancia de la explicabilidad en IA médica
- Técnicas como Grad-CAM o mapas de activación para visualizar qué regiones influyen en la predicción
- Limitación del modelo actual como "caja negra"
- Necesidad de técnicas XAI (Explainable AI) para confianza clínica

**Justificación:** La explicabilidad es un requisito creciente en IA médica para aceptación clínica y regulatoria.

---

### 5. Análisis económico y de viabilidad
**Contenido añadido:** Subsección (~250 palabras) sobre:
- Costo estimado de implementación del modelo (hardware, software, mantenimiento)
- Costo de inferencia por imagen
- Comparación con costo de consulta oftalmológica tradicional
- Análisis costo-beneficio en programas de tamizaje masivo
- ROI (retorno de inversión) esperado para sistemas de salud

**Justificación:** Las decisiones de implementación clínica dependen fuertemente de viabilidad económica.

---

### 6. Subsección de aspectos regulatorios y éticos
**Contenido añadido:** Nueva subsección (~300 palabras) que discute:
- Regulación de dispositivos médicos basados en IA (FDA, EMA, INVIMA en Colombia)
- Necesidad de estudios clínicos prospectivos para aprobación regulatoria
- Consideraciones éticas: sesgo algorítmico, equidad, privacidad de datos
- Responsabilidad legal en caso de errores diagnósticos
- Consentimiento informado para uso de IA en diagnóstico

**Justificación:** Estos aspectos son fundamentales para traducir investigación a práctica clínica.

---

### 7. Análisis de tiempo de inferencia y escalabilidad
**Contenido añadido:** Párrafos (~200 palabras) que discuten:
- Tiempo de inferencia por imagen de cada arquitectura
- Viabilidad de procesamiento en tiempo real en clínicas
- Requisitos de hardware para implementación a escala
- Posibilidad de implementación en dispositivos móviles o edge computing
- Throughput esperado (imágenes procesadas por hora)

**Justificación:** La eficiencia computacional es crítica para viabilidad de implementación masiva.

---

### 8. Discusión sobre integración multimodal
**Contenido añadido:** Subsección (~200 palabras) sobre:
- Cómo el modelo de imágenes podría integrarse con otros datos clínicos (HbA1c, glucosa, años de diabetes)
- Potencial de modelos multimodales que combinen imágenes + datos tabulares
- Trabajos previos que han explorado esta integración
- Mejora esperada en desempeño con enfoque multimodal

**Justificación:** La medicina moderna integra múltiples fuentes de datos, no solo imágenes.

---

### 9. Análisis profundo de confusión multiclase
**Contenido mejorado:** Expandir la discusión sobre clasificación multiclase (~250 palabras adicionales):
- Análisis cuantitativo de la matriz de confusión: qué porcentaje de errores son entre clases adyacentes vs no adyacentes
- Discusión sobre si un error RD1→RD2 es menos grave clínicamente que RD1→RD4
- Propuesta de métricas alternativas como Cohen's kappa ponderado
- Comparación con variabilidad inter-observador reportada en literatura (oftalmólogos también difieren en ~15-20%)

**Justificación:** El bajo desempeño multiclase requiere análisis más profundo y contextualizado.

---

### 10. Subsección de lecciones aprendidas
**Contenido nuevo:** Subsección (~250 palabras) que reflexiona sobre:
- Decisiones metodológicas que funcionaron bien (ej. preprocesamiento de Graham)
- Decisiones que en retrospectiva podrían mejorarse (ej. estrategia de balanceo de clases)
- Desafíos inesperados encontrados durante el desarrollo
- Insights sobre transferibilidad de modelos entre datasets médicos
- Recomendaciones para futuros investigadores que aborden problemas similares

**Justificación:** Las lecciones aprendidas añaden valor a la investigación y ayudan a futuros trabajos.

---

### 11. Referencias cruzadas a resultados específicos
**Contenido mejorado:** Añadir en cada subsección referencias explícitas a tablas y figuras:
- "Como se observa en la Tabla~\ref{tab:comparacion_redes}..."
- "Las matrices de confusión (Figuras~\ref{fig:conf-matrix-original} y~\ref{fig:conf-matrix-filtrado}) revelan..."
- "Los resultados de validación externa (Tabla~\ref{tab:validacion_externa}) muestran..."

**Justificación:** Conecta la discusión con evidencia específica presentada en Resultados.

---

### 12. Conexión explícita con objetivos
**Contenido añadido:** Al inicio de subsecciones relevantes, mencionar qué objetivo se cumple:
- "Estos resultados cumplen el objetivo OE5 de desarrollar un clasificador binario..."
- "El análisis de canales RGB (OE7) reveló que..."
- "La validación externa (OE9) demostró..."

**Justificación:** Demuestra alineación entre objetivos planteados, resultados obtenidos y discusión.

---

### 13. Discusión sobre limitación de labels ruidosos
**Contenido añadido:** Párrafo (~150 palabras) que discute:
- El problema de labels ruidosos en datasets médicos
- Variabilidad inter-observador en gradación de RD (estudios reportan kappa ~0.5-0.7)
- Cómo esto establece un límite superior teórico al desempeño del modelo
- Propuestas para mitigar: múltiples anotadores, consulta con gold standard, learning from noisy labels

**Justificación:** Es una limitación fundamental que afecta toda la literatura y debe reconocerse.

---

### 14. Análisis de casos edge y manejo de incertidumbre
**Contenido añadido:** Subsección (~200 palabras) sobre:
- Cómo el modelo debería manejar imágenes de baja calidad (desenfocadas, mal iluminadas)
- Propuesta de un clasificador de calidad previo al modelo diagnóstico
- Uso de la salida softmax como medida de confianza
- Definición de umbrales de confianza para derivar a evaluación humana
- Porcentaje de casos que requerirían revisión manual con diferentes umbrales

**Justificación:** El manejo de incertidumbre es crítico para implementación clínica segura.

---

### 15. Validación clínica prospectiva necesaria
**Contenido añadido:** Subsección (~250 palabras) sobre:
- Diferencia entre validación retrospectiva (este estudio) y prospectiva
- Diseño de estudio clínico prospectivo necesario: criterios de inclusión/exclusión, tamaño muestral, gold standard
- Endpoints primarios y secundarios para evaluar utilidad clínica real
- Timeline estimado para completar validación clínica
- Necesidad de estudios multicéntricos para demostrar generalización

**Justificación:** Establece la brecha entre este TFG y un sistema listo para uso clínico.

---

### 16. Discusión sobre sesgo algorítmico
**Contenido añadido:** Párrafo (~200 palabras) que discute:
- Potencial sesgo del modelo hacia poblaciones representadas en el dataset de entrenamiento (Kaggle)
- Subrepresentación de ciertas etnias, edades, o condiciones comórbidas
- Necesidad de datasets más diversos y representativos
- Evaluación de equidad del modelo en subgrupos poblacionales
- Riesgo de amplificar disparidades en salud si se implementa sin validación equitativa

**Justificación:** La equidad en IA médica es un tema crítico de investigación actual.

---

### 17. Conclusión del capítulo y transición
**Contenido nuevo:** Subsección de conclusión (~200 palabras) que:
- Sintetiza los 5 hallazgos principales discutidos
- Reafirma la viabilidad del enfoque propuesto como herramienta de apoyo diagnóstico
- Reconoce limitaciones principales
- Anticipa el siguiente capítulo: "En el capítulo siguiente se presentan las conclusiones generales del trabajo y se delinean direcciones específicas para investigación futura que aborden las limitaciones identificadas."

**Justificación:** Cierre claro del capítulo con transición fluida al siguiente.

---

## RESUMEN DE CAMBIOS

**Total de correcciones:** 12 errores (referencias bibliográficas, numeración, formato, estructura)
**Total de mejoras:** 17 elementos añadidos para profundizar análisis y completitud

**Cambios estructurales principales:**
1. Introducción del capítulo (~150 palabras)
2. Renumeración de subsecciones (de \subsection* a \subsection)
3. Adición de 7 nuevas subsecciones temáticas
4. División de párrafos largos para mejor legibilidad
5. Adición de 1 tabla comparativa ampliada con literatura
6. Integración de referencias cruzadas a tablas/figuras de Resultados
7. Conclusión del capítulo con transición (~200 palabras)

**Extensión:** De ~3,500 palabras a ~6,200 palabras (aumento de ~77%)

**Contenido nuevo añadido:**
- Introducción del capítulo (~150 palabras)
- Tabla comparativa ampliada con 6-8 trabajos previos
- Subsección de trade-off sensibilidad-especificidad (~250 palabras)
- Subsección de interpretabilidad y XAI (~300 palabras)
- Subsección de análisis económico (~250 palabras)
- Subsección de aspectos regulatorios y éticos (~300 palabras)
- Análisis de tiempo de inferencia y escalabilidad (~200 palabras)
- Subsección de integración multimodal (~200 palabras)
- Análisis profundo de confusión multiclase (~250 palabras adicionales)
- Subsección de lecciones aprendidas (~250 palabras)
- Análisis de limitación de labels ruidosos (~150 palabras)
- Subsección de casos edge y manejo de incertidumbre (~200 palabras)
- Subsección de validación clínica prospectiva (~250 palabras)
- Discusión sobre sesgo algorítmico (~200 palabras)
- Referencias cruzadas a resultados específicos (distribuidas)
- Conexión explícita con objetivos OE1-OE10 (distribuidas)
- Conclusión del capítulo (~200 palabras)

**Impacto:**
- Discusión ahora contextualiza resultados en marco más amplio (económico, regulatorio, ético)
- Análisis crítico más profundo de limitaciones
- Conexiones explícitas con capítulo de Resultados mediante referencias cruzadas
- Reconocimiento de brecha entre investigación y aplicación clínica
- Consideración de aspectos prácticos de implementación
- Análisis de escalabilidad y viabilidad económica
- Discusión de interpretabilidad y explicabilidad (XAI)
- Reflexión sobre lecciones aprendidas
- Transición clara hacia Conclusiones

**Alineación con objetivos:**
- ✅ Discute cumplimiento de OE5 (clasificador binario: 96.5% sensibilidad)
- ✅ Analiza OE6 (clasificador multiclase: limitaciones identificadas)
- ✅ Contextualiza OE7 (hallazgo canal verde en marco fisiológico)
- ✅ Interpreta OE8 (significado clínico de métricas obtenidas)
- ✅ Evalúa OE9 (capacidad de generalización en validación externa)
- ✅ Contextualiza OE10 (comparación con literatura ampliada)

**Subsecciones:**
- Antes: 7 subsecciones (todas sin numerar)
- Después: 14 subsecciones (todas numeradas con labels)

**Tablas/Figuras nuevas:**
- 1 tabla comparativa ampliada con literatura (múltiples dimensiones)
- Referencias cruzadas a 8+ tablas/figuras del capítulo de Resultados

**Profundidad analítica:**
- Discusión técnica ✅
- Discusión clínica ✅
- Discusión económica ✅ (NUEVA)
- Discusión regulatoria ✅ (NUEVA)
- Discusión ética ✅ (NUEVA)
- Discusión de escalabilidad ✅ (NUEVA)
- Lecciones aprendidas ✅ (NUEVA)
