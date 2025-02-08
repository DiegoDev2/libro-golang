Go tiene varios tipos de datos, divididos en:

 **Primitivos:**

- `int`, `float64`, `bool`, `string`
- `rune` (carácter Unicode), `byte` (alias de `uint8`)

**Compuestos:**

- Arrays, Slices, Structs, Maps

**Ejemplo de diferentes tipos de datos:**
```go
package main

import "fmt"

func main() {
    var entero int = 42
    var decimal float64 = 3.14
    var texto string = "Hola, Go"
    var booleano bool = true

    fmt.Println(entero, decimal, texto, booleano)
}

```

