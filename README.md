# Caso 1 – Análisis de Ventas e Inventario (Google Sheets)

## 📌 Descripción del Proyecto

Proyecto práctico orientado al análisis de ventas e inventario en un entorno de e-commerce.  
Simula tareas propias de un Analista Junior de Operaciones, Logística o Inventarios.

El objetivo fue limpiar datos inconsistentes, controlar calidad de información y generar análisis mediante tablas dinámicas y visualizaciones ejecutivas.

---

## 🧹 Proceso de Limpieza de Datos

Se trabajó sobre una base con errores intencionales:

- Inconsistencias en mayúsculas y acentos
- Formatos de fecha distintos
- Valores nulos en cantidad y proveedor
- Estados de pedido con diferentes formatos
- Precio unitario en 0
- Registro sin fecha

### Acciones realizadas:

- Normalización de texto (Proveedor, Categoría, Estado)
- Validación de fechas
- Creación de columna `Ventas = Cantidad * Precio_Unit`
- Tratamiento de cantidades nulas sin inferir valores
- Clasificación de proveedor vacío como **"Anónimo"** únicamente para análisis
- Registro sin fecha etiquetado como **"Sin Fecha"** para mantener trazabilidad

No se modificó el dataset original.

---

## 📊 Análisis Realizado

Se desarrollaron tablas dinámicas para:

- Ventas por Producto
- Ventas por Proveedor
- Ventas por Región
- Evolución temporal de ventas
- Estado de pedidos

Para el análisis de ingresos reales se filtraron únicamente pedidos con estado **"Entregado"**.

---

## 📈 Visualización

Se diseñaron gráficos ejecutivos con formato profesional:

- Columnas → Ingresos por Producto
- Barras → Ingresos por Proveedor
- Línea → Evolución de Ventas
- Circular → Distribución por Región

Se utilizó una paleta corporativa en verde oscuro y formato limpio orientado a presentación ejecutiva.

---

## 🔎 Principales Hallazgos

- Producto con mayor ingreso: **Mouse USB**
- Proveedor con mayor facturación: **Proveedor ABC**
- Región con mayor volumen de ventas: **Norte**
- Se detectó 1 registro sin fecha (excluido del análisis temporal)
- Existen pedidos pendientes y cancelados que no impactan ingresos reales

---

## 🛠 Herramientas Utilizadas

- Google Sheets
- Tablas dinámicas
---

## 💼 Competencias Demostradas

- Limpieza y normalización de datos
- Control de calidad de información
- Análisis de desempeño de productos y proveedores
- Interpretación de datos para toma de decisiones
- Presentación ejecutiva de resultados

- Enfoque en trazabilidad y transparencia
