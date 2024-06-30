**

### Redes Neuronales Artificiales (RNA)

#### ¿Qué son las redes neuronales?

Una red neuronal es un modelo de machine learning inspirado en la estructura y el funcionamiento del cerebro humano. Está diseñada para tomar decisiones imitando cómo las neuronas biológicas trabajan juntas para identificar fenómenos, sopesar opciones y llegar a conclusiones.

![](https://assets.isu.pub/document-structure/210510021110-9ddcf1449571f5a351db79d67bf90513/v1/1850068f7d951490560789f46cb9c89f.jpg)

Las redes neuronales constan de múltiples capas de nodos o neuronas artificiales: una capa de entrada, una o varias capas ocultas y una capa de salida. Cada nodo está conectado a otros nodos y tiene su propia ponderación y umbral asociados. Si la salida de un nodo individual está por encima del valor umbral especificado, ese nodo se activa y envía datos a la siguiente capa de la red. De lo contrario, no se pasa ningún dato a la siguiente capa.

![](https://www.droneguru.es/wp-content/uploads/2019/11/004.png)

Estos sistemas se basan en datos de entrenamiento para aprender y mejorar su precisión con el tiempo. Una vez entrenadas, las redes neuronales se convierten en herramientas poderosas en informática e inteligencia artificial, permitiendo clasificar y agrupar datos a gran velocidad. Por ejemplo, el algoritmo de búsqueda de Google es una de las aplicaciones más conocidas de redes neuronales.

![](https://www.xeridia.com/wp-content/uploads/2020/08/entrenar-redes-neuronales-artificiales.jpg.webp)

Las redes neuronales, también conocidas como redes neuronales artificiales (ANN) o redes neuronales simuladas (SNN), son un subconjunto del machine learning y forman el núcleo de los modelos de deep learning.

#### ¿Cómo funcionan las redes neuronales?

**

Cada nodo individual en una red neuronal puede pensarse como un modelo de regresión lineal, compuesto por datos de entrada, ponderaciones, un sesgo (o umbral) y una salida. La fórmula básica sería la siguiente:

∑wixi + sesgo = w1x1 + w2x2 + w3x3 + sesgo

salida = f(x) = 1 if ∑w1x1 + b>= 0; 0 if ∑w1x1 + b < 0

Una vez determinada la capa de entrada, se asignan las ponderaciones. Estas ponderaciones ayudan a determinar la importancia de cualquier variable, ya que las más grandes contribuyen de forma más significativa a la salida en comparación con otras entradas. A continuación, todas las entradas se multiplican por sus respectivas ponderaciones y se suman. Después, la salida se pasa a través de una función de activación, que determina la salida. Si esa salida supera un umbral determinado, se «dispara» (o activa) el nodo, pasando los datos a la siguiente capa de la red. Esto da como resultado que la salida de un nodo se convierta en la entrada del siguiente nodo. Este proceso de pasar datos de una capa a la siguiente capa define esta red neuronal como una red de proalimentación.

  

Desglosemos el funcionamiento utilizando un ejemplo práctico:

Supongamos que estamos tratando de decidir si ir a surfear o no. Hay tres factores que influyen en la decisión:

1.  ¿Las olas son buenas? (Sí: 1, No: 0)
    
2.  ¿Está el pico despejado? (Sí: 1, No: 0)
    
3.  ¿Ha habido un ataque de tiburones recientemente? (Sí: 0, No: 1)
    

Asignamos valores a estas entradas y ponderaciones según su importancia:

* X1 = 1 (olas buenas)
    
* X2 = 0 (pico lleno)
    
* X3 = 1 (no ha habido ataque de tiburones)
    

Ponderaciones:

* W1 = 5 (olas buenas son importantes)
    
* W2 = 2 (multitudes son tolerables)
    
* W3 = 4 (miedo a los tiburones es significativo)
    

Umbral: -3

La fórmula para calcular la salida sería: Y=(1∗5)+(0∗2)+(1∗4)−3=6

Usando una función de activación simple, si el resultado es mayor que 0, el nodo se activa (en este caso, iríamos a surfear) pero si ajustamos las ponderaciones o el umbral, podemos obtener resultados diferentes del modelo. Cuando observamos una decisión, como en el ejemplo anterior, podemos ver cómo una red neuronal podría tomar decisiones cada vez más complejas en función de la salida de las decisiones o capas anteriores.

**

#### Estructura y componentes básicos de una red neuronal

* Capa de entrada: Recibe los datos de entrada. Esta capa no está formada por neuronas artificiales, sino que simplemente actúa como un receptor de información.
    
* Capas ocultas: Procesan la información recibida. El número de capas ocultas puede variar según la complejidad del problema que se quiere resolver.
    
* Capa de salida: Entrega el resultado final del procesamiento de la red, que puede ser una clasificación, predicción, etc.
    

El aprendizaje de la red neuronal implica presentar muchos ejemplos para los cuales se conoce el resultado, comparar las predicciones de la red con los resultados reales, y ajustar las ponderaciones para reducir el error. Este proceso se repite muchas veces hasta que la red mejora su precisión.

![](https://miro.medium.com/v2/resize:fit:1156/format:webp/1*DzPv2JB24A9Po7sblKs5EA.jpeg)

#### Tipos de redes neuronales

1.  Por número de capas:
    

* Monocapas: La capa de entrada se conecta directamente con la de salida. Estas son las redes más simples.
    
* Multicapas: Cuentan con una o más capas ocultas entre la entrada y la salida, permitiendo el procesamiento de datos más complejo.
    

3.  Por tipo de conexiones:
    

* No recurrentes: No tienen memoria y procesan cada entrada de manera independiente.
    
* Recurrentes: Tienen memoria, permitiendo que las salidas de etapas anteriores influyan en las etapas posteriores. Esto es útil para tareas que requieren contexto, como el procesamiento del lenguaje natural.
    

5.  Por grado de conexiones:
    

* Totalmente conectadas: Cada nodo en una capa está conectado a todos los nodos en la capa siguiente.
    
* Parcialmente conectadas: No todos los nodos están conectados, lo que puede reducir la complejidad y el tiempo de procesamiento.
    

7.  Convolucionales: Simulan las neuronas de la corteza visual primaria y son especialmente efectivas para tareas de visión artificial, como la clasificación de imágenes.
    

#### Aplicaciones de las redes neuronales

* Reconocimiento: Diferenciación de elementos, como el reconocimiento facial o de voz. Gracias a su capacidad de aprendizaje y de entrenamiento, una red neuronal puede diferenciar entre diferentes elementos.
    
* Clasificación: Clasificación de datos, como la categorización de correos electrónicos en spam y no spam.
    
* Predicción y diagnóstico: Predicción de eventos futuros, como la previsión de ventas, y diagnóstico de problemas de salud en medicina.
    

#### Ventajas de las redes neuronales

* Aprendizaje autónomo: Las RNA pueden aprender de los datos de entrada sin intervención constante.
    
* Autoorganización: Pueden crear su propia representación de la información interna.
    
* Tolerancia a fallos: Pueden seguir funcionando incluso si están parcialmente dañadas.
    
* Flexibilidad: Manejan múltiples cambios en la entrada sin problemas significativos.
    
* Tiempo real: Pueden proporcionar respuestas en tiempo real debido a su estructura paralela.
    

#### Desventajas de las redes neuronales

* Complejidad de aprendizaje: Enseñar a una red neuronal para tareas grandes puede ser complicado.
    
* Tiempo de aprendizaje elevado: El tiempo necesario para el aprendizaje aumenta con la cantidad de datos y la flexibilidad requerida.
    
* Interpretabildad: La salida de la red requiere interpretación por parte del programador para entender su significado.
    
* Elevada cantidad de datos: Se necesita una gran cantidad de datos para entrenar adecuadamente la red.
    

### Conclusión

Las redes neuronales artificiales son herramientas poderosas para la inteligencia artificial, capaces de aprender y mejorar con el tiempo. Sin embargo, presentan desafíos como la complejidad del aprendizaje y la necesidad de grandes cantidades de datos. Su estructura y funcionamiento permiten aplicaciones en diversos campos, desde el reconocimiento de patrones hasta la predicción y diagnóstico en medicina, mostrando su versatilidad y capacidad para abordar problemas complejos.


### Bibliografía

[https://www.ibm.com/es-es/topics/neural-networks](https://www.ibm.com/es-es/topics/neural-networks)  

[matich-redesneuronales.pdf (utn.edu.ar)](https://www.frro.utn.edu.ar/repositorio/catedras/quimica/5_anio/orientadora1/monograias/matich-redesneuronales.pdf)  

[https://www.inesdi.com/blog/que-son-las-redes-neuronales/](https://www.inesdi.com/blog/que-son-las-redes-neuronales/)  

[https://www.ibm.com/docs/es/spss-modeler/saas?topic=networks-neural-model](https://www.ibm.com/docs/es/spss-modeler/saas?topic=networks-neural-model) 

**