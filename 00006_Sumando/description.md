### Como sumamos en papel... casi

Recordemos cómo realizamos la suma “en papel”. Para eso analizamos los signos y luego operamos con las magnitudes. Por ejemplo: 

* 5+3: Fácil, el resultado es 8
* 5+ (-3) como son diferentes los signos, restamos: 5-3 

Pero también veamos otros casos:

* -5+3 también son signos diferentes, restamos: 5-3 pero ponemos signo negativo ¿por qué?? Porque usamos el signo del número de mayor magnitud
* (-5) +(-3): Es fácil tb, sumamos las magnitudes y ponemos el signo (que coincide): -8

Estamos preparados para generalizar lo anterior mediante el siguiente algoritmo

* Si alguno de los dos operandos es cero, el resultado será el otro operando.
* Si los signos son iguales (ambos 0 o ambos 1), el resultado tendrá el mismo signo y sumaremos las magnitudes usando la suma de BSS de (N-1) bits.
* Si los signos son diferentes, debemos identificar cual de los dos operandos tiene la magnitud mayor.
  * Si las dos magnitudes son iguales, el resultado será cero.
  * Si no, el signo del resultado será el signo del operando que tiene la magnitud mayor y la magnitud del resultado se obtendrá restando en BSS de (N-1) bits la magnitud menor de la magnitud mayor.

Veamos cómo se aplica este algoritmo en cadenas del sistema Signo-Magnitud

#### Un ejemplo con igual signo

Por ejemplo, sumemos las cadenas ```0001 + 0110```. Al ser signos iguales se suman solamente las magnitudes: ```001 + 110=111```. Además se debe usar el mismo signo, entonces se obtiene: ```0111```

Veamos si lo que hicimos es correcto, interpretando operandos y resultado:

* I(0001)=1
* I(0110)=6
* I(0111)=7


#### Un ejemplo con diferente signo
Por ejemplo, sumemos las cadenas ```1001 + 0110```. Como los signos son diferentes, se analiza por separado:

* Signo: debe ser el de la mantisa con mayor magnitud. En este caso ```0110```
* Magnitud: Es una resta entre magnitudes. En este caso: ```110-001=101```



### Poniendo en práctica

¿Cual es la cadena resultante de la suma ```0001 + 1110```?
