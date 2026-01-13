# 📊 Portafolio de Análisis de Datos: Mercado Inmobiliario USA

¡Bienvenido! En este repositorio te presento un proyecto integral de Ingeniería y Análisis de Datos utilizando **SQL Server** y **Power BI**.

## 🏗️ Fase 1: Ingeniería de Datos (SQL ETL)
He diseñado un proceso ETL (Extracción, Transformación y Carga) siguiendo una arquitectura de capas para organizar la información de precios de viviendas.

* **Capa Bronze (`brz_housing`):** Ingesta de datos crudos en formato texto para asegurar la captura total de la información.
* **Capa Silver (`slv_housing`):** Limpieza de datos y modelado dimensional. 
* **Modelo de Datos:** Implementé un **Esquema en Estrella** creando tablas de dimensiones (`dimCity`, `dimTime`, `dimFeatures`) y una tabla de hechos (`fctSales`) para optimizar el rendimiento de las consultas y reportes.

> Puedes ver el script completo de SQL en este repositorio como: `Analisis_Inmobiliaria_UsaHousePrices.sql`.

---

## 📈 Fase 2: Visualización en Power BI
Con el modelo de datos optimizado en SQL, creé un dashboard interactivo para identificar hallazgos clave.

### 🖼️ Dashboard de Análisis Inmobiliario
![Dashboard](./dashboard_final.png)

### ⚙️ Modelo de Datos y Medidas DAX
Se implementó un esquema de estrella para optimizar el rendimiento y se organizaron las medidas DAX para facilitar el mantenimiento.

![Modelo de Datos](./modelo_datos_dax.png)

## 💡 Hallazgos y Conclusiones del Análisis
1. **Dominio de Mercado:** Seattle lidera en volumen, pero Bellevue domina en margen de lujo.
2. **Ciclo de Vida:** La antigüedad promedio de 43 años sugiere un mercado de reventa maduro donde la renovación es el principal motor de plusvalía.
3. **Optimización de Producto:** Las viviendas de 3-4 habitaciones son el "sweet spot" del mercado, equilibrando precio elevado y alta rotación.

---

## 🛠️ Herramientas Utilizadas
* **Base de Datos:** SQL Server Management Studio (SSMS).
* **Lenguaje:** T-SQL (Transact-SQL).
* **Visualización:** Power BI Desktop.
