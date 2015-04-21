#Introducción

El objetivo de este ejemplo es de familiarizarse con el ambiente de **R - project**, así como el de poder realizar gráficas con el paquete **lattice**. Al final de esta introducción sabrás realizar satisfactoriamente gráficas sofisticadas de una forma muy sencilla.

## Directorio de trabajo

El directorio de trabajo o *Work Directory* en **R - project** es en donde tu decides trabajar con los datos, es decir, la dirección de la **carpeta** donde se encuentran todos los archivos (datos). Por default el directorio de **R - Project** es en **Documentos**. Para verificar el directorio de trabajo, escribe el comando en la **consola** de **R**:

````{r}
getwd()
````
Éste te arrojará el directorio de trabajo, en mi caso el directorio es el siguiente:

````{r}
[1] "C:/Users/Vic/Documents"
````
### Cambio de directorio de trabajo

Para poder usar tus datos es necesario cambiar el directorio (salvo que quieras guardar todos los archivos en el directorio que está por Default). Existen dos maneras de cambiar el directorio de trabajo:   

1. Ésta manera consiste en realizar el cambio directamente de la GUI de **R - Project**
  + Ve a **File**  
  + **Change Dir...**
  + Selecciona la carpeta en donde se encuentran tus archivos a analizar

2. La segunda forma es un poco mas complicada, ya que tu especificas manualmente la dirección en donde se encuentran tus archivos. Esto es recomendado cuando ya se tiene un *script* y se indica al inicio del programa para que automaticamente **R** sepa en donde están los datos con los que se trabajará.

  + Un ejemplo de especificación manual del directorio en *R* se vería de esta manera:

````{r}
setwd("C:/Users/Vic/Documents/Tu_carpeta_de_datos")
````
## Cargar los datos

Antes de poder realizar cualquier gráfica es necesario cargar los datos; en este ejemplo se cargaron los datos en formato **.csv**, no obstannte **R - Project** puede cargar los datos de una variedad de formatos tales como: **.txt**, **.xlsx**, **.json** por mencionar algunos.

Los datos de la prueba se pueden descargar de este [link] (https://www.dropbox.com/s/w5baas7f2b0wptm/Prueba_12_Abril_2015.csv?dl=0). Asegurate de guardarlos en la carpeta donde es tu directorio de trabajo.

El código en **R** se debe de ver de esta manera:

````{r}
dat <- read.csv("Prueba_12_Abril_2015.csv", header =TRUE)
````
Para verificar si se cargaron satisfactoriamente los datos, se puede utilizar la funcion **head**, que en **R** quedaria de la siguiente manera:

````{r}
head(dat)
````
dando como resultado las primeras observaciones del conjunto de datos.

## Preproceso de datos

