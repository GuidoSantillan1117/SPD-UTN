# Examen Practico Arduino - Estaciones y Alarma Anti-incendios
![Segundo Parcial  Parte Domiciliaria _ Guido Santillan DIV D](https://github.com/GuidoSantillan1117/SPD-UTN/assets/137585994/d0235458-763d-48c2-9b70-2ea65c02ca34)

## Integrantes
Guido Santillán

## 🤖 Link al proyecto
https://www.tinkercad.com/things/e5RfPeHnbFD-segundo-parcial-parte-domiciliaria-guido-santillan-div-d/editel?sharecode=BY7cw4XETulfK1eznTsinehnxqVYt3AdofY474UHUu0

## Descripción del Proyecto
El siguiente código implementa un sistema de estaciones y alarma anti-incendios utilizando un Arduino. El proyecto utiliza un LCD de 16x2, un control remoto IR, un servo motor y un sensor de temperatura para mostrar la temperatura actual y la estación correspondiente en el LCD, y simular una respuesta al incendio.

## Código y Funcionamiento
El código implementa las siguientes funciones:

- `prenderLed(int led)`: Enciende el LED especificado.
- `apagarLed(int led)`: Apaga el LED especificado.
- `controlRemoto()`: Controla el sistema utilizando un control remoto IR.
- `mostrarTemperaturaEstacion()`: Muestra la temperatura actual y la estación correspondiente en el LCD.
- `simularIncendio()`: Simula una respuesta del sistema de incendio.

La función `mostrarTemperaturaEstacion()` lee la temperatura del sensor y la muestra en el LCD. Además, determina la estación correspondiente y enciende el LED verde si todo se encuentra en orden.

La función `simularIncendio()` verifica si la temperatura es superior a 60 grados y simula una respuesta al incendio mediante el servo motor y el led rojo que empieza a titilar.

## Configuración de los pines

- LCD: Se configuran los pines 5, 4, 8, 10, 12 y 13 como los pines del LCD.
- Servo: Se utiliza el pin 9 para controlar el servo motor.
- LEDS: Se utilizan los pines 7 y 6 para los LEDS rojo y verde, respectivamente.
- Buzzer: Se utiliza el pin 3 para el buzzer.
- Control Remoto: Se utiliza el pin 11 para conectar el sensor IR con el control remoto.

## Variables

- `lecturaSensor`: Almacena la lectura del sensor de temperatura.
- `temperatura`: Almacena el valor de temperatura calculado a partir de la lectura del sensor.
- `sistemaActivado`: Indica si el sistema está activado o desactivado.
- `lcdEncendido`: Indica si el LCD está encendido o apagado.
- `alertaFuego`: Indica si se ha detectado una alerta de fuego.



