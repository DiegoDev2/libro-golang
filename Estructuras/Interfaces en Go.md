Las interfaces permiten definir comportamientos sin necesidad de implementarlos directamente.

Ejemplo de una interfaz en Go:
```go
package main

import "fmt"

// Interfaz
type Animal interface {
	HacerSonido()
}

// Implementación de la interfaz en un struct
type Perro struct{}

func (p Perro) HacerSonido() {
	fmt.Println("Guau guau")
}

func main() {
	var a Animal = Perro{}
	a.HacerSonido()
}

```
