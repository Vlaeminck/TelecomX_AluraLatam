# TelecomX_AluraLatam

# 📊 Análisis de Evasión de Clientes (Churn) - TelecomX

## 📝 **Descripción del Proyecto**
Este proyecto tiene como objetivo **analizar la evasión de clientes (Churn)** en la empresa de telecomunicaciones **TelecomX**, identificando patrones que expliquen **por qué los clientes cancelan el servicio**.  

El análisis proporciona **insights estratégicos** para reducir la evasión, mejorar la retención de clientes y optimizar los ingresos.

---

## 🎯 **Objetivos**
1. **Medir la proporción de evasión (Churn)** en la base de clientes.  
2. **Explorar factores categóricos y numéricos asociados a la cancelación**, como:
   - Tipo de contrato
   - Método de pago
   - Tiempo de permanencia
   - Facturación mensual y total
3. **Detectar segmentos de clientes en riesgo** para diseñar estrategias de retención.

---

## 🛠 **Metodología**
El análisis se realizó en **Python** con **Pandas, Seaborn y Matplotlib** e incluyó las siguientes etapas:

### ✅ 1. **Limpieza y Tratamiento de Datos**
- **Importación y normalización:** Se aplanó el archivo `TelecomX_Data.json` (datos anidados).  
- **Tratamiento de valores nulos y duplicados.**  
- **Conversión de tipos y estandarización:**  
  - Variables textuales (Sí/No → 1/0).  
  - Unificación de categorías (`"No internet service"` → `"No"`).  
- **Creación de nuevas variables:**  
  - **`Cuenta_Diaria`** = `Factura_Mensual / 30` para análisis más granular.

### ✅ 2. **Análisis Exploratorio de Datos (EDA)**
Incluyó visualizaciones y estadísticas descriptivas:

#### 🔹 **Distribución de Churn**
- **27% de los clientes cancelaron** (Evasión = 1) y **73% permanecen**.

#### 🔹 **Variables Categóricas vs Churn**
- Contrato mensual y método de pago con *Electronic Check* → **mayor riesgo de cancelación**.

#### 🔹 **Variables Numéricas vs Churn**
- Clientes con **baja permanencia (<12 meses)** y **alta facturación mensual** presentan mayor tendencia a cancelar.

---

## 📈 **Principales Visualizaciones**
- ✅ **Gráficos de barras y pastel**: Distribución general de Churn.  
- ✅ **Gráficos de barras (por categoría)**: Contrato, método de pago, género.  
- ✅ **Boxplots y violin plots**: Comparación de facturación y tiempo de contrato entre churners y no churners.

*(Todos los gráficos están diseñados en estilo amigable para stakeholders, con colores corporativos y etiquetas claras).*

---

## 🔍 **Conclusiones e Insights**
1. **Contratos mensuales y pagos manuales (Electronic Check)** son el principal segmento de riesgo.  
2. **Clientes de corta antigüedad** cancelan más rápido → se deben reforzar acciones en los primeros meses.  
3. **Sensibilidad al precio**: Los clientes con facturas más altas muestran mayor tendencia a darse de baja.

---

## 💡 **Recomendaciones Estratégicas**
✔ **Incentivar contratos anuales** con descuentos y beneficios.  
✔ **Promover métodos de pago automáticos** con bonificaciones.  
✔ **Campañas de retención temprana**: Soporte especial en los primeros 6 meses.  
✔ **Revisar planes de alto costo**: Ofrecer paquetes personalizados o descuentos.  
✔ **Desarrollar un modelo predictivo de Churn** para identificar clientes en riesgo antes de que cancelen.

---

## 🚀 **Próximos Pasos**
✅ Construir un **modelo de Machine Learning (Random Forest o Regresión Logística)** para predecir Churn.  
✅ Implementar un **dashboard en tiempo real** (Looker Studio / Power BI) para monitorear métricas clave.

---

## 🖥 **Tecnologías Utilizadas**
- **Python 3.10+**
- **Pandas, Numpy** (procesamiento de datos)
- **Seaborn, Matplotlib** (visualización)
