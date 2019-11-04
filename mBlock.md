# Scratch y Arduino

## CEP Motril


### José Antonio Vacas @javacasm

[![CCbySA](imagenes/CCbySQ_88x31.png)](./imagenes/Licencia_CC.png)

## https://github.com/javacasm/ScratchArduinoMotril



## Entornos de programación

Se puede programar con cualquier entorno donde se programe Arduino (IDE, Arduinoblocks, biblock, mBlock, etc.)

## Programación

### Usaremos el IDE de mBlock https://ide.mblock.cc 

Soporta Bluetooth Controller, Codey Rocky, HaloCode, mBot, MotionBlock, Neuron, mBot Ranger, Ultimate 2.0, Arduino Uno, Arduino Mega2560, Nova Pi, MegaPi Pro


### Necesitamos el mblock mlink  https://www.mblock.cc/en-us/download/

![mlink instalar](./imagenes/InstalarMlink.png)

[Guía de instalación](https://www.mblock.cc/doc/en/basics/mlink-quick-start-guide.html#mlink-quick-start-guide)

### Ejecutamos mLink

En windows
 
![mLink icon](https://www.mblock.cc/doc/en/basics/images/mlink-4.png)

En osX

![mlink osX](https://www.mblock.cc/doc/en/basics/images/mlink-8.png)

En linux

    sudo mblock-mlink start 
  

### Seleccionamos el dispositivo

Y pulsamos conectar

![conectar](https://www.mblock.cc/doc/en/basics/images/chromebook-7.png)

## Ejemplos

### Hello LED!!

Haremos parpadear el led Rojo

![Hello LED!](./imagenes/HelloLed!.png)

[Proyecto](https://planet.mblock.cc/project/102035)

### Led RGB

![Mezcla colores](./imagenes/Colores-MezclaRGB.jpeg)

[Selector de colores](https://htmlcolorcodes.com/es/)

Utilizamos el led RGB (conectado a lo pines digitales 9,5,6)

Y a la vez haremos que se vayan leyendo los colores en inglés, con la extensión Text To Speech.

Parece que hay algo de desajuste. Tendremos que mejorar la comunicación con ... mensajes    

![Programa Arduino](./imagenes/Colores-Arduino.png)
![Programa Osito](./imagenes/Colores-Osito.png)

[Programa](https://planet.mblock.cc/project/projectshare/101707)


### Nivel de luz

Usaremos los 3 leds de colores para indicar el nivel de luz:
* Rojo: luz baja
* Amarillo: nivel de luz medio
* Verde: luz suficiente

![NivelLuminoso](./imagenes/NivelLuminoso.png)

[Proyecto](https://planet.mblock.cc/project/102785)

### Controlando el movimiento de Osito con el Joystick

Sabemos que el joystick está conectado a los pines analógicos A0 (eje x) y A1 (eje y). Vamos a ver los valores que encontramos.

Vemos como la lectura de los sensores analógicos fluctúa, es algo normal. Un hardware más preciso (y caro) tendría una lectura más exacta.

Creamos una variables x e y para Arduino y comprobamos los valores del joystick

![Joystick Arduino](./imagenes/Joystick-Arduino.png)

![Joystick Osito](./imagenes/Joystick-Osito.png)

[Proyecto](https://planet.mblock.cc/project/102052) 

### Controlar el movimiento de Osito con el acelerómetro

Modificar el ejemplo anterior para que controlemos a Osito con el acelerómetro

Pista: modificar el programa para usar el sensor adecuado

[Proyecto](https://planet.mblock.cc/project/102061)

### Controlamos la posición de 2 servos usando el joystick

![2xServos-Joystick](./imagenes/2xServos-Joystick.png)

Controlamos la posición de 2 servos usando el joystick

[Proyecto](https://planet.mblock.cc/project/102156)

### Haciendo ruído

Veamos como hacer sonido con el zumbador: activamos y desactivamos rápidamente

Un poquito de física sobre frecuencias y periodos....

![Frecuencias y periosdos](./imagenes/frecuenciaYperiodo.png)

![Sonido 440Hz Original](./imagenes/Sonido440HzOrig.png)

Veremos que en modo "en vivo" no es suficientemente rápido y tenemos que irnos a modo Arduino

![Sonido 440Hz](./imagenes/Sonido440.png)

[Programa](https://planet.mblock.cc/project/102073)

Ejercicio: Ver como cambia el movimiento al enviar el programa anterior de los servos en modo Arduino
