Para leer un archivo Excel haremos uso de una librería externa llamada
openpyxl, a continuación coloco la insttrucción para realizar la
instalación de la misma:

```
pip3 install openpyxl
```

Ya con la librería instalada realizaremos el ejercicio de lectura de un
archivo.

Verifica que en la raíz del directorio se encuentre el archivo products.xlsx

```python
import openpyxl

excel_file = openpyxl.load_workbook('products.xlsx')

excel_file.worksheets
excel_file['Hoja1']['A1'].value
```

Con la primera línea importamos la librería que instalamos en el paso
anterior, a continuación cargamos el archivo excel, con la siguiente
instrucción checamos las hojas que contiene y finalmente en la
última línea leemos el contenido de una celda.


