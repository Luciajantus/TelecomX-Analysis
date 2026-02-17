# TelecomX-Analysis
Análisis de evasión de clientes y limpieza de datos con Python y Pandas

---

# Análisis de Evasión de Clientes - TelecomX

Este proyecto consiste en un análisis exhaustivo de una base de datos de telecomunicaciones con el objetivo de identificar patrones que llevan a la pérdida de clientes. A través de la limpieza, transformación y visualización de datos, se proponen estrategias para mejorar la retención.

## 🚀 Descripción del Problema

La empresa **TelecomX** presentaba una tasa de evasión preocupante. El desafío fue procesar un archivo JSON con datos anidados de más de 7,000 clientes para entender las variables numéricas y categóricas que influyen en la decisión de abandonar el servicio.

## Tecnologías Utilizadas

* **Python** (Lenguaje principal)
* **Pandas** (Limpieza y manipulación de datos)
* **NumPy** (Operaciones matemáticas)
* **Matplotlib** (Visualización de datos)
* **Google Colab** (Entorno de desarrollo)

## Procesamiento de Datos

Para este análisis, se realizaron los siguientes pasos de "Data Wrangling":

1. Conversión de JSON anidado a un DataFrame plano.
2. Eliminación de **224 registros** con valores inconsistentes en la columna de evasión.
3. Transformación de cargos totales de `object` a `float64` para permitir cálculos.
4. Creación de la columna `Cargos_Diarios` dividiendo la facturación mensual por 30.
5. Uso de funciones **Lambda** y `.map()` para convertir variables de texto ("Yes"/"No") a formato binario (1/0).

---

## Insights

* El análisis de los **Meses de Permanencia** reveló que la mayor fuga de clientes ocurre durante el primer año de contrato.
* Mediante gráficos, se observó que los clientes con cargos mensuales superiores a los **$70** tienen una probabilidad de evasión significativamente mayor.
* }Los contratos mensuales presentan la tasa de evasión más alta, mientras que los contratos a largo plazo (1 o 2 años) aseguran la fidelidad.

## Recomendaciones

* Implementar un **programa de fidelización** específico para los primeros 6 meses de contrato.
* Incentivar la migración de contratos mensuales a anuales mediante descuentos estratégicos.
* Revisar la propuesta de valor para clientes con facturas altas para evitar que migren a la competencia.

---

### 🖋️ Autor

* **Lucía E. Jantus**
* Análisis realizado como parte del desafío de Ciencia de Datos - 2026.
