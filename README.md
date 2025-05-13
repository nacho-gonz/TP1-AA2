# Instrucciones.

## Instalación 

- *1* **clonar el repositorio**

  - git clone https://github.com/nacho-gonz/TP1-AA2

- *2* **Instalar las librerias y dependencias necesarias**:
  - pip install -r requirements.txt
  - pip install ipykernel -U --force-reinstall

- *3* **Hardware necesario**:
  - Para el Problema 2 es necesario tener una camara web conectada a la computadora.

## Ejecución del código:

 - **Problema 1**:
    - Ejecutar todo el notebook.

 - **Problema 2**:
   
    - **record-dataset.py**: Este script te permite utilizar la cámara web para grabar imágenes y utilizarlas como dataset para el próximo script. Es necesario que se vea una mano en la imágen, ya que sino el modelo de detección de manos no encontrará la misma y el modelo de detección de piedra papel o tijera no se podrá entrenar. 
      - Ejecutar la siguiente línea en la terminal: **python record-dataset.py**
        
    - **train-gesture-classifier.py**: Este script entrena una red neuronal densa con un dataset de puntos x e y de los 21 puntos de la mano encontrados por Mediapipe, para ver métricas observar el notebook del TP1_P2.ipynb. Es necesario tener el dataset de puntos de la mano para poder correr este script.
      - Ejecutar la siguiente línea en la terminal: **python train-gesture-classifier.py**
        
    - **rock-paper-scissors.py**: Este script te permite ver la camara web en tiempo real e identificar que gesto entre piedra, papel o tijera se esta realizando, además te permite capturar imágenes de las predicciones hechas. Es necesario tener un modelo de clasificación de gestos entrenado para poder ejecutar este script.
      - Ejecutar la siguiente línea en la terminal: **python rock-paper-scissors.py**

 
 - **Problema 3**:
   
   - Ejecutar todo el notebook.

## Personalización

 - El problema 2 ya tiene incluido todo el dataset de entrenamiento y predicciones hechas, en caso de querer ejecutar el script record-dataset.py se borrará el dataset existente para reemplazarlo por el nuevo, lo mismo para los modelos de predicción.
