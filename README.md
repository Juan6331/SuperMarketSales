# SuperMarketSales
El análisis de ventas se realiza en tres ciudades (que son las ciudades más importantes de Myanmar/Birmania):  Naypyitaw  Yangon  Mandalay, corresponden al primer trimestre del año 2019.
Diapositiva 1: Título y Problema a Resolver
Título del Proyecto: Análisis de Ventas de Supermercado (Supermarket Sales Analysis)

Autor: Juan Jesus Antonio Gonzalez Gonzalez

El Problema: * Los supermercados generan grandes volúmenes de datos transaccionales, pero los datos crudos no ofrecen valor estratégico.

Objetivo del proyecto: Extraer insights accionables sobre el comportamiento del consumidor para responder preguntas clave: ¿Quién compra más? ¿Qué métodos de pago prefieren? ¿En qué ciudades hay mayor rendimiento? ¿La hora de compra afecta el volumen de ventas?

Solución: Un Análisis Exploratorio de Datos (EDA) para identificar patrones que permitan optimizar el inventario, el marketing y las estrategias de fidelización.

Diapositiva 2: Metodología y Herramientas
Metodología:

Extracción: Lectura del conjunto de datos histórico de ventas.

Transformación: Adecuación de formatos y creación de nuevas variables.

Análisis Descriptivo: Cálculo de medidas de tendencia central (media, mediana, moda).

Análisis Comparativo: Agrupaciones cruzadas (Pivot) por demografía, geografía y producto.

Correlación y Visualización: Identificación de relaciones entre variables clave mediante gráficos de dispersión.

Herramientas Utilizadas:

Lenguaje: Python 3

Entorno: Jupyter Notebook

Librerías: * pandas (Manipulación y agrupación de datos)

numpy (Conversión a arrays y cálculos estadísticos)

seaborn & matplotlib.pyplot (Visualización de datos)

Diapositiva 3: Limpieza y Transformación de Datos
Procesamiento Inicial:

Carga del archivo supermarket_sales.csv utilizando Pandas.

Extracción de columnas clave (Unit price, Quantity) y conversión a estructuras de alto rendimiento (numpy.ndarray).

Ingeniería de Características (Feature Engineering):

Transformación de Tiempo: Conversión de la columna Time a formato datetime para extraer específicamente la Hour (Hora del día).

Métricas de Valor: Creación de nuevas columnas analíticas como:

Rank: Clasificación de ventas.

Porcentaje_aporte: Porcentaje de contribución de cada segmento al Total general de ventas de la cadena.

Diapositiva 4: Análisis Realizado
Estadística Básica: Evaluación del ticket promedio, unidades por compra y precios más frecuentes.

Agrupaciones Estratégicas (Groupby & Pivot):

Ticket promedio por Ciudad, Línea de Producto y Género.

Volumen total de ventas segmentado por Tipo de Cliente (Miembro vs Normal).

Distribución de ingresos según el Método de Pago.

Análisis de Correlación:

¿A mayor precio, mejor calificación (Rating) del cliente?

¿Hay una relación entre la hora del día y el total del ticket?

¿Cómo impacta el precio unitario en el ingreso bruto (Gross Income)?

Diapositiva 5: Resultados Clave
Desempeño Geográfico y de Lealtad:

Mercado muy equilibrado: Naypyitaw lidera con 34.2% de las ventas, seguido de cerca por Yangon y Mandalay (~32.8% cada uno).

Los clientes "Member" (50.8%) superan ligeramente a los "Normal" (49.1%).

Pagos y Consumo:

El pago en efectivo (Cash) es el #1 con 34.7%, pero E-wallet (34%) y Tarjeta de Crédito (31.2%) tienen una fuerte penetración.

La moda (valor más frecuente) en cantidad de productos llevados es 10 unidades, con un ticket promedio global de 55.67 por producto.

Correlaciones Descubiertas:

Positiva: Productos más caros generan un mayor ingreso bruto (Correlación: 0.63).

Nula: El precio del producto no afecta la calificación que le da el cliente (Corr: -0.008). Tampoco hay relación entre la hora de compra y el monto gastado.

Diapositiva 6: Conclusiones
Balance del Mercado: La empresa tiene una distribución de ingresos excepcionalmente sana; no depende de una sola ciudad, de un solo tipo de cliente, ni de un solo método de pago.

Marketing Segmentado: El análisis cruzado demostró claras preferencias por género (Ej. Mujeres lideran en "Hogar/Estilo de vida"; Hombres en "Salud/Belleza"). Se recomienda lanzar promociones dirigidas basadas en estos perfiles.

Estrategia Comercial: Dado que la hora no afecta el volumen de ventas, las operaciones y el personal en tienda pueden distribuirse uniformemente.

Fidelización: Existe una gran oportunidad para convertir a los clientes "Normales" (49%) en "Miembros" mediante incentivos, para asegurar su retención.
