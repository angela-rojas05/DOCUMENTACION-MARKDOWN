# Tecnológico de Software
## Actividad #18: Documentación de matrices dos
## Alumno: Ángela Yaritzi Rojas Brito
## Asignatura: Fundamentos de álgebra
## Maestro: Jorge Javier Pedroza Romero

---
# Objetivo 

Comprender de manera sólida el concepto de matrices y sus determinantes, incluyendo sus propiedades y la aplicación de operaciones básicas para su cálculo.

---
# Ejercicio 1: Calcula los determinantes

### 1.- 

$$ A =
\begin{pmatrix}
5 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

1. Identifica los elementos de la matriz
2. Multiplica los números de la diagonal principal: 5 * 1 = 5
3. Multiplica los números de la diagonal secundaria: 3 * (-2) = -6
4. Restamos ambos resultados, poniendo el positivo primero: 5 - 6 = -1
5. Por lo tanto, el resultado es: det(A) = -1

El determinante puede ser positivo, negativo o cero

### 2.-  

$$ B =
\begin{pmatrix}
-1 & 4 \\
2 & -8 \\
\end{pmatrix}
$$

1. Identifica los elementos de la matriz
2. Multiplica los números de la diagonal principal: (-1) * (-8) = +8
3. Multiplica los números de la diagonal secundaria: 2 * (-4) = -8
4. Restamos ambos resultados, poniendo el positivo primero: 8 - 8 = 0
5. Por lo tanto, el resultado es: det(B) = 0

Si det(A) = 0 , la matriz es singular (no tiene inversa)

### 3.- 

$$ C =
\begin{pmatrix}
6 & 9 \\
2 & 3 \\
\end{pmatrix}
$$

1. Identifica los elementos de la matriz
2. Multiplica los números de la diagonal principal: 6 * 3 = 18
3. Multiplica los números de la diagonal secundaria: 2 * (-9) = -18
4. Restamos ambos resultados, poniendo el positivo primero: 18 - 18 = 0
5. Por lo tanto, el resultado es: det(C) = 0

Si det(A) = 0 , la matriz es singular (no tiene inversa)
 
### 4.- 

$$ D =
\begin{pmatrix}
0 & 5 \\
-5 & 0 \\
\end{pmatrix}
$$

1. Identifica los elementos de la matriz
2. Multiplica los números de la diagonal principal: 0 * 0 = 0
3. Multiplica los números de la diagonal secundaria: (-5) * (5) * (-1) = 25
4. Restamos ambos resultados, poniendo el positivo primero: 25 - 0 = 25
5. Por lo tanto, el resultado es: det(D) = 25

Si det(A) NO ES IGUAL A 0 , la matriz es no singular (tiene inversa)

---

# Ejercicio 2: Usa Sarrus para calcular

### 1.-

$$ E =
\begin{pmatrix}
1 & 2 & 3\\
0 & 1 & 4\\
5 & 6 & 0\\
\end{pmatrix}
$$

1. Se dibuja una linea recta debajo de nuestra matriz y posterior a eso solo copiamos la fila 1 y dos asi como estan.

$$ E =
\begin{pmatrix}
1 & 2 & 3\\
0 & 1 & 4\\
5 & 6 & 0\\
\\
1 & 2 & 3\\
0 & 1 & 4\\
\end{pmatrix}
$$

2. Multiplicamos todas las diagonales 3x3 de arriba hacia abajo: 1 * 1 * 0 = 0, 0 * 6 * 3 = 0, 5 * 2 * 4 = 40. Total = 40
   
3. Multiplicamos todas las diagonales 3x3 de abajo hacia arriba: 5 * 1 * (-3) = -15, 1 * 6 * (-4) = -24, 0 * 2 * 0 = 0. Total = -39
   
4. Al final se hace la resta correspondiente, dejando de primer lugar el número positivo: 40 - 39 = 1

5. det(E) = 1

### 2.-

$$ F =
\begin{pmatrix}
2 & -1 & 3\\
1 & 4 & 0\\
3 & 2 & -2\\
\end{pmatrix}
$$

1. Se dibuja una linea recta debajo de nuestra matriz y posterior a eso solo copiamos la fila 1 y dos asi como estan.

$$ F =
\begin{pmatrix}
2 & -1 & 3\\
1 & 4 & 0\\
3 & 2 & -2\\
\\
2 & -1 & 3\\
1 & 4 & 0\\
\end{pmatrix}
$$

2. Multiplicamos todas las diagonales 3x3 de arriba hacia abajo: 2 * 4 * (-2) = -16, 1 * 2 * 3 = 6, 3 * (-1) * 0 = 0. Total = -10

3. Multiplicamos todas las diagonales 3x3 de abajo hacia arriba: 3 * 4 * (-3) = -36, 2 * 2 * 0 = 0, (-1) * 1 * (-2) * (-1) = -2. Total = -38

4. Al final se hace la resta correspondiente: -10 - 38 = -48

5. det(F) = -48


# Ejercicio 3: Calcula usando cofactores (expandir por la fila o columna más conveniente) 

### 1.- 

$$ G =
\begin{pmatrix}
1 & 0 & 2\\
-1 & 3 & 1\\
2 & 0 & 1\\
\end{pmatrix}
$$

1. A la primera columna se agrega un símbolo positivo y en la siguiente negativo, asi sucesivamente con todas las columnas.
   
2. Tomamos el +1 de la fila 1 y columna 1, tapamos los números que estan debajo de el y tomamos solo los restantes de las filas 2 y 3.

