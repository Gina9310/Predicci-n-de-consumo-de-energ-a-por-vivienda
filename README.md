
## 📂 Contenido del repositorio
- `código para el modelo` → Notebook principal con el análisis paso a paso.
- `Dataset con información de ENCEVI`.
- `README.md` → Documentación del proyecto.

## ⚙️ Requisitos

- Jupyter Notebook
- Librerías:
  - pandas
  - from sklearn

## HALLAZGOS:
- No existe información disponible acerca de la generación de RSU por Entidad.

- Existe una relación entre número de municipios de cada Estado con la cantidad de servicios de recolección, Estados con mayor número de municipios mayor número de servicios de recolección.

- Existe una relación entre la actividad economica y la cantidad promedio recolectada al día. Estados con mayor aportación al PIB presentan mayor cantidad de RSU recolectados. Los estados que más cantidad de RSU recolectan son la Ciudad de México, México, Jalisco, Nuevo León, Puebla, Veracruz, Guanajuato y coincide con los estados que más aportan al PIB, lo cual quiere decir que existe más una relación de la cantidad de recolección de RSU con las actividades economicas que con la densidad poblacional.

- No existe relación entre número de municipios y cantidad recolectada de RSU.

- En méxico más del 93% de los residuos van directo a disposición final.

- únicamente 11 Estados cuentancon estaciones de transferencia.

- 19 Estados cuentan con plantas de tratamiento de RSU.


# Predicción-de-consumo-de-energía-por-vivienda
ingresando número de focos, número de ocupantes, si se cuenta con aire acondicionado, refri etc se predice el consumo de energía de la vivienda

### Objetivo:

Crear un modelo que permita predicir el consumo de energía por vivienda (un hogar) considerando caracteristicas de la vivienda como: existencia de refrigerador, número de focos, número de tvs, número de habitantes entre otras.
### Conclusión 

Dentro del modelo la variable que más influye en el consumo eléctrico por vivienda es la existencia de aire acondicionado, suena lógico y poco influye si se tiene o no refrigerador.

El modelo parece no ser tan útil, pues presenta un error relativo de 67%. Se esplorará que otras caracteristicas pueden ser añadidas para entrenar al modelo y llegar a un eror relativo de 20%-30%.
