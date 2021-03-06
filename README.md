# IRC_Analysis
Dockerfiles para montar un cliente y servidor IRC de manera muy facil, con el fin de generar y analizar el trafico IRC generado por los mismos.
Por Pablo Ahumada y Joaquín Fernández.

## Instalación

Clona el directorio:
```sh
$ git clone https://github.com/ColaDuMacaco/IRC_Analisis_udp
```

Para instalar el servidor Inspircd:
```sh
$ docker build -t inspircd IRC_Analisis_udp/Servidor/
```

Para instalar el cliente Irssi:
```sh
$ docker build -t irssi IRC_Analisis_udp/Cliente/
```

Para instalar Polimorph:
```sh
$ docker build -t polymorph IRC_Analisis_udp/Polymorph/
```


## Uso

Crear un contenedor con la imagen del servidor:
```sh
$ docker run -it -p 6667:6667 --name servidorIRC inspircd
```

Crear un contenedor con la imagen del cliente:
```sh
$ docker run -it --name clienteIRC irssi
```

Crear un contenedor con la imagen de Polymorph
```sh
$ docker run --privileged -it --name Polymorph polymorph
```

## Video capturando trafico generado entre el servidor y cliente

[![Watch the video](https://img.youtube.com/vi/LIOw5wZKxmw/hqdefault.jpg)](https://youtu.be/LIOw5wZKxmw)

## Video Modificanco trafico IRC

[![Watch the video](https://img.youtube.com/vi/YPfMYmFvTxk/hqdefault.jpg)](https://youtu.be/YPfMYmFvTxk)

## Metricas de red en IRC

[![Watch the video](https://img.youtube.com/vi/zn3H9JhrvcU/hqdefault.jpg)](https://youtu.be/zn3H9JhrvcU)

## Detección de paquetes IRC maliciosos con Snort

[![Watch the video](https://img.youtube.com/vi/te29QGevanA/hqdefault.jpg)](https://youtu.be/te29QGevanA)


