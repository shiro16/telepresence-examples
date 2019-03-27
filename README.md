# telepresence-examples

## setup

see > https://www.telepresence.io/reference/install

## examples

### apply

```
$ kubectl apply -f ./
$ curl telepresence-example-svc-EXTERNAL-IP:3000
Telepresence Example 0.0.1
```

### local

```
$ telepresence --swap-deployment telepresence-example-deployment --run go run main.go
Telepresence Example local
```

### docker

```
$ telepresence --swap-deployment telepresence-example-deployment --docker-run shiro16/telepresence-examples:0.0.2
Telepresence Example 0.0.2
```

### cleanup

```
$ kubectl delete -f ./
```
