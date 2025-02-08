Go solo tiene un tipo de bucle: **`for`**, pero se usa de diferentes maneras.

### **`for` clásico**

Se usa para ejecutar un bloque de código un número determinado de veces.

**Ejemplo:**
```go
package main

import "fmt"

func main() {
    for i := 0; i < 5; i++ {
        fmt.Println("Iteración:", i)
    }
}

```

### **`for` como `while`**

Si omites la inicialización y el incremento, puedes hacer un bucle tipo `while`.

```go
package main

import "fmt"

func main() {
    num := 0

    for num < 5 {
        fmt.Println("Número:", num)
        num++
    }
}

```

### **`for range`**

Se usa para recorrer arrays, slices, maps o strings.
```go
package main

import "fmt"

func main() {
    numeros := []int{10, 20, 30}

    for indice, valor := range numeros {
        fmt.Println("Índice:", indice, "Valor:", valor)
    }
}

```
