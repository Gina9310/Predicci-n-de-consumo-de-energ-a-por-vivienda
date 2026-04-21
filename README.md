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

### Objetivo:

Crear un modelo que permita predicir el consumo de energía por vivienda (un hogar) considerando caracteristicas de la vivienda como: existencia de refrigerador, número de focos, número de tvs, número de habitantes entre otras.
### Conclusión 

Dentro del modelo la variable que más influye en el consumo eléctrico por vivienda es la existencia de aire acondicionado, suena lógico y poco influye si se tiene o no refrigerador.

El modelo parece no ser tan útil, pues presenta un error relativo de 67%. Se esplorará que otras caracteristicas pueden ser añadidas para entrenar al modelo y llegar a un eror relativo de 20%-30%.
