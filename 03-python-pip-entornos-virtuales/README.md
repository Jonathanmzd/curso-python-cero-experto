## Curso de Python: PIP y Entornos Virtuales

### Python en tu propio entorno de desarrollo local

![Alt text](image.png)

![Alt text](image-1.png)

![Alt text](image-2.png)

### Instalación en Windows (WSL) y Linux

Instalacion de WSL

1) PowerShell con permisos de administrador
2) comando para ver las distribuciones

```bash
 wsl --list --online
```

![Alt text](image-3.png)

3) instalar la distribucion que se quiere este caso ubuntu

![Alt text](image-4.png)

4) instala ubuntu asignar el user y pass en linux

![Alt text](image-5.png)

username: mized

5) comando para revisar las versiones instaladas
   
```bash
# listado 
 wsl --list

# ver la version en concreto
wsl -l -v
```
![Alt text](image-6.png)

![Alt text](image-7.png)

6) si ubuntu no esta con la version 1 

```bash
# Instalar Ubuntu 2
 wsl --set-version Ubuntu 2

# actualizar el kerner
wsl --update

# nuevamente la install Ubuntu 2

# para revisar el estado de lo instalado
wsl --status
```

7) ingresar a la terminal 

![Alt text](image-8.png)

![Alt text](image-9.png)



Python ya se encuentra instalado en wsl para comprovar desde la terminal de Ubuntu colocar python3 nos brindara la informacion.

![Alt text](image-10.png)

Comandos Utilizados

```bash
python

# interprete de python
python3

# para salir de la interfaz de python
exit()
```

Instalación

```bash
apt update

sudo apt update

sudo apt -y upgrade
```

```bash
# Verificar Instalación de python
python3 -V
```

```bash
# Instalación de gestor de paquetes de dependencias
sudo apt install -y python3-pip
```

```bash
# Verificar Instalación del gestor
pip3 -V
```
![Alt text](image-12.png)

```bash
# Alternative Installation
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
sudo python3 get-pip.py
```

![Alt text](image-11.png)

```bash
# Dependencias en entorno profesional
sudo apt install -y build-essential libssl-dev libffi-dev python3-dev
```
![Alt text](image-13.png)

### Instalación en Mac

![Alt text](image-14.png)

Comandos utilizados

```bash
python o python3

exit()
```

Normalmente viene instalado en Mac, en caso de que no lo tenga continuar con estos comandos Herramientas de codigo

```bash
sudo xcode-select --install

sudo xcode-select --reset
```

Instalación de python

```bash
brew install python3
```

Verificar la Instalación

```bash
python3
```

### Python con VSCode

![Alt text](image-15.png)

adicional si se esta usando WSL

![Alt text](image-16.png)

creamos el proyecto ingresamos a la carpeta y abrimos el visual

```bash
code .
```

![Alt text](image-17.png)

![Alt text](image-18.png)