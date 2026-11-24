# CTRL-02 — Controlador físico USB
**Asignatura:** Diseño de Interfaces (2026) | Universidad Adolfo Ibáñez  
**Entrega:** Entrega 1 · Unidad 2: Interfaces Físicas  
**Estudiante:** Martín Donoso  
**Página del proyecto:** [Ver CTRL-02 desplegado](https://martindonoso2005-cell.github.io/Interfaz-Midi/)

---

## Descripción
CTRL-02 es un controlador físico con carcasa impresa en 3D que se conecta por USB al computador y maneja un sintetizador en el navegador. Toca, cambia el tipo de onda y modula el tono y el volumen en tiempo real, con un osciloscopio que muestra la onda mientras suena.

## Controles
| Control | Función | Pin |
|---|---|---|
| Botón A (blanco) | Play / mute | D3 |
| Botón B (azul) | Cambia el tipo de onda | D2 |
| Perilla | Tono (frecuencia) | A1 |
| Fader | Nivel (volumen) | A0 |

## Cómo funciona
- **Hardware:** Arduino con shield, 2 botones (resistencia pull-up interna) y 2 potenciómetros de 10 bits (0–1023), con 5 V y GND común.
- **Conexión:** USB serial a 9600 baud, leída desde la página con Web Serial.
- **Sonido:** Web Audio API, con osciloscopio en vivo.

## Cómo probarlo
1. Conecta el CTRL-02 por USB.
2. Abre la [página del proyecto](https://martindonoso2005-cell.github.io/Interfaz-Midi/) en **Chrome o Edge** en un computador.
3. Entra a **Probar producto** y toca **Conectar Arduino**.

## Contenido del repositorio
- `index.html`: dashboard del sintetizador y documentación.
- `lamina_CTRL-02.png`: lámina de producto.
- `Cableado.png`: diagrama esquemático.
- `ENS_1.jpeg` a `ENS_6.jpeg`: fotos del proceso de fabricación y ensamble.

Video de funcionamiento: [YouTube](https://youtube.com/shorts/uGYHcVdGSDg)
