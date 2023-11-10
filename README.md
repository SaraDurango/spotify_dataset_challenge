# The Spotify Million Playlist Dataset Challenge

Este repositorio contiene los datos y el código relacionado con el procesamiento del conjunto de datos del Reto The Spotify Million Playlist Dataset Challenge para continuar automáticamente las listas de reproducción. 

## Contenido del Repositorio
*Datos Crudos en Formato JSON*

Los datos crudos se encuentran en un archivo llamado "challenge_set" en formato JSON.
Estos datos son proporcionados directamente por Spotify y constituyen una muestra de 10,000 registros. Cada registro representa una playlist con información detallada como nombre, duración, género, pistas, número de seguidores, entre otros.

*Archivo de Google Colab con el Código de Obtención de la Tabla Origen*

Se proporciona un archivo de Google Colab que contiene el código necesario para transformar los datos crudos en una tabla llamada "Tabla Origen".
Antes de ejecutar el código, se debe descargar previamente una carpeta ZIP llamada "Spotify Million Playlist Dataset Challenge" desde el siguiente link de Google Drive https://drive.google.com/file/d/1VTgm7UdzeTlqfrymG_o_niVIK_EeYFM6/view?usp=drive_link. Luego, esta carpeta debe subirse a Google Colab. Esto debido a que, por restricciones de tamaño en dichos archivos, no fue posible subirlos a plataformas como Git. 

*Tabla Origen en Formato CSV*

La "Tabla Origen" es el resultado de la transformación del  archivo JSON en una tabla con formato CSV.
Esta tabla representa una estructura más organizada y manejable de los datos originales.

*Archivo de Google Colab con el Código de Transformación a Tabla de Salida*

Otro archivo de Google Colab está disponible con el código necesario para transformar la "Tabla Origen" en una nueva tabla llamada "Tabla de Salida".
La "Tabla de Salida" es el dataset final con los datos limpios, comprendiendo sólo las columnas relevantes, con las variables categóricas convertidas a dummies y las variables numéricas escaladas.

## Instrucciones de Uso
*Descarga el archivo ZIP "Spotify Million Playlist Dataset Challenge" desde el enlace de Google Drive https://drive.google.com/file/d/1VTgm7UdzeTlqfrymG_o_niVIK_EeYFM6/view?usp=drive_link 

*Sube la carpeta ZIP a Google Colab.

*Abre y ejecuta los archivos de Google Colab proporcionados para transformar los datos y obtener las tablas mencionadas.


