🚀 TelecomX2: Predicción de Cancelación de Clientes (Churn)

📌 Descripción del Proyecto
En este proyecto desarrollé un modelo de Machine Learning capaz de predecir qué clientes tienen mayor probabilidad de cancelar sus servicios (Churn) en una empresa de telecomunicaciones.
El objetivo principal es anticiparse a la pérdida de clientes, permitiendo a la empresa tomar decisiones estratégicas basadas en datos para mejorar la retención.


🎯 Problema de Negocio
La cancelación de clientes representa una pérdida directa de ingresos.
Identificar quiénes están en riesgo de abandonar permite:
    • Reducir el churn
    • Optimizar campañas de retención
    • Aumentar el valor del cliente a largo plazo (LTV)

🧠 Enfoque del Proyecto
Se desarrolló un pipeline completo de Data Science que incluye:
    • Limpieza y preparación de datos
    • Análisis exploratorio (EDA)
    • Feature Engineering
    • Balanceo de clases
    • Entrenamiento de modelos
    • Evaluación y selección del modelo óptimo

📊 Dataset
Se utilizó el dataset:
📁 datos_TelecomX_Fla.json
Contiene información sobre:
    • Datos demográficos
    • Servicios contratados
    • Facturación
    • Métodos de pago
    • Estado de cancelación (Churn)

⚙️ Tecnologías y Herramientas
    • Python 🐍
    • Pandas / NumPy
    • Scikit-learn
    • Imbalanced-learn (SMOTE)
    • Matplotlib / Seaborn
    • Jupyter Notebook / Google Colab

🤖 Modelos Implementados
Se evaluaron múltiples algoritmos de clasificación:
    • Regresión Logística
    • Árbol de Decisión
    • K-Nearest Neighbors (KNN)
    • Support Vector Machines (SVM)
    • Random Forest

📈 Evaluación de Modelos
Dado que el dataset está desbalanceado, se priorizaron métricas relevantes:
    • ✅ Recall (Sensibilidad) (clave para detectar clientes en riesgo)
    • Precision
    • F1-score
    • ROC AUC
    • Matriz de confusión
    • Curvas ROC y Precision-Recall

🏆 Modelo Seleccionado (Champion)
El modelo final fue seleccionado en base a su capacidad para:
    • Maximizar el recall
    • Detectar la mayor cantidad posible de clientes en riesgo
    • Mantener un buen equilibrio con otras métricas
📌 En problemas de churn, es más importante detectar clientes que se van que minimizar falsos positivos.

🔍 Insights Clave
🔺 Factores que aumentan el churn
    • Altos cargos mensuales
    • Facturación electrónica
    • Clientes con perfil digital
    • Menor antigüedad
🔻 Factores que reducen el churn
    • Mayor tiempo como cliente (tenure) 🔥
    • Contratos a largo plazo
    • Pagos automáticos
    • Servicios adicionales (soporte técnico, seguridad)

💼 Impacto de Negocio
Este modelo permite:
    • Identificar clientes en riesgo de cancelación
    • Diseñar campañas de retención personalizadas
    • Reducir pérdidas económicas
    • Mejorar la fidelización

💡 Recomendaciones Estratégicas
    • 🎯 Fidelizar clientes en los primeros meses
    • 💳 Incentivar pagos automáticos
    • 📉 Optimizar planes con altos costos
    • 🔒 Ofrecer servicios de valor agregado
    • 📊 Segmentar campañas según perfil del cliente

📦 Cómo usar el modelo
import joblib

modelo = joblib.load('churn_model.pkl')
prediccion = modelo.predict(nuevo_cliente)

🚀 Storytelling del Proyecto
Las empresas de telecomunicaciones enfrentan un problema constante: los clientes se van.
Pero… ¿y si pudiéramos predecirlo antes de que ocurra?
En este proyecto transformé datos en decisiones.
Analicé el comportamiento de miles de clientes, identifiqué patrones ocultos y construí un modelo capaz de anticipar el churn.
El resultado no es solo un modelo predictivo, sino una herramienta estratégica que permite actuar antes de perder al cliente.

📌 Próximos pasos
    • Implementación en producción (API / Dashboard)
    • Monitoreo del modelo
    • Actualización periódica con nuevos datos

👨‍💻 Autor
Proyecto desarrollado como parte de un desafío de Data Science aplicado a negocio.


