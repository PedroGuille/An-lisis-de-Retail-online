# Análisis de Retail online

# Análisis Exploratorio de Datos y Segmentación de Clientes

## Descripción del Proyecto

Este proyecto tiene como objetivo realizar un análisis exploratorio de datos (EDA) y una segmentación de clientes utilizando el conjunto de datos `Online_Retail.csv`. El análisis se centra en aplicar el modelo RFM (Recency, Frequency, Monetary) para segmentar a los clientes de una tienda en línea basada en el Reino Unido que vende regalos únicos para todas las ocasiones. El proyecto incluye la limpieza de datos, análisis descriptivo y la segmentación de clientes utilizando el algoritmo K-Means.

## Conjunto de Datos

**Fuente:**

Dr. Daqing Chen, Director del grupo de Public Analytics, chend '@' lsbu.ac.uk, Escuela de Ingeniería, London South Bank University, Londres SE1 0AA, Reino Unido.

**Información del Conjunto de Datos:**

Este conjunto de datos contiene todas las transacciones ocurridas entre el 01/12/2010 y el 09/12/2011 para una tienda en línea registrada en el Reino Unido. La compañía vende principalmente regalos únicos para todas las ocasiones. Muchos de los clientes son mayoristas.

**Atributos:**

- `InvoiceNo`: Número de factura. Nominal, un número entero de 6 dígitos asignado de forma única a cada transacción. Si este código comienza con la letra 'c', indica una cancelación.
- `StockCode`: Código del producto. Nominal, un número entero de 5 dígitos asignado de forma única a cada producto distinto.
- `Description`: Nombre del producto. Nominal.
- `Quantity`: Cantidades de cada producto por transacción. Numérico.
- `InvoiceDate`: Fecha y hora de la factura. Numérico, el día y la hora en que se generó cada transacción.
- `UnitPrice`: Precio por unidad. Numérico, el precio del producto por unidad en libras esterlinas.
- `CustomerID`: Número de cliente. Nominal, un número entero de 5 dígitos asignado de forma única a cada cliente.
- `Country`: Nombre del país. Nominal, el nombre del país en el que reside cada cliente.

**Artículos Relevantes:**

- Webber, Richard. "The evolution of direct, data and digital marketing." _Journal of Direct, Data and Digital Marketing Practice_ (2013) 14, 291–309.
- Singh, Ashishkumar, Rumantir, Grace, South, Annie, Bethwaite, Blair. "Clustering Experiments on Big Transaction Data for Market Segmentation." Proceedings of the 2014 International Conference on Big Data Science and Computing.
- You, Zhen, Si, Yain-Whar, Zhang, Defu, Zeng, XiangXiang, Leung, Stephen C.H., Li, Tao. "A decision-making framework for precision marketing." _Expert Systems with Applications_ (2015) 42, 3357–3367.

**Solicitud de Citación:**

Chen, Daqing, Sain, Sai Liang, y Guo, Kun. "Data mining for the online retail industry: A case study of RFM model-based customer segmentation using data mining." _Journal of Database Marketing and Customer Strategy Management_ Vol. 19, No. 3, pp. 197–208, 2012. (Publicado en línea antes de la impresión: 27 de agosto de 2012. doi: 10.1057/dbm.2012.17).

## Análisis Realizado

1. **Carga de Datos:** Se carga el archivo `Online_Retail.csv` y se revisa la estructura del conjunto de datos.
2. **Limpieza de Datos:** Se eliminan las filas con datos faltantes y se manejan las cancelaciones. Se convierte la fecha de factura a un formato de fecha y hora adecuado.
3. **Análisis Exploratorio de Datos (EDA):** Se exploran las ventas totales por país y por producto. Se generan gráficos para visualizar estas métricas.
4. **Análisis RFM:** Se calculan los indicadores Recency, Frequency, y Monetary para cada cliente.
5. **Segmentación de Clientes:** Se realiza una segmentación de clientes utilizando el algoritmo K-Means y se visualizan los resultados mediante gráficos de barras que comparan las métricas promedio de cada clúster.

## Cómo Ejecutar el Proyecto

1.  Solo es neccesario ejecutar el archivo en Jupyter notebook, en caso de no tener las dependencias necesarias, quitar el asterisco de la primera celda, que contiene el código para instalarlas
    
    
