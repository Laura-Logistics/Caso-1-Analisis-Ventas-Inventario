# Caso 1 – Análisis de Ventas e Inventario
Proyecto aplicado a Logística, Operaciones y Análisis de Datos

## 🎯 Objetivo del Caso

Simular un escenario real de análisis en un entorno de e-commerce, donde se requiere:

- Depurar información operativa con inconsistencias

- Controlar la calidad de datos comerciales

- Analizar desempeño de ventas e inventario

- Generar insights útiles para toma de decisiones

Este ejercicio refleja funciones propias de roles como:

- Analista de Logística / Inventarios

- Analista de Operaciones

- Analista de Abastecimiento

- Analista de Información Junior

- Analista de Datos / E-commerce

## 🗂 Contexto del Problema

Se trabajó con una base de datos con errores intencionales que simulaban problemas comunes en entornos reales:

- Estados de pedidos inconsistentes

- Fechas mal formateadas

- Proveedores sin identificar

- Cantidades nulas

- Registros incompletos

- Precios unitarios en 0

En entornos logísticos y operativos, este tipo de errores impacta directamente:

- Reportes financieros

- Planeación de inventarios

- Seguimiento de pedidos

- Evaluación de proveedores

## 📂 Archivos del Proyecto

### 🔹 Datos

- [Dataset original](data/ventas_inventario_dataset_original.csv)
- [Dataset limpio](data/ventas_inventario_limpieza_datos.csv)
- [Archivo de trabajo en Excel](data/ventas_inventario.xlsx)

### 🔹 Visualizaciones

#### Ingresos por Producto
![Ingresos por Producto](images/grafico_ingresos_producto.png) 

#### Ventas por Proveedor
![Ventas por Proveedor](images/grafico_proveedor.png)

#### Evolución de Ventas
![Evolución de Ventas](images/grafico_evolucion.png)
> NOTA: 1 Registro sin fecha fue excluido del analisis temporal para mantener coherencia cronologica.					

#### Distribución de Ventas por Región (%)
![Distribución de Ventas por Región (%)](images/Distribución_Ventas.png)

#### Tabla Dinámica Resumen
![Tabla Dinámica](images/tabla_dinamica_resumen.png)

## 🧹 Gestión y Control de Calidad de Datos

Se implementó un proceso estructurado de limpieza:

-  Normalización de proveedor, categoría y estado de pedido

- Validación y estandarización de fechas

- Creación de variable clave:

    - Ventas = Cantidad × Precio_Unit


- No se asumieron valores faltantes (criterio conservador de análisis)

- Proveedores vacíos clasificados como "Anónimo" solo para análisis

- Registro sin fecha identificado como "Sin Fecha" para mantener trazabilidad

- El dataset original se mantuvo intacto

## 🔎 Enfoque aplicado: control, trazabilidad y transparencia de información.

### 📊 Análisis Desarrollado

Se construyeron tablas dinámicas para evaluar:

- Desempeño de productos

- Rendimiento por proveedor

- Distribución de ventas por región

- Evolución temporal

- Estado operativo de pedidos

Para análisis de ingresos reales, se consideraron únicamente pedidos con estado "Entregado", separando resultados financieros de la operación en curso.

Este criterio refleja buenas prácticas en control de operaciones y análisis financiero.

### 📈 Hallazgos Clave

- Producto con mayor ingreso: **Mouse USB**

- Proveedor con mayor facturación: **Proveedor ABC**

- Región con mayor volumen de ventas: **Norte**

- Identificación de pedidos pendientes y cancelados que no impactan ingresos reales

- Detección de registro sin fecha (riesgo en reportes temporales)

### 🧠 Enfoque Analítico Aplicado

Este proyecto demuestra capacidad para:

✔ Identificar riesgos en calidad de datos
✔ Separar operación activa vs resultados consolidados
✔ Analizar desempeño comercial y logístico
✔ Evaluar proveedores
✔ Apoyar decisiones de abastecimiento
✔ Generar reportes claros para áreas ejecutivas

### 🛠 Herramientas Utilizadas

- Google Sheets

- Tablas dinámicas

- Validación y estructuración de datos

## 📌 Relevancia para Áreas Profesionales
### 🔹 Logística & Supply Chain

- Control de estados de pedido

- Evaluación de proveedores

- Análisis de rotación y desempeño por región

- Soporte a decisiones de abastecimiento

### 🔹 Operaciones & Planeación

- Análisis de información para toma de decisiones

- Seguimiento de desempeño operativo

- Identificación de inconsistencias en reportes

### 🔹 Datos & E-commerce

- Limpieza y estructuración de datasets

- Construcción de métricas comerciales

- Visualización ejecutiva de resultados

> Este es el primero de una serie de casos prácticos enfocados en análisis aplicado a Logística, Operaciones y Datos.




Este es el primero de una serie de casos prácticos enfocados en análisis aplicado a Logística, Operaciones y Datos.
Visualización ejecutiva de resultados
