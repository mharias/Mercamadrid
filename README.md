# Mercamadrid
Hemos preparado un [código](https://github.com/mharias/Mercamadrid/blob/main/code/evolucion_precios.ipynb) para bajar datos de la actividad comercial de mayoristas en Mercamadrid. Estos datos se pueden bajar desde este [link](https://datos.madrid.es/sites/v/index.jsp?vgnextoid=a4df993ae322b610VgnVCM1000001d4a900aRCRD&vgnextchannel=374512b9ace9f310VgnVCM100000171f5a0aRCRD) del [portal de datos abiertos del Ayuntamiento de Madrid](https://datos.madrid.es/portal/site/egob)

La información esta estructura en una serie de campos tales como:
  * Fecha inicial del segmento de tiempo al que se refieren los datos
  * Fecha final del segmento de tiempo al que se refieren los datos
  * Descripción de la mercancia
  * Código de la mercancia
  * Origen de la mercancia
  * Código de este origen
  * Peso de la mercancia en Kilos
  * Precio mínimo registrado
  * Precio máximo registrado
  * Precio más frecuente

He intentado  minimizar el tamaño del pandas con el modelo propuesto por @mattharrison, estoy haciendo un esfuerzo para seguir el "chaining" siempre que sea posible.

Presentamos el código necesario para bajar la información desde su respositorio en datos Madrid, y preparamos una rejilla de datos con los mismos..
En cada subgráfica, una por cada producto, presentamos la evolución del consumo como barras (eje "y" izquierda) )y la evolución de precios (eje "y" derecha). Para claridad se han codificado las barras según temperatura del mes..

![](https://github.com/mharias/Mercamadrid/blob/main/img/evolucion_consumo_precio.png)
