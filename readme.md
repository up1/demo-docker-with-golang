## 1. Working with command line

```
$docker container run --rm -w /xxx -v $(pwd):/xxx golang:1.11.2-alpine3.8 go run hello.
```


```
$docker container run --rm -w /xxx -v $(pwd):/xxx golang:1.11.2-alpine3.8 go build -o ./app
$docker container run --rm -w /xxx -v $(pwd):/xxx golang:1.11.2-alpine3.8 ./app
```

### 2. Working with Dockerfile_dev

```
$docker image build -t demo -f Dockerfile_dev .
$docker container run --rm demo
```

### 3. Working with depedencies and testing

```
$docker image build -t demo -f Dockerfile_testing .
$docker container run --rm -t demo
```
