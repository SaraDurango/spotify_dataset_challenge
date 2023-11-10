# The Spotify Million Playlist Dataset Challenge

Este repositorio contiene los datos y el código relacionado con el procesamiento del conjunto de datos del Reto The Spotify Million Playlist Dataset Challenge para continuar automáticamente las listas de reproducción. 

Los datos crudos se encuentran en un archivo llamado "challenge_set" en formato JSON.
Estos datos son proporcionados directamente por Spotify y constituyen una muestra de 10,000 registros. Cada registro representa una playlist con información detallada como nombre, duración, pistas, número de seguidores, entre otros.
Estos datos se encuentran disponibles en el siguiente link de Google Drive https://drive.google.com/file/d/1VTgm7UdzeTlqfrymG_o_niVIK_EeYFM6/view?usp=drive_link dentro de la carpeta ZIP llamada "Spotify Million Playlist Dataset Challenge".

## Contenido del Repositorio

### *Archivo de Google Colab con el Código de Obtención de la Tabla Origen*

Se proporciona un archivo de Google Colab que contiene el código necesario para transformar los datos crudos en una tabla llamada "Tabla Origen". 
Antes de ejecutar el código, se debe descargar previamente una carpeta ZIP llamada "Spotify Million Playlist Dataset Challenge" desde el siguiente link de Google Drive https://drive.google.com/file/d/1VTgm7UdzeTlqfrymG_o_niVIK_EeYFM6/view?usp=drive_link. Luego, esta carpeta debe subirse a Google Colab. Esto debido a que, por restricciones de tamaño en dichos archivos, no fue posible subirlos a plataformas como Git. 

### *Tabla Origen en Formato CSV*

La "Tabla Origen" es el resultado de la transformación del  archivo JSON en una tabla con formato CSV, la cual representa una estructura más organizada y manejable de los datos originales. Esta tabla excluye las listas de reproducción vacías, es decir, que no se componen de ninguna canción, pues proporcionan datos irrelevantes para el proyecto.  

### *Archivo de Google Colab con el Código de Transformación a Dataset -Tabla de Salida*

Otro archivo de Google Colab está disponible con el código necesario para transformar la "Tabla Origen" en una nueva tabla llamada "Tabla de Salida".
Además del procesamiento para el datast de origen, se incluye un acercamiento previo al modelo de KNN que se desarrollará y mejorará más adelante con las herramientas que se aprendan en el curso de Big Data. 

### *Dataset - Tabla de Salida en formato CSV*

La "Tabla de Salida" es el dataset final con los datos limpios, comprendiendo sólo las columnas relevantes, con algunas variables categóricas convertidas a dummies y las variables numéricas escaladas.
Cabe resaltar que variables categóricas correspondientes a nombres de canción, nombres de artistas y de álbumes musicales, no se convirtieron en dummies y se transformarán más adelante con las herramientas que podamos adquirir en el curso de BIG DATA; pues éstas comprenden infinidad de posibilidades y podrían requerir métodos de transformación y/o clasificación más robustos que aprenderemos posteriormente. 

## Instrucciones de Uso
### *Para Ejecutar el Colab de Obtención de Tabla Origen*
*Descarga el archivo ZIP "Spotify Million Playlist Dataset Challenge" desde el enlace de Google Drive https://drive.google.com/file/d/1VTgm7UdzeTlqfrymG_o_niVIK_EeYFM6/view?usp=drive_link 

*Sube la carpeta ZIP a Google Colab.

*Abre y ejecuta el archivo "Obtención de Tabla Origen" de Google Colab proporcionado para transformar los datos y obtener la tabla mencionada.

### *Para Ejecutar el Colab de Transformación de Dataset - Tabla de Salida*
*Descarga el archivo CSV con la tabla origen proporcionado en este repositorio o descárgalo del link de Google Drive https://drive.google.com/file/d/1owU5YhizDMaotWrwNXFaZ8SbzNtLdbjt/view?usp=drive_link 

*Sube la tabla origen a Google Colab.

*Abre y ejecuta el archivo "Transformación Dataset" de Google Colab proporcionado para transformar la tabla origen y obtener el dataset final. 