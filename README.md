# Predicción-de-consumo-de-energía-por-vivienda
ingresando número de focos, número de ocupantes, si se cuenta con aire acondicionado, refri etc se predice el consumo de energía de la vivienda

## 📂 Contenido del repositorio
- `código para el modelo` → Notebook principal con el análisis paso a paso.
- `Dataset con información de ENCEVI`.
- `README.md` → Documentación del proyecto.

## ⚙️ Requisitos

- Jupyter Notebook
- Librerías:
  - pandas
  - sklearn

## Objetivo

Construir un modelo que permita estimar el consumo eléctrico de un hogar en función de variables como:

Número de focos
Número de ocupantes
Presencia de aire acondicionado
Presencia de calefactor
Presencia de refrigerador
Número de televisores
Región geográfica

## Datos

Se utilizaron datos de ENCEVI, los cuales contienen información sobre:

Equipamiento energético del hogar: focos, tvs, aire acondicionado, calentador
Uso de electrodomésticos: refrigerador
Consumo de energía

La unidad de análisis utilizada fue vivienda, de acuerdor a los datos por vivienda sólo se registra un hogar.

## Preparación de datos

Se realizaron los siguientes pasos:


Agrupación de datos a nivel hogar (folioviv, foliohog)
Unión de diferentes módulos mediante merge
Conversión de variables categóricas a numéricas (ej. 1/2 → 1/0)
Creación de variables dummy para región
Eliminación de valores negativos y outliers (percentil 99)
Relleno de valores NaN con 0

## Variables utilizadas
Variables explicativas (X):
refrigerador (0/1)
ocupantes (numérica)
calefactor (0/1)
focos (numérica)
aire_acon (0/1)
num_tvs (numérica)
region_2, region_3 (dummies)
Variable objetivo (y):
consumo_electricidad

## Modelo utilizado

1. Regresión lineal
Modelo base para interpretar relaciones entre variables.

## Evaluación del modelo

Se utilizaron las siguientes métricas:

MAE (Mean Absolute Error)
Error relativo (MAE / promedio)
R² (coeficiente de determinación)
Resultados:
Consumo promedio: 468.4
MAE: 312.8
Error relativo: 67%
R²: 0.034

## Conclusión
Dentro del modelo la variable que más influye en el consumo eléctrico por vivienda es la existencia de aire acondicionado, suena lógico y poco influye si se tiene o no refrigerador.

El modelo parece no ser tan útil, pues presenta un error relativo de 67%. Se esplorará que otras caracteristicas pueden ser añadidas para entrenar al modelo y llegar a un eror relativo de 20%-30%.

## Trabajo futuro
Incorporar variables socioeconómicas

Incluir más electrodomésticos

Probar modelos más avanzados

