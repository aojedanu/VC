## Práctica 1. Primeros pasos con OpenCV


### Ejercicio 1 

En este primer ejercicio se dibuja un tablero de ajedrez sobre  imagen en blanco de 800×800 píxeles en escala de grises.
Recorre 8 filas para dibujar un patrón alternado tipo tablero pintando cuadrados blancos de 100×100 píxeles en posiciones alternadas según la fila.
finalmnete se muestra el resultado  usando matplotlib.

![Imagen tablero de ajedrez](Imagen_Ajedrez.png)


### Ejercicio 2

Para esta segunda etrega se plantea dos composiciones al estilo de Piet Mondrian rellenando varias zonas rectangulares en posiciones bien definidas.
La intencin del codigo mediante el uso de funciones como cv2.rectangle es imita el estilo Mondrian: formas rectangulares limpias, colores planos primarios, sin degradados. Los dos cuadros son identicos pero el segundo fue generado mediante colores aleatorios.

![Imagen Mondrian](Imagen_Mondrian.png)

### Ejercicio 3

Este código captura video en tiempo real desde la cámara.
Invierte el canal rojo de cada fotograma y le añade franjas horizontales con el rojo original.
Primero muestra la imagen modificada en color, luego un collage con los tres canales separados (R, G, B).
Finalmente, libera la cámara y cierra las ventanas al presionar ESC.

![Imagen separacion de canales](Imagen_Saturacion.png)

### Ejercicio 4

Este código captura vídeo en tiempo real desde la cámara.
Convierte cada fotograma a escala de grises para localizar el píxel más oscuro y el más claro mediante la función minMaxLoc.
Tras localizar dichos pixeles dibuja un círculo azul en la posición más oscura y uno amarillo en la más brillante.
Finalmente Muestra el resultado en una ventana hasta que se presiona ESC.

![Imagen Busqueda de pixeles](Imagen_Busqueda.png)



### Ejercicio 5

Este código captura video en tiempo real y lo divide en 16 versiones más pequeñas.
A cada una le aplica un cambio distinto de tono y saturación para generar variaciones de color.
Estas transformaciones se hacen en el espacio HSV, ideal para manipular colores fácilmente.
Luego organiza todas las versiones en un collage 4×4 con un borde negro.
El resultado recuerda al estilo Pop Art, especialmente a los retratos repetidos y coloreados de Andy Warhol.
Combina repetición, colores intensos y composición cuadriculada para lograr un efecto artístico vibrante



![Propuesta de pop Art](Imagen_Pop.png)
