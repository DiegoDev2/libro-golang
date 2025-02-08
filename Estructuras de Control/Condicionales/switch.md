
Se usa para evaluar múltiples casos sin necesidad de escribir múltiples `if`.

**Ejemplo de `switch`:**
```go
package main

import "fmt"

func main() {
    dia := "lunes"

    switch dia {
    case "lunes":
        fmt.Println("Inicio de semana")
    case "viernes":
        fmt.Println("Casi fin de semana")
    default:
        fmt.Println("Es un día cualquiera")
    }
}
```