```
1 | 3 1 |
  | 0 1 |
```

3. Hacemos lo mismo con el 0, es decir, tapamos los números debajo de el y agarramos los restantes de la fila 2 y 3.

```
0 | -1 1 |
  | 2 1  |
```

4. Lo mismo con el +2, ahora solo con los números restantes que no esten debajo de el.

```
2 | -1 3 |
  | 2 0  |
```

5. Hacemos multiplicaciones cruzadas de los números dentro de la matriz, como al sacar determinante, solo que despues multiplicamos por el número de afuera.

```
1 | 3 1 | = 1 + 3 = 3, 0 * 1 = 0. ENTONCES: 1(3 - 0)
  | 0 1 |
```

```
0 | -1 1 | = -1 * 1 = -1, 2 * -1 = -2. ENTONCES: 0(-1-2)
  | 2 1  |
```

```
2 | -1 3 | = -1 * 0 = 0, 2 * -3 = -6. ENTONCES: 2(0-6)
  | 2 0  |
```

6. Juntamos y resolvemos, respetando signos

det(G) = 1(3-0) -0(-1-2) +2(0-6)
det(G) = 3 - 12
det(G) = -9

---


$$ G =
\begin{pmatrix}
1 & 0 & 2\\
-1 & 3 & 1\\
2 & 0 & 1\\
\end{pmatrix}
$$


### c) \( AB \)
$$ AB = \begin{bmatrix}
2\cdot5+(-1)\cdot(-1) & 2\cdot2+(-1)\cdot3\\
3\cdot5+4\cdot(-1)    & 3\cdot2+4\cdot3
\end{bmatrix} = \begin{bmatrix}
10 + 1 & 4 - 3\\
15 - 4 & 6 + 12
\end{bmatrix} = \begin{bmatrix}
11 & 1 \\
11 & 18
\end{bmatrix} $$

### d) \( BA \)
$$ BA = \begin{bmatrix}
(5\cdot2) + (2\cdot3) & (5\cdot-1) + (2\cdot4) \\
(-1\cdot2) + (3\cdot3) & (-1\cdot-1) + (3\cdot4)
\end{bmatrix} = \begin{bmatrix}
10 + 6 & -5 + 8 \\
-2 + 9 & 1 + 12
\end{bmatrix} = \begin{bmatrix}
16 & 3 \\
7 & 13
\end{bmatrix} $$

### e) \( A^T \)
$$ A^T = \begin{bmatrix}
2 & 3 \\
-1 & 4
\end{bmatrix} $$

---

# Ejercicio 3: Verifica que (AB)C = A(BC)

$$ A = \begin{bmatrix}
1 & 2 \\
3 & 4 
\end{bmatrix}, \quad B = \begin{bmatrix}
2 & 0 \\
1 & 3 
\end{bmatrix}, \quad C = \begin{bmatrix}
1 & 1 \\
0 & 2
\end{bmatrix} $$

### 1) Calcular la matriz de (AB)C

Para empezar hay que sacar el resultado de la multiplicación de AB para que despues el resultado se multiplique con C.

$$ AB = \begin{bmatrix}
(1\cdot2) + (2\cdot1) & (1\cdot0) + (2\cdot3) \\
(3\cdot2) + (4\cdot1) & (3\cdot0) + (4\cdot3)
\end{bmatrix} = \begin{bmatrix}
2 + 2 & 0 + 6 \\
6 + 4 & 0 + 12
\end{bmatrix} = \begin{bmatrix}
4 & 6 \\
10 & 12
\end{bmatrix} $$

$$ (AB)C = \begin{bmatrix}
(4\cdot1) + (6\cdot0) & (4\cdot1) + (6\cdot2) \\
(10\cdot1) + (12\cdot0) & (10\cdot1) + (12\cdot2)
\end{bmatrix} = \begin{bmatrix}
4 + 0 & 4 + 12 \\
10 + 0 & 10 + 24
\end{bmatrix} = \begin{bmatrix}
4 & 16 \\
10 & 34
\end{bmatrix} $$

### 2) Calcular la matriz de A(BC)

Ahora aqui debemos sacar primero el resultado de la multiplicación de BC y la matriz que obtengamos de ahi la vamos a multiplicar por la matriz de A, al final comparamos ambos resultados para saber si son o no iguales.

$$ BC = \begin{bmatrix}
(2\cdot1) + (0\cdot0) & (2\cdot1) + (0\cdot2) \\
(1\cdot1) + (3\cdot0) & (1\cdot1) + (3\cdot2)
\end{bmatrix} = \begin{bmatrix}
2 + 0 & 2 + 0 \\
1 + 0 & 1 + 6
\end{bmatrix} = \begin{bmatrix}
2 & 2 \\
1 & 7
\end{bmatrix} $$
$$ A(BC) = \begin{bmatrix}
(1\cdot2) + (2\cdot1) & (1\cdot2) + (2\cdot7) \\
(3\cdot2) + (4\cdot1) & (3\cdot2) + (4\cdot7)
\end{bmatrix} = \begin{bmatrix}
2 + 2 & 2 + 14 \\
6 + 4 & 6 + 28
\end{bmatrix} = \begin{bmatrix}
4 & 16 \\
10 & 34
\end{bmatrix} $$

### 3) Conclusiones

En base a los resultados obtenidos se puede comprobar que **(AB)C ES IGUAL QUE A(BC)** ya que contienen los mismos elementos, incluso en el mismo orden.

---







