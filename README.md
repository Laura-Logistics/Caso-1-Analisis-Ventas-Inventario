# Caso 1 – Análisis de Ventas e Inventario
Proyecto aplicado a Logística, Operaciones y Análisis de Datos

---

## Índice

1. [Objetivo del Caso](#-objetivo-del-caso)
2. [Archivos del Proyecto](#-archivos-del-proyecto)
3. [Análisis Desarrollado](#-análisis-desarrollado)
6. [Hallazgos Clave](#-hallazgos-clave)
7. [Enfoque Analítico Aplicado](#-enfoque-analítico-aplicado)
8. [Relevancia Profesional](#-relevancia-para-áreas-profesionales)

---

## Objetivo del Caso

Simular análisis de ventas e inventario en un entorno de **Supply Chain / operaciones**, depurando datos y generando insights para la toma de decisiones.

## Archivos del proyecto

- 📊 [Dataset original](data/ventas_inventario_dataset_original.csv)
  
| ID_Venta | Fecha | Producto | Categoria | Proveedor | Región | Cantidad | Precio_Unit | Stock | Estado |				
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |				
| V001 | 05/01/2024 | Mouse USB | Perifericos | Proveedor ABC | norte | 10 | 15,5 | 50 | entregado |				
| V002 | 06-01-24 | Teclado | Perifericos | proveedor abc | Centro |  | 20 | 30 | Pendiente |				
| V003 | 2024/01/07 | Monitor 24" | Monitores | Proveedor XYZ | Sur | 2 | 0 | 20 | ENTREGADO |				
| V004 | 08/01/2024 | Laptop | Computo | Proveedor 123 | Norte | 1 | 850 | -5 | Cancelado |				
| V005 | 09/01/2024 | Mouse USB | Periféricos | Prov. ABC | Centro | 100 | 15,5 | 100 | entregado |				
| V006 |  | Mouse USB | Perifericos | Proveedor ABC | Norte | 1000 | 15,5 | 100 | Entregado |				
| V007 | 10/01/2024 | Tablet | Computo |  | Centro | 2 | 250 | 10 | Entregado |

- 📊 [Dataset limpio](data/ventas_inventario_limpieza_datos.csv)
  
| **ID_Venta** | **Fecha** | **Fecha_Analisis** | **Producto** | **Categoria** | **Proveedor** | **Proveedor_Normalizado** | **Región** | **Cantidad** | **Precio_Unit** | **Stock** | **Estado** | **Ventas** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| V001 | 5/01/2024 | 5/01/2024 | Mouse USB | Perifericos | Proveedor ABC | Proveedor ABC | Norte | 10 | 15,5 | 50 | Entregado | $155 |
| V002 | 6/01/2024 | 6/01/2024 | Teclado | Perifericos | Proveedor ABC | Proveedor ABC | Centro |  | 20,0 | 30 | Pendiente | $0 |
| V003 | 7/01/2024 | 7/01/2024 | Monitor 24" | Monitores | Proveedor XYZ | Proveedor XYZ | Sur | 2 | 0,0 | 20 | Entregado | $0 |
| V004 | 8/01/2024 | 8/01/2024 | Laptop | Computo | Proveedor 123 | Proveedor 123 | Norte | 1 | 850,0 | 5 | Cancelado | $850 |
| V005 | 9/01/2024 | 9/01/2024 | Mouse USB | Perifericos | Proveedor ABC | Proveedor ABC | Centro | 100 | 15,5 | 100 | Entregado | $1.550 |
| V006 |  | Sin Fecha | Mouse USB | Perifericos | Proveedor ABC | Proveedor ABC | Norte | 1000 | 15,5 | 100 | Entregado | $15.500 |
| V007 | 10/01/2024 | 10/01/2024 | Tablet | Computo |  | Anonimo | Centro | 2 | 250,0 | 10 | Entregado | $500 |

- 📊 [Archivo de trabajo en Google Sheets](data/ventas_inventario.xlsx)

## Visualizaciones

#### Ingresos por Producto
![Ingresos por Producto](images/grafico_ingresos_producto.png) 

#### Ventas por Proveedor
![Ventas por Proveedor](images/grafico_proveedor.png)

#### Evolución de Ventas
![Evolución de Ventas](images/grafico_evolucion.png)
> NOTA: 1 Registro sin fecha fue excluido del analisis temporal para mantener coherencia cronologica.					

#### Distribución de Ventas por Región (%)
![Distribución de Ventas por Región (%)](images/Distribución_Ventas.png)

## Gestión y limpieza de datos
- Normalización de proveedores, categorías y estado de pedidos
- Validación y estandarización de fechas
- Cálculo de ventas: `Ventas = Cantidad × Precio_Unit`
- Registro sin fecha identificado como "Sin Fecha" para mantener trazabilidad

## Hallazgos Clave
- Producto con mayor ingreso: **Mouse USB**
- Proveedor con mayor facturación: **Proveedor ABC**
- Región con mayor volumen de ventas: **Norte**
- Identificación de pedidos pendientes y cancelados que no impactan ingresos reales

## Relevancia para Supply Chain
- Control de estados de pedido
- Evaluación de proveedores
- Análisis de rotación y desempeño por región
- Apoyo en decisiones de abastecimiento





