## Decisiones con Datos: Análisis Financiero 
## Base de datos utilizada
Se encuentra en Learn.Microsoft: [FinancialSample](https://go.microsoft.com/fwlink/?LinkID=521962)  
Esta base de datos tiene una tabla de datos de ventas y ganancias ordenados por segmento de mercado y país.  
Se compone de 16 columnas y 701 filas.  
Segment - Segmento  
Country - País  
Product - Producto  
Discount Band - Banda de descuento  
Units Sold – Unidades vendidas  
Manufacturing Price – Precio de manufactura  
Sale Price – Precio de venta  
Gross Sales – Ventas brutas  
Discounts - Descuentos  
Sales - Ventas  
COGS – Costo de producto vendido  
Profit - Ganancias  
Date - Fecha  
Month Number – Número del mes  
Month Name – Nombre del mes  
Year - Año  

## Descripción Proyecto
Este proyecto se centra en Power Bi. Utilizando diferentes técnicas se crean gráficos que ayudan a analizar de manera visual la información. Se utilizan gráficos como:  
•	Linea de tiempo: para marcar o definir los periodos a analizar de la información.  
•	Gráfico de líneas: permite ver temporalidad y oscilación, para comparar una fecha de un año a otro.  
•	Cartas: foto estática de valores claves para tener presente.  
•	Tabla: presentar cada país con su variación mensual, más semáforo, para ver el deseméño de cada uno de los países, logrando monitorear aquellos con alto y bajo resultado.  
•	Gráfico de torta: permite ver los segmentos con mayor venta.  
•	Gráfico de barras apiladas: muestra las ganancias por producto.  
•	Gráfico de dispersión: presenta el margen de ganancia por tasa de descuento.  
A través de estos gráficos se puede inferir múltiple información, que serán explicados en el siguiente paso del informe.  
________________________________________
## Desarrollo  
La base de datos se encuentra completa y sin valores nulos. El periodo de análisis es desde septiembre del 2013 a diciembre del 2014. Siguiente paso es cargar lo datos, sin la necesidad de transformarlos. Seguido, se crea una nueva tabla, para facilidad de ubicación, y se crean nuevas medidas. Estas medidas calculadas permitirán obtener información más detallada y formar nuevos gráficos.  
•	Precio de Venta Promedio por Unidad = Ventas / Unidades Vendidas  
•	Margen de Beneficio (%) = (Beneficio / Ventas)  
•	Tasa de Descuento (%) = (Descuentos / Ventas Brutas)  
•	COV por Unidad = COV / Unidades Vendidas  
•	Beneficio por Unidad = Beneficio / Unidades Vendidas  
•	Crecimiento Mensual de Ventas = Comparar las Ventas mes a mes  
•	Contribución del Segmento = % de las Ventas totales o Beneficio por Segmento  
•	Índice de Rendimiento del Producto = Puntuación compuesta basada en el Margen de Beneficio, las Unidades Vendidas y las Ventas

Luego de la creación de medidas, sigue el crear el dashboard:
1.	Título: Decisiones con Datos: Análisis Financiero Interactivo  
2.	Linea de tiempo: para crear la linea de tiempo se debe descargar material adicional en “Obtener más objetos visuales”. Este permite definir los periodos que se quieren indagar.  
3.	Gráfico de líneas: este representa las ventas totales a través del tiempo con una jerarquía temporal de año, trimestres, mes y día.  
4.	Cartas: muestran cuatro valores a tener presente, el total de ventas, el total de ganancias, la media del margen de ganancias y la variación mensual.  
5.	Tabla: presenta cada país, ordenado de mayor a menor, con su variación mensual y además, un semáforo, que muestra diferentes colores, verde para alto, amarillo para intermedio y rojo para bajo, dependiendo del desempeño mensual de cada uno.  
6.	Gráfico de torta: muestra las ventas totales por segmento.  
7.	Gráfico de barras apiladas: muestra las ganancias por producto.  
8.	Gráfico de dispersión: presenta el margen de ganancia por tasa de descuento.

### Analisis de los gráficos:

Análisis de Ventas
•	Ventas Totales: 118,73 millones.  
•	Evolución Temporal: El comportamiento de las ventas presenta oscilaciones, con picos destacados en noviembre 2013 y noviembre 2014, lo que podría estar asociado a temporadas de mayor consumo.  
•	Segmentación de Ventas:  
o	Enterprise: 52,5 millones (44,22 %).  
o	Small Business: 42,43 millones (35,74 %).  
o	Government: 19,61 millones (16,52 %).  
o	Midmarket: 1,8 millones (1,52 %).  
o	Channel Partners: participación mínima.  
La mayor parte de las ventas proviene del segmento Enterprise, seguido por Small Business.  

Análisis de Utilidad  
•	Utilidad Total: 16,89 millones.  
•	Margen Promedio: 27,90 %.  
•	Variación Mensual Promedio: 11,24 %.  
•	Por Producto:  
o	Paseo: 4,8 millones (producto más rentable).  
o	VTT: 3,0 millones.  
o	Amarilla: 2,8 millones.  
o	Velo: 2,3 millones.  
o	Montana: 2,1 millones.  
o	Carretera: 1,8 millones.  
Los productos Paseo y VTT concentran gran parte de la utilidad, mientras que Carretera es el de menor contribución.  

Análisis por País  
La variación mensual de ventas por país indica:  
•	Canadá: +18,92 % (mejor desempeño).  
•	Francia: +10,88 %.  
•	Alemania: +10,76 %.  
•	México: +8,46 %.  
•	Estados Unidos: +7,43 % (crecimiento más moderado).  
Canadá lidera el crecimiento, mientras que EE. UU., pese a ser un mercado clave, presenta un aumento menor.  

Relación Descuentos - Rentabilidad  
El análisis de dispersión entre tasa de descuento y margen de ganancia muestra:  
•	Una tendencia negativa: a mayor descuento, menor margen de rentabilidad.  
•	Se identifican algunos outliers con márgenes altos incluso con descuento, pero en general, los descuentos erosionan la utilidad.  
Es necesario revisar las políticas de descuentos, ya que afectan directamente la rentabilidad.  
________________________________________
### Resumen  
El análisis financiero muestra un total de ventas acumuladas de 118,73 millones, con una utilidad total de 16,89 millones y un margen de ganancia promedio de 27,90 %. La variación mensual general es positiva, con un crecimiento del 11,24 %.  
Se observa un desempeño favorable en ciertos países y productos, mientras que el análisis de márgenes revela un impacto negativo de los altos descuentos sobre la rentabilidad.  
________________________________________
## Conclusiones y Recomendaciones  
1.	Concentración de ventas en Enterprise: Se recomienda diversificar esfuerzos hacia Small Business, dado su peso del 35 %, para reducir la dependencia del segmento Enterprise.  
2.	Productos líderes: Fomentar la promoción de los productos Paseo y VTT, pero diseñar estrategias para mejorar la rentabilidad de Carretera y Montana.  
3.	Canadá como mercado en expansión: Aumentar la inversión comercial en Canadá, ya que presenta la mayor variación positiva mensual.  
4.	Descuentos: Redefinir la estrategia de descuentos, priorizando promociones más inteligentes y segmentadas para evitar la erosión del margen de utilidad.  
5.	Estacionalidad: Aprovechar los picos de noviembre o fin de año con campañas específicas para maximizar ventas en esos periodos.  

En conclusión, la empresa presenta buenos resultados financieros con márgenes saludables, pero debe vigilar el impacto de los descuentos y buscar un mayor equilibrio en la diversificación de productos y mercados.  

