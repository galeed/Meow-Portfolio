# 🖥️ Quantum-TUI Portfolio v6.2

Portfolio interactivo con estética de terminal retro (TUI), inspirado en **Hyprland** 
con tiling automático de ventanas, juegos, música, drum machine y utilidades.

![version](https://img.shields.io/badge/version-6.2.0-00ff9c?style=flat-square)
![license](https://img.shields.io/badge/license-MIT-ff79c6?style=flat-square)

---

## ✨ Features

### 🪟 Window Manager (estilo Hyprland)
- **Tiling automático**: hasta 4 ventanas se acomodan solas sin superponerse
- **Layouts dinámicos**: 1 ventana = fullscreen · 2 = split 50/50 · 3 = master + 2 stack · 4 = grid 2×2
- **3 botones estilo macOS**: cerrar / minimizar / maximizar
- **Snap manual**: arrastra a bordes (izq/der/arriba) con preview animado
- **Drag & resize** con mouse y touch
- **Al abrir la 5ª**: toast de aviso, rechaza la apertura

### 🎮 Juegos
| Juego | Controles |
|-------|-----------|
| 🐍 Snake | `↑↓←→` mover · `Space` pausa |
| 🧱 Tetris | `←→` mover · `↑` rotar · `↓` soft · `Space` hard drop · `P` pausa |
| 🔢 2048 | `↑↓←→` mover · `R` reiniciar |

### 🎵 Audio
- **Reproductor** con 4 tracks sintetizados y visualizador
- **Drum machine** 16 pasos × 4 canales + 3 presets
- **Sonido de tecleo** sintetizado (toggle con `sound`)

### 💻 Shell interactiva
Comandos: `help`, `about`, `skills`, `collabs`, `system`, `shell`, 
`music`, `drum`, `snake`, `tetris`, `2048`, `ls`, `whoami`, `sound`, `exit`

### 📱 Responsive
- Toggle **móvil/PC** en el dock (o `Ctrl+M`)
- Detección automática inicial por `max-width: 768px`
- Preferencia persistida en `localStorage`
- En móvil: ventanas en columna vertical, sin drag/snap

### 🎨 Efectos visuales
- Matrix rain animado de fondo
- Scanlines + viñeta CRT
- Boot screen cinematográfico
- Glow neón por zona de snap

---

## 🚀 Uso

```bash
# Opción 1: doble click
#   → Abre index.html directamente (funciona sin servidor)

# Opción 2: servidor local (recomendado para desarrollo)
python -m http.server 8000
# o
npx serve