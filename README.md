# GO

## Checar si si se instalo

>go version

## Compilacion Basica

> go buiild test.go

## Para compilar un archivo y hacelo mas ligero

> go build  -ldflags "-s -w" .

> upx brute chisel

## Compilacion cruzada

Muestra la lista de sistemas operativos y arquitecturas para los cuales se puede compilar

>go tool dist list


### GOOS

En Go, estos sistemas operativos son posibles valores para la variable de entorno GOOS, que se pronuncia como “goose” y significa Go Operating System (Sistema operativo GO).

### GOARCH

GOARCH. Esto se pronuncia como “gore-ch” y significa Go Architecture (Arquitectura de Go).

***Estas dos variables se usan para compilar desde ubuntu un programa que correra en windows***

### Compilacion cruzada comandos

> GOOS=windows GOARCH=386 go build


## go build vs go install:
go build just compiles the executable file and moves it to the destination. go install does a little bit more. It moves the executable file to $GOPATH/bin and caches all non-main packages which are imported to $GOPATH/pkg. The cache will be used during the next compilation provided the source did not change yet.

Fuente:https://stackoverflow.com/questions/24069664/what-does-go-install-do



