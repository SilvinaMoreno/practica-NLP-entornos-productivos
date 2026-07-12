# NLP en Entornos Productivos
## Análisis de Soporte al Cliente en Twitter

Implementación de un pipeline automático de Procesamiento de Lenguaje Natural (NLP) para el análisis de consultas de soporte al cliente utilizando datos reales de Twitter.

Proyecto académico realizado en el marco del curso **Data Science III – Procesamiento de Lenguaje Natural (NLP)**  
**Coderhouse**

**Año:** 2026

**Moreno, Silvina Danisa**  
📧 silvina.danisa.moreno@gmail.com  
🐙 GitHub: **SilvinaMoreno**

---

# Descripción

El objetivo de este proyecto es desarrollar un pipeline automático capaz de procesar grandes volúmenes de consultas provenientes de Twitter, aplicando técnicas de Procesamiento de Lenguaje Natural para obtener información útil desde una perspectiva de negocio.

A lo largo del proyecto se implementan tareas de limpieza de texto, análisis de sentimiento y clasificación de consultas, con el propósito de identificar clientes insatisfechos, organizar solicitudes por categoría y generar métricas que faciliten la toma de decisiones del área de soporte.

---

# Objetivos

- Procesar automáticamente grandes volúmenes de texto.
- Implementar un pipeline de limpieza de datos.
- Aplicar análisis de sentimiento sobre los tweets.
- Clasificar consultas en categorías simples.
- Generar métricas útiles para el negocio.
- Analizar el impacto de la automatización y la escalabilidad en un entorno productivo.

---

# Dataset

Se utilizó el dataset público **Customer Support on Twitter**, disponible en Kaggle.

Este conjunto de datos contiene conversaciones reales entre usuarios y empresas a través de Twitter, permitiendo simular escenarios de soporte técnico y atención al cliente.

---

# Pipeline implementado

El proyecto desarrolla un flujo automático compuesto por las siguientes etapas:

### 1. Carga del dataset

- Lectura del archivo CSV.
- Exploración inicial de la información.

### 2. Limpieza del texto

- Conversión a minúsculas.
- Eliminación de URLs.
- Eliminación de menciones.
- Eliminación de hashtags.
- Eliminación de caracteres especiales.
- Eliminación de espacios innecesarios.

### 3. Análisis de sentimiento

Se utiliza **TextBlob** para estimar la polaridad de cada tweet y clasificarlo como:

- Positivo
- Neutral
- Negativo

### 4. Clasificación automática

Las consultas se clasifican mediante reglas simples en categorías como:

- Soporte técnico
- Facturación
- Reclamos
- Otros

### 5. Métricas de negocio

Se calculan indicadores como:

- Cantidad total de consultas.
- Distribución de sentimientos.
- Distribución por categoría.
- Cantidad de consultas críticas.
- Porcentaje de reclamos.

---

# Tecnologías utilizadas

- Python
- Pandas
- NumPy
- TextBlob
- Matplotlib
- Google Colab

---

# Resultados

El pipeline permite automatizar tareas que normalmente requerirían intervención manual.

Los resultados obtenidos permiten:

- Detectar clientes con experiencias negativas.
- Clasificar automáticamente consultas.
- Obtener indicadores para el área de soporte.
- Priorizar reclamos críticos.
- Reducir tiempos de análisis.

---

# Escalabilidad

La arquitectura implementada puede procesar grandes cantidades de tweets de forma automática gracias a un pipeline secuencial de limpieza, análisis y clasificación.

No obstante, el uso de reglas y modelos basados en polaridad presenta limitaciones cuando aparecen ironías, sarcasmos o expresiones ambiguas.

En escenarios productivos se recomienda reemplazar estas técnicas por modelos basados en **Transformers**, capaces de comprender mejor el contexto y ofrecer resultados más robustos.

---

# Impacto en el negocio

Automatizar el procesamiento de consultas permite reducir considerablemente el tiempo necesario para analizar grandes volúmenes de mensajes.

Además, facilita la detección temprana de reclamos, mejora la asignación de casos al área correspondiente y proporciona indicadores que ayudan a medir la calidad del servicio ofrecido al cliente.

---

# Limitaciones

El análisis de sentimiento implementado mediante TextBlob constituye una aproximación sencilla basada en polaridad.

Asimismo, la clasificación por palabras clave puede no identificar correctamente consultas complejas o expresiones propias del lenguaje utilizado en redes sociales.

En implementaciones reales sería recomendable utilizar modelos de clasificación supervisada o arquitecturas basadas en Transformers para mejorar la precisión.

---

# Cómo ejecutar el proyecto

1. Clonar el repositorio.

```bash
git clone https://github.com/SilvinaMoreno/NOMBRE_DEL_REPOSITORIO.git
```

2. Instalar las dependencias.

```bash
pip install -r requirements.txt
```

3. Ejecutar el notebook en Google Colab o Jupyter Notebook.

---

# Conclusiones

El proyecto demuestra cómo un pipeline de NLP puede automatizar el procesamiento de consultas provenientes de redes sociales, facilitando el análisis de grandes volúmenes de información.

La incorporación de técnicas de limpieza, análisis de sentimiento y clasificación automática permite transformar datos no estructurados en información útil para el negocio.

Aunque la solución desarrollada cumple adecuadamente los objetivos de la práctica, en un entorno productivo sería conveniente incorporar modelos basados en Transformers, capaces de ofrecer mayor precisión, escalabilidad y comprensión del contexto.

---

# Autor

**Silvina Danisa Moreno**

📧 silvina.danisa.moreno@gmail.com

🐙 GitHub: https://github.com/SilvinaMoreno

**Curso:** Data Science III – Procesamiento de Lenguaje Natural

**Año:** 2026
