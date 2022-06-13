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
  ### Características categóricas
  1. Type: tipo de propiedad. 3 valores posibles
  2. ...
  Todas las características categóricas fueron codificadas con un
  método OneHotEncoding utilizando como máximo sus 30 valores más 
  frecuentes.
  
  ### Características numéricas
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
