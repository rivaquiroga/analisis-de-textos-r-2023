# Análisis de texto con R

En este módulo del [Diplomado en Ciencia de Datos UC](https://datascience.uc.cl/) nos aproximaremos al análisis de textos usando R. Abordaremos algunas técnicas que se enmarcan en lo que usualmente se denomina _Minería de texto_ y otras propias del _Procesamiento del Lenguaje Natural_. Existe una sección paralela en la que abordamos casi los mismos contenidos, pero [usando Python](https://github.com/rivaquiroga/analisis-de-texto-python-2023).

## Preparación


### Primera sesión

Para realizar las actividades planificadas para la primera sesión necesitarás una versión reciente de R (> 4.1), los paquetes contenidos en el Tidyverse y el paquete **guaguas**. Puedes instalarlos con la siguiente línea de código:

```
install.packages("tidyverse")
install.packages("guaguas")
```

### Segunda sesión

Durante esta sesión ocuparemos los siguentes paquetes (además de los instalados en la sesión anterior):

```
install.packages(c("pdftools", "tokenizers", "SnowballC", "udpipe", "tidytext", "wordcloud"))
```

Hay personas que trabajan con Windows a las que a veces el paquete **pdftools** no les funciona correctamente porque sus computadores requieren que se instale además una herramienta llamada [Poppler](https://poppler.freedesktop.org/). Si ese es el caso, hay dos opciones: trabajar en [Posit Cloud](https://posit.cloud) durante esta sesión o utilizar el "plan B" que se indicará en clases (básicamente, descargar el objeto que crearemos usando una función de pdftools). 

### Tercera sesión

Durante esta sesión ocuparemos los siguentes paquetes (además de los instalados en las sesiones anteriores):

```
install.packages(c("quanteda", "quanteda.textplots", "quanteda.textstats", "topicmodels", "broom"))
```

## Actividades 

Durante las tres sesiones del módulo realizaremos una serie de actividades para poner en práctica lo aprendido. Iremos escribiendo el **código "en vivo"** en la clase, por lo que el contenido de los archivos con código se irá actualizando a medida que escribamos en ellos. Si bien las actividades de la sección presencial y online son las mismas, es posible que avancemos a un ritmo distinto o que el código difiera un poco producto de cómo se da la discusión en clases. 


🖥️ [materiales sección online](https://github.com/rivaquiroga/analisis-de-textos-r-2023/blob/main/actividades-online.md)

🏢 [materiales sección presencial](https://github.com/rivaquiroga/analisis-de-textos-r-2023/blob/main/actividades-presencial.md)


Todo el código que escribamos en clases asumirá que estás trabajando en un "projecto" de RStudio que tiene una subcarpeta para guardar el código y otra para guardar los datos. Crearemos esta estructura de carpetas durante la primera sesión, así que no es necesario que lo hagas con anticipación.

```
📂 analisis-texto-r
    |
    |-- 📁 codigo
    |-- 📁 datos
    |-- 🔵 analisis-texto-r.Rproj
```

## Recursos adicionales

### Documentación librerías utilizadas
- [stringr](https://stringr.tidyverse.org/index.html)
- [Hoja de referencia del paquete stringr en español](https://github.com/rstudio/cheatsheets/blob/main/translations/spanish/strings_es.pdf)
- [Quanteda](https://tutorials.quanteda.io/)

### Sobre expresiones regulares

- [regex101](https://regex101.com/): un sitio web para probar nuestras expresiones regulares
- [Hoja de referencia de la sintaxis de expresiones regulares](https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Regular_expressions/Cheatsheet)

### Libros, artículos y tutoriales en línea

- [AnalizaR datos Políticos](https://arcruz0.github.io/libroadp/)
- [Programming Historian (tutoriales en línea)](http://programminghistorian.org/es/)
- [Text Mining with R](https://www.tidytextmining.com/)
- [Supervised Machine Learning for Text Analysis](https://smltar.com/)
- [Probabilistic Topic Models](http://www.cs.columbia.edu/~blei/papers/Blei2012.pdf)
