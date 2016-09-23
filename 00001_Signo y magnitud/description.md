En el sistema decimal se utiliza el caracter “-” para representar los números negativos. Entonces, ¿cómo es posible “simular” el signo en una computadora? Reservando un bit para eso! 
¿Y qué significado tiene ese bit?

* Si bit=0 entonces el número representado es mayor a cero
* Si bit=1 entonces el número representado es menor a cero

Por ejemplo, si se tiene cadenas de 8 bits, podría definirse que el signo está en el extremo derecho o el extremo izquierdo de la cadena. Supongamos lo siguiente:

| Sig | Magnitud |
|-----|-----|
| 1 bit | 7 bits |


### Interpretación en Signo Magnitud

En un sistema **Signo-Magnitud de n bits**, denotado **SM(n)**, la magnitud puede verse como una cadena en **BSS(n-1)**, y entonces puede interpretarse de esa manera. 

Veamos un ejemplo, interpretando la cadena ```01010101``` en SM(8):
1. Signo: positivo (```0```)
2. Magnitud = Ibss(1010101) = 2^6 + 2^4 + 2^2 + 2^0 = 64 + 16 + 4 + 1


### A trabajar

¿Cuál es la interpretación de la cadena ```10000001```?