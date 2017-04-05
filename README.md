## Description

Golang on CentOS 7

## Build Docker Image

docker build -t golang_centos7 .

## Build app on Linux

```
cd [application directory]
docker run --rm -ti -v `pwd`:/app -p 9080:9080  -w /app charlestg/golang_centos7 bash
go build
```

## Build app on Cygwin

```
cd [application directory]
docker run --rm -ti -v "$(cygpath -w $PWD)":/app -p 9080:9080  -w /app charlestg/golang_centos7 bash
go build
```

