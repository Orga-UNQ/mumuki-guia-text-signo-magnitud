### De punta a punta

Necesitamos calcular cuál es el mínimo y máximo valor representable en este sistema. Pensemos en un sistema SM(3) y completemos una tabla asociando cadenas con sus valores:

| Cadena | Valor |
|---|---|
|000| 0 |
|001| 1 |
|010| 2 |
|011| 3 |
|100| -0 |
|101| -1|
|110| -2 |
|111| -3 |


Con este desarrollo eshaustivo podemos encontrar fácilmente que el minimo es -3 y el máximo es 3.

De manera general, vemos que el mínimo se construye con signo negativo y magnitud máxima, y que el máximo es el opuesto del primero. Es decir que el máximo es el valor absoluto del mínimo.

### Poniendo en práctica

¿Cual es el mínimo valor representable en el sistema SM(4)?