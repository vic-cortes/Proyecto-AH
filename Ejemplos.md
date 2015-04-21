#Introduccion

El objetivo de este ejemplo es el de familiarizarce con el ambiente de **R - project** asi como el poder realizar graficas con el paquete **lattice**. Al final de esta introduccion sabras realizar satisfactoriamente graficas sofisticadas de una forma muy sencilla.

## Adquisicion de datos

Antes de poder realizar cualquier grafica es necesario cargar los datos, en este ejemplo se cargaron los datos en formato **.csv**, no obstannte **R - Project** puede cargar los datos de una variedad de formatos *.txt*, *.xlsx*, *.json* por mencionar algunos.

El codigo en **R** se debe de ver de esta manera:

````{r}
dat <- read.csv("Prueba_12_Abril_2015.csv", header =TRUE)
````
