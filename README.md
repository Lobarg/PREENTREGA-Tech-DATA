PRE-ENTREGA PYTHON – DATA ANALYTICS
Autora: Adriana A. Cruz – DNI 26689598
Comisión: 25262

------------------------------------------------------------

DESCRIPCIÓN GENERAL
Este proyecto corresponde a la pre-entrega del curso de Data Analytics, desarrollado en Python dentro de Google Colab.
El trabajo implementa un proceso ETL completo (Extracción, Transformación y Carga) sobre tres datasets:
- clientes.csv
- ventas.csv
- marketing.csv

A partir de ellos se realiza:
- Análisis exploratorio (EDA) de calidad de datos.
- Limpieza y normalización (duplicados, nulos, formatos, tipos).
- Conversión de fechas y campos numéricos.
- Cálculo de métricas clave: ventas mensuales, top 20 % de productos, ventas por categoría.
- Integración con campañas de marketing y evaluación de desempeño por canal.
- Generación automática de reportes en Google Drive.

------------------------------------------------------------

ESTRUCTURA DEL REPOSITORIO
CRUZ pre_entrega.ipynb     → Notebook principal
EN archivo ZIP:
/originales                 → Archivos de entrada (clientes, ventas, marketing)
/Datos Limpios              → Datasets luego del proceso ETL
/reportes                   → Archivos de salida (ventas mensuales, top80, etc.)
README.txt                  → Este documento

------------------------------------------------------------

LIBRERÍAS PRINCIPALES
pandas, numpy, os, datetime, google.colab.drive

------------------------------------------------------------

EJECUCIÓN

Abrir el notebook en Google Colab
El notebook puede ejecutarse sin autenticación local porque los datasets están disponibles mediante links públicos de Google Drive:
https://drive.google.com/drive/folders/1EHY2gIL_DjFQQDvZLbwvqYScVxKyMrAl?usp=drive_link


------------------------------------------------------------

RESULTADOS GENERADOS
El notebook produce automáticamente los siguientes reportes (guardados en /reportes):

ventas_totales_mensuales.csv            → Ventas agregadas por mes
ventas_top80_completo.csv               → Productos del top 20 % en ventas
ventas_por_categoria.csv                → Resumen de ingresos por categoría
comparativo_ventas_producto_canal.csv   → Ventas por producto y canal
ventas_indice_diario_por_canal.csv      → Índice de venta diaria ($/día)
ventas_promedio_general_por_canal.csv   → Promedio diario por canal

------------------------------------------------------------

PRINCIPALES CONCLUSIONES
- Solo el dataset Ventas requería limpieza (duplicados = 35 registros y 2 valores nulos).
- La conversión y depuración permitieron unificar estructuras y generar reportes consistentes.
- Productos líderes: lámpara de mesa, auriculares, microondas, cafetera, cuadro decorativo y smartphone.
- Categorías más rentables:
  * Electrodomésticos (34.4 %)
  * Electrónica (32.9 %)
  * Decoración (32.7 %)
- Canal más efectivo: Email (387.35 $/día promedio de ventas).

------------------------------------------------------------

REQUISITOS
- Python 3.10 o superior
- Jupyter Notebook / Google Colab
- Conexión a Google Drive (para guardar resultados)

------------------------------------------------------------

AUTORÍA
Adriana Anabel Cruz
Auditoría Interna | Data Analytics | 
https://www.linkedin.com/in/adrianacruz

------------------------------------------------------------

LICENCIA
Este proyecto puede utilizarse con fines académicos y de aprendizaje.
