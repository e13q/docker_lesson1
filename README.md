Контеиниризация [StaticJinjaPlus](https://github.com/MrDave/StaticJinjaPlus/tree/main).

## building commands for python-slim base

latest version:

```
docker build -f dockerfile.python-slim --build-arg VERSION=latest -t static-jinja-plus-slim:latest .
 ```

version 0.1.0:

```
docker build -f dockerfile.python-slim --build-arg VERSION=0.1.0 -t static-jinja-plus-slim:0.1.0 . 
```

version 0.1.1:

```
docker build -f dockerfile.python-slim --build-arg VERSION=0.1.1 -t static-jinja-plus-slim:0.1.1 .
```

## building commands for ubuntu base

latest version:

```
docker build -f dockerfile.ubuntu --build-arg VERSION=latest -t static-jinja-plus-ubuntu:latest .
```

version 0.1.0:

```
docker build -f dockerfile.ubuntu --build-arg VERSION=0.1.0 -t static-jinja-plus-ubuntu:0.1.0 .
 ```

version 0.1.1:

```
docker build -f dockerfile.ubuntu --build-arg VERSION=0.1.1 -t static-jinja-plus-ubuntu:0.1.1 .
 ```

## run example

```
docker run --rm -v C:\Users\e13\Desktop\dvmn\Docker\test2\templates_example:/app/templates_example -v C:\Users\e13\Desktop\dvmn\Docker\test2\out:/app/built/site -it --rm staticjinjaplus-ubuntu:0.1.1
```

or change docker compose file and use it like:

```
docker-compose up && docker-compose rm -fsv
```
