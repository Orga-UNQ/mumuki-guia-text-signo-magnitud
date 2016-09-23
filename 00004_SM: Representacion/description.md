### Siendo económicos

Así como para el caso de la interpretación aplicamos el mecanismo de BSS sobre los bits de la magnitud, en este caso buscamos aplicar el mecanismo de representación de BSS.

Entonces, a la hora de representar un número X:

* Signo: Si x>0 entonces b_(n-1)=0, si x<0 entonces  b_(n-1)=1
* Magnitud: Se representa |x| en BSS(n-1): usando el método de las divisiones sucesivas

Veamos un ejemplo de representación en SM(18)

1. Construir la cadena como en bss: Rbss(18)=10010
2. Completar los 7 bits de la magnitud: 0010010
3. Anteponer el signo: 0 0010010

Fácilmente, podemos ver el ejemplo de representación del **-18**: Rsm(-18)= ```10010010```

#### A practicar

¿Cuál es la representación del valor 63 en SM(8)?
