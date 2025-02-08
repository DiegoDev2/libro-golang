#### **Introducción a Goroutines**

Las **goroutines** son hilos de ejecución ligeros que permiten ejecutar funciones de manera concurrente.

Ejemplo de una goroutine:
```go
package main

import (
	"fmt"
	"time"
)

func decirHola() {
	fmt.Println("Hola desde una goroutine")
}

func main() {
	go decirHola() // Se ejecuta en una goroutine
	time.Sleep(time.Second) // Espera para que la goroutine termine
	
}

```
