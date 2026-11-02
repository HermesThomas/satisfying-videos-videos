# satisfying-videos

Repository pour la génération de vidéos animées avec algorithme de physique réaliste.

## Architecture

### Python
- `python/bouncing_ball.py` — Algorithme de calcul physique
- `python/generate_data.py` — Script de génération de la trace

### HTML / Canvas
- `html/animation.html` — Animation dans un canvas

### Hyperframes
- `my-video/` — Projet hyperframes pour la génération vidéo
  - `index.html` — Composition HTML avec l'animation
  - `video.mp4` — Vidéo générée
  - `frames/` — Frames intermédiaires
  - `trace.json` — Données de trace pour l'animation

## Génération

### Avec hyperframes

```bash
cd my-video
npx hyperframes render
```

### Avec Python

```bash
python generate_data.py --config config/bouncing_ball_v4.json --output trace.json
```

## Structure

- `my-video/index.html` — Composition hyperframes
- `my-video/video.mp4` — Vidéo générée
- `my-video/frames/` — Frames PNG (debug)
- `config/bouncing_ball_v4.json` — Configuration de l'algorithme
- `html/animation.html` — Animation canvas
- `python/bouncing_ball.py` — Algorithme de physique
- `python/generate_data.py` — Générateur de trace
