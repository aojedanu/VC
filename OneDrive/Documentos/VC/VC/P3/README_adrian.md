### Primer Ejercicio 

Este código implementa un sistema de detección y clasificación de monedas mediante visión por computadora. El programa identifica monedas en una imagen, permite seleccionar una moneda de referencia (1 euro) mediante clic del mouse, y luego clasifica automáticamente todas las monedas detectadas calculando el valor total.

El codigo paraa realizar esta funcion  en primer lugar carga la imagen correspondiente, para el caso base'monedas.jpg'.
Convierte a escala de grises y aplica filtro de desenfoque para mejorar la detección. 

Como segundo paso trata de detectar los circulos de las monedas para ello utiliza la transformada de Hough para detectar formas circulares (monedas)

A continuación utiliza un sistema de clasificación para saber qeu moneda la que esta tratando existen dos estructuras:

Diccionario de proporciones: Relaciona tamaños relativos entre monedas

Diccionario de valores: Asigna valor monetario a cada tipo de moneda

La moneda de 1 euro sirve como referencia para calcular proporciones

Finalemtne el programa interactua con el usuario mediante el siguiente flujo: 

1) Usuario hace clic en la moneda de 1 euro para establecer referencia

2) Muestra imagen con círculos detectados

3) Calcula automáticamente todas las monedas basándose en proporciones para ello realiza un bucle en el que para cada moneda detectada, calcula la proporción entre su diámetro y el de referencia. Compara esta proporción con valores predefinidos de las monedas euro. Identifica cada moneda encontrando la proporción más cercana y calcula el valor total.

Paraa realizar la interpretación de los resultados  se dibuja círculos verdes alrededor de monedas detectadas, se etiqueta cada moneda con su denominación y finalmente se muestra el valor total calculado en euros.

### Segundo Ejercicio

