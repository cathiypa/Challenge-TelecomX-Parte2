# Telecom X - Análisis y Predicción de Cancelación de Clientes (Churn)

## 📌 Descripción del Proyecto
Este proyecto se centra en **analizar y predecir la cancelación de clientes** (Churn) en Telecom X.  
El objetivo es comprender los factores que llevan a la pérdida de clientes y construir **modelos predictivos** para anticipar cancelaciones, ayudando a la empresa a implementar estrategias de retención.

---

## 🧾 Objetivos
1. Importar, limpiar y preparar los datos de clientes.  
2. Realizar un **Análisis Exploratorio de Datos (EDA)** para identificar patrones y tendencias en la cancelación.  
3. Crear nuevas variables derivadas, como `Cuentas_Diarias`, para obtener insights más detallados.  
4. Desarrollar y evaluar modelos de Machine Learning:
   - **Regresión Logística** (requiere normalización).  
   - **Random Forest** (no requiere normalización).  
5. Analizar la **importancia de las variables** y generar recomendaciones estratégicas para reducir la evasión.

---

## 📂 Dataset
El dataset se encuentra en formato JSON y contiene información sobre:
- Datos demográficos de los clientes (edad, género, estado civil, dependientes, etc.)
- Tipo de servicios contratados (teléfono, internet, streaming, soporte técnico, etc.)
- Información de facturación (mensual y total)
- Estado de cancelación (`Churn`)

**Fuente:** [TelecomX_Data.json](https://github.com/ingridcristh/challenge2-data-science-LATAM/blob/main/TelecomX_Data.json)

---

## 🛠 Tecnologías Utilizadas
- **Python**: lenguaje principal para análisis y modelado.  
- **Pandas & NumPy**: manipulación y limpieza de datos.  
- **Matplotlib & Seaborn**: visualización de datos.  
- **Scikit-learn**: preprocesamiento, construcción y evaluación de modelos.  
- **Imbalanced-learn (SMOTE)**: balanceo de clases para evitar sesgo en modelos.  

---

## 🔍 Análisis Realizado
1. **Limpieza y transformación de datos**:
   - Eliminación de columnas no relevantes (IDs).  
   - Conversión de variables categóricas a numéricas (One-Hot Encoding).  
   - Balanceo de clases con SMOTE.  

2. **Análisis Exploratorio de Datos (EDA)**:
   - Distribución de `Churn` entre clientes.  
   - Correlación entre variables numéricas y Churn.  
   - Boxplots de tiempo de contrato y facturación según Churn.  

3. **Modelos de Machine Learning**:
   - **Regresión Logística**:
     - Sensible a escala, requiere normalización.  
     - Métricas: Accuracy, Precision, Recall, F1-score.  
   - **Random Forest**:
     - No sensible a escala.  
     - Métricas: Accuracy, Precision, Recall, F1-score.  

4. **Análisis de importancia de variables**:
   - Variables más influyentes: `customer_tenure`, `account_Charges.Total`, servicios contratados.  
   - Permite identificar clientes de alto riesgo para acciones de retención.

---

## 📊 Resultados y Conclusiones
- Clientes con **contratos cortos** y **altos cargos totales** presentan mayor riesgo de cancelación.  
- Servicios adicionales como **Streaming** y **Tech Support** impactan en la retención.  
- Los modelos predictivos permiten **identificar clientes de alto riesgo** y focalizar estrategias preventivas.

---

## 💡 Recomendaciones Estratégicas
1. Diseñar **promociones y beneficios** para clientes con contratos cortos.  
2. Revisar políticas de **facturación y cobros** para clientes con altos cargos.  
3. Implementar **seguimiento proactivo** para clientes con alto riesgo según los modelos predictivos.  
4. Optimizar servicios adicionales que influyen en la retención de clientes.


