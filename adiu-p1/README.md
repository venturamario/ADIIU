# ADIIU-P1
Estudios: Grado en Ingeniería Informática (GIN3)<br>
Asignatura: ADIIU<br>
Trabajo: Práctica 1<br>
Autores: Mario Ventura Burgos & Luis Miguel Vargas Durán<br>
Fecha: Noviembre 2023

# Observaciones
1- Todo el código y todas las funcionalidades han sido probadas en diferentes dispositivos y se ha comprobado el correcto funcionamiento en todos ellos.
Si surge algún problema o algo no funciona como debería, por favor, comuníquese con alguno de los autores.

2- Se ha usado *Highcarts* para crear los gráficos (https://www.highcharts.com/), *Bootstrap* (https://getbootstrap.com/) para la interfaz de usuario y *JQuery* (https://jquery.com/).

3- El dataset (original) se ha obtenido de Kaggle, y es el siguiente: https://www.kaggle.com/datasets/brunoalarcon123/top-200-spotify-songs-dataset/data

4- El **dataset original se ha tratado** de forma que se han eliminado algunas columnas que se consideraban irrelevantes. Se adjuntará el dataset modificado para que se pueda trabajar con él, ya que el codigo SQL de creación de la base de datos está basado en este dataset modificado y no en el original.

5- Este dataset (el original y el tratado) viene en formato **.csv** y cuenta con aproximadamente 650.000 filas. Esto hace que, al importar los datos mediante el código proporcionado en el paso 3 del documento **"databse creation.txt"**, salgan algunos warnings debido al gran tamaño de los datos.
Por ello, se ha añadido una línea de código comentada (LIMIT X;) para que, en caso de que así se desee, se establezca un límite de filas a importar (sustituir X por el número de filas a importar). De todas formas, el código proporcionado para importar los datos es correcto.

6- Por último, aclarar que la información mostrada en los gráficos se obtiene mediante solicitudes al servidor procesadas por los dos archivos PHP (back-end), que se conectan directamente a la base de datos para hacer operaciones de consulta.

# Tutorial
1- Abrir XAMPP e iniciar Apache y MySQL.

2- Descargar y descomprimir el zip y obtener la carpeta con todos los documentos de la práctica incluyendo el dataset ya tratado.

3- Ir a localhost/phpmyadmin y crear una nueva base de datos siguiendo los pasos detallados en el documento "database creation.txt". Estos pasos son:

  &ensp;&ensp;**Paso 1:** Crear la nueva base de datos de nombre "spotify2023" (Step 1 en el documento).
  
  &ensp;&ensp;**Paso 2:** Crear una tabla llamada "spotifyinfo" con las columnas necesarias para el dataset tratado (código de creación de la tabla detallado en el paso 2 del documento).
  
  &ensp;&ensp;**Paso 3:** Acceder a la tabla creada, ir apartado de SQL e importar los datos del documento .csv directamente en la base de datos mediante el código proporcionado (el paso 3 del documento "database creation.txt"), añadiendo un límite de filas a importar mediante la línea comentada, si así se desea.

4- Mover o copiar la carpeta "adiu-p1" obtenida al hacer el paso 1 en C:/xampp/htdocs.

5- Buscar en cualquier navegador: http://localhost/adiu-p1/
