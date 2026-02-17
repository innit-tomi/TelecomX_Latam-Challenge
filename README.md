# TelecomX_Latam-Challenge


# 📊 Churn Analysis – Análisis de Evasión de Clientes

## 📌 Descripción del Proyecto

Este proyecto analiza el fenómeno de **evasión de clientes (Churn)** con el objetivo de identificar patrones y factores que influyen en la cancelación del servicio.

La evasión impacta directamente en:

- Ingresos recurrentes  
- Estabilidad financiera  
- Crecimiento sostenible  

Comprender qué perfiles presentan mayor probabilidad de abandono permite diseñar estrategias de retención basadas en datos.

---

# 🧹 1. Limpieza y Preparación de Datos

Durante la fase de preparación se realizaron los siguientes pasos:

- Importación del dataset  
- Verificación de registros duplicados (no se encontraron duplicados)  
- Identificación de valores faltantes en la variable **Cargos Totales** (11 registros)  
- Análisis de los registros con valores nulos (clientes con 0 meses de contrato)  
- Reemplazo de valores nulos por `0`  
- Normalización y estandarización de nombres de columnas  

**Resultado final:**  
El dataset quedó conformado por **7043 registros completos**, listo para el análisis exploratorio.

---

# 🔎 2. Análisis Exploratorio de Datos (EDA)

## 2.1 Distribución General de Abandono

| Estado        | Proporción |
|--------------|------------|
| No Abandona  | 73.46%     |
| Abandona     | 26.53%     |

Aproximadamente **1 de cada 4 clientes cancela el servicio**, lo que representa un nivel significativo de evasión.

---

## 2.2 Análisis de Variables Numéricas

### Meses de Contrato

- Promedio: **32 meses**
- Desviación estándar: ≈ 24.5
- Rango: 0 – 72 meses

**Insight:**  
Los clientes que abandonan se concentran principalmente en los primeros 20 meses, lo que indica mayor riesgo en etapas tempranas del ciclo de vida.

---

### Cargos Mensuales

- Promedio: **64.76**
- Rango: 18.25 – 118.75

**Insight:**  
Se observa mayor abandono en el rango de 70 a 110 unidades monetarias, lo que sugiere posible sensibilidad al precio en planes más costosos.

---

### Cargos Totales

- Promedio: **2279.73**
- Alta variabilidad

**Insight:**  
Los clientes que abandonan presentan menor gasto acumulado, lo que indica que cancelan antes de generar alto valor para la empresa.

---

## 2.3 Análisis por Variables Categóricas

### Género

La proporción de abandono es similar entre hombres y mujeres.

**Conclusión:**  
El género no es un factor determinante en la evasión.

---

### Tipo de Contrato

| Tipo de Contrato | Nivel de Retención |
|------------------|-------------------|
| Month-to-Month   | Baja (Mayor abandono) |
| One Year         | Alta |
| Two Year         | Muy Alta |

**Insight clave:**  
Los contratos mensuales presentan mayor riesgo de abandono.  
Los contratos de largo plazo generan mayor estabilidad y fidelización.

---

### Método de Pago

| Método de Pago    | Nivel de Retención |
|-------------------|-------------------|
| Bank Transfer     | Alta |
| Credit Card       | Alta |
| Mailed Check      | Alta |
| Electronic Check  | Baja (Mayor abandono) |

**Posibles interpretaciones:**

- Menor compromiso del cliente  
- Mayor sensibilidad al precio  
- Fricción en el proceso de pago  

---

# 📌 3. Conclusiones

- La evasión afecta al **26.53%** de los clientes.
- El mayor riesgo se encuentra en los primeros 20 meses.
- Los contratos mensuales presentan la tasa más alta de abandono.
- Los clientes con cargos mensuales elevados muestran mayor probabilidad de cancelar.
- El método de pago Electronic Check está asociado a mayor abandono.
- El género no influye significativamente.
- El abandono está más relacionado con comportamiento contractual y financiero que con variables demográficas básicas.

---

# 🚀 4. Recomendaciones Estratégicas

### 1. Incentivar contratos de largo plazo
Ofrecer descuentos o beneficios para migrar clientes de contrato mensual a contratos de 1 o 2 años.

### 2. Estrategia de retención temprana
Implementar campañas de seguimiento en los primeros 6 a 12 meses.

### 3. Revisión de planes de alto costo
Analizar la percepción de valor en planes entre 70 y 110 unidades monetarias.

### 4. Optimización del método Electronic Check
Evaluar fricciones en el proceso de pago e incentivar migración a tarjeta o transferencia.

### 5. Implementación de modelo predictivo
Desarrollar un modelo de Machine Learning para anticipar la probabilidad de abandono y aplicar estrategias preventivas.

---

# 🎯 Conclusión Final

La evasión no ocurre de manera aleatoria. Está fuertemente asociada a:

- Tipo de contrato  
- Antigüedad del cliente  
- Método de pago  

Con una estrategia enfocada en retención temprana, migración a contratos largos y optimización de planes y métodos de pago, la empresa puede reducir significativamente la pérdida de clientes.
