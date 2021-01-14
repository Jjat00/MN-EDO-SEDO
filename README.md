<div align="center">
    <h1>
        Ecuaciones diferenciales ordinarias y sistemas de ecuaciones diferenciales ordinarias
    </h1>
</div>

<p style="text-align: justify;">
El presente documento es una guía cuyo objetivo es resolver problemas asociados con ecuaciones diferenciales ordinarias (EDO) y sistemas de ecuaciones diferenciales ordinarias (SEDO), a través de los métodos numéricos Euler y Runge Kutta orden 2 y 4.
</p>

<h2>Problema 1:</h2>

<p style="text-align: justify;"> 
    Un tanque perfectamente agitado contiene 400L de una salmuera en la cual están disueltos     25kg de sal común (NaCl), en un instante de tiempo entra al tanque un flujo de 80L/min       de una salmuera que contiene 0.5kg de sal/L. Si se tiene un flujo de salida de 80 L/min,     responda:
<p>

<ol type="a">
    <li>¿Qué cantidad de sal hay en el tanque transcurridos 10min?</li>
    <li>Si pasa mucho tiempo, ¿qué pasa con la cantidad de sal en el tanque?</li>
</ol> 

<p style="text-align: justify;">
Use el principio de conservación de la masa (para la sal), relacionando las variables mediante el balance de masa (𝑎𝑐𝑢𝑚𝑢𝑙𝑎𝑐𝑖ó𝑛=𝑒𝑛𝑡𝑟𝑎−𝑠𝑎𝑙𝑒) para obtener la ecuación diferencial correspondiente que deberá resolver por el método de Euler y Heun.
</p>

<h2>Problema 2</h2>

<p style="text-align: justify;">
    El atractor de Lorenz es una relación caótica caracterizada por su forma de mariposa.        Esta relación permite ver como evoluciona un sistema dinámico en un patrón no repetitivo     complejo. El atractor de Lorenz es un sistema dinámico, determinista, tridimensional, no     lineal, derivado a partir de una simplificación de las complejas ecuaciones de la            atmosfera convectiva. Ciertos parámetros del sistema exhiben un comportamiento caótico y     despliegan lo que se conoce como el atractor extraño. Este atractor es un fractal, que       surge en láseres, dinamos y algunos generadores de energía mecánica que aprovechan el        flujo de agua en ríos y cascadas.
</p>

<p>
    Las ecuaciones de Lorenz están dadas por:
</p>

<div style="text-align: center;">
<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{dx}{dt}&space;=&space;\sigma&space;(y&space;-&space;x)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{dx}{dt}&space;=&space;\sigma&space;(y&space;-&space;x)" title="\frac{dx}{dt} = \sigma (y - x)" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{dx}{dt}&space;=&space;\sigma&space;(y&space;-&space;x)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{dx}{dt}&space;=&space;\sigma&space;(y&space;-&space;x)" title="\frac{dx}{dt} = \sigma (y - x)" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{dz}{dt}&space;=&space;x&space;y&space;-&space;\beta&space;z" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{dz}{dt}&space;=&space;x&space;y&space;-&space;\beta&space;z" title="\frac{dz}{dt} = x y - \beta z" /></a>
</div>


<p>
    Donde 𝜎 es el número de Prandtl y 𝜌 el número de Rayleigh. Generalmente 𝜎=10, 𝛽=8/3     y 𝜌 suele variar siendo positivo, exhibiendo un valor de 𝜌=28 para un sistema caótico.
</p>

<ol type="a">
    <li>
        Resolver el sistema de Lorenz con las siguientes condiciones iniciales 𝑥(0)=2, 𝑦(0)        =6, 𝑧(0)=4. Use el método de Runge Kutta de orden 4.
    </li>
    <li>
        Defina tamaño de paso y use como punto el final de iteración 𝑡=60. Realice las              gráficas de 𝑥 vs 𝑦 y 𝑥 vs 𝑧.
    </li>
    <li>
        Realizar una grafica de las tres variables (𝑥,𝑦,𝑧 vs 𝑡)
    </li>
</ol>

<h2>Problema 3</h2>

<p style="text-align: justify;">
    Un lago contaminado tiene una concentración inicial de bacterias de 107 partes/L,            mientras que el nivel aceptable de partes/L es de solo de 5×106 partes/L. La                 concentración de bacterias se reducirá a medida que el agua dulce ingrese al lago. La        ecuación diferencial que gobierna la concentración C del contaminante en función del         tiempo (en semanas) viene dada por:
</p>

<div style="text-align: center;">
<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{dC}{dt}&space;&plus;&space;0.06&space;C&space;=&space;0" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{dC}{dt}&space;&plus;&space;0.06&space;C&space;=&space;0" title="\frac{dC}{dt} + 0.06 C = 0" /></a>
</div>

<ol type="a">
    <li>
        Use el método de Euler, un método de Runge Kutta de orden 2 y Runge Kutta de orden 4         para determinar la concentración del contaminante después de 7 semanas.
    </li>
    <li>
        Use diferentes tamaños de pasos (mínimo 3) ¿por qué escogió estos tamaños de paso?
    </li>
    <li>
        Analice la respuesta obtenida por los diferentes métodos numéricos y los diferentes          tamaños de paso.
    </li>    
</ol>

<h2>Problema 4</h2>
<p>
    Las dinámicas de un sistema forzado resorte-masa- amortiguador se representa con la          siguiente EDO de segundo orden:
</p>
<div style="text-align: center;">
<a href="https://www.codecogs.com/eqnedit.php?latex=m&space;\frac{d^2x}{dt^2}&space;&plus;&space;c&space;\frac{dx}{dt}&space;&plus;&space;k_1&space;x&space;&plus;&space;k_3&space;x^3&space;=&space;P&space;cos(wt)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?m&space;\frac{d^2x}{dt^2}&space;&plus;&space;c&space;\frac{dx}{dt}&space;&plus;&space;k_1&space;x&space;&plus;&space;k_3&space;x^3&space;=&space;P&space;cos(wt)" title="m \frac{d^2x}{dt^2} + c \frac{dx}{dt} + k_1 x + k_3 x^3 = P cos(wt)" /></a>
</div>
<p>
    donde 𝑚 = 1 𝑘𝑔, 𝑐 = 0.4 𝑁𝑠/𝑚, 𝑃 = 0.5 𝑁 y 𝜔 = 0.5/𝑠.
</p>

<p style="text-align: justify;"> 
    Utilice un método numérico de su preferencia para resolver cuál es el desplazamiento 𝑥      y la velocidad 𝑣 como función del tiempo con condiciones iniciales 𝑥 = 𝑢 = 0. Exprese     sus resultados en forma gráfica, como gráficas de series de tiempo (𝑥 y 𝑣 𝑣𝑒𝑟𝑠𝑢𝑠     𝑡) y gráfica del espacio-fase (𝑣 𝑣𝑒𝑟𝑠𝑢𝑠 𝑥). Haga simulaciones para un resorte       lineal (𝑘1 = 1; 𝑘3= 0) y no lineal (𝑘1 = 1; 𝑘3 = 0.5).
</p>