# Práctica 1 - Vision por Computador
En esta primera práctica, tendremos que instalar Anaconda para poder crear un *environment* de Python y asegurar que la instalación de los paquetes necesarios para esta actividad no generen conflicto con los ya instalados en cada equipo.
Tras dicha instalación y la creación de un primer *environment*, se comenzarán a realizar cada una de las tareas especificadas en el repositorio original.
## Primera tarea: crear una imagen con la textura de un tablero de ajedrez.
En este primer apartado de la práctica, se empleará matplotlib para generar una imagen, de tamaño 800x800, que tenga la textura de un tablero de ajedrez. Para ello se empleará la creación de una matriz de ceros gracias a NumPy, y se rellenarán los distintos recuadros blancos a lo largo de la imagen, de forma iterativa.
## Segunda tarea: crear una imagen estilo Mondrian.
Para esta actividad, el contexto cambia un poco, pues la idea es generar una imagen que se asemeje a un cuadro del artista **Mondrian**, pero sin una estructura fija, empleando la creatividad. En este caso, además, en lugar de modificar manualmente la matriz, se emplearán las funciones de OpenCV para generar rectángulos de diferentes colores. Además de generarlo con colores elegidos a mano, hemos añadido la opción de generarlo con colores aleatorios.
## Tercera tarea: modificar de forma libre los valores de uno de los planos de la imagen por webcam.
Ahora tratamos directamente con vídeo en directo, capturado por la webcam en tiempo real, y modificamos uno de los 3 planos para cambiar el color de la imagen sin necesidad de grabar el vídeo y editarlo tras su captura.
## Cuarta tarea: pintar círculos en los píxeles más claro y más oscuro de la imagen.
Durante la cuarta actividad, se empleará vídeo en tiempo real igual que en el apartado anterior, pero buscando mediante los valores de los diferentes canales aquellos píxeles que sean el más claro y el más oscuro, y dibujando círculos en donde están situados. Además, también se realiza dividiendo la imagen en zonas de 8x8 y buscando la más clara y la más oscura.
## Quinta tarea: propuesta propia de pop art.
Finalizando, esta quinta y última tarea propone realizar un filtro para la webcam con un estilo pop art, asemejándose al estilo de los 50-70s, modificando los valores de los diferentes canales de la imagen en distintas partes de esta, haciendo que se genere un efecto visual atractivo y similar al movimiento artístico del pop art.
