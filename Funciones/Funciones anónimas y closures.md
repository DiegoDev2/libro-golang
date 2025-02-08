### **Funciones anónimas**

Son funciones sin nombre, útiles para operaciones rápidas.

```go
package main

import "fmt"

func main() {
    anonima := func() {
        fmt.Println("Soy una función anónima")
    }

    anonima() // Llamando la función anónima
}

```

### **Closures**

Las closures pueden capturar variables del entorno en el que se definen.
```go
package main

import "fmt"

func contador() func() int {
    count := 0
    return func() int {
        count++
        return count
    }
}

func main() {
    next := contador()
    fmt.Println(next()) // 1
    fmt.Println(next()) // 2
}

```
