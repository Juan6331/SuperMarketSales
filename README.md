🛒 Análisis de Ventas — SuperMarket Sales
![Python](https://img.shields.io/badge/Python-3.9-blue)
![pandas](https://img.shields.io/badge/pandas-1.4-green)
![Status](https://img.shields.io/badge/Status-Completado-brightgreen)
## 🏪 Contexto de negocio
Una cadena de supermercados con 3 sucursales en Myanmar necesitaba entender qué
segmento de clientes generaba mayor revenue y en qué horarios se concentraban las ventas,
para optimizar staffing y campañas de fidelización.
## ❓ Pregunta analítica
> Qué patrones de compra y características del cliente están asociados con un ticket más alto en cada sucursal?
## 🔧 Herramientas y proceso
- **Python** (pandas, numpy) → Limpieza y transformación de datos
- **Matplotlib / Seaborn** → Visualización de distribuciones y tendencias
- **Análisis de correlación** → Identificar variables con mayor impacto en el ticket
```
Datos → Limpieza → EDA → Segmentación → Visualización → Conclusiones
## 📊 Hallazgos principales
| Hallazgo | Dato |
|----------|------|
| Las clientas generan mayor revenue | 51.0% del total vs 49.0% de clientes masculinos |
| Horario de mayor venta | Martes entre 19:00–20:00 hrs |
| Categoría más rentable | Food & Beverages ($56K en el trimestre) |
| Método de pago preferido | E-wallet (34.5% de transacciones) |
## 💡 Recomendación
Concentrar campañas de fidelización en clientes femeninas y ajustar el staffing los
martes por la tarde. Priorizar la categoría Food & Beverages en las promociones
mensuales dado su mayor volumen de transacciones.
