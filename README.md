# House Prices Prediction  

**Pedro Ruiz - October 2023**  

## 📖 Descripción  

Este proyecto aborda el famoso desafío de predicción de precios de viviendas en Ames, Iowa, utilizando varios modelos de regresión. El objetivo principal es predecir los precios de venta de las casas basándose en múltiples características y atributos proporcionados en el conjunto de datos.  

A lo largo del proyecto, se exploraron y compararon diferentes enfoques de modelado, desde regresiones lineales básicas hasta técnicas avanzadas como Random Forest y Gradient Boosting.  

<div align="center">
    <img src="./house price prediction.jpg" alt="HousePrice" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
</div>

## 📂 Archivos del Proyecto  

- **`train.csv`**: Conjunto de datos de entrenamiento con las características y precios de las viviendas.  
- **`test.csv`**: Conjunto de datos de prueba sin los precios, utilizado para realizar predicciones.  
- **`data_description.txt`**: Descripción detallada de las características incluidas en el dataset.  
- **`sample_submission.csv`**: Ejemplo de un archivo de predicción de precios.  

## 🎯 Objetivos  

1. Preparar y limpiar los datos para garantizar una base sólida para el modelado.  
2. Analizar las relaciones entre las características y el precio de venta (`SalePrice`) utilizando estadísticas descriptivas y visualizaciones.  
3. Implementar y comparar diversos modelos de regresión:  
   - Regresión Lineal Simple y Múltiple  
   - Ridge y Lasso Regression  
   - KNeighborsRegressor  
   - ElasticNet  
   - GradientBoostingRegressor  
   - RandomForestRegressor  
   - GLM  
4. Evaluar los modelos mediante métricas como el **RMSE** y el **R²** para determinar su precisión.  

## 🛠 Tecnologías y Librerías Utilizadas  

- **Python**: Lenguaje principal para la implementación.  
- **Bibliotecas**:  
  - Manipulación de datos: `numpy`, `pandas`  
  - Visualización: `matplotlib`, `seaborn`, `folium`  
  - Modelado y evaluación: `scikit-learn`, `statsmodels`  

## 🔍 Análisis de Datos  

Se realizó un análisis exhaustivo de los datos, identificando y resolviendo valores nulos, transformando variables categóricas y analizando correlaciones. Las visualizaciones revelaron insights clave, como:  
- La influencia de variables como `OverallQual`, `GrLivArea` y `GarageCars` en los precios de venta.  
- Correlaciones positivas entre la calidad de los materiales y los precios.  
- Outliers significativos en características como `GrLivArea`.  

## 🧠 Modelos Implementados  

Los modelos evaluados incluyen:  

| Modelo                     | RMSE (Log)   | R²       |  
|----------------------------|--------------|----------|  
| RandomForestRegressor      | 0.1542       | 0.8924   |  
| GradientBoostingRegressor  | 0.1483       | 0.8873   |  
| Ridge Regression           | 0.1749       | 0.8493   |  
| GLM                        | 0.1871       | 0.8487   |  
| Multiple Linear Regression | 0.1867       | 0.8486   |  
| Lasso Regression           | 0.1835       | 0.8483   |  
| ElasticNet                 | 0.1603       | 0.8386   |  
| KNeighborsRegressor        | 0.2011       | 0.7835   |  
| Simple Linear Regression   | 48589.4471   | 0.6257   |  

### 🏆 Modelo Seleccionado  

Aunque **RandomForestRegressor** obtuvo el mejor R², se seleccionó **GradientBoostingRegressor** por su menor RMSE, indicando una mayor precisión en las predicciones.  

## 📊 Conclusiones  

1. **Preparación de datos:** Eliminar valores nulos y transformar variables categóricas mejoró la precisión de los modelos.  
2. **Modelado:** Los modelos avanzados como Gradient Boosting y Random Forest superaron significativamente a las regresiones lineales básicas.  
3. **Insights clave:** La calidad y el tamaño de las viviendas son factores determinantes en los precios de venta.  
4. **Mejoras futuras:** Implementar técnicas de deep learning o trabajar más en el feature engineering podría mejorar los resultados.  

## 🙏 Agradecimientos  

Gracias por dedicar tiempo a leer este notebook. Si te ha gustado, **no olvides dar un UPVOTE** 😉  

**¡Seguimos trabajando!**
