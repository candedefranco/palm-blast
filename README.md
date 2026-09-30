# Palm Blast

**▶ Probalo en vivo:** https://candedefranco.github.io/palm-blast/ (Chrome, con webcam)

Efecto de "poderes" en tiempo real con la webcam: abrís la palma y aparece una bola de energía que sigue tu mano. Cerrás el puño y explota.

Es una sola página web. Usa [MediaPipe Hand Landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker) para detectar la mano y dibuja las partículas en un canvas. No hay que instalar nada.

## Cómo usarlo

Desde esta carpeta:

```bash
python3 -m http.server 8000
```

Después abrí <http://localhost:8000> en Chrome y tocá **Activar cámara**.

## Gestos

| Gesto | Efecto |
|---|---|
| Palma abierta | Se carga la bola de energía, que sigue la mano |
| Puño cerrado | Explosión: onda expansiva, chispas, flash y temblor de pantalla |
| Dos manos | Cada mano tiene su propia bola |

## Teclas

| Tecla | Acción |
|---|---|
| `R` | Grabar / detener (cuenta regresiva de 3 s). Descarga un `.mp4` con los efectos |
| `V` | Cambiar entre horizontal y vertical 9:16 (para reels) |
| `1`–`4` | Color: azul, fuego, verde, violeta |
| `H` | Ocultar controles |
| `D` | Mostrar el esqueleto de la mano (para depurar) |

## Tips para el reel

- Grabá en vertical (`V`) y con poca luz en el cuarto: la energía brilla mucho más.
- Cargá la bola despacio y cerrá el puño de golpe para que la explosión se vea más fuerte.
- El video se graba con los efectos incluidos; la música la agregás después en la app.
