# TFM: El valor de la vivienda en la Smart City a partir de la ISO-37120 mediante modelos de Forecasting

## Descripción

Este proyecto de Trabajo de Fin de Máster (TFM) se centra en analizar el valor de la vivienda en la ciudad de Barcelona, considerada una Smart City, utilizando los indicadores establecidos en la norma ISO-37120 y aplicando modelos de forecasting. El objetivo principal es determinar un valor unitario de compraventa por distritos a partir de estos indicadores, ofreciendo una herramienta de análisis y predicción útil para la gestión urbana y la planificación de la vivienda.

## Objetivos del Proyecto

1. **Análisis de Indicadores ISO-37120**: Investigar y comprender los indicadores establecidos en la norma ISO-37120 que miden el desempeño de los servicios urbanos y la calidad de vida en las ciudades.
2. **Recopilación de Datos**: Buscar y obtener conjuntos de datos abiertos que permitan cuantificar los indicadores ISO-37120 en la ciudad de Barcelona.
3. **Modelado Predictivo**: Desarrollar modelos de forecasting que utilicen los indicadores obtenidos para predecir el valor de la vivienda por distritos.
4. **Resultados y Conclusiones**: Presentar los resultados obtenidos de los diferentes modelos aplicados y extraer conclusiones relevantes.

## Estructura del Proyecto

- **Introducción**: Contexto y justificación del trabajo, objetivos del proyecto, impacto en sostenibilidad, ético-social y de diversidad, enfoque y método seguido, planificación del trabajo.
- **Estado del Arte**: Revisión de la literatura sobre Smart Cities, la norma ISO-37120, y la problemática de la vivienda en Barcelona.
- **Materiales y Métodos**: Descripción de los datos recopilados, preprocesamiento, y los modelos utilizados para el análisis y predicción.
- **Resultados**: Presentación y análisis de los resultados obtenidos.
- **Conclusiones y Trabajos Futuros**: Conclusiones del estudio y propuestas de futuras investigaciones.
- **Anexos**: Información adicional relevante, como detalles de los indicadores y scripts utilizados.

## Requisitos

- Python 3.x
- Jupyter Notebook
- Librerías necesarias: pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels

## Instalación 

Para replicar este trabajo, sigue estos pasos:

1. Clona este repositorio:
    ```bash
    git clone https://github.com/dmunozbe/TFM_DataScience.git
    ```
2. Navega al directorio del proyecto:
    ```bash
    cd TFM_DataScience
    ```
3. Instala las librerías necesarias:
    ```bash
    pip install -r requirements.txt
    ```
    
## Conjuntos de datos obtenidos
- En la capeta de datasets, ordenados por carpetas para cada indicador, se encuentran los conjuntos de datos obtenidos para cada indicador.
- Estos conjuntos de datos tienen formatos diferentes y estructuras de datos diferentes.

## Carga de datos
- En la carpeta CargaDatos, se encuentran para cada indicador, un notebook para la carga de datos de los conjuntos de datos obtenidos.
- El resultado de estos notebooks es un conjunto de datos por indicador en formato CSV, alojados en la carpeta DatasetsResultantes

## Union de datos
- En el notebook `Union_Datasets.ipynb` se realiza la unicon de todos los CSV, ubicados en la carpeta DatasetsResultantes
- El resultado de la union de todos estos CSV, se encuentra en el archivo `Final.csv`.

## Exploracion de datos
- En el notebook `ExploracionDatos.ipynb` se realiza la exploracion de datos del conjunto de datos `Final.csv`.

## Forcasting
- En la carpeta de Forecasting se encuentran ordenados por distritos los diferentes Notebooks realizados para cada par de indicador/variable
- Cada Notebook contiene los resultados del analisis y los modelos predictivos.

## Uso
Tal y como esta estructurado el proyecto y los notebooks, la puesta en marcha se puede realizar desde las diferentes etapas realizadas:

### Realizar la carga de datos
1. Abre Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
2. Descarga los conjuntos de datos ubicados en la carpeta `Datasets`.

