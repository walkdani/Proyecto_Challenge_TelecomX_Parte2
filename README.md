# 📊 Análisis Predictivo de Cancelación de Clientes (Churn) - Telecom X

Este repositorio contiene el desarrollo completo de un proyecto de análisis y modelado predictivo para identificar los factores que influyen en la cancelación de clientes (churn) en la empresa ficticia **Telecom X**.

## 🔍 Objetivo

El objetivo principal de este proyecto es identificar patrones y variables clave que afectan la cancelación de clientes, con el fin de ayudar a la empresa a implementar estrategias de retención más efectivas y prevenir la pérdida de usuarios.

---

## 🧱 Estructura del Proyecto

### 1. **Preparación de los Datos**
- Normalización de archivos JSON para dividir la información en múltiples DataFrames.
- Limpieza de valores nulos, transformación de variables categóricas y numéricas.
- Generación de nuevas variables útiles, como el gasto diario (`cuentas_diarias`).
- Consolidación final en un único DataFrame para facilitar el análisis.

### 2. **Análisis Exploratorio (EDA)**
- Evaluación del churn por categorías como contrato, método de pago, seniority, etc.
- Visualización y análisis de variables numéricas como:
  - `Charges.Total` (Gasto total)
  - `Tenure` (Tiempo como cliente)
- Identificación de correlaciones importantes y patrones de comportamiento.

### 3. **Modelado Predictivo**
Se entrenaron tres modelos para predecir la cancelación de clientes:
- **Dummy Classifier:** Usado como línea base (accuracy: 0.50).
- **Decision Tree Classifier:** Árbol de decisión básico (accuracy: 0.80).
- **Random Forest Classifier:** Mejor desempeño general (accuracy: 0.86).

### 4. **Análisis de Variables Relevantes**
Se utilizó la importancia de variables (feature importance) en los modelos para identificar los factores más influyentes en el churn, confirmando hallazgos del análisis exploratorio:
- Tipo de contrato (`Contract_Month-to-month`)
- Tiempo como cliente (`tenure`)
- Método de pago (`Electronic check`)
- Tipo de servicio de internet
- Servicios adicionales como `TechSupport` y `OnlineSecurity`

### 5. **Estrategias de Retención Propuestas**
Basado en los resultados, se plantearon acciones para reducir el churn:
- Fortalecer el onboarding de nuevos clientes
- Promover contratos a largo plazo
- Incentivar métodos de pago más estables
- Detectar y actuar sobre clientes de bajo compromiso

---

## 🧠 Conclusión

El proyecto combina análisis estadístico, machine learning e interpretación de resultados para entregar una solución aplicable a problemas reales de retención de clientes. El uso de modelos como Random Forest permite no solo predecir cancelaciones, sino también entender qué variables influyen más en esa decisión.

---

## ⚙️ Tecnologías Utilizadas

- Python 3.10
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 📬 Contacto

Desarrollado por **Francisco Javier Alvarado Márquez**  
Si tienes preguntas o sugerencias, puedes abrir un *issue* o contactarme directamente.

---

