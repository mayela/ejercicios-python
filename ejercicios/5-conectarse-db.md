Para el siguiente ejercicio haremos uso de la librería sqlite3 para 
abrir una base de datos, a continuación coloco el código necesario 
para que lo pruebes tú mismo:

```python
import sqlite3

con = None
try:
  con = sqlite3.connect('store.db')
except sqlite3.Error:
  print("Error, la base de datos no puede ser abierta")
finally:
  if con:
    con.close()
```