3. Navega a los notebooks correspondientes dentro de la carpeta `CargaDatos`y ejecutalos en el orden deseado ya que son independientes los unos de los otros. Ten en cuenta modificar la ruta de donde se encuentran los conjuntos de datos.

    - `NB_Paro.ipynb`
    - `NB_EstudiosObligatorios.ipynb`
    - `NB_EnergiaElectricaResidencial.ipynb`
    - `NB_PM2_5.ipynb`
    - `NB_PM10.ipynb`
    - `NB_ParticipacionElecciones.ipynb`
    - `NB_EsperanzaVida.ipynb`
    - `NB_Internet.ipynb`
    - `NB_Movil.ipynb`
    - `NB_Motorizacion.ipynb`
    - `NB_SuperficieVerde.ipynb`
    - `NB_Compraventa.ipynb`


### Union
1. Abre Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
2. Descarga los conjuntos de datos resultantes ubicados en la carpeta `DatasetsResultantes` o bien utiliza los obtenidos en el paso anterior.
   
3. Navega y ejecuta el notebook correspondiente `Union_datasets.ipynb` ubicado en la carpeta raiz del proyecto. Recuerda modificar la ruta de donde se encuentran los conjuntos de datos.


### Exploracion de datos
1. Abre Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
2. Descarga el conjunto de conjuntos de datos final `Final.csv` ubicado en la carpeta raiz del proyecto o utiliza el obtenido en el paso anterior.
   
3. Navega y ejecuta el notebook correspondiente `ExploracionDatos.ipynb` ubicado en la carpeta raiz del proyecto. Recuerda modificar la ruta de donde se encuentra el conjuntos de datos.


### Forecasting
1. Abre Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
2. Descarga el conjunto de conjuntos de datos final `Final.csv` ubicado en la carpeta raiz del proyecto o utiliza el obtenido en el paso anterior.
   
3. Navega y ejecuta los notebooks correspondientes al distrito de interes ubicados en la carpeta `Forecasting`. Cada distrito contiene 11 notebook's. Recuerda modificar la ruta de donde se encuentra el conjuntos de datos.

    - `Forecasting_(Indicador_1).ipynb`
    - `Forecasting_(Indicador_10).ipynb`
    - `Forecasting_(Indicador_15).ipynb`
    - `Forecasting_(Indicador_22).ipynb`
    - `Forecasting_(Indicador_23).ipynb`
    - `Forecasting_(Indicador_40).ipynb`
    - `Forecasting_(Indicador_46).ipynb`
    - `Forecasting_(Indicador_73).ipynb`
    - `Forecasting_(Indicador_74).ipynb`
    - `Forecasting_(Indicador_79).ipynb`
    - `Forecasting_(Indicador_85).ipynb`
  
4. En caso de querer realizar el analisis de datos de otro distrito no analizado, se recomienda copiar estrutura/carpeta de distrito y modificar los notebooks con los parametros necesarios para modificar el distrito en cuestion.
    

## Resultados

Los resultados del análisis y los modelos predictivos se encuentran en la carpeta `Forecasting`. Aquí se incluyen gráficos, tablas y modelos entrenados que reflejan las principales conclusiones del estudio.

## Contribuciones

Este trabajo está abierto a contribuciones. Si deseas mejorar algún aspecto del proyecto o añadir nuevas funcionalidades, por favor sigue estos pasos:

1. Haz un fork de este repositorio.
2. Crea una rama con la nueva funcionalidad:
    ```bash
    git checkout -b nueva-funcionalidad
    ```
3. Realiza tus cambios y haz un commit:
    ```bash
    git commit -m "Añadida nueva funcionalidad"
    ```
4. Envía tus cambios al repositorio remoto:
    ```bash
    git push origin nueva-funcionalidad
    ```
5. Crea un Pull Request en GitHub.

## Licencia

Este proyecto está bajo la Licencia Creative Commons Reconocimiento-NoComercial-SinObraDerivada 3.0 España.

## Contacto

Para cualquier consulta o sugerencia, puedes contactar con el autor del proyecto:

- **Nombre**: David Muñoz Bertrán
- **Correo Electrónico**: maxpainegt@hotmail.com, dmunozbe@uoc.edu
