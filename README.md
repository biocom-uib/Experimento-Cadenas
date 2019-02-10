# Experimento-Cadenas

Información sobre una muestra sintética de 10000 cadenas de bases "a", "c", "g" y "t" para usar en la lección sobre contrastes de independencia y homogeneidad del testo AprenderR. El fichero LeemeGeneracionDatos.Rmd ha generado estas tablas y explica qué contienen. El resultado html de compilar este fichero R Markdown se puede leer [aquí](http://biocom-uib.github.io/Experimento-Cadenas).

Las direcciones de las tablas de datos que tenéis que usar para cargarlas en R son:

* "MuestraTotalBases.txt": https://raw.githubusercontent.com/biocom-uib/Experimento-Cadenas/master/MuestraTotalBases.txt
* "MuestraTipoAbases.txt": https://raw.githubusercontent.com/biocom-uib/Experimento-Cadenas/master/MuestraTipoAbases.txt
* "MuestraTipoBbases.txt": https://raw.githubusercontent.com/biocom-uib/Experimento-Cadenas/master/MuestraTipoBbases.txt
* "MuestraTipoCbases.txt": https://raw.githubusercontent.com/biocom-uib/Experimento-Cadenas/master/MuestraTipoCbases.txt

Para cargar una de ellas en un *data frame*, hay que instalar y cargar el paquete **RCurl** y usar la instrucción siguiente, entrando su url donde pone "aquí el url" (manteniendo las comillas) y dándole un *Nombre* adecuado al *data frame* resultante: 

```{r, eval=FALSE}
library(RCurl)
Nombre=read.csv(text=getURL("aquí el url"))
```

