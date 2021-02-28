# go-example

En este readme, me descargo los ejemplos principales, los compilo y entrego las trazas de su compilación y ejecución. 

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

Purebo con linux y lo mismo, parece que hay que descargarse los proyectos y ejecutarlos.

- 2. Pruebo cada función:

- hello, works

 Directory of C:\Users\ablaz\PycharmProjects\go\example

```
02/27/2021  06:05 PM    <DIR>          .
02/27/2021  06:05 PM    <DIR>          ..
02/27/2021  06:05 PM    <DIR>          .git
02/27/2021  06:05 PM    <DIR>          appengine-hello
02/27/2021  06:05 PM               100 go.mod
02/27/2021  06:05 PM             2,452 go.sum
02/27/2021  06:05 PM    <DIR>          gotypes
02/27/2021  06:05 PM    <DIR>          hello
02/27/2021  06:05 PM            11,358 LICENSE
02/27/2021  06:05 PM    <DIR>          outyet
02/27/2021  06:05 PM             2,634 README.md
02/27/2021  06:05 PM    <DIR>          stringutil
02/27/2021  06:05 PM    <DIR>          template
               4 File(s)         16,544 bytes
               9 Dir(s)  50,116,382,720 bytes free

C:\Users\ablaz\PycharmProjects\go\example>cd hello

C:\Users\ablaz\PycharmProjects\go\example\hello>dir
 Volume in drive C has no label.
 Volume Serial Number is 289A-53B1

 Directory of C:\Users\ablaz\PycharmProjects\go\example\hello

02/27/2021  06:05 PM    <DIR>          .
02/27/2021  06:05 PM    <DIR>          ..
02/27/2021  06:05 PM               701 hello.go
               1 File(s)            701 bytes
               2 Dir(s)  50,116,186,112 bytes free

C:\Users\ablaz\PycharmProjects\go\example\hello>go run hello.go
Hello, Go examples!
```

- stringutil

```
 Directory of C:\Users\ablaz\PycharmProjects\go\example\stringutil

02/27/2021  06:05 PM    <DIR>          .
02/27/2021  06:05 PM    <DIR>          ..
02/27/2021  06:05 PM               883 reverse.go
02/27/2021  06:05 PM               888 reverse_test.go
               2 File(s)          1,771 bytes
               2 Dir(s)  50,119,602,176 bytes free

C:\Users\ablaz\PycharmProjects\go\example\stringutil>go run reverse.go
go run: cannot run non-main package
```

-  outyet : http://localhost:8080/, Is Go 1.4 out yet? YES!


- app engine, not in teh main package
```
 Directory of C:\Users\ablaz\PycharmProjects\go\example\appengine-hello

02/27/2021  06:05 PM    <DIR>          .
02/27/2021  06:05 PM    <DIR>          ..
02/27/2021  06:05 PM             1,041 app.go
02/27/2021  06:05 PM               887 app.yaml
02/27/2021  06:05 PM               432 README.md
02/27/2021  06:05 PM    <DIR>          static
               3 File(s)          2,360 bytes
               3 Dir(s)  50,106,765,312 bytes free

C:\Users\ablaz\PycharmProjects\go\example\appengine-hello>go run app.go
go run: cannot run non-main package
```

- y cómo usar go types y go doc?
