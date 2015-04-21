#Introducción

El objetivo de este ejemplo es de familiarizarse con el ambiente de **R - project** así como el de poder realizar gráficas con el paquete **lattice**. Al final de esta introducción sabrás realizar satisfactoriamente gráficas sofisticadas de una forma muy sencilla.

## Directorio

El directorio en **R - project** es en donde tu decides trabajar con los datos, es decir, la direccion de la **carpeta** donde se encuentran todos los archivos (datos). Por default el directorio de **R - Project** es en **Documentos** de tu computadora. Para poder verificar tu directorio de trabajo, escribe lo siguiente en la **consola** de **R**:

````{r}
getwd()
````
Esta te arrojara tu directorio de trabajo, en mi caso mi directorio es el siguiente:

````{r}
[1] "C:/Users/Vic/Documents"
````

## Cargar los datos

Antes de poder realizar cualquier gráfica es necesario cargar los datos; en este ejemplo se cargaron los datos en formato **.csv**, no obstannte **R - Project** puede cargar los datos de una variedad de formatos tales como: *.txt*, *.xlsx*, *.json* por mencionar algunos.

El código en **R** se debe de ver de esta manera:

````{r}
dat <- read.csv("Prueba_12_Abril_2015.csv", header =TRUE)
````
