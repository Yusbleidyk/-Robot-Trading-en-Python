# -Robot Trading en Python
Proyecto de construcción de un Robot Trading en Python capaz de tomar decisiones de compra y venta de Bitcoin en tiempo real! En este proyecto, utilizaremos Python y diversas librerías para desarrollar un algoritmo que nos ayude a tomar decisiones de inversión en el mercado de Bitcoin.
# Obtención de datos
se  accedera a una API que proporcione datos históricos de precios de Bitcoin en formato JSON. Además, se realizara Web Scraping en un sitio de noticias para obtener el precio actual y algunos indicadores de tendencias del Bitcoin.

# Limpieza de datos
Una vez que obtenidos los datos históricos y los datos actuales, se cargara los datos en un DataFrame de Pandas para manipularlos y analizarlos. En esta etapa, se realizara las siguientes tareas:

1. Identificar y eliminar los outliers.
2. Tratar los valores nulos o duplicados en la base.
3. Calcular el precio promedio del Bitcoin.
   
# Toma de decisiones
Con el precio promedio, se comparara este valor con el precio actual y la tendencia del Bitcoin obtenida previamente mediante Web Scraping. Si el precio actual es mayor o igual que la media y la tendencia es a la baja, entonces se deberá vender. Por otro lado, si el precio actual es menor que la media y la tendencia es al alza, entonces se deberá comprar.

# Visualización
Se utilizara la librería Matplotlib para crear un gráfico que muestre la evolución del precio del Bitcoin durante el periodo seleccionado. Además, se traza una línea recta que represente el precio medio. Por último, se mostrara un mensaje en el gráfico que indique "Vender", "Comprar" o "Mantener" según sea la decisión del algoritmo.

# Automatización
Una vez que tengamos el algoritmo de decisión, será el momento de automatizar el proceso, con la librería "time" de Python para ejecutar el algoritmo cada 5 minutos y actualizar el gráfico de forma automática.
