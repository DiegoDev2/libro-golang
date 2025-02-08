Las variables en Go se declaran con `var` y pueden ser de diferentes tipos. También se pueden definir con `:=` para inferencia de tipos.

**Ejemplo de variables:**
```go
package main

import "fmt"

func main() {
    var nombre string = "Diego"
    edad := 16
    fmt.Println("Nombre:", nombre, "Edad:", edad)
}

```
Las constantes se definen con `const` y su valor no puede cambiar.

**Ejemplo de constantes:**
```go
package main

import "fmt"

const PI = 3.1415

func main() {
    fmt.Println("El valor de PI es:", PI)
}
```
