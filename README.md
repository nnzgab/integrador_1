## Teclado de Alarma: Firmware de Prueba Funcional

### Introducción

Los teclados de alarma son componentes cruciales en los sistemas de seguridad, ya que permiten a los usuarios interactuar con el sistema y controlar sus funciones. Es fundamental garantizar que estos teclados funcionen correctamente para asegurar la protección adecuada de los hogares o negocios. La implementación de un firmware de prueba funcional en los teclados de alarma durante el proceso de producción puede ayudar a identificar y corregir fallas temprano, antes de que lleguen a los clientes.

### Objetivo principal

El objetivo principal de este proyecto es desarrollar e implementar un firmware que permita realizar una prueba funcional completa de los teclados de alarma durante la etapa de producción. Este firmware debe evaluar todos los componentes del teclado, incluyendo:

* **Teclado matricial:** Verificar la correcta respuesta de cada tecla al ser presionada, detectando posibles fallos en los contactos o la matriz de teclas.
* **LEDs:** Asegurar que los 9 LEDs (6 para zonas y 3 para sistema) funcionen correctamente, indicando los estados correspondientes de manera precisa.
* **Buzzer:** Probar el funcionamiento del buzzer, generando sonidos de alerta y notificaciones según lo especificado en el diseño del teclado.
* **Entradas analógicas:** Interpretar los valores analógicos leídos para determinar el estado de la batería y las zonas del teclado.
* **Puerto de comunicación UART:** Validar la correcta comunicación entre el teclado y el panel de alarma, enviando y recibiendo mensajes de prueba.

### Descripción del programa de prueba de teclado

#### Inicio y cuenta regresiva

* El programa comienza con una cuenta regresiva de 6 segundos visible en el monitor serial.
* Durante este tiempo, tres LEDs de sistema se encenderán secuencialmente.

#### Inicio del test

* Para iniciar el test, el usuario debe presionar una combinación específica de dos teclas (por ejemplo, '#' y '6') dentro del período de la cuenta regresiva.
* Si se inicia el test correctamente, se mostrará el mensaje "INICIO DE TEST" en el monitor serial.

#### Prueba de ingreso de teclas

* El programa solicitará al usuario que ingrese cada tecla del teclado de manera secuencial.
* Cada vez que se ingrese una tecla correcta, se avanzará a la siguiente.

#### Prueba de LEDs

* Una vez finalizada la prueba de ingreso de teclas, se procederá a evaluar el funcionamiento de cada LED, encendiéndolos secuencialmente.
* Para avanzar a la siguiente prueba, el usuario debe presionar la tecla '#'.

#### Prueba de buzzer y entradas analógicas

* Seguidamente, se evaluarán el buzzer y las entradas analógicas del teclado.

#### Finalización del test

* El test concluirá con el mensaje "FINAL DEL TEST" en el monitor serial.
* La finalización del test se verá con todos los leds parpadeando intermitentemente.
* Durante la ejecución del test, si el usuario no pasa al siguiente estado dentro de un período de 6 segundos, el test se finalizará automáticamente.

### Aclaración sobre las funcionalidades de la primera entrega del proyecto

Es importante destacar que esta entrega representa una fase inicial del desarrollo, y se prevén mejoras e implementaciones adicionales en entregas posteriores.

#### Funcionalidades de la primera entrega

* **Prueba de pulsadores individuales:** El sistema permitirá la prueba de tres pulsadores individuales, simulando el ingreso de teclas. Esta funcionalidad se implementará como paso previo a la futura integración de un teclado matricial completo.
* **Control de LEDs de sistema:** Se implementará el control de tres LEDs de sistema, permitiendo verificar su correcto funcionamiento.
* **Prueba de buzzer:** Se incluirá la prueba del buzzer, evaluando su capacidad para emitir sonidos de alerta o notificación.
* **Lectura básica de entrada analógica:** Se implementará una lectura básica de la entrada analógica del teclado, utilizando el conversor analógico-digital (ADC). Esta funcionalidad se mejorará en entregas

-------------------
necesito que formatees el siguiente texto con la sintaxis de markdown de modo que quede presentable para un ambito academico a nivel universitario por que es parte de un readme de un proyexto, necesito que me pases el Formatted Text with Markdown Syntax, el texto es el siguientes:
Teclado de Alarma: Firmware de Prueba Funcional
Introducción

