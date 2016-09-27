### Sumar es humano... restar es divino

Aprovechando que el sistema Signo-Magnitud permite calcular el **opuesto aditivo de cualquier cadena**, con la simple operación de invertir el bit de signo, es posible transformar cualquier resta en... una suma!

Veamos: ```A - B = A + inv(B)```, donde ```inv(B)``` es el opuesto aditivo.

De esta manera, vemos el algoritmo de la resta consiste en:

1. Invertir el signo del sustrendo (segundo operando)
2. Proceder como una suma de cadenas.


Veamos un ejemplo en SM(4):  ```1001-1110```

1. Se invierte el signo del segundo operando: ```0 110```
2. Se suma: ```1 001 + 0 110```. Como son diferentes signos:
  * Se restan las magnitudes: ```110-001=101```
  * Se aplica el signo de la magnitud mayor: ```0 101```
  

### Poniendo en práctica

¿Cuál es el resultado de ```0001-0110```?