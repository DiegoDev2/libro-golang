#### **Uso de panic y recover**

- `panic`: Se usa cuando ocurre un error crítico del que el programa no puede recuperarse.
- `recover`: Permite recuperar la ejecución después de un `panic`, evitando que el programa se cierre abruptamente.
Ejemplo de `panic` y `recover`:
```go
package main

import "fmt"

func puedeFallar() {
	defer func() {
		if r := recover(); r != nil {
			fmt.Println("Recuperado de:", r)
		}
	}()
	panic("Ocurrió un error crítico")
}

func main() {
	fmt.Println("Iniciando programa")
	puedeFallar()
	fmt.Println("Programa finalizado correctamente")
}

```
