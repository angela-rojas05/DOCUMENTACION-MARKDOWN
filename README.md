# Tecnológico de Softwaare
## Actividad #16: Documentación de matrices
## Alumno: Ángela Yaritzi Rojas Brito
## Asignatura: Fundamentos de álgebra
## Maestro: Jorge Javier Pedroza Romero

---
# Objetivo 

Obtener un aprendizaje amplio y claro sobre las matrices, desde sus operaciones básicas hasta comprender los diferentes tipos.

---
# Ejercicio 1: Identifica el tipo de cada matriz

### a) 

$$A = \begin{bmatrix}
1 & 0 \\
0 & 1 
\end{bmatrix}$$

Esta es una **matriz de identidad** porque en la diagonal principal contiene solo el número 1, mientras que los otros elementos serán el número 0.

### b) 

$$ B = \begin{bmatrix}
3 & 0 & 0 \\
0 & -2 & 0 \\
0 & 0 & 5 
\end{bmatrix}  $$

La segunda es una **matriz diagonal** debido a que los elementos que estan dentro de ella son números aleatorios por asi decirlo, y el resto siempre serán el número 0.

### c)

$$C = \begin{bmatrix}
2 & 1 & 4 \\
1 & 3 & 5 \\
4 & 5 & 6 
\end{bmatrix}  $$

Esta es una **matriz simétrica** porque las filas se pueden repetir en las columnas, es decir, estan los mismos números acomodados en el mismo orden solo que unos estan en una fila y otros en una columna.

### d)

$$ D = \begin{bmatrix}
1 & 2 & 3 \\
0 & 4 & 5 \\
0 & 0 & 6 
\end{bmatrix}  $$

Corresponde a una **matriz triangular superior** ya que todos los elementos que se encuentran **por debajo** de la diagonal siempre serán ceros.

---

# Ejercicio 2: Calcula dada las matrices

$$ A = \begin{bmatrix}
2 & -1 \\
3 & 4 
\end{bmatrix}, \quad B = \begin{bmatrix}
5 & 2 \\
-1 & 3 
\end{bmatrix} $$

$$ A + B =
\begin{pmatrix}
1 + 9 & 2 + 10 & 3 + 11 \\
4 + 12 & 5 + 13 & 6 + 14 \\
\end{pmatrix}
$$

### a) \( A + B \)
$$ A + B = \begin{bmatrix}
2 + 5 & -1 + 2 \\
3 + (-1) & 4 + 3
\end{bmatrix} = \begin{bmatrix}
7 & 1 \\
2 & 7
\end{bmatrix} $$

### b) \(2A - B \)

$$ 2A = \begin{bmatrix}
2(2) & 2(-1) \\
2(3) & 2(4)
\end{bmatrix} = \begin{bmatrix}
4 & -2 \\    
6 & 8
\end{bmatrix} $$
$$ 2A - B = 2 \begin{bmatrix}
4-5 & -2-2 \\
6-(-1) & 8-3
\end{bmatrix} = \begin{bmatrix}
-1 & -4 \\
7 & 5
\end{bmatrix} $$

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







