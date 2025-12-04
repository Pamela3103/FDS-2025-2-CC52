# Proyecto de Ciencia de Datos – Análisis de Compradores de Bicicletas

## Objetivo del Proyecto
El objetivo de este proyecto es analizar el comportamiento de los clientes de la empresa **Peru_Bike** para identificar las características que influyen en la compra de una bicicleta.  
Además, se desarrolla un **modelo de scoring** que permite estimar la probabilidad de compra de futuros clientes, apoyando la toma de decisiones comerciales mediante técnicas de Ciencia de Datos.

---

## Integrantes del Equipo
- **Pamela Ivonne Rivera Contreras - U202216662**
- **Sebastián Rodrigo Luna Centeno - U202224404**
- **Jesús Andrés Millones Espinoza - U20211b598**
- **Linda Libertad Leon Quispe - U202322089**

---

## Descripción del Dataset
El dataset utilizado, denominado **bike_buyers.csv**, contiene información de **1000 clientes** y múltiples atributos relacionados con su perfil demográfico, socioeconómico y estilo de vida.  
Incluye variables como:
- Ingresos
- Edad
- Número de hijos
- Número de vehículos
- Estado civil
- Nivel educativo
- Ocupación
- Distancia de transporte diario
- Si compró o no una bicicleta (*variable objetivo*)

Se adjunta el archivo del dataset y su diccionario de datos (PDF) dentro del repositorio.

---

## Tecnologías Utilizadas
- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
- Jupyter Notebook
- Git / GitHub

---

## Conclusiones
**A. Comprensión del negocio y los datos:**<br>

El análisis exploratorio permitió identificar patrones importantes en el comportamiento de los clientes, destacando que variables como edad, ingresos, estado civil, ocupación y cantidad de vehículos muestran relación con la compra de bicicletas.<br>

Se evidenció que los compradores tienden a presentar mayores ingresos y que ciertos perfiles demográficos concentran un mayor interés en la compra.<br>

**B. Preparación de los datos:**<br>

Se ejecutó un proceso sólido de limpieza, imputación, tratamiento de outliers mediante winsorización, codificación de variables categóricas y normalización.<br>

El dataset final quedó listo para ser utilizado en modelos de Machine Learning sin pérdida significativa de información ni sesgo introducido por valores atípicos o faltantes.<br>

**C. Modelado:**<br>

Se evaluaron tres tipos de modelos representando los tres paradigmas solicitados:<br>
- Regresión Logística (inductivo)<br>
- Árbol de Decisión (divide y vencerás)<br>
- Red Neuronal MLP (bioinspirado).<br>

Tras comparar los resultados, el modelo seleccionado fue la Regresión Logística, al mostrar el mejor desempeño en la métrica principal (ROC-AUC = 0.6958) y ofrecer la interpretabilidad necesaria para justificar decisiones de negocio.<br>

La validación cruzada evidenció buen comportamiento general y ausencia significativa de sobreajuste.<br>

**D. Scoring comercial:**<br>

Se generó la variable score_buy, que permite priorizar a los clientes según su probabilidad estimada de compra.<br>

El ranking permitió construir el archivo top50_prospects.csv, que ofrece a Peru_bike una herramienta directa para dirigir campañas personalizadas, focalizar recursos de marketing y mejorar el proceso de conversión.<br>


---

## Licencia
Este proyecto está disponible bajo la licencia **MIT**, que permite el uso, copia, modificación y distribución del código sin restricciones, siempre que se incluya la declaración de copyright correspondiente.

---
