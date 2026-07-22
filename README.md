# sql-data-warehouse-project
Construcción de un almacén de datos moderno con SQL Server, incluyendo procesos ETL, modelado de datos y análisis de datos.

## Arquitectura de datos

La arquitectura de datos de este proyecto sigue las capas
**Bronze** (Bronce)
**Silver** (Plata) 
**Gold** (Oro) de la arquitectura Medallion.
1. **Capa Bronze**: Almacena datos sin procesar (*raw data*) tal como provienen de los sistemas de origen. Los datos se ingieren desde archivos CSV a una base de datos SQL Server.
2. **Capa Silver**: Esta capa incluye procesos de limpieza, estandarización y normalización para preparar los datos para su análisis.
3. **Capa Gold**: Contiene datos listos para el negocio, modelados en un esquema de estrella (*star schema*) necesario para la generación de informes y el análisis.

## Requisitos del proyecto

### Construcción del almacén de datos (Ingeniería de datos)

#### Objetivo

Desarrollar un almacén de datos moderno utilizando SQL Server para consolidar información de ventas, facilitando la generación de informes analíticos y la toma de decisiones fundamentadas.

#### Especificaciones
- **Fuente de datos**: Importar datos de dos sistemas de origen (ERP y CRM) suministrados en formato CSV.
- **Calidad de los datos**: Depurar y resolver problemas de calidad de los datos antes del análisis.
- **Integración**: Combinar ambas fuentes en un modelo de datos único e intuitivo, diseñado para consultas analíticas.
- **Alcance**: Centrarse únicamente en el conjunto de datos más reciente; no se requiere la historización de los datos.
- **Documentación**: Proporcionar documentación clara del modelo de datos para apoyar tanto a las partes interesadas del negocio como a los equipos de análisis

### BI: Análisis y generación de informes (Análisis de datos)
#### Objetivo
Desarrollar análisis basados ​​en SQL para obtener información detallada sobre:
- **Comportamiento del cliente**
- **Rendimiento del producto**
- **Tendencias de ventas**

Esta información proporciona a las partes interesadas métricas empresariales clave, facilitando la toma de decisiones estratégicas.
