# traefik
Projeto teste para proxy reverse Traefik

## Requisitos
- Docker 
- Docker-compose
- Git

## Curso Traefik 
[codigofacilito](https://codigofacilito.com/cursos/traefik)

## Clone Project 
```console
$ git clone git@github.com:leonardodg/traefik.git
```

### Comandos

> Run Traefik
```console
$ docker-compose up -d
```

> Build imagem Dockerfile PHP:7.4
  "-t" TAG app  AND "." path folder ./docker
```console
$ docker build -t app . 
```


### Config

> Add Hosts file windows - After GET IP - Sample IP 127.0.0.1 AND HOST`s nginx.app.test,apache.app.test
```console
$ echo. && echo 127.0.0.1 nginx.app.test >> %WINDIR%\System32\Drivers\Etc\Hosts
$ echo. && echo 127.0.0.1 apache.app.test >> %WINDIR%\System32\Drivers\Etc\Hosts
```