Los operadores en Go se dividen en:

**Aritméticos**: `+`, `-`, `*`, `/`, `%`  
**Comparación**: `==`, `!=`, `>`, `<`, `>=`, `<=`  
**Lógicos**: `&&`, `||`, `!`  
**Asignación**: `=`, `+=`, `-=`, `*=`, `/=`  
**Bitwise**: `&`, `|`, `^`, `<<`, `>>`

```go
package main

import "fmt"

func main() {
    a, b := 10, 5

    fmt.Println("Suma:", a+b)
    fmt.Println("Multiplicación:", a*b)
    fmt.Println("Mayor que:", a > b)
    fmt.Println("AND lógico:", (a > 5) && (b < 10))
}

```
