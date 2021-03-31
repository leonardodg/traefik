# traefik
Projeto teste para proxy reverse Traefik

## Requisitos
- Docker 
- Docker-compose
- Git
- mkcert

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
$ echo. && echo 127.0.0.1 app.test >> %WINDIR%\System32\Drivers\Etc\Hosts
$ echo. && echo 127.0.0.1 nginx.app.test >> %WINDIR%\System32\Drivers\Etc\Hosts
$ echo. && echo 127.0.0.1 apache.app.test >> %WINDIR%\System32\Drivers\Etc\Hosts
```

### Link's Traefik

[Dashboard] -> http://app.test:8080/dashboard/#/ \
[API] - > http://app.test:8080/api/rawdata \
[Nginx] -> http://nginx.app.test/ \
[Apache] -> http://apache.app.test/ \

### Mkcert

- Link Install mkcert -> https://github.com/FiloSottile/mkcert

> If it's the firt install of mkcert, run
```console
$ mkcert -install
```

> Generate certificate for domain "docker.localhost", "domain.local" and their sub-domains
```console
$ mkcert -cert-file certs/local-cert.pem -key-file certs/local-key.pem  app.test "*.app.test" apache.app.test nginx.app.test localhost 127.0.0.1 ::1
```

# License
MIT