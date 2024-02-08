# Saludos en Go

Este paquete proporciona una forma simple de obtener saludos poersonalizados en Go

## Instalación

Ejecuta el siguiente comando para instalar el paquete:

```bash
go get -u github.com/RoboticNotes/greetings
```

##Uso
Aquí tienes un ejemplo de cómo utilizar el paquete en tu código:

```go
package main

import (
	"fmt"
	"log"
	"github.com/RoboticNotes/greetings"
)

func main() {
	log.SetPrefix("greetings: ")

	names := []string{"ulisses", "Cesar", "Brandon"}
	messages, err := greetings.Hellos(names)
	if err != nil {
		log.Fatal(err)
	}

	fmt.Println(messages)

}
```
