# TFM_BIO_2025

En este repositorio te subiré los ficheros sobre los que estaré trabajando.

- Los "Data_check..." son un primer vistazo a los ficheros Clinic, etc donde elimino alguna columna no necesaria. Los data-frame resultantes los guardo a formato pickcle (a la hora de cargar van mejor en python y los tipos de datos se mantienen).

- He empezado la imputación de los ceros y corrección por sexo y edad para las matrices FA (Pre_processing_FA_Null_Age_Sex-HCB / NAPLES.ipynb). 
Verás que he generado carpetas nuevas a las proporcionadas donde guardo las matrices de conectividad corregidas.En el fichero las primeras líneas son una explicación de lo realizado.

06_Apr

- He añadido un Pre_processing_FA_Corrected_Analysis_HCB / Naples que cubriría todo el preprocesado:
    - Imputación
    - Covaraibles
    - Normalización
    - Combat
    - Visualizaciones de matrices por tipos 