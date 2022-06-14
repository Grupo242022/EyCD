# EyCD2022
Repositorio de respuestas de la materia: Exploración y curación de datos (2022), en el marco de la Diplomatura en Ciencia de Datos - Universidad Nacional de Córdoba.

# **DIPLOMATURA 2022**

# EXPLORACIÓN Y CURACIÓN DE DATOS

## GRUPO Nº24

## INTEGRANTES:
   - [x] Nico Rosales 
   - [x] Daniel Rubio
   - [x] Diana Fonnegra
   - [x] Clarisa Manzone

   
En este repositorio se encuentran las entregas con resultados correspondientes a la asignatura de _Exploración y curación de datos_.

## **Requerimientos - Librerías necesarias**:
   - [x] matplotlib
   - [x] pandas
   - [x] seaborn
   - [x] numpy
   - [x] missingno
   - [x] plotly
   - [x] sqlalchemy
   - [ ] 


----



  ## Criterios de exclusión de ejemplos
  1. Se eliminan ejemplos donde el año de construcción es previo a 1900

  ## Características seleccionadas
  
  RangeIndex: 12138 entries, 0 to 12137
Data columns (total 20 columns):
 #   Column               Non-Null Count  Dtype  
---  ------               --------------  -----  
 0   Suburb               12138 non-null  object 
 1   Rooms                12138 non-null  int64  
 2   Type                 12138 non-null  object 
 3   Price                12138 non-null  float64
 4   Date                 12138 non-null  object 
 5   Distance             12138 non-null  float64
 6   Postcode             12138 non-null  float64
 7   Bathroom             12138 non-null  float64
 8   Car                  12138 non-null  float64
 9   Landsize             12138 non-null  float64
 10  BuildingArea         6316 non-null   float64
 11  YearBuilt            7243 non-null   float64
 12  CouncilArea          10940 non-null  object 
 13  Lattitude            12138 non-null  float64
 14  Longtitude           12138 non-null  float64
 15  Propertycount        12138 non-null  float64
 16  zipcode              12138 non-null  float64
 17  airbnb_record_count  12138 non-null  float64
 18  airbnb_price_mean    12138 non-null  float64
 19  airbnb_price_median  12138 non-null  float64
dtypes: float64(15), int64(1), object(4)
memory usage: 1.9+ MB
  
  
  
  
  ### Características categóricas
  ![image](https://user-images.githubusercontent.com/11649711/173637836-f62defba-a55c-4aee-b1ce-cf4d8c8679cd.png)

  categorical_cols = ['Type', 'Suburb','CouncilArea']
  1. Type: tipo de propiedad. 3 valores posibles
  2. ...
  Todas las características categóricas fueron codificadas con un
  método OneHotEncoding utilizando como máximo sus 30 valores más 
  frecuentes.
  
  ### Características numéricas
  ![image](https://user-images.githubusercontent.com/11649711/173637936-53cf4ffa-9253-4812-84a8-3a0cb5528258.png)

  1. Rooms: Cantidad de habitaciones
  2. Distance: Distancia al centro de la ciudad.
  3. airbnb_mean_price: Se agrega el precio promedio diario de 
     publicaciones de la plataforma AirBnB en el mismo código 
     postal. [Link al repositorio con datos externos].

  ### Transformaciones:
  1. Todas las características numéricas fueron estandarizadas.
  2. La columna `Suburb` fue imputada utilizando el método ...
  3. Las columnas `YearBuilt` y ... fueron imputadas utilizando el 
     algoritmo ...
  4. ...

  ### Datos aumentados
  1. Se agregan las 5 primeras columnas obtenidas a través del
     método de PCA, aplicado sobre el conjunto de datos
     totalmente procesado.
