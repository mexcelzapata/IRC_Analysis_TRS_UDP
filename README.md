
# IRC_Analysis_TRS_UDP
Dockerfiles para cliente y servidor IRC, por Pablo Ahumada y Joaquín Fernández 

## Instalación

Clona el directorio:
```sh
$ git clone https://github.com/ElSacoWeant/IRC_Analysis_TRS_UDP
```

Para instalar el servidor Inspircd:
```sh
$ docker build -t inspircd IRC_Analysis_TRS_UDP/Servidor/
```

Para instalar el cliente Irssi:
```sh
$ docker build -t irssi IRC_Analysis_TRS_UDP/Cliente/
```


## Uso
Crear un contenedor con la imagen del servidor:
```sh
$ docker run -it -p 6667:6667 --name servidorirc inspircd
```

Crear un contenedor con la imagen del cliente:
```sh
$ docker run -it --name clienteirc irssi
```



