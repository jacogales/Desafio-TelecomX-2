#  Predicción de Cancelación de Clientes — Telecom X

##  Descripción
Este proyecto utiliza técnicas de **Machine Learning** para predecir la cancelación de clientes (*Churn*) en una empresa de telecomunicaciones ficticia llamada **Telecom X**.  
A partir de datos históricos de clientes, se analizan los factores que más influyen en la decisión de cancelar el servicio y se construyen modelos para anticipar este comportamiento, permitiendo implementar estrategias de retención.

---

##  Objetivos
- Identificar los **factores clave** que influyen en la cancelación.
- Entrenar y evaluar modelos predictivos para detectar clientes en riesgo.
- Proponer **estrategias de retención** basadas en los hallazgos.
- Implementar un flujo reproducible para análisis y predicción.

 ##  Tecnologías utilizadas
- **Python 3.x**
- **Pandas** — Manipulación y análisis de datos.
- **Matplotlib / Seaborn** — Visualización de datos.
- **Scikit-learn** — Modelado y evaluación.
- **Imbalanced-learn** — Manejo de clases desbalanceadas (SMOTE).
- **Google Colab** — Entorno de desarrollo.

---

##  Flujo de trabajo
1. **Carga de datos** tratados (`datos_tratados.csv`).
2. **Eliminación de columnas irrelevantes** (e.g., `customerID`).
3. **Codificación One-Hot** de variables categóricas.
4. **Análisis exploratorio** (EDA) y visualizaciones.
5. **Balanceo de clases** usando **SMOTE**.
6. **Entrenamiento de modelos** (Árbol de Decisión, Random Forest).
7. **Evaluación de métricas**: Accuracy, Precision, Recall, F1-score.
8. **Análisis de importancia de variables**.
9. **Recomendaciones de negocio**.

---

##  Resultados principales
- **Mejor modelo**: Random Forest (Accuracy: 77%, Recall Churn=1: 62%).
- **Factores clave**:
  - Tenure bajo → Mayor riesgo de cancelación.
  - Contratos largos → Menor riesgo.
  - Cargos mensuales altos → Mayor riesgo.
  - InternetService_Fiber optic → Mayor riesgo.
  - Métodos de pago Electronic check → Mayor riesgo.

