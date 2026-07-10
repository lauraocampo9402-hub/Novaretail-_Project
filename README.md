# Novaretail-_Project
# 📊 Proyecto 7: Explorando drivers de comportamiento en NovaRetail+

## 📌 Descripción

Este proyecto tiene como objetivo identificar qué factores del comportamiento de los clientes están más fuertemente asociados con el **ingreso anual generado para la empresa**.

A través de un Análisis Exploratorio de Datos (EDA) y diferentes técnicas de correlación, se estudian las relaciones entre variables numéricas, binarias y categóricas para obtener evidencia que ayude a comprender el comportamiento de los clientes.

---

## 🎯 Objetivos

- Explorar la calidad y estructura de los datos.
- Analizar la distribución de las variables numéricas, binarias y categóricas.
- Identificar relaciones entre variables mediante técnicas estadísticas apropiadas.
- Interpretar los resultados desde una perspectiva de negocio sin asumir causalidad.

---

## 📁 Dataset

El conjunto de datos contiene **15.000 registros** y **12 variables**, entre ellas:

- `edad`
- `nivel_ingreso`
- `visitas_mes`
- `compras_mes`
- `gasto_publicidad_dirigida`
- `satisfaccion`
- `miembro_premium`
- `abandono`
- `tipo_dispositivo`
- `region`
- `ingreso_anual`

---

## 🔄 Etapas del análisis

### 1. Exploración inicial
- Revisión de la estructura del dataset.
- Verificación de tipos de datos.
- Identificación de variables numéricas, binarias y categóricas.

### 2. Análisis descriptivo
- Estadísticas descriptivas.
- Distribución de variables.
- Revisión de valores únicos y categorías.

### 3. Visualización de datos
- Histogramas.
- Boxplots.
- Heatmap de correlación.
- Scatterplots para relaciones relevantes.

### 4. Análisis de correlación
Se aplicó el método más adecuado según el tipo de variables:

- **Pearson** para relaciones lineales entre variables numéricas.
- **Spearman** para relaciones monotónicas entre variables numéricas.
- **Punto biserial** para variables binarias y numéricas.
- **V de Cramér** para variables categóricas.

### 5. Interpretación para el negocio
- Identificación de los principales hallazgos.
- Evidencia visual y numérica.
- Interpretación de resultados.
- Limitaciones del análisis.
- Posibles líneas de trabajo futuras.

---

## 📊 Principales hallazgos

- Se identificó una **correlación positiva muy fuerte** entre **`compras_mes`** e **`ingreso_anual`** (Pearson ≈ **0.97**), lo que indica que ambas variables presentan una asociación lineal de alta intensidad.

- Se observó una **correlación positiva moderada** entre **`visitas_mes`** e **`ingreso_anual`** (Spearman ≈ **0.32**), lo que sugiere que, en general, un mayor número de visitas mensuales tiende a asociarse con mayores ingresos anuales, aunque con una dispersión considerable.

- La relación entre **`abandono`** e **`ingreso_anual`**, evaluada mediante la correlación punto-biserial, fue prácticamente nula, por lo que no se observó una asociación lineal relevante entre ambas variables.

- La relación entre **`miembro_premium`** e **`ingreso_anual`**, evaluada mediante la correlación punto-biserial, fue positiva pero de **baja magnitud**, indicando una asociación débil.

- El análisis mediante **V de Cramér** mostró que las asociaciones entre **`abandono`** y las variables categóricas (`tipo_dispositivo`, `region` y `miembro_premium`) fueron **débiles o prácticamente inexistentes**. La mayor asociación se observó con `miembro_premium` (V ≈ **0.12**), aunque su intensidad continúa siendo baja.

- En todos los casos, los resultados describen **asociaciones estadísticas** y **no permiten establecer relaciones de causalidad**.

---

## 🛠️ Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy

---

## ▶️ Cómo ejecutar el proyecto

1. Clona este repositorio.

```bash
git clone https://github.com/lauraocampo9402-hub/Novaretail-_Project.git
```

2. Abre el notebook con:

- Jupyter Notebook
- Visual Studio Code
- Google Colab

3. Instala las dependencias necesarias:

```bash
pip install pandas numpy matplotlib seaborn scipy
```

4. Ejecuta las celdas en orden.

---

## 👩‍💻 Autor

**Laura Ocampo**

Proyecto desarrollado como parte del Bootcamp de Data Analytics de TripleTen.
