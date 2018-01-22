Ahora veremos como podemos escribir en un archivo haciendo uso de la librería
openpyxl

```python
from openpyxl import Workbook

frutas = Workbook()
frutas_uno = frutas.active
frutas_uno['A2'] = "Pera"
frutas.save('frutas.xlsx')
```

En la primera línea importamos de la librería el objeto Workbook, a 
continuación instaciamos el objeto y luego, en la tercera línea obtenemos
la hoja activa del archivo que en este momento aún no está guardado. 
Seguido de esto escribimos un valor en la celda A2 y finalmente 
guardamos el archivo con el nombre frutas.xlsx.


