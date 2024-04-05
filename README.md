# Balanz - Desafío de Lógica!

Se tiene una matriz cuadrada de tamaño `n x n`, donde `n` está entre 2 y 20.
Además, se tiene una lista de comandos, donde cada comando puede ser `'IZQUIERDA'`, `'DERECHA'`, `'ARRIBA'`, o `'ABAJO'`. La longitud de la lista de comandos es mayor o igual que 2.

El objetivo es escribir una función que reciba dos parámetros:

1. `n`: El tamaño de la matriz cuadrada (un entero entre 2 y 20).
2. `commands`: Una lista que representa los comandos (`'IZQUIERDA'`, `'DERECHA'`, `'ARRIBA'`, `'ABAJO'`).

La posición inicial será la esquina superior izquierda de la matriz (posición 0).

La función debe retornar la posición final (número entero) donde se encontrará despues de ejecutar los comandos de la lista.

Si al ejecutar un comando de la lista, la nueva posición resultante quedara fuera de los límites de la matriz, ese comando deberá ser ignorado y no deberá modificar la posición actual.

---

Por ejemplo, si n = 4, la matriz estará numerada de la siguiente manera:

| 0   | 1   | 2   | 3   |
| --- | --- | --- | --- |
| 4   | 5   | 6   | 7   |
| 8   | 9   | 10  | 11  |
| 12  | 13  | 14  | 15  |

Ejemplos de comandos y posición final:

- `['DERECHA', 'ABAJO', 'IZQUIERDA', 'ARRIBA']`: la posición final sería 0.
- `['DERECHA', 'ABAJO', 'DERECHA', 'ABAJO']`: la posición final sería 10.
- `['DERECHA', 'ABAJO', 'IZQUIERDA', 'IZQUIERDA', 'ABAJO']`: la posición final sería 8.
- `['ABAJO', 'ABAJO', 'IZQUIERDA', 'ABAJO']`: la posición final sería 12.
