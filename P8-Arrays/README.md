## Asignación y acceso a un índice

```go
a[4] = 100
fmt.Println("set:", a)
fmt.Println("get:", a[4])
```

* Se asigna el valor `100` en la posición `4`.
* Luego se imprime el array completo y el valor en el índice `4`.

---

## Longitud del array

```go
fmt.Println("len:", len(a))
```

* La función `len` devuelve la **longitud del array**, en este caso `5`.

---

## Declaración con valores iniciales

```go
b := [5]int{1, 2, 3, 4, 5}
fmt.Println("dcl:", b)
```

* Se declara e inicializa un array de 5 enteros.

---

## Uso de `[...]` para inferir tamaño

```go
b = [...]int{1, 2, 3, 4, 5}
fmt.Println("dcl:", b)
```

* El compilador infiere el tamaño del array a partir del número de elementos.

---

## Inicialización por índice

```go
b = [...]int{100, 3: 400, 500}
fmt.Println("idx:", b)
```

* Se inicializa un array usando índices específicos:

  * Posición `0`: 100
  * Posición `3`: 400
  * Posición `4`: 500
* Resultado: `[100 0 0 400 500]`

---

## Arrays bidimensionales

```go
var twoD [2][3]int
for i := range 2 {
    for j := range 3 {
        twoD[i][j] = i + j
    }
}
fmt.Println("2d: ", twoD)
```

* Se crea un array de **2 filas y 3 columnas** (`[2][3]int`).
* Cada celda se llena con la suma de sus índices.
* Resultado: `[[0 1 2] [1 2 3]]`

---

## Inicialización directa de un array 2D

```go
twoD = [2][3]int{
    {1, 2, 3},
    {1, 2, 3},
}
fmt.Println("2d: ", twoD)
```

* Se inicializa manualmente el array 2D.
* Resultado: `[[1 2 3] [1 2 3]]`

---

# Conclusión

* Los **arrays en Go** son de tamaño fijo.
* Pueden inicializarse vacíos, con valores o usando índices.
* También se pueden anidar para crear arrays multidimensionales.
  """)
