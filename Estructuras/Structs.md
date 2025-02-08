Las `structs` son estructuras de datos personalizadas que permiten agrupar diferentes tipos de datos.

Ejemplo de una `struct` con un método:
```go
package main

import "fmt"

// Definición de la struct
type Persona struct {
	Nombre string
	Edad   int
}

// Método asociado a la struct
func (p Persona) Saludar() {
	fmt.Println("Hola, mi nombre es", p.Nombre, "y tengo", p.Edad, "años.")
}

func main() {
	p := Persona{"Diego", 16}
	p.Saludar()
}

```
