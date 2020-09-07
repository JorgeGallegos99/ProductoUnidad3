# ProductoUnidad3

## 1. PLANTEAMIENTO DEL PROBLEMA

## 2. OBJETIVOS

**General**

* Entender el funcionamiento de las máquinas de estado, y aplicarlo en la resolución de los ejercicios propuestos. 

**Específicos**

* Analizar los ejercicios propuestos para determinar el diagrama de estado de cada uno de los ejercicios.

* Construir para cada ejercicio una tabla de transición a partir de un diagrama de estados.

## 3. ESTADO DEL ARTE

* **Detector de bordes negativos de Moore y Mealy Un ejemplo de VHDL para máquina de estados finitos**

En el articulo *Detector de bordes negativos de Moore y Mealy Un ejemplo de VHDL para máquina de estados finitos* se mencionan dos variedades FSM, Moore y Mealy. Los diagramas de estado de la máquina de Moore y Mealy se diseñan e implementan mediante el uso de un circuito detector de borde negativo. Las máquinas de estado diseñadas se implementan en VHDL. Para ambas máquinas de estado también se hace una comparación.En las sociedades modernas, somos más dependientes de las herramientas informáticas, que nos ayudan a afrontar las vidas modernas recientes. Las máquinas automáticas realizan una variedad de operaciones adaptando los cambios en el entorno físico. 

**Autores:**

**Pradeep Garapati**

Ingeniería electrónica y de la comunicación Fundación de Vignan para la ciencia, la tecnología y la investigación Vadlamudi

**Sarada Musala**

Ingeniería electrónica y de la comunicación Fundación de Vignan para la ciencia, la tecnología y la investigación Vadlamudi

**Fecha y lugar de publicación:**

*Fecha:*  28-30 de julio de 2020 en la conferencia Conferencia internacional de 2020 sobre comunicaciones y procesamiento de señales (ICCSP)  Chennai, India, India


* **Un ejemplo de FSM de Moore y Mealy basado en VHDL para la educación**

Las máquinas automatizadas modernas adaptan su secuencia de acciones en función de su entorno y eventos. La FSM (máquina de estados finitos) se utiliza para expresar matemáticamente esas secuencias de acciones o instrucciones. En el articulo *Un ejemplo de FSM de Moore y Mealy basado en VHDL para la educación*, se analizan dos tipos de máquinas FSM, Moore y Mealy. Mostrando diferentes resultados para demostrar la importancia del modelado FSM. Un circuito detector de bordes se diseña empleando máquinas Moore y Mealy. Es un ejemplo de diseño de FSM, se puede utilizar para la construcción y demostración de conceptos de los estudiantes. Estos diseños se implementan en VHDL. También se hace una comparación basada en ambas implementaciones.

**Autores:**

**Sultana Alsubaei**

Departamento de Ingeniería Eléctrica e Informática, Universidad de Effat, Jeddah, KSA

**SM Qaisar**

Departamento de Ingeniería Eléctrica e Informática, Universidad de Effat, Jeddah, KSA

**W. Alhalabi**

Departamento de Ciencias de la Computación, Universidad de Effat, Jeddah, KSA

**Fecha y lugar de publicación:**

*Fecha:*  4-6 de agosto de 2017 en 2017 IEEE 2nd International Conference on Signal and Image Processing (ICSIP)

**Realización de circuito secuencial usando máquina de estados finitos**

La teoría de los autómatas es una herramienta que se utiliza en la informática multidisciplinar y la investigación científica. Es la base detrás del modelo tradicional de cálculo y se usa para muchos propósitos, como diseño de circuitos de controlador, diseño de circuitos secuenciales, etc. Un detector de secuencia es una máquina de estado secuencial que se usa para detectar bits consecutivos en una cadena binaria.

Este documento técnico examina varias secuencias y da un resultado como 1 si se detecta la secuencia 1101. Los tipos de secuencia examinados son secuencias superpuestas. El algoritmo diseñado para detectar la secuencia 1101 usa flip-flops. Las chanclas ayudan a detectar el patrón en la cadena dada.

**Autores:**

**Urvashi Kodwani**

Departamento de Ingeniería Informática, Facultad de Ingeniería y Gestión Shri Ramdeobaba, Nagpur, India

**Sonal Rajurkar**

Departamento de Ingeniería Informática, Facultad de Ingeniería y Gestión Shri Ramdeobaba, Nagpur, India

