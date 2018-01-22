En la raíz de este directorio encontrarás un archivo csv llamado
swimming_pools.csv, lo utilizaremos para mostrar como se puede
abrir un archivo csv en Python. A continuación el código:

```python
import csv

with open('swimming_pools.csv') as csv_file:
    csv_reader = csv.reader(csv_file, delimiter=',')
    for row in csv_reader:
      print(', '.join(row))
```

En la primera línea lo que hacemos es importar la librería _csv_, 
siguiente a esto abrimos el archivo y el asignamos un nombre
_alias_. Luego declaramos el _lector_ del archivo csv, finalmente,
mediante el uso del ciclo for recorremos las filas del archivo
que para este momento se han vuelto una lista de Python, para
mostrar el contenido en un formato con comas hacemos uso de
la instrucción join.
