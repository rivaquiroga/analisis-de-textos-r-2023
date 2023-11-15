## Materiales actividades sección presencial

### Ejercicio 1: el mágico mundo de las expresiones regulares

:page_facing_up: [Código escrito en clases](https://www.dropbox.com/scl/fi/m7mwpcjgiejhbtetsp792/01_regex.R?rlkey=w7izz5z8jvvi48lsblysbvxpu&dl=0)


#### Desafío de práctica
A continuación encontrarás dos archivos CSV (separados por `;`) en que la forma en que se escribieron los nombres de las personas no coinciden: en uno aparecen como "Nombre Apellido" y en el otro como "Apellido, Nombre".

:card_file_box: [Datos matemáticas](https://www.dropbox.com/scl/fi/0r0m3ttp5cagybvk5quhu/matematicas.csv?rlkey=5xddjevkgl0zd2dc7pzxpbweo&dl=0)

:card_file_box: [Datos lenguaje](https://www.dropbox.com/scl/fi/zoh7n0mfhh51539rtmpl6/lenguaje.csv?rlkey=ah9tekr76iwiymm11vo5kdknm&dl=0)

Si utilizamos algún tipo de join para unir ambos dataframes, R no podrá hacer que coincidan las filas (es decir, que cada persona esté en una sola fila y tenga una columna para el puntaje de matemáticas y otra para el puntaje de lenguaje) porque, tal como están los datos, no tiene cómo saber que las dos formas de escribir el nombre corresponden a la misma persona. Para resolver el problema es necesario utilizar una expresión regular que te permita capturar grupos dentro de una cadena de caracteres.

Hay dos aproximaciones para resolver el problema:
 - Separar apellido y nombre en columnas distintas en ambos dataframes y luego hacer el merge con esas dos columnas como elemento común.
 - Modificar la columna "estudiante" en uno de los dataframes para que el formato coincida con la forma en que se escribieron los nombres en el otro.

:sparkles: [Solución]() (¡pronto!)


### Ejercicio 2: Extracción de texto de un archivo en PDF + limpieza y preprocesamiento

📄 [Código escrito en clases](﻿https://www.dropbox.com/scl/fi/q60c0f5mzgholj3igtxgm/02_extraccion-preprocesamiento.R?rlkey=gkcf7vnlx9ll32js1c6pdgkoc&dl=0)

🗣️ [Ejemplo de archivo PDF](https://www.dropbox.com/scl/fi/7ubt6pceaw4hxfxgy75f7/20140521.pdf?rlkey=ggnx71ufih6jbtnlmf1nglvv6&dl=0)

🔡 [Ejemplo de lista de "stopwords" en español](https://raw.githubusercontent.com/7PartidasDigital/AnaText/master/datos/diccionarios/vacias.txt)
