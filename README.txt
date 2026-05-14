# Optimización de Pozos Petroleros para OilyGiant 🛢️📊

Este proyecto aplica **Ciencia de Datos** y **Modelado Predictivo** para maximizar el margen de beneficio en la apertura de 200 nuevos pozos petroleros para la compañía OilyGiant, minimizando el riesgo financiero mediante simulaciones estadísticas avanzadas.

---

## 🛠️ Objetivos del Proyecto
* **Modelado Predictivo:** Desarrollar un modelo de regresión lineal para estimar el volumen de reservas en tres regiones geológicas distintas.
* **Análisis Económico:** Calcular el umbral de rentabilidad por pozo frente a un presupuesto asignado de $100M USD.
* **Evaluación de Riesgo Avanzada:** Implementar la técnica de **Bootstrapping** para determinar la distribución de beneficios, intervalos de confianza del 95% y la probabilidad de pérdida para cada región.
* **Toma de Decisiones Estratégica:** Recomendar la región óptima para la inversión basada en el beneficio promedio más alto y un límite estricto de riesgo (< 2.5%).

---

## 🚀 Tecnologías y Habilidades Aplicadas
* **Lenguaje:** Python
* **Bibliotecas Clave:** `pandas`, `numpy`, `scikit-learn` (`LinearRegression`), `matplotlib`, `seaborn`
* **Conceptos Clave:** Regresión Lineal, Métricas de Evaluación (RMSE), Bootstrapping (1,000 muestras), Intervalos de Confianza, Análisis de Riesgo Financiero.
* **Buenas Prácticas:** Modularización mediante funciones para evitar duplicidad de código (DRY) y código limpio/legible.

---

## 📉 Parámetros del Negocio y Condiciones
* **Presupuesto total (200 pozos):** \$100,000,000 USD.
* **Ingreso por unidad de producto:** \$4,500 USD (1 unidad = 1,000 barriles).
* **Punto de equilibrio por pozo:** 111.1 unidades (~\$500,000 USD) para evitar pérdidas.
* **Metodología de exploración:** Evaluación de 500 puntos por región para seleccionar los mejores 200 basados en predicciones.
* **Restricción de Riesgo:** Solo se consideran regiones con un riesgo de pérdida menor al **2.5%**.

---

## 📂 Estructura del Repositorio
* `notebooks/` - Jupyter Notebook con el análisis completo paso a paso (EDA, Modelado, Simulación).
* `src/` - Funciones modulares para procesamiento de datos, entrenamiento y Bootstrapping.
* `datasets/` - Referencias a los datos de exploración geológica (`geo_data_0.csv`, `geo_data_1.csv`, `geo_data_2.csv`).

---

## 📊 Metodología e Impacto del Proyecto

### 1. Preparación de Datos y Modelado
* Análisis Exploratorio de Datos (EDA) para asegurar la integridad de las variables numéricas (`f0`, `f1`, `f2`) e identificación de registros únicos.
* División de datos (75:25) y entrenamiento de **Regresión Lineal** para cada una de las tres regiones.
* **Métricas Obtenidas:** Evaluación del volumen medio predicho frente al RMSE de cada modelo para comprender la precisión de la estimación.

### 2. Análisis del Umbral de Rentabilidad
* Determinación matemática del volumen mínimo necesario (111.1 unidades).
* Comparación del rendimiento medio natural de cada región frente a este umbral, justificando la necesidad de un modelo predictivo para seleccionar solo los pozos de alto valor.

### 3. Estrategia de Selección de Pozos y Cálculo de Ganancias
* Implementación de lógica para extraer los 200 pozos con mayores reservas predichas a partir de muestras aleatorias de 500 puntos.
* Cálculo del beneficio bruto y neto potencial por región.

### 4. Simulación Estadística (Bootstrapping)
* Ejecución de **1,000 iteraciones** de muestreo para modelar la distribución del beneficio real.
* Cálculo preciso del beneficio promedio esperado, el **intervalo de confianza del 95%** y cuantificación exacta del riesgo de pérdida (frecuencia de escenarios con beneficio neto negativo).

---

## 🏆 Conclusiones y Recomendación Profesional
El proyecto concluye con una recomendación de negocio explícita orientada a la mesa directiva de OilyGiant, seleccionando la región que cumple rigurosamente con la tolerancia al riesgo (< 2.5%) y ofrece el mayor retorno de inversión (ROI) estimado.

---

## 👥 Contacto
* **Nombre:** Susan Renee Girón Tena
* **Rol:** Ingeniera Industrial / Científica de Datos en Formación
* **LinkedIn:** www.linkedin.com/in/susan-giron-tena-7b03a1149gmail.com
* **Email:** reneegiront@gmail.com

