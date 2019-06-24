Existe un gran numero de imagenes disponbibles para poder utilizar en [https://hub.docker.com](https://hub.docker.com/search?q=&type=image).

Se pide siempre utilizar las imagenes oficiales, (las que dicen: "Official Image" o "Verified Publisher"), en caso contrario revisar siempre el archivo `Dockerfile`. Si ese archivo no esta disponible para revisar, desconfiar inmediatamente de ese repositorio.

Para descargar una imagen al ambiente local, se utiliza el comando `docker pull [imagen]:[version]`. Como ejemplo descargaremos la imagen whalesay que solo se usa para mostrar un texto desde la linea de comandos: `docker pull docker/whalesay:latest`{{execute}}.

```bash
$ docker pull docker/whalesay:latest
latest: Pulling from docker/whalesay
e190868d63f8: Pull complete
909cd34c6fd7: Pull complete
0b9bfabab7c1: Pull complete
a3ed95caeb02: Pull complete
00bf65475aba: Pull complete
c57b6bcc83e3: Pull complete
8978f6879e2f: Pull complete
8eed3712d2cf: Pull complete
Digest: sha256:178598e51a26abbc958b8a2e48825c90bc22e641de3d31e18aaf55f3258ba93b
```

Podemos revisar que efectivamente la imagen se descargó al ambiente local con el comando `docker images`{{execute}}.

```bash
$ docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
docker/whalesay     latest              6b362a9f73eb        4 years ago         247MB
```

Podemos saber que el peso de la imagen es de 247MB y tenemos la version "latest".
