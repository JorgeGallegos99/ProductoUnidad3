# ProductoUnidad3

## 1. PLANTEAMIENTO DEL PROBLEMA

## 2. OBJETIVOS

**General**

* Entender el funcionamiento de las máquinas de estado, y aplicarlo en la resolución de los ejercicios propuestos. 

**Específicos**

* Analizar los ejercicios propuestos para determinar el diagrama de estado de cada uno de los ejercicios.

* Construir para cada ejercicio una tabla de transición a partir de un diagrama de estados.

## 3. ESTADO DEL ARTE


* **Identificación de una limitación específica en las redes recurrentes de retroalimentación local que actúan como máquinas Mealy-Moore**

















## 4. MARCO TEÓRICO

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

## 5. DIAGRAMAS

**Ejercicio 1**

**Ejercicio 2 **

**Ejericicio 3**

**Ejercicio 4**




## 6. EXPLICACIÓN DEL CÓDIGO FUENTE

**6.1. Dibuje el diagrama de estados para la máquina de estado finito cuya tabla de estados es la siguiente:**  

![jf4](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf4.PNG)

Para poder realizar nuestro diagrama de estado debemos guiarnos de nuestra tabla de transición.
Nos ubicamos en la primera fila de la tabla, este es nuestro estado inicial y el estado actual, el estado siguiente será el que toma la maquina cuando la entrada es 0, y su salida correspondiente es 1 es decir S0. Debemos dibujar esta transición en el diagrama e indicar cuál es la entrada del estado siguiente y su correspondiente salida.

![jf5](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf5.png)

Luego debemos ubicarnos en el estado siguiente cuando nuestro estado actual toma el valor de 1, podemos observar que el estado siguiente es S4, dibujamos la transición en la cual indicamos que la entrada del estado siguiente es uno y su salida correspondiente es 1.

![jf6](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf6.png)

Repetimos este procedimiento con todos los estados tomando en cuenda cuál es su estado próximo cuando toma el valor de “1” y “0”.
 De esta forma construimos nuestro diagrama de estados, una forma de verificar que nuestro diagrama de estados es que cada estado debe tener dos transiciones. De esta forma verificamos que nuestro diagrama este realizado correctamente.
 
 
 ![Diagrama%20estado%20ej1.PNG](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/Diagrama%20estado%20ej1.PNG)
 
 ![tablaEjercicio11.PNG](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/tablaEjercicio11.PNG)
 
 ![tablaEjercicio12.PNG](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/tablaEjercicio12.PNG)
 
 Para calcular la cadena de entrada debemos nos apoyamos de la tabla de transición
Empezamos en el estado inicial S0 (morado).
En la columna “Transición” nos ubicamos en la subcolumna que tenga el dato que estamos ingresando “1” la celda que corresponda al estado inicial y la columna del dato representa el estado siguiente de nuestra cadena S4 (celeste).
Luego, nos ubicamos en la Columna salida y de igual forma buscamos la subcolumna que tenga el dato que estamos ingresando, la celda correspondiente nos dará el valor de la salida actual de nuestra tabla.
Como siguiente paso nos dirigimos al estado siguiente obtenido en la primera transición en nuestro ejemplos S4 (celeste), le asignamos el siguiente dato de entrada “0”, de la misma forma debemos ir a la columna Transición y debemos localizarnos en la subcolumna que tenga el dato que estamos ingresando en este caso ingresamos un “0”, de la misma forma este nos data el estado siguiente S1 (amarillo), por ultimo verificamos en la subcolumna de salida el dato que ingresamos y colocamos la salida del dato actual en la fila salida.
Repetimos este procedimiento con todas las entradas de la cadena.
Con el último estado al no tener una entrada tampoco sabemos que salida tendrá por lo tanto solo dejamos indicado el estado siguiente que la tabla nos devuelve.

**6.2. Dibuje el diagrama de estados para la máquina de estado finito cuya tabla de estados es la siguiente. Partiendo del estado inicial s0, calcula la salida para la cadena de entrada abbccc.**

![jf7](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf7.PNG)

![Diagramaestadoej2]()

Para poder dibujar nuestro Diagrama de estados partimos del primer estado (S0) el cual se ubica en la primera fila de nuestra tabla. En el estado siguiente está dado por el estado que toma la maquina cuando toma el valor de a, en este caso S0, debemos dibujar esa transición y colocar la entrada y su correspondiente salida.

![jf8](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf8.PNG))

Continuamos con la siguiente subcolumna, la maquina salta de S0 a S3 debido a que es el estado que toma la maquina cuando toma el valor de B, dibujamos la transición y colocamos la correspondiente entrada y salida de esta subcolumna. Realizamos el mismo procedimiento con cada estado y con cada posible valor que puede tomar la máquina.

![jf9](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf9.PNG))

![jf10](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf10.PNG))

Al igual que en el primer ejercicio debemos apoyarnos en la tabla de transición 
El primer estado es S0 y cuando toma el valor de “a” su salida correspondiente es  “0” y el estado siguiente es S0, nos posicionamos en la fila que tenga S0, cuando este estado toma el valor de b su salida correspondiente es “1” y el estado siguiente que genera es S3, repetimos el procedimiento con todos los estados hasta que llegamos al estado final el cual solo se deja indicado ya que no tenemos una entrada y por lo tanto no podemos calcular su salida solo sabemos que será el estado siguiente.

Partiendo del estado S0, calcula la salida para la cadena de entrada 1000110



## 7. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

La herramienta que utilizamos para la creacio de nuestros diagramas de estados es Creadly.com
Una herramienta online con la cual podemos realizar variso tipos de apas mentales y conceptuales.

Ingresamos en la página https://creately.com/

Damos clic en sign in 

![jf11](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf11.PNG))

En la siguiente pagina damos clic en Sign in with google o ingresamos con nuestro correo electronico con el que nos registramos.

![jf12](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf12.PNG))

Para crar un nuevo diseño damos clic en el boton “añadir documento”

![jf13](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf13.PNG))

Se abritra una nueva pestaña en nuestro navegador, aquí debemos elegir el tipo de diseñoq eu queremos usar, para nuetro caso usaremos abriremos una hoja de trabajo en blanco

![jf14](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf14.PNG))

Una vez dentro de la hoja de, al lado izquiedo de la pagina se encuntran todas las formass que podemos usar para nuestro diseño. Seleccionamos uno y lo arrastramos al centro de la hoja de trabajo 

![jf15](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf15.PNG)

![jf16](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf16.PNG)

Seleccionamos tantas figuras como sean necesarias cuando damos clic en alguna figura de despliega un menu con opciones para editar nuestra figura, como por ejempllo darle color o poner un texto dentro

![jf17](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf17.PNG)

Basta con tener un poco de creatividad para sacarle el maximo provecho a esta herramienta! 

![jf18](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf18.PNG)


## 8. APORTACIONES

## 9. CONCLUSIONES

## 10. RECOMENDACIONES

## 11. CRONOGRAMA

![jcronograma](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jcronograma.PNG)

## 12. BIBLIOGRAFÍA

https://www.tecbolivia.com/index.php/articulos-y-tutoriales-microcontroladores/13-introduccion-a-las-maquinas-de-estado-finito

https://bloganalisis1.files.wordpress.com/2011/01/apuntesdsd10_mealy_moore.pdf

https://espe28.monday.com/boards/673079331/


## 13. ANEXOS
