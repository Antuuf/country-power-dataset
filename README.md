# 🌍 Geopolitical and Military Power Analysis

Este proyecto realiza un análisis multidimensional de la geopolítica, economía y fuerza militar global utilizando un dataset completo de 192 países con datos que abarcan del 2023 al 2025.

El análisis principal se encuentra consolidado en el Jupyter Notebook interactivo [country_power_analysis.ipynb](country_power_analysis.ipynb).

---

## 📊 Estructura del Dataset

El conjunto de datos (`country_power_dataset.csv`) cuenta con **192 registros** y **68 columnas** que abarcan:
* **Datos Demográficos**: Población, densidad poblacional, tasa de urbanización, crecimiento de población y edad promedio.
* **Datos Geográficos**: Área terrestre, fronteras terrestres, elevación máxima y longitud de costas.
* **Indicadores Económicos**: PIB nominal, PIB PPA, PIB per cápita, tasas de inflación y desempleo, balanza comercial, reservas de divisas y porcentaje de deuda sobre el PIB.
* **Fuerza Militar**: Cantidad de tropas activas/reserva/paramilitares, conteo detallado de activos físicos (tanques, blindados, aviones de combate, helicópteros, barcos, submarinos), capacidad/ojivas nucleares y presupuesto de defensa (SIPRI y oficial).
* **Rankings de Referencia**: Rango e índice del Global Firepower (GFP) y el Military Power Index (2023-2025).

---

## 🛠️ Proyectos de Data Science Incluidos

El notebook principal desarrolla cuatro análisis con machine learning y visualización interactiva:

### 1. 🔍 Modelado Predictivo e Importancia de Variables (XAI)
Utiliza un modelo de regresión `RandomForestRegressor` para modelar y predecir el índice de poder militar global. A través de la importancia de características, revela cuáles de las 23 variables seleccionadas (demográficas, económicas o de armamento específico) ejercen mayor influencia sobre los rankings globales de poder.

### 2. 🌐 Clustering Geopolítico
Aplica algoritmos de aprendizaje no supervisado (`K-Means` y `PCA`) para agrupar automáticamente a los países del mundo según sus similitudes socio-militares reales, sin sesgos geopolíticos preestablecidos. Los resultados se grafican en un plano bidimensional dinámico e interactivo mediante `Plotly`.

### 3. 💸 Análisis de Eficiencia del Gasto en Defensa
Calcula un ratio de eficiencia de gasto militar para cada país. Mide el "retorno de poder militar obtenido por cada millón de dólares invertido" y detecta a los países que logran un alto rendimiento militar con presupuestos muy ajustados, destacando la frontera de rendimiento mundial.

### 4. ⚠️ Detección de Anomalías Geopolíticas
Implementa `IsolationForest` para detectar "Outliers" geopolíticos y macroeconómicos: países que poseen una relación totalmente atípica de su PIB y escala de desarrollo con respecto a su presupuesto y capacidad de defensa militar instalada.

---

## 🚀 Cómo Empezar

### Requisitos Previos

Asegúrate de tener instalado Python 3.10 o superior y las librerías necesarias. Puedes instalar las dependencias directamente con:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn plotly
```

### Ejecutar el Análisis

1. Clona el repositorio:
   ```bash
   git clone https://github.com/Antuuf/country-power-dataset.git
   cd country-power-dataset
   ```
2. Inicia tu entorno de Jupyter o abre la carpeta en Visual Studio Code.
3. Abre y ejecuta las celdas de [country_power_analysis.ipynb](country_power_analysis.ipynb).
