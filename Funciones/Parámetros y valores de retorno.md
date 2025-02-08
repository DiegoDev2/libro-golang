Las funciones pueden recibir parámetros y devolver valores.

**Ejemplo con parámetros y retorno:**
```go
package main

import "fmt"

func sumar(a int, b int) int {
    return a + b
}

func main() {
    resultado := sumar(5, 3)
    fmt.Println("Suma:", resultado)
}

```

Go también permite devolver múltiples valores.

```go
package main

import "fmt"

func dividir(dividendo, divisor int) (int, int) {
    cociente := dividendo / divisor
    residuo := dividendo % divisor
    return cociente, residuo
}

func main() {
    c, r := dividir(10, 3)
    fmt.Println("Cociente:", c, "Residuo:", r)
}

```
