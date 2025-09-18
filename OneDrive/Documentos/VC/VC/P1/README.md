# Práctica 1 - Vision por Computador
En esta primera práctica, tendremos que instalar Anaconda para poder crear un *environment* de Python y asegurar que la instalación de los paquetes necesarios para esta actividad no generen conflicto con los ya instalados en cada equipo.
Tras dicha instalación y la creación de un primer *environment*, se comenzarán a realizar cada una de las tareas especificadas en el repositorio original.
## Primera tarea: crear una imagen con la textura de un tablero de ajedrez.
En este primer apartado de la práctica, se empleará matplotlib para generar una imagen, de tamaño 800x800, que tenga la textura de un tablero de ajedrez. Para ello se empleará la creación de una matriz de ceros gracias a NumPy, y se rellenarán los distintos recuadros blancos a lo largo de la imagen, de forma iterativa.

<img width="425" height="418" alt="image" src="https://github.com/user-attachments/assets/aa84f01c-eee2-46c1-baa6-f0934b0122da" />

## Segunda tarea: crear una imagen estilo Mondrian.
Para esta actividad, el contexto cambia un poco, pues la idea es generar una imagen que se asemeje a un cuadro del artista **Mondrian**, pero sin una estructura fija, empleando la creatividad. En este caso, además, en lugar de modificar manualmente la matriz, se emplearán las funciones de OpenCV para generar rectángulos de diferentes colores. Además de generarlo con colores elegidos a mano, hemos añadido la opción de generarlo con colores aleatorios.

<img width="425" height="418" alt="image" src="https://github.com/user-attachments/assets/58c5dc49-a62e-40d6-9277-f275c155870f" />
<img width="425" height="418" alt="image" src="https://github.com/user-attachments/assets/eb5bf4cf-08da-40eb-8caf-9d8aa858139e" />

## Tercera tarea: modificar de forma libre los valores de uno de los planos de la imagen por webcam.
Ahora tratamos directamente con vídeo en directo, capturado por la webcam en tiempo real, y modificamos uno de los 3 planos para cambiar el color de la imagen sin necesidad de grabar el vídeo y editarlo tras su captura.

<img width="793" height="629" alt="image" src="https://github.com/user-attachments/assets/adfbef2c-65da-445d-ad40-41755d7be38c" />
<img width="1183" height="326" alt="image" src="https://github.com/user-attachments/assets/6e1ed006-7eb9-4174-be2f-a92f277a489d" />

## Cuarta tarea: pintar círculos en los píxeles más claro y más oscuro de la imagen.
Durante la cuarta actividad, se empleará vídeo en tiempo real igual que en el apartado anterior, pero buscando mediante los valores de los diferentes canales aquellos píxeles que sean el más claro y el más oscuro, y dibujando círculos en donde están situados. Además, también se realiza dividiendo la imagen en zonas de 8x8 y buscando la más clara y la más oscura.
<img width="796" height="632" alt="image" src="https://github.com/user-attachments/assets/d8525880-8eb1-49a2-9e21-1bdf133ea497" />

## Quinta tarea: propuesta propia de pop art.
Finalizando, esta quinta y última tarea propone realizar un filtro para la webcam con un estilo pop art, asemejándose al estilo de los 50-70s, modificando los valores de los diferentes canales de la imagen en distintas partes de esta, haciendo que se genere un efecto visual atractivo y similar al movimiento artístico del pop art.

<img width="791" height="625" alt="image" src="https://github.com/user-attachments/assets/64d83f91-705e-48f8-9540-479b754c4702" />

