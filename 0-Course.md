## 0) Install (https://go.dev/doc/install)

```
sudo tar -C /usr/local/ -xzf go1.19.3.linux-amd64.tar.gz
vim ~/.profile
source ~/.profile
go version
```

## 1) Hello World

```
go run Tutorial/hello-world.go
```

## 2) [Create module](https://go.dev/doc/tutorial/create-module)

```
mkdir greetings
cd greetings
go mod init example.com/greetings
```

## 3) [Call function from another module](https://go.dev/doc/tutorial/call-module-code)

```
mkdir hello
cd hello

go mod init example.com/hello
go mod edit -replace example.com/greetings=../greetings

go mod tidy

go run .
```

## 4) [Handle an error](https://go.dev/doc/tutorial/handle-errors)

## 5) [Return a random greeting](https://go.dev/doc/tutorial/random-greeting)

## 6) [Add a test](https://go.dev/doc/tutorial/add-a-test)

## 7) [Compile and install](https://go.dev/doc/tutorial/compile-install)

## 8) [More resources](https://go.dev/doc/tutorial/module-conclusion)

## 9) [Go Clean code](https://go.dev/doc/effective_go)

## 10) [First Server](https://www.youtube.com/watch?v=juVYPx0UG80)
