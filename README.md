# Trabajo Práctico N.º 7: Entorno Gráfico (E/S)

Repositorio correspondiente al Trabajo Práctico N.º 7 de la materia Informática II de la carrera de Ingeniería Electrónica (UTN FRM).

 Descripción del Proyecto
Este proyecto implementa un sistema de control y monitoreo de Entradas y Salidas (E/S) utilizando una placa de desarrollo ESP32 en conjunto con una interfaz gráfica desarrollada en **Processing**. La comunicación entre ambos entornos se realiza mediante protocolo serie (UART vía USB) a una velocidad de 9600 baudios

 Características de la Aplicación
1. Entradas (E1 y E2): Monitoreo en tiempo real del estado de dos pulsadores físicos conectados a la ESP32, reflejando su cambio de estado visualmente en la interfaz de Processing
2. Salidas (L1 y L2): Control remoto de dos LEDs conectados a la ESP32 mediante clics sobre los elementos gráficos interactivos de la interfaz
3. Comunicación Bidireccional: Intercambio síncrono de tramas de datos por puerto serie

Hardware Utilizado
* Microcontrolador: ESP32 Dev Module (ESP32-D0WD-V3)
* 2x Pulsadores (configurados con `INPUT_PULLUP`)
* 2x LEDs con resistencias de protección de 300 ohms
* Conexión USB a PC

 Distribución de Pines (Pinout)

| Pulsador 1 (E1) -> GPIO 4 -> Entrada digital con resistencia de pull-up interna 
| Pulsador 2 (E2) -> GPIO 16 -> Entrada digital con resistencia de pull-up interna 
| LED 1 (L1) -> GPIO 12 -> Salida digital para control de L1 
| LED 2 (L2) -> GPIO 14 -> Salida digital para control de L2 

 Instrucciones de Ejecución
1. Conectar la ESP32 a la PC y verificar el puerto COM asignado (ej. `COM6`).
2. Cargar el código fuente de Arduino (`.ino`) en la placa utilizando el IDE de Arduino.
3. Asegurarse de cerrar el Monitor Serial de Arduino para liberar el puerto COM.
4. Abrir y ejecutar el script en Processing (`.pde`) para iniciar la interfaz gráfica de control.



Link del video del  funcionamiento: https://drive.google.com/file/d/1d2FuKTUydpbLV7qU1pbR2yxKZtie5o1J/view?usp=sharing
