# Remap---ROS
Se cambia provisionalmente el nombre del topic "/cmd_vel" del nodo "arbotix" a "/turtle1/cmd_vel".

*El ejercicio consiste en que utilizando el comando del teleoperado(turtle_teleop_key), del paquete de "turtlesim", se controla utilizando las flechas del teclado el robot del paquete "rbx1"; aprovechando que tanto "turtlesim" como "rbx1" tienen el mismo tipo de mensaje en el comando de velocidad se puede utilizar el comando "remap" para cambiar el nombre del topic suscriptor del nodo "arbotix" de "rbx1".*

*-------------------------------------------------------------------------------------------------------------------------------------------------------*

**Descargar Paquetes:**

- ***Paquete rbx1:***

*1. El paquete "rbx1" se debe descargar dentro de un workspace; por ejemplo: "/home/workspace/src/paquete_pkg"*

```
$ cd workspace/src

$ git clone https://github.com/pirobot/rbx1.git
```

*2. Utilizando el terminal se abre el archivo ".bashrc" y se agrega el workspace en caso de que no este agregado:*

```
$ cd

$ sudo gedit .bashrc 
```

- *Al final del archivo .bashrc se agrega la siguiente linea:*

```
source ~/workspace/devel/setup.bash
```

- *luego en una ventana de terminal estando en "/home" nos dirigimos al workspace y compilamos:*

```
$ cd workspace

$ catkin_make
```
*-------------------------------------------------------------------------------------------------------------------------------------------------------*
