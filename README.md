# go-example

Descargarse los ejemplos principales, compilarlos y entregar las trazas de su compilación y ejecución. Escribo pq llevo dos hroas y no consgo sacrlo.

```
C:\Users\ablaz\PycharmProjects\go>go get github.com/golang/example/hello
go: downloading github.com/golang/example v0.0.0-20210113200257-bcf50bfd7dcd
go get: github.com/golang/example@none updating to
        github.com/golang/example@v0.0.0-20210113200257-bcf50bfd7dcd: parsing go.mod:
        module declares its path as: golang.org/x/example
                but was required as: github.com/golang/example

C:\Users\ablaz\PycharmProjects\go>go run hello
package hello is not in GOROOT (C:\Program Files\Go\src\hello)
```

- 1. Descargarse: go get y el paquete, pero salta este error
```
                   module declares its path as: golang.org/x/example
                but was required as: github.com/golang/example
```

Purebo con linux. Más que usar go get es descargarlo con clone y ejercutarlo, no?

- 2. CLonándolo el hello funciona pero el stirngotil se queja por main y el outyet no corre el puerto. Es sea juagad biena?

- hwo to depurate it

- hello works

- string says soemthign does not work

-  outyet : http://localhost:8080/, Is Go 1.4 out yet? YES!
