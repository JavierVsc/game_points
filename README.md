# Marcador de puntajes para juegos de mesa

Aplicación web para registrar partidas, rondas y puntajes de cuatro juegos de mesa. Funciona directamente en el navegador, sin cuenta ni instalación de dependencias. El marcador acompaña el juego físico: los participantes ingresan los puntos de cada ronda.

**Abrir la aplicación:** [GitHub Pages](https://javiervsc.github.io/game_points/) o `index.html` en un navegador.

## Juegos

| Juego | Registro de puntajes | Ganador |
| --- | --- | --- |
| **Scrabble** | Puntos obtenidos en cada ronda. | Mayor puntaje acumulado. |
| **Carioca** | Once rondas de combinaciones de tríos y escalas; permite registrar una ronda omitida. | Menor puntaje acumulado. |
| **Escoba** | Desglose de puntos por escobas, oros, sietes y otros logros de cada ronda. | Mayor puntaje acumulado. |
| **Tren Mexicano** | Dominó doble doce de 91 fichas. Trece rondas, una por cada «Chancho» del 12 al 0; pueden jugarse en cualquier orden, una vez cada uno. | Menor puntaje acumulado. |

## Cómo usar el marcador

1. En la página principal, abre el juego que quieras anotar.
2. Asigna un nombre a la partida y agrega al menos dos participantes.
3. Inicia la partida e ingresa los puntajes al finalizar cada ronda. La tabla muestra el total y ordena a los participantes según quién va ganando.
4. Puedes volver más tarde y reanudar una partida en curso por su nombre, fecha de inicio y participantes. También puedes borrar una partida concreta o usar la opción de limpieza de partidas del juego.

En Tren Mexicano, selecciona para cada ronda el chancho que se haya jugado. La partida se completa al registrar los trece chanchos, independientemente del orden.

## Guardado y límites

Las partidas se guardan en el almacenamiento local del navegador. Permanecen disponibles al cerrar y volver a abrir la página **en el mismo navegador y dispositivo**. No se sincronizan con GitHub ni entre dispositivos. Borrar los datos del sitio, usar otro navegador o navegar en modo privado puede hacer que dejen de estar disponibles. Conviene evitar esas acciones si hay partidas que se quieren retomar.

## Desarrollo local

El proyecto está compuesto por archivos HTML, CSS y JavaScript sin dependencias de instalación ni proceso de compilación. Puedes abrir `index.html` directamente o servir el directorio con un servidor HTTP local:

```bash
python3 -m http.server 8000
```

Luego visita `http://localhost:8000/`. Las páginas de cada juego también se pueden abrir directamente: `scrabble.html`, `carioca.html`, `escoba.html` y `tren_mexicano.html`.
