# RouterSploit - Framework de Explotación para Dispositivos Embebidos

[![Python 3.6](https://img.shields.io/badge/Python-3.6-yellow.svg)](http://www.python.org/download/)
[![Build Status](https://travis-ci.org/threat9/routersploit.svg?branch=master)](https://travis-ci.org/threat9/routersploit)

El Marco de RouterSploit es un marco de explotación de código abierto dedicado a dispositivos integrados.

[![asciicast](https://asciinema.org/a/180370.png)](https://asciinema.org/a/180370)

Consiste en varios módulos que ayudan a las operaciones de pruebas de penetración:

* exploits - módulos que aprovechan las vulnerabilidades identificadas
* creds: módulos diseñados para probar las credenciales de los servicios de red.
* escáneres: módulos que verifican si un objetivo es vulnerable a cualquier explotación
* Carga útil: módulos que son responsables de generar cargas útiles para diversas arquitecturas y puntos de inyección
* genéricos - módulos que realizan ataques genéricos
# Instalacion

## Requerimientos

Required:
* future
* requests
* paramiko
* pysnmp
* pycrypto

Optional:
* bluepy - bluetooth low energy 

## Installation on Kali Linux

```
apt-get install python3-pip
git clone https://www.github.com/threat9/routersploit
cd routersploit
python3 -m pip install -r requirements.txt
python3 rsf.py
```

Bluetooth Low Energy support:
```
apt-get install libglib2.0-dev
python3 -m pip install bluepy
python3 rsf.py
```

## Installation on Ubuntu 18.04 & 17.10

```
sudo add-apt-repository universe
sudo apt-get install git python3-pip
git clone https://www.github.com/threat9/routersploit
cd routersploit
python3 -m pip install setuptools
python3 -m pip install -r requirements.txt
python3 rsf.py
```

Bluetooth Low Energy support:
```
apt-get install libglib2.0-dev
python3 -m pip install bluepy
python3 rsf.py
```


## Installation on OSX

```
git clone https://www.github.com/threat9/routersploit
cd routersploit
sudo python3 -m pip install -r requirements.txt
python3 rsf.py
```

## Running on Docker

```
git clone https://www.github.com/threat9/routersploit
cd routersploit
docker build -t routersploit .
docker run -it --rm routersploit
```

# Update


Actualice RouterSploit Framework a menudo. El proyecto está en desarrollo y los nuevos módulos se envían casi todos los días.

```
cd routersploit
git pull
```

# License


El Framework RouterSploit está bajo una licencia BSD.
Consulte [LICENCIA] (LICENCIA) para obtener más detalles.
