# Actividad 5
# Juego Memory

> Este proyecto es una copia de Memory en Python utilizando las librerías `turtle` y `freegames`. Permite al usuario jugar al juego de memoria destapando parejas de fichas.
> Versión: 2

## Funcionalidades Base
- **Tablero:** Un tablero de 8x8 con 64 fichas organizadas en cuadrícula que ocultan pares de números del 0 al 31.
- **Mecánica de juego:** 
  - Al hacer clic en un cuadro blanco, este se destapa mostrando su número.
  - Al seleccionar un segundo cuadro, si ambos números coinciden, se revelan de forma permanente dejando ver la imagen de fondo.
  - Si los números no coinciden, la marca cambia a la nueva casilla seleccionada.
- **Imagen de fondo:** Oculta detrás de las fichas se muestra la imagen de un carro (`car.gif`).

## Funcionalidades agregadas
- **Centrado de texto en casillas:** Se mejoró el centrado del contenido de las fichas para que los números queden bien centrados dentro del cuadro.
- **Símbolos en vez de números:** Se cambiaron los números del 0 al 31 por 32 parejas de símbolos para ayudar a la memoria del jugador.
- Se cuenta y muestra el numero de taps del usuario en la parte superior del tablero
- Se muestra un mensaje de victoria cuando todos los cuadros fueron detectados frfr 
## Cambios en el código
- Se modificó `draw()` para ajustar la posición de escritura con `goto(x + 25, y + 5)`.
- Se añadió el `align="center"` a la función `write()` y se ajustó el tamaño de fuente a 25 en `font=('Arial', 25, 'normal')` para lograr un mejor centrado..
- Se creó la lista `SIMBOLOS` con 32 símbolos y se asignó a `tiles=SIMBOLOS*2`
## Requisitos e Instalación
1. Asegurarse de tener Python 3 instalado.
2. Instalar la librería requerida:
```bash
pip install freegames
