Escribir un archivo en Python es una tarea igual de sencilla que leerlo,
a continuación el ejemplo:

```python
import csv

datos = [["Nombre", "Apellido", "Edad"], ["Ana", "Sevilla", "20"]]

with open('nombres.csv', 'w') as csv_file:
  writer = csv.writer(csv_file)
  writer.writerows(datos)
```

En la primera línea, y como lo hicimos en el ejercicio anterior, importamos
la librería csv, luego definimos una lista de listas, cada lista será una
fila dentro de nuestro archivo csv. Continuamos abriendo un archivo con 
las sentencias with y open, y le ponemos un alias al archivo que crearemos
en este caso nombres.csv. En las dos últimas líneas definimos un writer para
nuestro archivo y finalmente escribimos los datos que definimos en la lista
de listas.

