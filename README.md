# “Análisis integral de acciones tecnológicas"
Antes de sumergirse en el análisis detallado de las oportunidades de inversión, es fundamental establecer una visión integral que considere los diversos factores que afectan el rendimiento de los activos financieros. Este enfoque holístico permite a los inversores evaluar no solo el potencial de retorno, sino también los riesgos asociados con cada inversión. 
Al examinar aspectos clave como la volatilidad, el volumen de negociación y la variación de precios, los inversores obtienen una comprensión completa que facilita una toma de decisiones más informada y estratégica, maximizando así las oportunidades de inversión y gestionando eficazmente el riesgo.

![](https://i0.wp.com/criptotendencia.com/wp-content/uploads/2017/09/10-consejos-para-invertir-en-la-bolsa-de-valores.png?fit=960%2C540&ssl=1)

# Menú
- [Objetivo](#Objetivo)
- [Herramientas y Tecnologías](#HerramientasyTecnologías)
- [Procesamiento y análisis](#Procesamientoyanálisis)
- [Resultados y Conclusiones](#ResultadosyConclusiones)
- [Enlaces de interés](#Enlacesdeinterés)

## Objetivo
Identificar oportunidades de inversión y riesgo, evaluando la volatilidad, el volumen de negociación y la variación, con el fin de proporcionar recomendaciones estratégicas para inversores en el sector.

## Herramientas y Tecnologías:

### Herramientas y/o plataformas
Power BI
Jupyter Notebook
Chat GPT

### Lenguajes
Python en Jupyter Notebook

## Procesamiento y análisis:

- ### Conectar/importar datos a herramientas
  Para conectar/importar datos a Jupyter Notebook, se tomó la decisión de descomprimir los archivos y guardarlos en una carpeta en una carpeta en la PC.
  ```df = pd.read_csv("C:\\Users\\LENOVO.USER\\Documents\\PROYECTO4\\csv_archivos\\big_tech_companies.csv")
  file_path = "C:\\Users\\LENOVO.USER\\Documents\\PROYECTO4\\big_tech_stock_prices.xlsx"
  df1 = pd.read_excel(file_path)```
- ### Unir tablas
  La unión de las dos tablas se hizo mediante el comando.
  ```df_merged = pd.merge(df, df1, on='stock_symbol', how='inner')```

- ### Identificar y manejar valores nulos
  Se utilizó una fórmula en la tabla para eliminar las filas que contienen cualquier valor nulo
  ```df_merged = df_merged.dropna()```

- ### Identificar valores duplicados  
  Se utilizó una fórmula en la tabla para identificar cuántos valores duplicados hay en la tabla
  ```df_merged = df_merged.drop_duplicates()```

- ### Guardar el DataFrame en un archivo Excel  
  Se utilizó una fórmula en la tabla para guardar en un archivo excel
  ```df_merged.to_excel("C:\\Users\\LENOVO.USER\\Documents\\PROYECTO4\\data01_P4.xlsx", index=False)```

- ### Crear nuevas variables
  Se crearon nuevas variables para el análisis, como la volatilidad, la variación y el volumen de negociación. 

- ### Agrupar datos según variables categóricas
  Las variables categóricas se agruparon a través de tablas matrix en Power BI.

- ### Visualizar las variables categóricas
  Para visualizar los datos de las variables categóricas que se agruparon se utilizó gráfico de barras en Power BI.

- ### Calcular cuartil, deciles o percentile
  Para crear categorías por percentiles para las variables de interés en el análisis se utilizó comandos en Jupyter. 

- ### Aplicar segmentación
  Las categorías creadas a través del percentil 75 para el análisis. 
  Se construyó una tabla donde se obtiene la clasificacion de las empresas dependiendo del nivel de riesgo.
  
- ### Representar datos a través de tabla resumen o scorecards
  La base de datos contiene la información relevante para realizar el analísis, junto con un dashboard para visualizar los resultados.

- ### Representar datos a través de gráficos simples
  Los gráficos utilizados para el proyecto fueron los gráficos de barra y gráficos circulares. debido a que son los más útiles al momento de presentar los resultados del análisis. 

## Resultados y Conclusiones:
  La clasificación de empresas tecnológicas según su nivel de volatilidad, variación de precios y volumen de negociación, permite identificar los niveles de riesgo de cada una. Empresas como Tesla y Netflix  presentan mayores riesgos debido a su alta volatilidad, mientras que otras como Apple y Microsoft son más estables. Esta información ayuda a los inversionistas a evaluar qué empresas se alinean mejor con su perfil de riesgo.

Para los inversionistas conservadores, se recomienda enfocarse en empresas estables con menor riesgo, como Apple y Microsoft. Por otro lado, los inversionistas activos, que buscan mayores retornos, pueden considerar empresas más riesgosas como Tesla y Netflix, siempre manteniendo un control sobre los riesgos asumidos. Una estrategia diversificada, combinando ambos tipos de empresas, puede ser una opción ideal para equilibrar riesgo y rendimiento.

## Enlaces de interés:
[Presentación Power BI](https://drive.google.com/file/d/1e44p6GRHkyoiD3R5H2_udV73olTpoUqd/view?usp=sharing)
