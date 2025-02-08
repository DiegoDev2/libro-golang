`sync`, `WaitGroup`
Los canales permiten la comunicación segura entre goroutines.

Ejemplo de canales:
```go
package main

import "fmt"

func main() {
	mensajes := make(chan string)

	go func() {
		mensajes <- "Hola desde una goroutine"
	}()

	fmt.Println(<-mensajes)
}

```

Ejemplo de `sync.WaitGroup` para esperar la ejecución de goroutines:

```go
package main

import (
	"fmt"
	"sync"
)

func tarea(wg *sync.WaitGroup) {
	defer wg.Done()
	fmt.Println("Ejecutando tarea")
}

func main() {
	var wg sync.WaitGroup

	wg.Add(2)
	go tarea(&wg)
	go tarea(&wg)

	wg.Wait()
	fmt.Println("Todas las tareas han finalizado")
}

```
