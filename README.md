# ProductoUnidad3

1. PLANTEAMIENTO DEL PROBLEMA

2. OBJETIVOS

3. ESTADO DEL ARTE

4. MARCO TEÓRICO

**MÁQUINAS DE ESTADO**

**Estado:** Se puede definir como el conjunto de valores almacenado en los biestables durante un determinado ciclo de reloj.
En general, un circuito con n biestables podrá tener 2^n estados posibles. Los estados contienen la información relevante que debe almacenar el circuito.

**Máquina de estados Finita**

Una Máquina de Estado Finito (Finite State Machine), llamada también Autómata Finito es una abstracción computacional que describe el comportamiento de un sistema reactivo mediante un número determinado de Estados y un número determinado de Transiciones entre dicho Estados.

Las Transiciones de un estado a otro se generan en respuesta a eventos de entrada externos e internos; a su vez estas transiciones y/o subsecuentes estados pueden generar otros eventos de salida. Esta dependencia de las acciones (respuesta) del sistema a los eventos de entrada hace que las Máquinas de Estado Finito (MEF) sean una herramienta adecuada para el diseño de Sistemas Reactivos y la Programación Conducida por Eventos (Event Driven Programming), cual es el caso de la mayoría de los sistemas embebidos basados en microcontroladores o microprocesadores.

Cualquier circuito con memoria puede verse como una máquina de estados. El diseño de FSMs involucra: 
* Definir estados
* Definir transiciones entre estados
* Optimizar / minimizar (fuera de esta asignatura)
* Definir los valores de las salidas en cada momento
Sin embargo este enfoque es práctico sólo para FSMs pequeñas.

**Diagrama de estados.-** Muestra la forma y la función de la máquina de estados. Normalmente un diagrama de círculos y flechas.

**Próximo estado.-** El estado al que irá la máquina de estados en la siguiente transición. Depende de los valores de entrada y salida.

**Rama.-** Indica un cambio del estado presente al próximo estado.

![jf1](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf1.PNG)

Esquema de Diagrama de Estados

**Máquina de Mealy**

Dado el estado actual Q. Si llega un valor a la entrada el circuito de lógica / combinacional (L/C) calcula el estado siguiente y la salida. Cuando llega un pulso de reloj, se captura el nuevo estado. Defecto: Con el pulso de reloj se captura el nuevo estado y el L/C recalcula otro estado y una nueva salida.

![jf2](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf2.PNG)

**Máquina de Moore**

Los estados de los circuitos son también las salidas del mismo. Es muy usado para generar secuencias de conteo ya que requiere menos circuitos combinacionales. En la maquina de moore, la salida se toma directamente del registro, por lo que no necesita logica combinacional para sintetizar la salida.

![jf3](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf3.PNG)

5. DIAGRAMAS

6. EXPLICACIÓN DEL CÓDIGO FUENTE

7. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

8. APORTACIONES

9. CONCLUSIONES

10. RECOMENDACIONES

11. CRONOGRAMA

![jcronograma](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jcronograma.PNG)

12. BIBLIOGRAFÍA

https://www.tecbolivia.com/index.php/articulos-y-tutoriales-microcontroladores/13-introduccion-a-las-maquinas-de-estado-finito

https://bloganalisis1.files.wordpress.com/2011/01/apuntesdsd10_mealy_moore.pdf

https://espe28.monday.com/boards/673079331/


13. ANEXOS