Los teclados de alarma son componentes cruciales en los sistemas de seguridad, ya que permiten a los usuarios interactuar con el sistema y controlar sus funciones. Es fundamental garantizar que estos teclados funcionen correctamente para asegurar la protección adecuada de los hogares o negocios. La implementación de un firmware de prueba funcional en los teclados de alarma durante el proceso de producción puede ayudar a identificar y corregir fallas temprano, antes de que lleguen a los clientes.

Objetivo principal

El objetivo principal de este proyecto es desarrollar e implementar un firmware que permita realizar una prueba funcional completa de los teclados de alarma durante la etapa de producción. Este firmware debe evaluar todos los componentes del teclado, incluyendo:

Teclado matricial: Verificar la correcta respuesta de cada tecla al ser presionada, detectando posibles fallos en los contactos o la matriz de teclas.
LEDs: Asegurar que los 9 LEDs (6 para zonas y 3 para sistema) funcionen correctamente, indicando los estados correspondientes de manera precisa.
Buzzer: Probar el funcionamiento del buzzer, generando sonidos de alerta y notificaciones según lo especificado en el diseño del teclado.
Entradas analógicas: Interpretar los valores analógicos leídos para determinar el estado de la batería y las zonas del teclado.
Puerto de comunicación UART: Validar la correcta comunicación entre el teclado y el panel de alarma, enviando y recibiendo mensajes de prueba.
Descripción del programa de prueba de teclado

Inicio y cuenta regresiva:

El programa comienza con una cuenta regresiva de 6 segundos visible en el monitor serial.
Durante este tiempo, tres LEDs de sistema se encenderán secuencialmente.
Inicio del test:

Para iniciar el test, el usuario debe presionar una combinación específica de dos teclas (por ejemplo, '#' y '6') dentro del período de la cuenta regresiva.
Si se inicia el test correctamente, se mostrará el mensaje "INICIO DE TEST" en el monitor serial.
Prueba de ingreso de teclas:

El programa solicitará al usuario que ingrese cada tecla del teclado de manera secuencial.
Cada vez que se ingrese una tecla correcta, se avanzará a la siguiente.
Prueba de LEDs:

Una vez finalizada la prueba de ingreso de teclas, se procederá a evaluar el funcionamiento de cada LED, encendiéndolos secuencialmente.
Para avanzar a la siguiente prueba, el usuario debe presionar la tecla '#'.
Prueba de buzzer y entradas analógicas:

Seguidamente, se evaluarán el buzzer y las entradas analógicas del teclado.
Finalización del test:

El test concluirá con el mensaje "FINAL DEL TEST" en el monitor serial.
La finalizacion del test se vera con todos los leds parpadeando intermitentemente.
Durante la ejecución del test, si el usuario no pasa al siguiente estado dentro de un período de 6 segundos, el test se finalizará automáticamente.
Aclaración sobre las funcionalidades de la primera entrega del proyecto

Es importante destacar que esta entrega representa una fase inicial del desarrollo, y se prevén mejoras e implementaciones adicionales en entregas posteriores.

Funcionalidades de la primera entrega:

Prueba de pulsadores individuales: El sistema permitirá la prueba de tres pulsadores individuales, simulando el ingreso de teclas. Esta funcionalidad se implementará como paso previo a la futura integración de un teclado matricial completo.
Control de LEDs de sistema: Se implementará el control de tres LEDs de sistema, permitiendo verificar su correcto funcionamiento.
Prueba de buzzer: Se incluirá la prueba del buzzer, evaluando su capacidad para emitir sonidos de alerta o notificación.
Lectura básica de entrada analógica: Se implementará una lectura básica de la entrada analógica del teclado, utilizando el conversor analógico-digital (ADC). Esta funcionalidad se mejorará en entregas posteriores para una medición más precisa.
Cambio de hardware

Inicialmente, se había planteado utilizar el microcontrolador STM32F031C6T6 compatible con la placa NUCLEO-F031K6. Sin embargo, debido a que este microcontrolador no es compatible con Keil Studio Cloud (y está marcado como descontinuado por Mbed), se ha decidido utilizar la placa Blue Pill basada en el microcontrolador STM32F103.

Conclusión

El desarrollo de un firmware de prueba funcional para teclados de alarma permitirá garantizar la calidad y el correcto funcionamiento de estos componentes durante el proceso de producción. La implementación
