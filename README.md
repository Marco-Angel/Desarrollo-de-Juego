# Desarrollo-de-Juego
Explicación de el codigo

--
## Asignacion de librerias y colores.
<img width="578" height="443" alt="image" src="https://github.com/user-attachments/assets/f2df5b73-0dd1-476d-b0cc-350f538d2037" />

- Importa librerías (pygame, threading, etc.), en este caso es importante lalibreria  **pygame** que si no esta instalada instalarla con **pip install pygame** es importante esta libreria para crear videojuegos en 2D, la libreria **threading** para manejar y crear hilos.
- Inicializa Pygame y crea una ventana de 800×600 con título “Desafío de Esquiva”.
- Define un reloj para controlar los FPS.
- Declara colores RGB para fondo, nave, meteoritos y texto.
- Crea una fuente Verdana de tamaño 28 para mostrar texto en pantalla.

--
## Configuración de la nave y semaforos
<img width="680" height="445" alt="image" src="https://github.com/user-attachments/assets/7d3b3d99-8e27-4702-be61-71aa398505d3" />

- Definir el tamaño y posición inicial de la nave.
- Crea cola y lista para manejar meteoritos.
- Configura su tamaño, velocidad y límite máximo.
- Inicializa puntuación y estado del juego.
- Usa un Lock para evitar conflictos entre hilos.
- Usa un Semáforo para limitar la cantidad de meteoritos activos.

--
## Uso de hilos y semaforos

<img width="843" height="691" alt="image" src="https://github.com/user-attachments/assets/de49c71d-f5ce-4c11-8fb0-68a001270482" />

- pintar_nave y pintar_meteorito: dibujan la nave y los meteoritos.
- productor_meteoritos: hilo que crea meteoritos nuevos usando un semáforo para limitar su cantidad.
- consumidor_meteoritos: hilo que mueve meteoritos, suma puntos y usa un Lock para evitar conflictos al modificar la lista compartida.

--

<img width="753" height="641" alt="image" src="https://github.com/user-attachments/assets/6670a3f5-8b9b-4410-b5d8-631c9c88f576" />
<img width="891" height="260" alt="image" src="https://github.com/user-attachments/assets/3912aba1-2fa0-4d36-b401-f65d7d82dd43" />