**SG Mundada**

Departamento de Ingeniería Informática, Facultad de Ingeniería y Gestión Shri Ramdeobaba, Nagpur, India

**Fecha y lugar de publicación:**

*Fecha:*  15-16 de junio de 2017 en la conferencia 2017 Congreso Internacional sobre Sistemas de Control e Informática Inteligente (ICICCS)

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

Diagramas de estado de los ejercicios propuestos

**Ejercicio 1**

![Diagrama%20estado%20ej1.PNG](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/Diagrama%20estado%20ej1.PNG)

**Ejercicio 2 **

![Diagrama_de%20_Estados%20_Ejercicio%20_2.png](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/Diagrama_de%20_Estados%20_Ejercicio%20_2.png)

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

![Diagrama_de%20_Estados%20_Ejercicio%20_2.png](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/Diagrama_de%20_Estados%20_Ejercicio%20_2.png)

Para poder dibujar nuestro Diagrama de estados partimos del primer estado (S0) el cual se ubica en la primera fila de nuestra tabla. En el estado siguiente está dado por el estado que toma la maquina cuando toma el valor de a, en este caso S0, debemos dibujar esa transición y colocar la entrada y su correspondiente salida.

![jf8](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf8.PNG)

Continuamos con la siguiente subcolumna, la maquina salta de S0 a S3 debido a que es el estado que toma la maquina cuando toma el valor de B, dibujamos la transición y colocamos la correspondiente entrada y salida de esta subcolumna. Realizamos el mismo procedimiento con cada estado y con cada posible valor que puede tomar la máquina.

![jf9](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf9.png)

![jf10](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/jf10.PNG)

Al igual que en el primer ejercicio debemos apoyarnos en la tabla de transición 
El primer estado es S0 y cuando toma el valor de “a” su salida correspondiente es  “0” y el estado siguiente es S0, nos posicionamos en la fila que tenga S0, cuando este estado toma el valor de b su salida correspondiente es “1” y el estado siguiente que genera es S3, repetimos el procedimiento con todos los estados hasta que llegamos al estado final el cual solo se deja indicado ya que no tenemos una entrada y por lo tanto no podemos calcular su salida solo sabemos que será el estado siguiente.

Partiendo del estado S0, calcula la salida para la cadena de entrada 1000110

**6.3. Halle la tabla de estados para la máquina de estado finito cuyo diagrama de estados es: **




**6.4. Construya una máquina de estado finito que modele una máquina expendedora de bebidas que acepta monedas de 5, 10 y 20 centavos. La máquina acepta monedas hasta que se introducen 25 centavos y devuelve cualquier cantidad que supere los 25 céntimos. Entonces, el cliente puede pulsar los botones y elegir una bebida de cola (C), cerveza (Z) o agua (A).**

**Explicación**



**Tabla**



**Diagrama de Estados**


![Diagrama_de_estados_ejercicio_4.png](https://github.com/JorgeGallegos99/ProductoUnidad3/blob/master/Img/Diagrama%20de%20estados%20ejercicio%204%20(1).png)



**6.5 Construya una máquina de estados finito que modele un circuito de riego automático como el mostrado en la figura. El circuito deberá accionar la bomba en las siguientes condiciones:
 a. El circuito accionará la bomba solamente cuando la tierra esté seca, pero antes debe comprobar
las siguientes condiciones:
    i. Para evitar que la bomba se estropee por funcionar en vacío, nunca se accionará la
    bomba cuando el depósito de agua esté vacío.
    ii. Si hay restricciones en el riego (época de verano), sólo se podrá regar de noche.
    iii. En el resto del año (si no hay restricciones) se podrá regar de día y de noche (si la tierra
    está seca).
 b. Para la implementación del circuito se dispone de las siguientes entradas:
    i. S: Señal que indica si la tierra está seca: Tierra seca: S=1; Tierra húmeda: S=0
    ii. R: Señal que indica si hay restricciones en el riego (es verano): Hay restricciones: R=1
    No hay restricciones: R=0
    iii. D: Señal que indica si es de día o de noche: Día: D=1; Noche: D=0
    iv. V: Señal que indica si el depósito de agua está vacío: Vacío: V=1; Hay agua: V=0
c. Y la salida B, que accionará la bomba para regar: Bomba funcionando: B=1; Bomba apagada
B=0.

**Explicación** 




**Tabla:**




**Diagrama de Estados**






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
