# Practica 5 


## Objetivo 

La meta de este proyecto es la creación de dos filtros mediante el uso de tecnologías de deteccion facial, para las implementaciones concretas se ha utilizado en primer lugar MTCCN (Multi-task Cascaded Convolutional Networks) para el desarrollo del primer filtro y, en el segundo filtro, un YOLOv8 preentrenado para detección de caras, y un segundo modelo YOLOv8 que hemos entrenado con el siguiente dataset (https://www.kaggle.com/datasets/fatihkgg/affectnet-yolo-format/data) para la detección de emociones.


### Primer Filtro

Primer Filtro

El primer filtro está inspirado en el cine mudo de los años 20, más concretamente en la figura de Charlie Chaplin. Para recrear la imagen del icónico personaje se superponen sobre el rostro del usuario un sombrero de bombín, un bigote y dos cejas.

El sistema carga previamente todas las imágenes PNG con canal alfa y utiliza el modelo MTCNN para detectar los puntos clave del rostro (ojos y boca). A partir de estos puntos, el código calcula dinámicamente el tamaño y la posición de cada accesorio para adaptarlos correctamente a la cara detectada en tiempo real.
Para insertar cada elemento en el fotograma se emplea una función auxiliar que realiza una superposición alfa, permitiendo mezclar la transparencia de los PNG con la imagen original sin perder calidad.

El proceso se repite en cada iteración de la cámara:

-Se detecta la cara y sus keypoints.

-Se calculan proporciones como la distancia entre ojos para escalar sombrero y cejas.

-Se obtiene el ancho de la boca para el tamaño del bigote.

-Se colocan los elementos en función del centro de ojos, posición de cejas y boca.

Finalmente, el fotograma resultante se convierte a escala de grises, manteniendo solo los accesorios a color para reforzar la estética del cine mudo.

### Segundo Filtro 

El segundo filtro se basa en un sistema de reconocimiento emocional capaz de reaccionar en tiempo real a la expresión detectada en el rostro del usuario. Para ello se emplean dos modelos YOLO: Un YOLOv8-lite-t para la detección de caras y un YOLOv8 entrenado específicamente con el dataset AffectNet para clasificar emociones.

El flujo de funcionamiento es el siguiente:

En primer lugar la webcam captura cada fotograma y el modelo YOLO de detección facial identifica las caras presentes, generando sus coordenadas. Para cada rostro encontrado se realiza un crop y se pasa al modelo YOLO de emociones, que predice la categoría emocional con mayor confianza entre las ocho posibles. En función de la emoción resultante, el sistema aplica un filtro visual distinto sobre la cara del usuario. Estos filtros incluyen superposición de imágenes PNG con canal alfa (como globos, regalos, vómito, puntos suspensivos…), efectos dibujados directamente (como la lluvia) o animaciones GIF convertidas frame a frame (como fuego o arañas).
Las imágenes y GIFs se colocan dinámicamente en relación a la bounding box de la cara detectada, garantizando una colocación coherente del filtro en cada expresión y para cualquier distancia a la cámara.
Finalmente, cada elemento gráfico se integra en el fotograma.

Además se ha añadido la opción de elegir dos modos: al tocar la tecla "c" se visualizará únicamente la cara detectada y la emoción, con su precisión, y al emplear la tecla "p" se verá dibujada la bounding box de la cara además del filtro.

### Resultados 




Este enfoque permite que el filtro responda de forma inmediata y visualmente llamativa al estado emocional del usuario, creando una experiencia interactiva y personalizada.
### Resultados 
